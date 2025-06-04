# Introduction
For synchronization with VTURB to work, you need to add the hidden class (which is a standard Tailwind CSS class for hiding elements) to the required elements. Also, apply this JavaScript code to the site. Copy and paste the same JavaScript code below as Codeblock JS to apply to the site, it should be exactly the same, just change the time from 10 seconds to what the user wants.

**IMPORTANT: the javascript below must be the same without modifications**

```js
document.addEventListener("DOMContentLoaded", function() {
    var SECONDS_TO_DISPLAY = 10;
    var CLASS_TO_DISPLAY = ".hidden";
    var EXPIRATION_DAYS = 14;
    var alreadyDisplayedKey = "alreadyElsDisplayed" + SECONDS_TO_DISPLAY;
    var elsHidden = document.querySelectorAll(CLASS_TO_DISPLAY);
    var elsDisplayed = false;
    var attempts = 0;

    class StorageHandler {
        static expiryTime = EXPIRATION_DAYS * 86400000;

        static set(key, value) {
            localStorage.setItem(
                key,
                JSON.stringify({ value, expiry: Date.now() + this.expiryTime })
            );
        }

        static get(key) {
            var item = localStorage.getItem(key);
            if (!item) return null;

            var { value, expiry } = JSON.parse(item);
            if (Date.now() > expiry) {
                localStorage.removeItem(key);
                return null;
            }
            return value;
        }
    }

    var alreadyElsDisplayed = StorageHandler.get(alreadyDisplayedKey);

    var showHiddenElements = function () {
        elsDisplayed = true;
        elsHidden.forEach((e) => e.classList.remove("hidden"));
        StorageHandler.set(alreadyDisplayedKey, true);
    };

    var startWatchVideoProgress = function () {
        if (typeof smartplayer === 'undefined' || !(smartplayer.instances && smartplayer.instances.length)) {
            if (attempts >= 10) return;
            attempts++;
            return setTimeout(startWatchVideoProgress, 1000);
        }
        smartplayer.instances[0].on('timeupdate', () => {
            if (elsDisplayed || smartplayer.instances[0].smartAutoPlay) return;
            if (smartplayer.instances[0].video.currentTime < SECONDS_TO_DISPLAY) return;
            showHiddenElements();
        });
    };

    if (alreadyElsDisplayed) {
        setTimeout(showHiddenElements, 100);
    } else {
        startWatchVideoProgress();
    }
});
```
