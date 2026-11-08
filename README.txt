ULAR TANGGA EDUKASI - 4 PEMAIN
================================

ISI FOLDER
- index.html  : halaman utama
- style.css   : tampilan game
- game.js     : aturan permainan, pertanyaan, dan sistem poin

CARA MENJALANKAN
1. Ekstrak file ZIP.
2. Buka index.html di browser untuk mencoba secara lokal.
3. Isi nama pemain (2 sampai 4 pemain), lalu tekan "Mulai / Terapkan Nama".
4. Pemain bermain bergantian di perangkat yang sama.

CARA HOSTING GRATIS (STATIC WEBSITE)
Pilihan Netlify:
1. Buka https://app.netlify.com/drop
2. Ekstrak ZIP ini terlebih dahulu.
3. Seret folder yang berisi index.html, style.css, dan game.js ke halaman Netlify Drop.
4. Tunggu proses selesai. Netlify akan memberikan link website.
5. Bagikan link tersebut. Semua pemain bisa bermain pada satu perangkat yang membuka link itu.

Atau upload ketiga file ke GitHub Pages / hosting static lain.
Tidak membutuhkan database, PHP, Node.js, atau konfigurasi server.

ATURAN DEFAULT
- Benar: +2 poin.
- Salah: mundur acak 2 atau 5 kotak.
- Serangan: 5 poin untuk membuat pemain pilihan mundur 3 kotak.
- Tangga dan ular aktif otomatis.
- Menang jika mencapai atau melewati kotak 100.

MENGUBAH PERTANYAAN
Buka game.js, cari bagian const QUESTIONS.
Format satu pertanyaan:
["Teks pertanyaan", ["Pilihan A","Pilihan B","Pilihan C","Pilihan D"], 0]
Angka terakhir adalah indeks jawaban benar: 0=A, 1=B, 2=C, 3=D.

CATATAN
Game ini adalah multiplayer lokal bergiliran (pass-and-play), bukan multiplayer online real-time antarperangkat.
Setiap perangkat yang membuka link memiliki sesi permainan sendiri.
