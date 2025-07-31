<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Kelas XI-7 SMAN Situraja</title>
  <link href="https://fonts.googleapis.com/css2?family=Bungee+Shade&family=Poppins:wght@300;600&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      scroll-behavior: smooth;
    }
    body {
      font-family: 'Poppins', sans-serif;
      background: linear-gradient(to bottom, #b3e5fc, #ffffff);
      overflow-x: hidden;
      color: #01579b;
      position: relative;
    }

    /* Gelembung Latar */
    .bubble {
      position: absolute;
      bottom: -100px;
      width: 20px;
      height: 20px;
      background: rgba(255, 255, 255, 0.5);
      border-radius: 50%;
      animation: bubbleUp 10s infinite ease-in;
    }
    @keyframes bubbleUp {
      0% { transform: translateY(0) scale(1); opacity: 1; }
      100% { transform: translateY(-120vh) scale(1.5); opacity: 0; }
    }
    .bubble:nth-child(odd) { left: 10%; animation-duration: 12s; }
    .bubble:nth-child(even) { left: 80%; animation-duration: 8s; }
    .bubble:nth-child(3) { left: 50%; width: 15px; height: 15px; }

    header {
      background: rgba(255, 255, 255, 0.9);
      padding: 20px;
      text-align: center;
      box-shadow: 0 2px 10px rgba(0,0,0,0.1);
      position: sticky;
      top: 0;
      z-index: 999;
    }

    header h1 {
      font-family: 'Bungee Shade', cursive;
      font-size: 3rem;
      background: linear-gradient(90deg, #0288d1, #26c6da, #0288d1);
      background-size: 200% auto;
      color: transparent;
      background-clip: text;
      -webkit-background-clip: text;
      animation: gradientMove 3s linear infinite;
    }

    @keyframes gradientMove {
      0% { background-position: 0% center; }
      100% { background-position: 200% center; }
    }

    .hero {
      height: 100vh;
      background: url('https://drive.google.com/uc?export=view&id=1eNK4wYyuZcmxthwuz16xrdS0Wh122jKE') center center/cover no-repeat;
      display: flex;
      justify-content: center;
      align-items: center;
      text-align: center;
      position: relative;
    }

    .hero h2 {
      font-size: 2.5rem;
      background: rgba(255, 255, 255, 0.75);
      padding: 20px 40px;
      border-radius: 20px;
      box-shadow: 0 8px 30px rgba(0,0,0,0.2);
      animation: fadeIn 1.5s ease-out;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(30px); }
      to { opacity: 1; transform: translateY(0); }
    }

    section.content {
      padding: 60px 20px;
      max-width: 1000px;
      margin: auto;
    }

    .content h3 {
      font-size: 2rem;
      text-align: center;
      margin-bottom: 30px;
      color: #0277bd;
    }

    .card {
      background: white;
      border-radius: 15px;
      padding: 25px;
      margin: 20px 0;
      box-shadow: 0 5px 15px rgba(0,0,0,0.1);
      animation: slideUp 1s ease forwards;
      opacity: 0;
    }

    .card:nth-child(1) { animation-delay: 0.3s; }
    .card:nth-child(2) { animation-delay: 0.6s; }

    @keyframes slideUp {
      to { transform: translateY(0); opacity: 1; }
      from { transform: translateY(40px); opacity: 0; }
    }

    .anggota-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 15px;
      margin-top: 40px;
    }

    .anggota-grid div {
      background: #ffffffcc;
      padding: 15px;
      border-radius: 12px;
      text-align: center;
      font-weight: 600;
      color: #0277bd;
      transition: 0.3s;
      box-shadow: 0 3px 10px rgba(0,0,0,0.05);
    }

    .anggota-grid div:hover {
      background: #81d4fa;
      transform: scale(1.05);
      color: #004d60;
      cursor: default;
    }

    footer {
      text-align: center;
      padding: 30px 10px;
      margin-top: 50px;
      background: #e1f5fe;
      color: #0277bd;
      font-weight: bold;
    }
  </style>
</head>
<body>

  <div class="bubble"></div>
  <div class="bubble"></div>
  <div class="bubble"></div>

  <header>
    <h1>XI-7 SMAN Situraja</h1>
  </header>

  <section class="hero">
    <h2>Selamat Datang di Dunia Kami yang Seru! 🌊</h2>
  </section>

  <section class="content">
    <h3>✨ Tentang Kami</h3>
    <p style="text-align: center; margin-bottom: 40px;">
      Kami adalah keluarga hebat dari SMAN Situraja, Kelas 11-7 yang kreatif, solid, dan selalu penuh semangat!
    </p>

    <div class="card">
      <h3>🌟 Visi & Misi</h3>
      <p>Membangun kekompakan, prestasi, dan kenangan manis bersama dalam suasana belajar yang penuh kebahagiaan.</p>
    </div>

    <div class="card">
      <h3>📅 Agenda Kelas</h3>
      <p>- Study tour ke pantai<br>- Classmeeting seru<br>- Persiapan ujian bareng-bareng</p>
    </div>

    <h3 style="margin-top: 60px;">👥 Anggota Kelas</h3>
    <div class="anggota-grid">
      <div>Adis Permata Rahayu</div>
      <div>Adly Firmansyah</div>
      <div>Ajmi Nafiiesha Ayu</div>
      <div>Alya Salsabila Putri</div>
      <div>Angger Deris Jatmiko</div>
      <div>Dafina Huwaida Nur Shabrina</div>
      <div>Devnika Al Anugrah</div>
      <div>Fakhrezi Ikhsa Akbar</div>
      <div>Fyrantica Restu Anggita</div>
      <div>Galih Aliyana</div>
      <div>Herlina</div>
      <div>Kharsia Putri</div>
      <div>M. Hilmy Nasrulloh</div>
      <div>Merinka Azzahra</div>
      <div>Mita Miftahul Jannah</div>
      <div>Muhamad Azis Solihin</div>
      <div>Muhammad Adlan Ramadhan</div>
      <div>Muhammad Ahlul Dzikri Kohari</div>
      <div>Muhammad Misbah</div>
      <div>Muhammad Wildan Abdul Rozak</div>
      <div>Naya Naura Sholihah</div>
      <div>Nazwa Anggraeni</div>
      <div>Novel Aulia Zalsabliah</div>
      <div>Okta Kurniawan</div>
      <div>Putri Setya Rahman</div>
      <div>Refandika Maulana Yusuf</div>
      <div>Rehan Kurniawan</div>
      <div>Reza Julian Saputra</div>
      <div>Risma Nur Ayustin</div>
      <div>Ristha Adhawidiani Setiawan</div>
      <div>Salsabana Nur Anisa</div>
      <div>Santi Amalia Dewi</div>
      <div>Sherly Hardianti</div>
      <div>Sifa Nur Rohmah</div>
      <div>Silfa Anjani Mega Utami</div>
      <div>Siti Fadilah Romdoni</div>
      <div>Wildan Zainuri Hermayadi</div>
      <div>Zahra Ramadani Putri</div>
    </div>
  </section>

  <footer>
    © 2025 Kelas 11-7 | SMAN Situraja | Dibuat dengan Semangat Laut 💙
  </footer>
</body>
</html>
