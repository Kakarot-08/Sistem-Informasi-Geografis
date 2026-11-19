Peta Interaktif Medan dan Latihan SDG 9 / SDG 11

Ini adalah tugas Pengembangan SIG Web yang saya buat dengan Leaflet. Halamannya menggabungkan peta interaktif, soal essay, papan Kanban, dan kuis, dengan tema SDG 9 (Industri, Inovasi, dan Infrastruktur) dan SDG 11 (Kota dan Permukiman Berkelanjutan).

- Isi halaman
  - Lab peta
    - Tiga basemap yang bisa dipilih: OpenStreetMap, CARTO Dark, dan Esri Satellite.
    - Empat lokasi di sekitar Medan lengkap dengan popup dan tooltip.
    - Layer control di pojok kanan atas untuk menyalakan atau mematikan layer.
    - Alat bantu: tambah titik, ukur jarak, ukur luas, dan lokasi saya.
  - Essay SDG
    - Sembilan soal dari level mudah, menengah, dan sukar.
    - Setiap soal punya penghitung karakter, tombol simpan, dan penilaian diri dengan bintang.
    - Ada dashboard ringkasan jumlah soal terjawab dan rata-rata panjang jawaban.
  - Kanban proyek
    - Sembilan kartu tugas yang bisa dipindah antara To-Do, In Progress, dan Done.
    - Persentase kemajuan ditampilkan juga per SDG.
  - Kuis cepat
    - Lima soal pilihan ganda tentang dasar SIG Web, lengkap dengan skor dan penjelasan.
  - Tampilan
    - Bisa diakses dari laptop maupun HP.
    - Tersedia tema terang dan gelap.

- Teknologi yang dipakai
  - HTML, CSS, dan JavaScript biasa dalam satu file, tanpa framework.
  - Leaflet 1.9.4 yang dimuat dari CDN.
  - Tile peta dari OpenStreetMap, CARTO, dan Esri.

- Isi folder
  - index.html: seluruh halaman dan kodenya.
  - README.md: dokumentasi ini.

- Menjalankan di komputer sendiri
  - Pasang ekstensi Live Server di VS Code.
  - Klik kanan index.html, lalu pilih Open with Live Server.
  - Atau jalankan server sederhana dari folder proyek dengan perintah: python -m http.server 5500
  - Buka alamat http://localhost:5500 di browser.
  - Pastikan perangkat terhubung ke internet agar Leaflet dan tile peta bisa dimuat.

- Panduan memakai lab peta
  - Tombol Tambah Titik: klik di peta untuk menaruh marker baru beserta koordinatnya.
  - Tombol Ukur Jarak: klik beberapa titik berurutan, total jarak muncul di garis.
  - Tombol Ukur Luas: klik minimal tiga titik, luas area muncul di tengah poligon.
  - Tombol Lokasi Saya: izinkan akses lokasi di browser, lalu peta pindah ke posisi kamu.
  - Tombol Ganti Basemap: berpindah antar tiga tampilan peta.
  - Tombol Bersihkan: menghapus semua titik dan hasil ukur buatan sendiri.

- Soal data tersimpan
  - Jawaban essay, bintang penilaian diri, progres Kanban, dan pilihan tema disimpan di localStorage browser.
  - Data hanya ada di browser dan perangkat yang dipakai, tidak dikirim ke server mana pun.
  - Kalau data browser dihapus atau pindah perangkat, data tersebut tidak ikut terbawa.

- Cara publikasi lewat GitHub Pages
  - Buat repository baru di GitHub dengan visibilitas Public.
  - Unggah index.html dan README.md ke repository itu.
  - Masuk ke menu Settings, lalu buka bagian Pages.
  - Di Build and deployment, pilih Deploy from a branch.
  - Pilih branch main dengan folder root, lalu klik Save.
  - Tunggu satu sampai tiga menit sampai alamat situs muncul di bagian atas halaman Pages.
  - Setiap kali index.html diperbarui dan diunggah ulang, situs ikut diperbarui otomatis.

- Kaitan dengan rubrik penilaian
  - Peta tampil dan stabil: ada kontrol zoom, tiga basemap, dan atribusi di pojok peta.
  - Data spasial terikat: lokasi ditulis sebagai koordinat dan ditampilkan sebagai marker berpopup.
  - Interaktivitas: layer control, tambah titik, ukur jarak, ukur luas, dan geolocation.
  - Desain dan aksesibilitas: tampilan responsif, kontras warna yang jelas, dan tombol dengan label teks.
  - Dokumentasi dan publikasi: README ini dan demo online di GitHub Pages.

- Sumber dan atribusi
  - Data peta oleh kontributor OpenStreetMap.
  - Basemap gelap oleh CARTO, citra satelit oleh Esri.
  - Pustaka peta: Leaflet.
  - Soal dan materi: Dr. Syahriol Sitorus, M.IT.

