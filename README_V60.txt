THE DESCRIBER v60
UPDATE v59 -> v60  (timpa index.html ke folder game; sudah mencakup semua perubahan sebelumnya)

1. Setelah misi selesai dan menekan "Lanjut ke Peta Kasus", pemain kembali ke PETA (tidak lagi langsung masuk narasi misi berikutnya).
2. Narasi misi 8 memakai karakter Kabut Si Malas (boss), bukan Ayu berkabut.
3. Setiap narasi misi menampilkan avatar detektif pilihan pemain di samping tokoh misi; layar "Identitas Dipulihkan" juga menampilkan avatar di samping tokoh.
4. Nama detektif: Raka->Beni, Dimas->Fian, Bima->Abian, Sari->Risa, Nadia->Veli, Laras->Adel.
5. Nama saksi: Pak Joko->Pak Zahrawi, Bu Aminah->Bu Fatim, Pak Budi->Pak Wahyudi, Bu Sari->Bu Maisunah, Bu Ratna->Bu Nur, Pak Slamet->Pak Nurhasan, Bu Lestari->Bu Rahma.
6. Narasi tiap misi hanya menampilkan DUA karakter: avatar detektif pilihan pemain + tokoh hero berkabut misi itu. Misi 8: avatar detektif + Kabut Si Malas (boss).
7. Ukuran avatar detektif dan tokoh berkabut/boss di narasi disamakan (tinggi sama, sejajar di bawah).

THE DESCRIBER v59
UPDATE v58 -> v59  (timpa index.html ke folder game; sudah mencakup semua perubahan v55-v58)

1. Misi 4: zoom kini TAJAM. Zoom tidak lagi memperbesar bitmap (transform scale), tetapi
   memperbesar ukuran area & gambar langsung sehingga detail ciri orang terlihat jelas.
   Kegelapan area di luar senter dipertegas (hampir gelap total) agar pemain wajib memakai senter untuk menemukan Aisyah.
2. Misi 6: hanya memakai worker_s2_A s/d worker_s2_D (jawaban benar = worker_s2_A,
   posisinya diacak, label Relawan A-D). Gambar worker_A..D lama tidak dipakai lagi.
3. Panel pojok kiri bawah: tombol "Teks besar" dihapus; tersisa "Kontras tinggi".
4. Teks pada menu Informasi disesuaikan (tombol Aa kini hanya untuk kontras tinggi).
5. Teks petunjuk salah-jawab di misi 8 tidak lagi menyebut "Kaka Robi" (diganti "Detektif"/"Catatan Detektif").

THE DESCRIBER v58
v58 (dari v57): blok <style id="v58-css"> dan <script id="v58-js"> di akhir index.html, plus dua perbaikan kecil di blok v56/v57.
- Perbaikan terpotong di bawah (misi 8 dan seluruh permainan):
  * Penyebab utama: kelas "boss" pada logo kebiasaan di header (v57) bentrok dengan aturan CSS bos lama (.boss{height:96px!important}), sehingga header misi 8 membengkak dari 65 px menjadi 116 px dan mendorong isi ke bawah. Kelas itu dihapus.
  * Tata letak level bos dipadatkan (banner, gambar bos, deretan hero, gambar tersangka, soal) agar muat di ruang yang tersedia tanpa diperkecil.
  * Pengaman otomatis di semua misi: bila isi layar permainan lebih tinggi dari ruangnya (mis. teks diperbesar, font terlambat dimuat), isi diperkecil otomatis (minimum 62%) sehingga tidak ada yang terpotong, dan kembali normal bila ruang cukup. Fungsi manual: window.v58fit().
- Perbaikan zoom misi 4: titik di bawah kursor kini tetap saat zoom dengan roda mouse atau geser, juga saat game diskalakan di layar besar.

