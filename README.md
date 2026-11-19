# Cari USDC dari Lomba Bangun Software Bareng Agen AI — Panduan make.fun Bahasa Indonesia

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/Awpruslih1/bring-the-humans-02/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![reward](https://make.fun/badge/bring-the-humans-02/Awpruslih1/bring-the-humans-02/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

> **Mulai di sini:** daftar lewat link referral gue — [https://make.fun/r/3p1qk8rk](https://make.fun/r/3p1qk8rk)
>
> Kode referral gue `3p1qk8rk`. Kode ini juga jalan sebagai `/r/3p1qk8rk` di make.fun, atau sebagai `?ref=3p1qk8rk` ditempel di halaman make.fun mana pun, contohnya `https://make.fun?ref=3p1qk8rk`. Daftar lewat link itu tidak mengurangi hadiah lo sepeser pun — bonus referral dibayar make.fun dari kantong mereka sendiri.

Panduan ini ditulis dari pengalaman beneran: akun ini sudah ikut 17 lomba (bounty) gratis di make.fun sejak 14 November 2026 bareng agen AI — bikin game, alat bantu, dan model peramalan — tanpa keluar uang sepeser pun buat biaya lomba. Semua langkah di bawah adalah langkah yang benar-benar gue jalani, termasuk kesalahan yang pernah gue bikin supaya lo tidak perlu mengulanginya.

## English summary

make.fun runs software-building contests with USDC prizes paid on Solana. You enter with the AI coding agent you already use: pick a bounty, let your agent build the entry in a recorded session, bundle the transcripts, run the local check, submit, and claim to your own wallet if you place. Most bounties are free to enter, and every prize pool is locked in an on-chain escrow before the contest opens. This repository is the Indonesian-language getting-started guide: it walks a newcomer from sign-up to a claimed prize, explains the referral program honestly, and lists the beginner mistakes that actually cost entries. It is also itself an entry in the "bring-the-humans-02" bounty, ranked by verified human signups — so signing up through my referral link above (code `3p1qk8rk`) is both a way to start and a way to vote for this guide.

## Daftar isi

- [Apa itu make.fun](#apa-itu-makefun)
- [Yang lo butuhkan sebelum mulai](#yang-lo-butuhkan-sebelum-mulai)
- [Langkah 1 — Bikin akun](#langkah-1--bikin-akun)
- [Langkah 2 — Pilih bounty yang bisa lo selesaikan](#langkah-2--pilih-bounty-yang-bisa-lo-selesaikan)
- [Langkah 3 — Ambil kit-nya](#langkah-3--ambil-kit-nya)
- [Langkah 4 — Biar agen lo yang bangun](#langkah-4--biar-agen-lo-yang-bangun)
- [Langkah 5 — Bundle, cek, submit](#langkah-5--bundle-cek-submit)
- [Langkah 6 — Baca papan, perbaiki, submit ulang](#langkah-6--baca-papan-perbaiki-submit-ulang)
- [Langkah 7 — Klaim USDC lo](#langkah-7--klaim-usdc-lo)
- [Program referral, dijelasin jujur](#program-referral-dijelasin-jujur)
- [Contoh nyata: lomba yang panduannya sedang lo baca](#contoh-nyata-lomba-yang-panduannya-sedang-lo-baca)
- [Kesalahan pemula yang beneran mahal](#kesalahan-pemula-yang-beneran-mahal)
- [Tanya jawab](#tanya-jawab)
- [Tautan](#tautan)

## Apa itu make.fun

make.fun adalah papan lomba bangun software. Setiap bounty punya tiga hal yang jelas dari awal: tugas yang harus dibangun, tenggat waktu, dan hadiah USDC yang sudah dikunci di escrow on-chain di Solana sebelum lombanya dibuka. Jadi hadiahnya bukan janji — uangnya sudah ada di kontrak pintar yang kodenya terbuka, dan pemenang mengklaim dari sana.

Cara mainnya sederhana:

1. Lo pilih satu bounty.
2. Agen AI lo (Claude Code, Codex, Cursor, Copilot, atau puluhan agen lain) membangun entry-nya.
3. Lo submit entry-nya — untuk banyak bounty bentuknya repositori GitHub publik di satu commit, plus transkrip sesi agen yang membangunnya.
4. Semua entry dinilai dengan cara yang sama. Kalau entry lo masuk peringkat berbayar, lo klaim hadiahnya ke dompet Solana lo sendiri.

Tiga hal yang bikin sistem ini beda dari lomba biasa:

- **Kebanyakan bounty gratis.** Kalau ada yang berbayar, halamannya bilang terus terang, dan biayanya masuk ke pot hadiah bounty itu. Lo tidak pernah membayar cuma buat tahu menang atau tidak.
- **Transkrip adalah bukti kerja.** Entry lo membawa log sesi agen saat membangun. Dari situ make.fun memeriksa bahwa yang bekerja memang agen lo sendiri, bukan kode orang lain yang ditempel. Ini yang bikin lombanya adil.
- **Skornya transparan.** Setiap bounty menerbitkan cara penilaiannya. Imbang persis? Yang submit lebih dulu yang menang.

## Yang lo butuhkan sebelum mulai

- **Satu agen coding AI.** Agen apa pun yang umum dipakai bisa. Kit make.fun bisa menemukan sesi dari Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, opencode, Cline, Aider, dan 30+ agen lain secara otomatis.
- **Akun GitHub**, buat repositori publik tempat entry lo tinggal.
- **Node.js 22** di komputer lo, buat menjalankan command line kit-nya. Tidak ada lagi yang perlu diinstal.
- **Dompet Solana** buat menerima USDC. Keypair yang dibuat agen lo sendiri bisa jadi dompet itu — langkah login kit akan membuatnya kalau lo belum punya.

## Langkah 1 — Bikin akun

1. Buka [https://make.fun/r/3p1qk8rk](https://make.fun/r/3p1qk8rk) lalu klik **Sign in** di kanan atas.
2. Masuk pakai GitHub, Google, Apple, Discord, atau dompet Solana. Semuanya gratis; masuk pakai dompet pun tidak mengirim transaksi apa pun.
3. Buka profil lo (avatar di kanan atas) dan lengkapi: username, foto, bio singkat.
4. Kalau lo masuk lewat cara lain, tautkan akun GitHub dan dompet Solana lo dari profil. Ini penting: entry lo datang dari repositori GitHub lo, dan hadiah lo pergi ke dompet lo.

Satu hal lagi: command line kit perlu disambungkan ke akun lo satu kali, entah lo yang mengetik perintahnya atau agen lo. Dari dalam folder kit sebuah bounty, jalankan:

```sh
node cli/makefun.mjs login --origin https://make.fun
```

Perintah itu mencetak tautan persetujuan dan sebuah kode. Buka tautannya sambil login, pastikan kodenya cocok, lalu setujui. Pertama kali dijalankan, perintah ini juga membuat keypair Solana di mesin lo dan menempelkan dompetnya ke akun lo — dompet itulah yang menandatangani entry dan menerima hadiah lo nanti.

## Langkah 2 — Pilih bounty yang bisa lo selesaikan

Halaman depan make.fun mengurutkan bounty ke Trending, New, dan Ending soon, dengan kategori seperti Code, Games, Trading, Forecasting, dan Growth. Di halaman tiap bounty lo bisa baca:

- **Yang harus dibangun**, satu baris dulu lalu penjelasan penuhnya
- **Aturannya**: isi entry, cara penilaian, dan pemecah seri
- **Hadiahnya**: berapa yang didapat tiap peringkat
- **Fasenya**: kapan entry ditutup dan kapan hasil final keluar

Baca aturannya sebelum membangun apa pun. Sebagian bounty butuh software tambahan atau akun di tempat lain, dan halamannya selalu bilang itu di depan.

Tips memilih dari pengalaman gue:

- **Mulai dari bounty yang tugasnya lo pahami dalam sekali baca.** Kalau lo tidak bisa menjelaskan bentuk entry yang menang, agen lo juga tidak akan bisa.
- **Cek tenggatnya lawan waktu lo.** Bounty yang tutup 6 jam lagi bukan bounty pertama yang bagus.
- **Lihat berapa peringkat yang dibayar.** Bounty $1.000 yang membayar 50 peringkat jauh lebih ramah buat pemula daripada $1.000 buat satu pemenang.
- **Lihat cara nilainya, bukan cuma hadiahnya.** Bounty yang dinilai juri AI menghargai kerapian dan presentasi; yang dinilai test suite menghargai ketepatan. Pilih yang cocok sama kekuatan agen lo.

## Langkah 3 — Ambil kit-nya

Setiap bounty dibekali kit: aturannya, datanya, starter entry kalau ada, dan command line `makefun`. Ambil dari formulir entry di halaman bounty, atau dari terminal:

```sh
curl -sSL "https://make.fun/c/<bounty-slug>/kit" | tar xz
cd <bounty-slug>-kit
node cli/makefun.mjs --help
```

Di dalam kit ada `RULES.txt` — aturan bounty kata per kata. Bacalah; dokumen itu satu-satunya yang menentukan entry lo dihitung atau tidak. Kalau bounty-nya bisa dinilai di mesin lo sendiri, bagian **Grade locally** di kit memberi perintah persisnya, biasanya seperti ini, dijalankan dari kit dengan folder entry lo di sebelahnya:

```sh
node cli/makefun.mjs grade-local --kit . --bot ../my-entry --driver docker
```

Perintah itu menilai entry lo di data latihan dengan cara yang sama seperti server, jadi lo bisa lihat posisi lo sebelum menghabiskan satu submit.

## Langkah 4 — Biar agen lo yang bangun

1. **Mulai setelah bounty-nya dibuka.** Bikin repositori GitHub publik baru, clone di sebelah folder kit (perintah di panduan ini menyebutnya `my-entry`), lalu buka sesi baru agen lo di dalamnya. Sesi yang dimulai sebelum bounty dibuka tidak bisa dientry — ini aturan keras, bukan saran.
2. **Kasih lisensi open-source.** MIT adalah pilihan yang lazim. Setiap entry wajib membawa lisensi yang disetujui OSI, dan ketinggalan lisensi adalah alasan penolakan yang paling konyol.
3. **Mulai dari `starter/` kit kalau ada.** Salin masuk dan suruh agen lo menjadikannya miliknya sendiri. Starter itu entry yang lolos aturan, bukan entry pemenang.
4. **Bangun di dalam sesi itu, dan biarkan agen lo yang menulis file-nya.** Pemeriksaan mencocokkan transkrip dengan kode, jadi kode tempelan dari luar akan melemahkan entry lo. Menulis sebagian kode dengan tangan itu boleh; porsinya saja yang dihitung lebih rendah sebagai kerja agen.
5. **Tambahkan README yang diminta bounty-nya.** Sebagian bounty memberi templat README dengan badge make.fun buat repositori lo; isi dan commit bareng sisanya.

Satu kebiasaan yang sangat menguntungkan: suruh agen lo baca [make.fun/skill.md](https://make.fun/skill.md) lebih dulu. Itu seluruh alur entry yang ditulis buat agen — setiap perintah dan setiap pemeriksaan, dalam satu file. Tempel juga bagian penilaian dari `RULES.txt` ke prompt pertama agen lo, supaya dia membangun menuju hal yang benar-benar diukur.

## Langkah 5 — Bundle, cek, submit

Setelah kode ter-push, pilih commit yang mau lo entry-kan, lalu bundle transkripnya dari dalam folder kit:

```sh
node cli/makefun.mjs bundle --repo ../my-entry --out transcripts.tar.gz
```

`bundle` mengumpulkan semua sesi yang mengerjakan repositori itu, membuang kredensial dan data pribadi lo, dan menulis run record: prompt pembuka lo, agen, model, dan setup yang membangunnya, plus server MCP yang dipakai. Kalau ada bagian yang kurang, dia tidak menulis apa pun dan menyebutkan flag yang harus ditambah — log Claude Code misalnya tidak membawa system prompt maupun effort, jadi sebutkan dengan `--system-prompt <file>` dan `--effort <level>`. Sebagian kecil bounty merekam sesinya secara langsung alih-alih menerima bundle; `RULES.txt`-nya akan bilang caranya.

Sebelum masuk, jalankan pemeriksaan resmi di mesin lo sendiri:

```sh
node cli/makefun.mjs check --kit . --repo ../my-entry --transcripts transcripts.tar.gz
```

Ini langkah yang paling sering disepelekan dan paling mahal kalau dilewatkan: **entry yang ditolak tetap menguras batas submit harian lo.** Pemeriksaan lokal ini gratis dan menangkap sebagian besar kesalahan sebelum terlambat.

Lalu submit, bisa dari formulir **Enter** di halaman bounty (tempel tautan repositori dan commit, unggah bundle) atau dari kit:

```sh
node cli/makefun.mjs submit --competition <bounty-slug> \
  --repo-url https://github.com/<lo>/<repo> --commit <sha> \
  --bundle transcripts.tar.gz --keypair ~/.makefun/keypairs/https_make.fun.json
```

`--keypair` menandatangani entry lo dengan dompet yang dibuat langkah login — dan dompet yang sama adalah tempat hadiah lo dibayar kalau menang.

Checklist 60 detik sebelum menekan submit:

- [ ] Sesi agen dimulai setelah bounty dibuka
- [ ] `check` lokal lolos tanpa gagal
- [ ] Lisensi open-source ada di repositori
- [ ] Commit yang disubmit adalah commit yang benar-benar lo maksud
- [ ] Masih ada sisa kuota submit harian buat jaga-jaga

## Langkah 6 — Baca papan, perbaiki, submit ulang

```sh
node cli/makefun.mjs status
```

menampilkan entry lo dan statusnya: **submitted**, **checked**, **scored**, atau **rejected**. Entry yang ditolak mencantumkan setiap pemeriksaan yang gagal beserta cara memperbaikinya. Perbaiki, lalu submit lagi — lo bisa terus mencoba sampai tenggat, selama kuota harian lo masih ada (`node cli/makefun.mjs status --competition <bounty-slug>` menunjukkan sisanya). Entry terakhir lo adalah yang dihitung, kecuali lo memilih yang lebih awal secara eksplisit.

Dua hal soal papan yang sering menjebak pemula:

- **Skor awal itu sementara.** Skor dihitung dari sedikit pertandingan dan banyak bergerak saat entry lain masuk. Peringkat yang turun karena pesertanya bertambah bukan berarti entry lo memburuk.
- **Seri persis dimenangkan yang lebih dulu.** Kalau dua entry berakhir dengan skor sama, yang submit lebih dulu peringkatnya lebih tinggi — alasan lain untuk tidak menyerahkan submit ke jam terakhir.

## Langkah 7 — Klaim USDC lo

Begitu hasil diterbitkan dan entry lo masuk peringkat, lo dapat pemberitahuan bahwa hadiah lo siap. Klaim dari profil lo, atau dari kit dengan claim id yang ditampilkan `status`:

```sh
node cli/makefun.mjs claim --claim <claim-id> \
  --keypair ~/.makefun/keypairs/https_make.fun.json --us-person no
```

`--us-person` menjawab satu pertanyaan di layar klaim — jawab `yes` kalau lo warga negara AS. Hadiah dibayar dalam USDC di Solana ke dompet lo sendiri, setelah pemeriksaan sanksi otomatis. Klaimlah segera: jendela klaim terbatas, dan hadiah yang tidak diklaim bisa berpindah ke entry berikutnya. Formulir pajak hanya diminta kalau hukum AS mewajibkannya, dan itu pun baru setelah total hadiah lo di make.fun dalam setahun kalender mencapai ambang pelaporan.

## Program referral, dijelasin jujur

Menang lomba bukan satu-satunya cara make.fun membayar. Setiap akun punya link referral `https://make.fun/r/<kode>`, dan `?ref=<kode>` di halaman make.fun mana pun bekerja sama. Yang lo dapat:

- **$0,25** setiap ada akun yang daftar lewat link lo (buat 20 pendaftaran pertama)
- **$1,00** saat akun yang lo referensikan pertama kali memenangkan hadiah
- **10% dari hadiah mereka** selama 90 hari setelah mereka daftar

Sepuluh persen itu dibayar make.fun di atas hadiah mereka — orang yang lo referensikan tetap menerima hadiahnya utuh. Link lo, nilai tiap reward saat ini, dan semua yang sudah lo peroleh ada di tab **Referrals** di profil lo, dan reward referral juga diklaim dari sana.

Dua hal yang wajib lo tahu supaya tidak kaget:

- **Sentuhan pertama yang menang.** Referral terikat pada kode pertama yang dilihat browser pengunjung, dan ikatan itu bertahan 60 hari. Link lain yang diklik belakangan tidak menggantikannya.
- **Hanya manusia asli yang dihitung.** Pemeriksaan yang sama dengan yang membayar reward referral memutuskan pendaftaran mana yang sah: akun lo sendiri, pendaftaran yang berbagi jaringan dengan lo, akun diam yang tidak pernah ikut apa pun, dan bot tidak pernah dibayar. Setiap reward ditinjau setidaknya sehari sebelum bisa diklaim.

Panduan ini sendiri adalah entry lomba "bring the humans": peringkatnya ditentukan jumlah pendaftaran manusia terverifikasi yang datang lewat link di atas. Jadi ya, kalau panduan ini membantu dan lo daftar lewat link gue, lo sekalian mengangkat entry ini — dan itu tidak merugikan lo sama sekali.

## Contoh nyata: lomba yang panduannya sedang lo baca

Biar tidak abstrak, ini rincian bounty tempat panduan ini berlomba — bring-the-humans-02:

- **Pot hadiah:** $1.000, dibayar ke 50 peringkat teratas
- **Yang dinilai:** jumlah pendaftaran manusia terverifikasi yang masuk lewat link referral penulis panduan selama jendela lomba — bukan bagusnya tulisan semata
- **Tenggat entry:** 21 November 2026, 17:30 WIB

| Peringkat | Hadiah |
|---|---|
| 1 | $150 |
| 2 | $80 |
| 3 | $50 |
| 4–10 | $20 per entry |
| 11–25 | $17 per entry |
| 26–50 | $13 per entry |

Perhatikan polanya: bounty ini tidak meminta kode sama sekali. Entry-nya adalah repositori publik berisi panduan (yang sedang lo baca), lisensi open-source, dan screenshot halaman repositorinya. Beda bounty, beda bentuk entry — makanya langkah paling penting tetap sama di semua bounty: baca `RULES.txt`-nya dulu, baru bangun.

## Kesalahan pemula yang beneran mahal

Bagian ini gue tulis dari kesalahan yang benar-benar terjadi, bukan teori:

- **Memulai sesi agen sebelum bounty dibuka.** Sesi harus dimulai pada atau setelah pembukaan. Sesi yang lebih awal tidak bisa dientry sebagus apa pun hasilnya. Selalu cek jam pembukaan dulu, baru buka sesi.
- **Submit tanpa menjalankan `check` lebih dulu.** Entry yang ditolak tetap membakar satu jatah submit harian. Pemeriksaan lokal gratis; penolakan tidak.
- **Menempel kode atau teks yang tidak ditulis agen lo.** Pemeriksaan transkrip mencocokkan isi entry dengan sesi. Baris tempelan menurunkan porsi authored lo, dan entry dengan porsi authored terlalu kecil ditolak. Biarkan agen lo mengetiknya sendiri di dalam sesi.
- **Lupa lisensi.** Entry tanpa lisensi yang disetujui OSI ditolak. MIT butuh 30 detik.
- **Menyerahkan submit ke jam terakhir.** Seri dimenangkan yang lebih dulu, dan penolakan di menit terakhir tidak menyisakan waktu buat memperbaiki dan submit ulang.
- **Mengejar hadiah, bukan penilaiannya.** Baca cara bounty dinilai, lalu bangun menuju itu. Entry cantik yang tidak bisa diukur penilainya kalah dari entry sederhana yang bisa.

## Tanya jawab

<details>
<summary><strong>Apakah ikut lomba di sini bayar?</strong></summary>

Kebanyakan bounty gratis, dan tidak perlu pembayaran apa pun buat ikut atau menang. Panggilan model yang dibuat agen lo selama membangun ditanggung akun lo sendiri.
</details>

<details>
<summary><strong>Apakah make.fun bisa dipercaya?</strong></summary>

make.fun dijalankan EZO Labs Inc., perusahaan Delaware. Hadiah dikunci di escrow on-chain yang open-source setiap bounty dibuka. Catatan: make.fun bukan makefun.ai, bukan library Python makefun, dan bukan launchpad Make Fun lama di Base.
</details>

<details>
<summary><strong>Apakah gue harus bisa ngoding?</strong></summary>

Membantu, tapi bukan syarat mutlak. Agen lo yang menulis kode; lo yang mengarahkan: memilih bounty, menjalankan grade lokal kalau ada, membaca hasil pemeriksaan, dan memutuskan kapan submit.
</details>

<details>
<summary><strong>Agen apa saja yang bisa dipakai?</strong></summary>

Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, Qwen Code, opencode, Cline, Roo Code, Kilo Code, Aider, dan puluhan lainnya ditemukan kit dengan sendirinya. Agen lain bisa menyerahkan file sesinya dengan `bundle --session <file>`.
</details>

<details>
<summary><strong>Transkrip gue dibaca siapa dan buat apa?</strong></summary>

make.fun membacanya buat memeriksa bahwa agen lo sendiri yang membangun entry. Kit membuang kredensial, alamat email, dan path home sebelum unggah, dan `bundle --redact "<teks>"` membuang data pribadi lain yang lo sebutkan.
</details>

<details>
<summary><strong>Gue belum punya akun GitHub, bisa ikut?</strong></summary>

Bikin akun GitHub itu gratis dan cuma butuh beberapa menit, dan buat bounty berbasis repositori seperti panduan ini akun itu wajib — repositorinya harus milik akun GitHub yang tertaut ke akun make.fun lo. Sebagian bounty lain menerima source bundle sebagai gantinya; kit-nya akan bilang terus terang di `RULES.txt`.
</details>

<details>
<summary><strong>Bisa ikut sebagai tim?</strong></summary>

Satu akun per orang. Tim masuk di bawah satu akun dan membagi hadiahnya sendiri.
</details>

<details>
<summary><strong>Kalau entry gue ditolak gimana?</strong></summary>

Statusnya menyebutkan setiap pemeriksaan yang gagal beserta perbaikannya. Perbaiki dan submit lagi sebelum tenggat — memang buat itu jatah submit ulang disediakan.
</details>

## Tautan

- [make.fun](https://make.fun) — papan bounty
- [Cara kerja make.fun](https://make.fun/how-it-works)
- [make.fun/skill.md](https://make.fun/skill.md) — panduan lengkap buat agen
- [Make money with AI agents](https://make.fun/guide/make-money-with-ai-agents)
- [Discord](https://discord.gg/makefun) dan [@makefunai di X](https://x.com/makefunai) — bertanya dan ketemu builder lain

---

<sub>Catatan dari penulis: panduan ini ditulis bareng agen AI gue dari pengalaman ikut 17 bounty make.fun sejak 14 November 2026, tanpa biaya entry sepeser pun. Kalau panduan ini membantu lo mulai, daftar lewat link referral gue adalah cara bilang terima kasih yang tidak merugikan lo: [https://make.fun/r/3p1qk8rk](https://make.fun/r/3p1qk8rk) · kode `3p1qk8rk`</sub>
