<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Página VSL</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>.esconder { display: none }</style>
</head>
<body class="bg-gray-50 min-h-screen">
    <div class="container mx-auto px-4 py-8 max-w-4xl">
        <!-- Headline -->
        <h1 class="text-3xl md:text-4xl font-bold text-center text-gray-800 mb-10 leading-tight">
            Descubra o Segredo que Está Transformando a Vida de Milhares de Pessoas
        </h1>
        
        <!-- Video Container -->
        <div class="w-full mb-10">
            <div id="vid_64af0cbdd66489000873b9d7" style="position:relative;width:100%;padding: 56.25% 0 0;">
                <img decoding="async" id="thumb_64af0cbdd66489000873b9d7" src="https://images.converteai.net/0ff61758-5662-4d0c-b77e-8b63b2d08493/players/64af0cbdd66489000873b9d7/thumbnail.jpg" style="position:absolute;top:0;left:0;width:100%;height:100%;object-fit:cover;display:block;">
                <div id="backdrop_64af0cbdd66489000873b9d7" style="position:absolute;top:0;width:100%;height:100%;-webkit-backdrop-filter:blur(5px);backdrop-filter:blur(5px);"></div>
            </div>
            <script type="text/javascript" id="scr_64af0cbdd66489000873b9d7">var s=document.createElement("script");s.src="https://scripts.converteai.net/0ff61758-5662-4d0c-b77e-8b63b2d08493/players/64af0cbdd66489000873b9d7/player.js",s.async=!0,document.head.appendChild(s);</script>
        </div>
        
        <!-- CTA Button -->
        <div class="text-center esconder">
            <button class="bg-green-600 hover:bg-green-700 text-white font-bold py-4 px-8 rounded-lg text-xl shadow-lg transition-all duration-300 transform hover:scale-105">
                Quero Adquirir o Produto
            </button>
        </div>
    </div>
    
    <!-- 10 Seconds with Delay in Components -->
    <script>
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
    </script>
</body>
</html>
