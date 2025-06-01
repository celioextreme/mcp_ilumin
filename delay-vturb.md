# Introduction
Use this code to synchronize the VTURB video (a video player) with the buttons, in the example below is the delay in 10 seconds (time in seconds), and the class that should be placed in the element to hide it is ".esconder"

It is mandatory to put the code exactly the same as provided below without any change

## STYLE FOR HEAD (<head>)
!IMPORTANT: Add to CSS a class (hide) with none display

```css
.esconder { display: none }
```

## JAVASCRIPT
Paste exactly the code below (without changing the JS), the only values that should be changed are the time, which is 10 seconds, and the class if you change it from ".esconder". But prefer to keep the same class.

```js
<script type="text/javascript">
document.addEventListener("DOMContentLoaded", function() {
/* Change the value 10 for the seconds where the sections will appear */
    var SECONDS_TO_DISPLAY = 10;
    var CLASS_TO_DISPLAY = ".esconder";
/* From now down don't have to change */
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
        elsHidden.forEach((e) => e.style.display = "block");
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
</script>
```
