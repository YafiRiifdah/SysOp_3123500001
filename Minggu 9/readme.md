<div align="center">
  <h1 style="text-align: center;font-weight: bold">Praktikum 9<br>Praktek Sistem Operasi</h1>
  <h4 style="text-align: center;">Dosen Pengampu : Dr. Ferry Astika Saputra, S.T., M.Sc.</h4>
</div>
<br />
<div align="center">
  <img src="https://upload.wikimedia.org/wikipedia/id/4/44/Logo_PENS.png" alt="Logo PENS">
  <h3 style="text-align: center;">Disusun Oleh : </h3>
  <p style="text-align: center;">
    <strong>Muhammad Yafi Rifdah Zayyan (3123500001) </strong><br>
    <strong>Muhammad Daffa Erfiansyah (3123500006) </strong><br>
    <strong>Maula Shahihah Nur Sa'adah (3123500008)</strong>
  </p>
<h3 style="text-align: center;line-height: 1.5">Politeknik Elektronika Negeri Surabaya<br>Departemen Teknik Informatika Dan Komputer<br>Program Studi Teknik Informatika<br>2023/2024</h3>
  <hr><hr>
</div>

## Producer-Consumer Semaphore
<img src= "https://github.com/YafiRiifdah/SysOp_3123500001/blob/main/Minggu%209/Image/producer-consumer-semaphore.jpeg">

**Analisa**
Semaphore adalah mekanisme sinkronisasi yang digunakan dalam pemrograman konkuren untuk mengontrol akses ke sumber daya bersama. Dengan dua operasi dasarnya, Wait (P) dan Signal (V), semaphore memungkinkan thread atau proses untuk memblokir atau melanjutkan eksekusi berdasarkan nilai semaphore. Dengan menggunakan semaphore, pengembang dapat mencegah race condition dan deadlock, serta mengkoordinasikan akses ke sumber daya bersama dalam lingkungan multithreading dan multiproses dengan efisien. Namun, perancangan yang cermat diperlukan untuk menghindari masalah deadlock dan mempertahankan kinerja sistem yang optimal.

## Producer-Consumer-Wake-Sleep-Thread
<img src= "https://github.com/YafiRiifdah/SysOp_3123500001/blob/main/Minggu%209/Image/wake-sleep.jpeg">

**Analisa**
Model Producer-Consumer dengan teknik "wake-sleep" pada threading menggambarkan sebuah skenario dimana produsen (producer) dan konsumen (consumer) berinteraksi dengan berbagi sumber daya bersama, seperti buffer. Produsen bertugas memasukkan data ke dalam buffer, sementara konsumen bertugas mengambil data dari buffer. Teknik "wake-sleep" diimplementasikan menggunakan semafor, dimana produsen menunggu hingga buffer kosong untuk menambahkan data, dan konsumen menunggu hingga buffer tidak kosong untuk mengambil data. Ketika sebuah thread memasukkan atau mengambil data dari buffer, ia "membangunkan" thread yang mungkin sedang "tidur" dan memberikan sinyal untuk memproses selanjutnya. Pendekatan ini memastikan sinkronisasi yang tepat antara produsen dan konsumen dalam lingkungan konkuren, menghindari kelebihan atau kekurangan penggunaan sumber daya, serta meminimalkan beban sistem dengan memperbolehkan thread untuk "tidur" ketika tidak ada tugas yang harus dilakukan.