THE DESCRIBER v57
v57 (dari v56): blok <style id="v57-css"> dan <script id="v57-js"> di akhir index.html, plus perubahan kecil.
- Pemilihan detektif: julukan di bawah nama (Si Mata Elang, Pemburu Petunjuk, Penjaga Cerdas, Ratu Detail, Penyelidik Cilik, Pemecah Teka-teki), menggantikan "Jaket ...".
- Header layar permainan: logo kebiasaan misi (misi 8 tanpa logo).
- Setelah misi selesai: (1) hero bebas kabut, (2) Kartu Pahlawan bingkai emas ditampilkan penuh, (3) gambar galeri yang didapat (latar misi) ditampilkan penuh, (4) baru modal Identitas Dipulihkan. Ketuk untuk melewati. Misi bos: ketujuh hero, tujuh kartu, lalu gambar galeri bos.
- Lanjutkan ke Peta Kasus: musik tema/peta tidak lagi terdengar sekilas sebelum briefing misi berikutnya.
- Misi 7: rintangan disebar (atas, tengah, bawah): konsol (kolom 3, baris 2), TV (6,2), camilan (1,3), HP (5,3), tablet (4,5). Rute jawaban tetap.
- Filter sementara tile misi 7 dihapus; sekarang memakai gambar tile_floor_2.webp dan tile_wall_2.webp apa adanya.

THE DESCRIBER v56
v56 (dari v55): blok <style id="v56-css"> dan <script id="v56-js"> di akhir index.html, plus beberapa perbaikan kecil.
- Logo kebiasaan di briefing misi dikecilkan (20 px, sebelumnya tampil 235 px).
- Setelah tiap misi selesai, muncul layar tokoh bebas kabut ("Kabut sirna!") sebelum modal Identitas Dipulihkan (ketuk atau otomatis 3,6 detik).
- Misi 4: tombol zoom (+, -, reset), roda mouse, dan seret untuk menggeser. Maksimal 3x.
- Misi 7: ditambah 3 petak rintangan di jalan buntu (konsol, tablet, camilan) selain HP dan TV. Rute jawaban tidak berubah.
- Misi 7: jalan dibuat lebih terang-hangat dan dinding lebih gelap lewat filter (sementara). Ganti tile_floor_2.webp dan tile_wall_2.webp dengan gambar baru lalu hapus aturan filter di v56-css bila tidak perlu.
- Sertifikat: tombol "SERTIFIKAT SAYA" di layar ending (narasi ending tetap). Unduh PNG atau cetak. Memakai certificate_template.webp.
- Bos: penggantian gambar fase 2 dihapus karena membuat bos tampak idle. Kini ronde 6 dst. bos worried, dan setiap kena serangan benar bos worried 1,5 detik. boss_kabut_malas_phase2.webp tidak dipakai lagi.

THE DESCRIBER v55
v55 (dari v54/v53): pemasangan aset gambar baru (blok <script id="v55-images-js"> + <style id="v55-css"> di akhir index.html).
- Briefing level: tokoh tampil versi terkena kabut (char_*_fogged) + ikon kebiasaan (icon_habit_*).
- Modal menang: tokoh versi pulih (char_*_restored); bintang pakai star_full/star_empty; medali bronze/silver/gold sesuai jumlah bintang.
- Koleksi Pahlawan: kartu terkunci = siluet_*, kartu terbuka = tokoh pulih.
- Peta: lapisan kabut menipis (fog_map_dense -> mid -> light) mengikuti progres; pulau bos memakai icon_island_boss_*.
- Level 4, 6, 8 (dan ronde pilih Ayu di bos): set pengecoh diacak antara set asli dan set s2 (npc_pasar_s2_*, worker_s2_*, suspect_s2_*). Jawaban benar ikut dipetakan otomatis.
- Level 7 (labirin): tema malam (tile_*_2), sprite Intan berjalan (sprite_intan_walk), kotak "?" memakai ikon TV/konsol/tablet/camilan.
- Bos: fase 2 (boss_kabut_malas_phase2) mulai ronde 6, efek kena (fx_hit_sheet), tameng + mantra saat salah (boss_shield, boss_spell), ledakan kabut saat kalah (fx_fog_burst_sheet).
- Tombol Grammar Clue memakai icon_hint. Favicon/og:image (icon_512, og_image) dan poster video pembuka (opening_poster).
- Aset gambar baru dikecilkan (gambar 21 MB -> 13 MB). tile_floor_2 dan tile_wall_2 diperbaiki (aslinya berlubang akibat hapus latar).
- Pengaturan: objek CFG di awal script v55 (VARIASI_SET, OBSTACLES) untuk mematikan acak set atau ikon rintangan.
- Belum dipasang (aset belum ada / belum ada fiturnya): galang_height_* dan galang_posture_*, certificate_template (belum ada fitur sertifikat).

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
