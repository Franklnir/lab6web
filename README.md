![image](https://github.com/user-attachments/assets/21628f3b-c636-4a8e-aca0-134e24549010)

# lab6web
1. Navigasi: Menyediakan link menuju bagian-bagian penting di halaman seperti Beranda, Proyek Saya, dan Kontak, serta memiliki fitur responsif agar tampil dengan baik di berbagai ukuran layar.
2. Header: Bagian pembuka yang menyambut pengunjung dengan informasi singkat tentang Irsyad dan dilengkapi dengan tombol untuk melihat proyek yang telah dikerjakannya.
3. Konten Proyek: Menampilkan beberapa proyek yang sedang dikerjakan, menggunakan komponen card untuk setiap proyek dengan tombol untuk melihat rincian lebih lanjut.
4. Footer: Menyediakan informasi hak cipta yang mencantumkan nama Irsyad dan jurusan yang diambilnya.
5. Bootstrap: Digunakan untuk styling halaman dan memastikan tampilan tetap responsif di berbagai perangkat.
    
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Profil Irsyad - Mahasiswa Teknik Informatika</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <nav class="navbar navbar-expand-lg navbar-dark bg-primary">
      <div class="container-fluid">
        <a class="navbar-brand" href="#">Profil Irsyad</a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" 
          aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav ms-auto">
            <li class="nav-item">
              <a class="nav-link active" aria-current="page" href="#">Beranda</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#projects">Proyek Saya</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#contact">Kontak</a>
            </li>
          </ul>
        </div>
      </div>
    </nav>
    <header class="bg-light text-center py-5">
      <div class="container">
        <h1 class="display-4">Selamat Datang di Profil Saya</h1>
        <p class="lead">Nama saya Irsyad, Mahasiswa Teknik Informatika Semester 3 di Universitas Pelita Bangsa.</p>
        <a href="#projects" class="btn btn-primary btn-lg">Lihat Proyek Saya</a>
      </div>
    </header>
<main id="projects" class="container my-5">
    <h2 class="text-center mb-4">Proyek Saya di Bidang IoT</h2>
    <div class="row">
      <div class="col-md-4">
        <div class="card h-100">
          <div class="card-body">
            <h3 class="card-title">Smart Home</h3>
            <p class="card-text">Proyek ini bertujuan untuk mengembangkan sistem rumah pintar yang memungkinkan pengendalian perangkat elektronik melalui aplikasi.</p>
            <a href="#" class="btn btn-secondary">Lihat Detail</a>
          </div>
        </div>
      </div>
      <div class="col-md-4">
        <div class="card h-100">
          <div class="card-body">
            <h3 class="card-title">Monitoring Kualitas Udara</h3>
            <p class="card-text">Proyek ini mengembangkan alat IoT untuk memantau kualitas udara dalam ruangan dan memberikan informasi secara real-time.</p>
            <a href="#" class="btn btn-secondary">Lihat Detail</a>
          </div>
        </div>
      </div>
      <div class="col-md-4">
        <div class="card h-100">
          <div class="card-body">
            <h3 class="card-title">Smart pertanian</h3>
            <p class="card-text">Proyek ini menciptakan sistem untuk pertanian pintar yang memungkinkan pemantauan kelembaban tanah secara otomatis.</p>
            <a href="#" class="btn btn-secondary">Lihat Detail</a>
          </div>
        </div>
      </div>
    </div>
  </main>
    
    <footer class="bg-dark text-white text-center py-3">
      <div class="container">
        <p>&copy; 2024 Irsyad - Mahasiswa Teknik Informatika, Universitas Pelita Bangsa</p>
      </div>
    </footer>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>






# style css
# Card (Proyek): 
# Setiap proyek ditampilkan dalam bentuk card yang memiliki bayangan untuk memberikan kesan modern.
# Card menggunakan warna cerah dan teks yang jelas dan mudah dibaca.
# Chat Button: Terdapat tombol chat yang selalu terlihat di sudut kanan bawah dengan desain bulat dan warna biru. 

body {
    font-family: Arial, sans-serif;
    background: linear-gradient(135deg,  #19cbeb,#006aff, #fe54f0d6);
    color: #333;
    margin: 0;
    padding: 0;
}
nav {
    background-color: transparent;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px 20px;
}
nav .navbar-brand {
    font-size: 1.5rem;
    font-weight: bold;
    color: #333;
}
nav ul {
    list-style-type: none;
    display: flex;
    gap: 20px;
}
nav ul li a {
    color: #333;
    text-decoration: none;
    font-weight: 600;
}
nav .auth-buttons a {
    margin-left: 15px;
    text-decoration: none;
}
nav .auth-buttons .login {
    color: #333;
}
nav .auth-buttons .signup {
    background-color: #FF6B6B;
    color: rgb(215, 30, 30);
    padding: 8px 16px;
    border-radius: 5px;
    border: 2px solid white;
    font-weight: bold;
}
.hero {
    background-color: transparent;
    padding: 50px 20px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    color: rgb(226, 27, 27);
}
.hero-content {
    max-width: 500px;
}
.hero h1 {
    font-size: 2.5rem;
    font-weight: bold;
    margin: 0 0 15px;
}
.hero p {
    font-size: 1.1rem;
    margin-bottom: 20px;
}
.hero .btn-primary {
    background-color: #00C1D4;
    color: white;
    padding: 10px 20px;
    font-size: 1rem;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    text-decoration: none;
}
.hero .btn-primary:hover {
    background-color: #008A9D;
}
.hero-illustration {
    max-width: 300px;
}
.chat-button {
    position: fixed;
    bottom: 20px;
    right: 20px;
    background-color: #00C1D4;
    color: rgb(255, 255, 255);
    padding: 15px;
    border-radius: 50%;
    font-size: 1.2rem;
    border: none;
    cursor: pointer;
}
.card {
    border: none;
    box-shadow: 0 4px 8px rgba(253, 215, 49, 0.897);
}
.card-title {
    font-size: 1.25rem;
    font-weight: bold;
}
.card-text {
    color: #555;
}



