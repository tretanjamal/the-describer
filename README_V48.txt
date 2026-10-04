THE DESCRIBER v48
v48 (dari v47):
- Mode offline: bila YouTube gagal dimuat (tanpa internet / diblokir / lebih dari 10 detik), game otomatis memutar video cadangan assets/video/opening.mp4.
  Video cadangan punya aturan sama: otomatis diputar, tidak bisa digeser maju, wajib selesai sebelum lanjut pilih avatar.
- Taruh file video di assets/video/opening.mp4 (lihat petunjuk kompres di folder itu).
- Opsi ALLOW_CONTINUE_IF_NO_VIDEO (script v43-js, default false): true = bila YouTube dan file lokal sama-sama gagal, pemain boleh lanjut tanpa video.
- Dengan file lokal, game yang dibuka dari file (bukan hosting) juga bisa memutar video.

THE DESCRIBER v47
v47 (dari v46):
- Video pembuka WAJIB ditonton sampai selesai sebelum pilih avatar. Tombol "Lewati" dihapus, tombol lanjut terkunci sampai video habis.
- Video tidak bisa digeser maju (kontrol YouTube dimatikan + penjaga yang mengembalikan posisi bila dilompati). Esc / klik luar tidak menutup video.
- Bila video gagal dimuat, pemain TIDAK bisa lanjut; muncul tombol "Muat Ulang Video".
- Tombol "Video Pengantar" di laman utama dihapus (Profil Pengembang dan Referensi kini berdampingan).

THE DESCRIBER v46
v46 (dari v45):
- Alur baru: isi Nama + Kelas -> MULAI PETUALANGAN -> video pembuka otomatis diputar -> setelah video selesai tombol "Lanjut Pilih Avatar" aktif -> pilih avatar -> prolog.
- Video pembuka tidak lagi muncul otomatis saat game dibuka; hanya muncul setelah klik Mulai Petualangan (tombol "Video Pengantar" di menu tetap bisa dipakai untuk menonton ulang).
- Link video diganti: https://youtu.be/sjIwf3Qz4hQ (atur di INTRO_VIDEO_URL, script id="v43-js").
- Perangkat yang sudah pernah menonton sampai selesai mendapat tombol "Lewati". Matikan dengan ALLOW_SKIP_IF_SEEN=false.
- Bila video gagal dimuat (offline / file lokal), pemain tetap bisa lanjut supaya tidak macet.
- Video YouTube hanya tampil bila game dibuka lewat http/https (hosting), bukan file lokal.

--- Riwayat sebelumnya ---
THE DESCRIBER v45
Struktur: 8 level = 7 pahlawan + 1 level bos (Kabut Si Malas).

v45 (dari v44):
- Teks "petualangan Desa Robatal" di menu Informasi dan Profil Pengembang diganti dengan "The Describer".
- Profil Pengembang: foto pengembang (bingkai bulat emas). Foto dimuat dari ImageKit, butuh internet. Bila gagal dimuat, tampil inisial "J".
  Atur posisi wajah di CSS: .v45-photo { --photo-pos: 50% 15%; } (x y).
- Referensi: sumber materi ditulis sebagai daftar pustaka (Emilia dkk., 2025).

v44: menu Informasi, Profil Pengembang, Referensi. v43: jarak aman bawah, video pengantar (INTRO_VIDEO_URL).
Catatan: video YouTube hanya tampil bila game dibuka lewat http/https (hosting), bukan file lokal.
