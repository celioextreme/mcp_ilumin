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
            <button id="cta-button" class="bg-green-500 hover:bg-green-600 text-white font-semibold py-3 px-8 rounded-lg shadow-lg text-xl transition">
                Quero Garantir Minha Vaga!
            </button>
        </div>
    </div>
    <!-- Utilize Exatamente Esse Código, apenas altere o src do vídeo e o poster nesse código javascript para usar o CDN do Vidstack. IMPORTANT: Precisa ser exatamente igual ao código abaixo! -->
    <script type="module">
        document.addEventListener('DOMContentLoaded', async () => {
            const { PlyrLayout, VidstackPlayer } = await import('https://cdn.vidstack.io/player');

            await VidstackPlayer.create({
                target: '#video-target',
                src: 'youtube/_cMxraX_5RE', // Altere o src do vídeo aqui
                poster: 'https://files.vidstack.io/sprite-fight/poster.webp', // Altere o poster (Thumbnail) aqui
                layout: new PlyrLayout({
                    controls: ['play-large', 'play'] // Devem ser exatamente esses controles (Mude apenas se o usuário pedir, se não, não mude)
                }),
            });

            // Exemplo de ação para o botão CTA
            document.getElementById('cta-button').addEventListener('click', () => {
                window.location.href = 'https://seu-link-de-conversao.com/'; // Altere o link de conversão aqui
            });
        });
    </script>
</body>
</html>
