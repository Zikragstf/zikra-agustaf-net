<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Zikra Agustaf - Pembelajaran Bahasa Arab</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f4f4f4;
      margin: 0;
      padding: 0;
    }

    header {
      background-color: #008080;
      color: white;
      padding: 20px;
      text-align: center;
    }

    nav {
      display: flex;
      justify-content: center;
      background-color: #004d4d;
    }

    nav button {
      background: none;
      border: none;
      color: white;
      padding: 15px 20px;
      font-size: 16px;
      cursor: pointer;
    }

    nav button:hover {
      background-color: #006666;
    }

    section {
      display: none;
      padding: 20px;
    }

    section.active {
      display: block;
      background-color: white;
      margin: 10px;
      border-radius: 8px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
    }

    footer {
      background: #ddd;
      text-align: center;
      padding: 10px;
    }
  </style>
</head>
<body>

  <header>
    <h1>Website Pembelajaran Bahasa Arab</h1>
    <p>Oleh Zikra Agustaf</p>
  </header>

  <nav>
    <button onclick="showSection('profil')">Profil</button>
    <button onclick="showSection('penjelasan')">Penjelasan</button>
  </nav>

  <section id="profil" class="active">
    <h2>Profil</h2>
    <p><strong>Nama:</strong> Zikra Agustaf</p>
    <p><strong>Tempat Lahir:</strong> Kuantan Singingi, Riau</p>
    <p><strong>Tanggal Lahir:</strong> 22 Agustus 2004</p>
    <p><strong>Pendidikan:</strong> Mahasiswa Pendidikan Bahasa Arab di UIN Suska Riau</p>
  </section>

  <section id="penjelasan">
    <h2>Penjelasan</h2>
    <p>
      Website ini dibuat sebagai media pembelajaran Bahasa Arab untuk siswa dan siapa saja yang tertarik mempelajarinya.
      Di dalamnya akan tersedia materi dasar, seperti mufradat, kalimat percakapan sehari-hari, hingga penjelasan tentang Nahwu dan Sharaf secara sederhana.
    </p>
    <p>
      Harapan saya, website ini bisa membantu teman-teman dalam memahami Bahasa Arab dengan lebih mudah dan menyenangkan.
    </p>
  </section>

  <footer>
    &copy; 2025 Zikra Agustaf
  </footer>

  <script>
    function showSection(id) {
      document.querySelectorAll('section').forEach(sec => sec.classList.remove('active'));
      document.getElementById(id).classList.add('active');
    }
  </script>

</body>
</html>
