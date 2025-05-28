<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>VSL com Vidstack</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdn.vidstack.io/player.css"/>
    <link rel="stylesheet" href="https://cdn.vidstack.io/plyr.css"/>
</head>
<body class="bg-gray-100 min-h-screen flex flex-col">
    <div class="container mx-auto px-4 py-8 flex-1 flex flex-col justify-center">
        <div class="text-center mb-8">
            <h1 class="text-4xl font-bold text-gray-800 mb-2">Assista ao VSL Exclusivo</h1>
            <p class="text-xl text-gray-600">Descubra como transformar seus resultados com nosso método</p>
        </div>
        <div class="max-w-3xl mx-auto w-full mb-8">
            <div id="video-target" class="aspect-video bg-black"></div>
        </div>
        <div class="text-center">
            <button id="cta-button" class="hidden bg-green-500 hover:bg-green-600 text-white font-semibold py-3 px-8 rounded-lg shadow-lg text-xl transition">
                Quero Garantir Minha Vaga!
            </button>
        </div>
    </div>
    <!-- Use exactly this code, just change the SRC of the video and the poster in this JavaScript code to use the Vidstack CDN. The controls should also be exactly the same (play-large and play only). Important: It needs to be exactly the same as the code below! -->
    <script type="module">
    document.addEventListener('DOMContentLoaded', async () => {
        const { PlyrLayout, VidstackPlayer } = await import('https://cdn.vidstack.io/player');

        const player = await VidstackPlayer.create({
            target: '#video-target',
            src: 'youtube/_cMxraX_5RE', // Change the video SRC here
            poster: 'https://files.vidstack.io/sprite-fight/poster.webp', // Change the poster (thumbnail) here
            layout: new PlyrLayout({
                controls: ['play-large', 'play'] // They must be exactly these controls (change only if the user asks, if not, do not change)
            }),
        });

        // JavaScript below to use delay on elements such as button or other components / sections
        // Variable to control if the button has already been shown
        let ctaButtonShown = false;
        const ctaButton = document.getElementById('cta-button');

        // Adds listener to monitor the video time
        player.addEventListener('time-update', () => {
            const currentTime = player.currentTime;

            // Shows the CTA button when the video reaches 10 seconds
            if (currentTime >= 10 && !ctaButtonShown) {
                ctaButton.classList.remove('hidden');
                ctaButtonShown = true;
            }
        });

        // Example action for the CTA button
        ctaButton.addEventListener('click', () => {
            window.location.href = 'https://seu-link-de-conversao.com/'; // Change the conversion link here
        });
    }); 
    </script>
</body>
</html>
