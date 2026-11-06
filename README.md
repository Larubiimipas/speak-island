# Speak Island

Game kota pulau 3D dunia terbuka (gaya GTA, ramah anak) untuk latihan berbicara bahasa Inggris tingkat pemula.

- Pilih karakter (Rani, Bima, atau Robo), jalan-jalan, lari, lompat ganda, nyetir mobil, dan main di Taman Lompat serta Menara Parkour.
- 20 misi percakapan sehari-hari: masuk ke lingkaran kuning di depan warga, lalu pilih balasan, tirukan kalimat, dan susun kalimat. Ucapan dinilai otomatis per kata (butuh Google Chrome dan izin mikrofon).
- Dimainkan dalam posisi landscape. Di HP, game otomatis meminta layar penuh mendatar.
- Ilustrasi karakter dan papan iklan dibuat dengan Canva. Model 3D dan animasi berasal dari contoh three.js (Mixamo).

Situs: https://larubiimipas.github.io/speak-island

## Karakter
- Pemain: Ziya dan Hisyam. Potret dibuat dengan Gemini dari foto, model 3D dan animasi dari Mixamo (folder `models/`).
- Warga kota memakai model Mixamo dengan animasi idle, jalan, lari, lompat, bicara, melambai, senang, dan joget.

## Fitur baru
- **Pilih kelas (1–6 SD) di layar depan** — tingkat soal Bahasa Inggris dan PPKn mengikuti kelas:
  - Kelas 1–2: kalimat pendek, 2 pilihan jawaban, arti bahasa Indonesia tampil, lulus ucapan ≥50%.
  - Kelas 3–4: 3 pilihan, arti disembunyikan (bisa dibuka), lulus ≥60%.
  - Kelas 5–6: kalimat lebih panjang, tanpa tombol arti, lulus ≥72%.
- **Motor & sepeda** — dekati lalu tekan **F** (atau tombol Naik) untuk naik/turun.
- **Negeri Pancasila** — ikuti gerbang "Jalan ke Negeri Pancasila", seberangi jembatan ke pulau kedua, dan belajar PPKn bersama 7 guru (soal pilihan ganda: 8 soal untuk kelas 1–2, 10 soal untuk kelas 3–6).
- **Kios mini game** — 3 kios di pulau utama (Bahasa Inggris) dan 3 kios di Negeri Pancasila (PPKn): *Tembak Balon*, *Mancing Kata*, *Pukul Tikus*. Soal mengikuti kelas; jawaban benar menambah uang dan rekor poin tersimpan.
- **Pulau Matematika** — ikuti gerbang biru "Jalan ke Pulau Matematika" (antara Pelabuhan dan Rumah Nenek), seberangi Jembatan Angka. 10 tahap di atas lava: baca soal di papan, lalu lewati jembatan papan dengan jawaban benar. Salah pilih, papan runtuh dan pemain kembali ke checkpoint dengan soal baru. Soal mengikuti kelas (kelas 1: + − sampai 20 … kelas 6: bilangan bulat negatif, pangkat tiga, operasi campuran).
- **Laut & speedboat** — Dermaga Speedboat di barat daya kota (antara Hotel Ombak dan Pelabuhan). Naik dengan F, berlayar keliling laut, turun di pantai mana saja.
- **Pulau IPAS** — pulau gunung di timur laut; jalan tanah melingkar naik ke puncak dengan 8 gerbang soal IPAS (sesuai kelas). Puncak: peti harta.
- **Berenang** — jalan ke laut dari pantai untuk berenang; **Memancing** di ujung dermaga (lempar, tunggu "!", tahan tombol untuk menarik), koleksi 10 jenis tangkapan.
- **Ayunan**, **tiang bendera yang bisa dipanjat** (kota, Negeri Pancasila, puncak IPAS) dengan bendera berkibar, dan **hewan yang bisa dielus** (kucing, anjing, ayam, kambing, sapi).
- Tekstur foto realistis dan gambar ikan dibuat dengan Canva; bank soal IPAS & fakta ikan diperiksa dengan Gemini.
- **Pose realistis**: duduk di bangku ayunan, memeluk tiang saat memanjat, berenang gaya bebas (mengapung tegak saat diam).
- **Menyelam** (tombol Selam/Naik) dengan **bar napas**; dasar laut berisi terumbu karang, kawanan ikan, penyu, ubur-ubur, rumput laut (nama Inggris muncul saat dilihat).
- **Sayap terbang** di lemari PAKAIAN TERBANG (puncak Pulau IPAS): tahan KEPAK untuk naik, ikuti cincin emas ke Negeri Pancasila.
- **Pangkas Rambut** (gaya & warna rambut) dan **Toko Baju** (atasan/bawahan termasuk batik, seragam SD, pramuka, jersey) dibeli dengan uang di kanan atas; **Pasar Ikan** di dermaga membeli tangkapan.
- **Peta dunia** (ketuk radar atau tekan M): bisa digeser & di-zoom, dengan nama pulau dan lokasi.
- **Main Bersama (2 pemain)** — tombol 👥 di kanan atas. Satu pemain *Buat Ruang* (dapat kode 4 angka), temannya *Gabung* dengan kode itu. Koneksi lewat server perantara MQTT publik (HiveMQ, cadangan EMQX) sehingga tembus jaringan seluler; tanpa akun. Saling melihat karakter (baju & rambut ikut), ucapan bahasa Inggris, lambai, joget, tos, dan tombol "Ke teman".
