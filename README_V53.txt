THE DESCRIBER v53
v53 (dari v52):
- Splash screen: logo di tengah layar gelap (~2,3 detik, bisa diklik untuk lanjut), lalu masuk laman utama. Atur durasi di script id="v53-splash-js" (SHOW).
- Musik laman utama (bgm_main_theme) diputar setelah splash. Bila browser memblokir autoplay, musik mulai pada klik/sentuhan pertama. Tombol suara kecil ditambahkan di pojok kanan atas laman utama.
- playBGM tidak lagi mengulang lagu bila lagu yang sama sedang diputar (musik berlanjut mulus ke prolog).
- Panduan_Penggunaan_The_Describer_v53.pdf (8 halaman) diperbarui: CP baru, splash dan musik beranda, suara pemandu Inggris+Indonesia, tangkapan layar baru, serta bagian Referensi dan keterangan AI.
- Profil Pengembang: tombol "Kirim Surel" (mailto) dihapus; alamat surel tetap tampil sebagai teks.
- Referensi: ditambah keterangan suara narasi (clue, vocab, guide) dibuat dengan Microsoft Edge TTS (edge-tts).

THE DESCRIBER v52
v52 (dari v51):
- CP Fase D di menu Informasi diganti: 3 elemen (Menyimak-Berbicara, Membaca-Memirsa, Menulis-Mempresentasikan) versi ringkas, sumber Panduan Mapel Bahasa Inggris BSKAP Kemendikdasmen 2025.
- Suara pemandu (menang/kalah/salah/bos) kini Inggris lalu Indonesia. Atur window.VOICE_GUIDE_LANG = 'en' | 'id' | 'both' (default 'both').
- Teks di bawah logo diganti slogan "DESCRIBE IT • SPOT IT • SOLVE IT!".
- Karakter di beranda diturunkan 34px agar kaki sejajar dasar panel registrasi.

THE DESCRIBER v51
v51 (dari v50):
- Tujuan Pembelajaran di menu Informasi diringkas menjadi 1 kalimat.
- Ditambahkan Panduan_Penggunaan_The_Describer_v51.pdf (user guide, 8 halaman) di root ZIP.

v50 (dari v49): pemasangan audio baru (blok <script id="v51-audio"> di akhir index.html).
- Musik: peta = bgm_map, level bos = bgm_boss, layar akhir = bgm_ending.
- Tombol dengar petunjuk: voice_clue_L1..L8 (klik 1x normal, klik lagi dalam 8 detik = pelan). Cadangan: suara browser.
- Klik chip kosakata = voice_vocab_<kata>.mp3 (bila tidak ada file, pakai suara browser).
- Efek bos: sfx_boss_hit (bos kena), sfx_boss_spell (jawaban salah di bos).
- Suara pemandu (voice_guide_*_id) saat modal menang / nyawa habis / salah.
- Menu Informasi: ditambah kotak Capaian Pembelajaran (CP) dan TP.
- Foto pengembang kini lokal: assets/images/foto_pengembang.webp (tidak lagi memakai URL ImageKit).
- Belum dipakai: amb_* (hanya 1-2 detik, sangat pelan), sfx lain (star, level_unlock, dll).

THE DESCRIBER v49
v49 (dari v48):
- Semua kode YouTube dihapus. Video pembuka kini hanya dari file lokal assets/video/opening.mp4 (bisa dimainkan offline).
- Aturan tetap: diputar otomatis setelah klik Mulai Petualangan, tidak bisa digeser maju, wajib selesai sebelum pilih avatar.
- Bila file video tidak ada / gagal dimuat, pemain terkunci dengan tombol "Muat Ulang Video" (atau set ALLOW_CONTINUE_IF_NO_VIDEO=true).
- PENTING: file assets/video/opening.mp4 harus diisi sebelum game dipublikasikan.

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
