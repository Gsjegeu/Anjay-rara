<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SABTU KITA JALAN"</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 50px;
        }
        img {
            width: 300px;
            height: auto;
            margin-bottom: 20px;
        }
        video {
            width: 400px;
            height: auto;
            margin-top: 20px;
            display: none; /* Sembunyikan video terlebih dahulu */
        }
        .container {
            margin-top: 20px;
        }
        button {
            padding: 10px 20px;
            font-size: 18px;
            margin: 10px;
            cursor: pointer;
        }
        #btnTidak {
            position: relative;
        }
    </style>
</head>
<body>
    <h1>SABTU KITA KEMANA NIH</h1>
    <img src="https://assets.onecompiler.app/42vcwzzkr/42vcwypxs/IMG-20241017-WA0070.jpg" alt="Makanan Lezat">
    
    <div class="container">
        <button id="btnIya">OPO JARE SAPTA</button>
        <button id="btnTidak">TERSERAHHH</button>
    </div>

    <!-- Video Ritsuki Senang -->
    <video id="ritsukiVideo" controls>
        <source src="ssstik.io_@queenzavannyaa_1729149305981.mp4" type="video/mp4">
        Browser Anda tidak mendukung elemen video.
    </video>

    <script>
        const btnTidak = document.getElementById('btnTidak');
        const btnIya = document.getElementById('btnIya');
        const ritsukiVideo = document.getElementById('ritsukiVideo');
        
        // Fungsi untuk mengacak posisi tombol "Tidak"
        btnTidak.addEventListener('click', function() {
            const randomX = Math.floor(Math.random() * 300) - 150; // Rentang acak posisi X
            const randomY = Math.floor(Math.random() * 300) - 150; // Rentang acak posisi Y
            btnTidak.style.transform = `translate(${randomX}px, ${randomY}px)`;
        });

        // Fungsi ketika tombol "Iya" diklik
        btnIya.addEventListener('click', function() {
            alert('POKOK SABTU KITA MAKAN PECEL🗿');
            ritsukiVideo.style.display = 'block'; // Tampilkan video
            ritsukiVideo.play(); // Putar video
        });
    </script>
</body>
</html>
