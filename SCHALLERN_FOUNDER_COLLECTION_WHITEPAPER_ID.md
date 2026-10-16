# Schallern — Whitepaper Founder Collection

**Versi 0.1 · Draf kerja · 16 Oktober 2026 · Culturetek Pte. Ltd., Singapura**

> Flip the World. Satu lemparan. Satu tembok. Milimeter yang menentukan.

## 1. Abstrak

Schallern adalah game lempar koin berfisika nyata yang dimainkan di browser: lempar koin ke tembok, koin yang tepinya berhenti paling dekat ke tembok menang. Game ini adalah versi modern dari permainan halaman sekolah yang dimainkan dengan uang susu di Jerman era 1980-an. Demo gratis yang bisa dimainkan dengan tiga arena dan tiga karakter sudah tersedia di https://schallern.io/play/.

**Founder Collection** adalah seri terencana berisi **10.000 koleksi digital di Solana** (koin dan karakter). Founder Collectibles bersifat kosmetik: mereka mengubah tampilan koin dan avatar pemain, tetapi tidak pernah mengubah fisika, geometri, atau peluang. Mint ini mendanai tahap pengembangan game berikutnya. Whitepaper ini menjelaskan game, koleksi, mekanisme mint, penggunaan dana, peta jalan, dan tim, serta memisahkan apa yang sudah aktif hari ini dari apa yang direncanakan.

## 2. Game

**Aturan.** Satu tembok, satu koin per lemparan, tiga ronde per pertandingan. Setelah tiga ronde, jumlah jarak terkecil menang. Lemparan yang tidak pernah menyentuh tembok, keluar jalur, melewati tembok, atau memantul balik lebih dari 150 cm adalah foul dan dihitung sebagai jarak maksimum yang dipublikasikan.

**Pengukuran.** Jarak diukur dari tepi koin terdekat ke tembok setelah koin berhenti, dikuantisasi ke grid milimeter yang dipublikasikan. Kamera, bayangan, dan visual tidak pernah menentukan pemenang; hasil fisikalah yang menentukan.

**Fisika.** Koin adalah cakram tipis kaku yang disimulasikan pada langkah tetap 240 Hz dengan restitusi yang bergantung pada kecepatan, gesekan gelinding per permukaan (aspal, pasir, marmer), dan material tembok (beton, batu pasir, lak). Setiap pemain dalam satu ronde melempar dengan jarak, permukaan, dan tembok yang sama. Lemparan bersifat deterministik untuk input yang sama.

**Kontrol.** Seret ke bawah untuk tenaga, seret ke samping untuk arah, slider untuk lengkung; mouse dan sentuhan berbagi batas input ternormalisasi yang sama. Pelepasan ditampilkan dalam gerak lambat dengan tangan lima jari dan jentikan jempol.

**Keadilan.** Tidak ada yang bisa dibeli pemain yang mengubah massa, diameter, gesekan, pantulan, atau presisi. Kelangkaan bersifat visual. Ini adalah aturan dasar proyek dan berlaku untuk setiap collectible yang dijelaskan di sini.

## 3. Status hari ini (apa yang aktif, apa yang belum)

| Aktif hari ini | Belum |
|---|---|
| Demo browser gratis di schallern.io/play/, desktop dan ponsel, tanpa dompet | Meja uang asli (hanya setelah lisensi, audit, dan persetujuan, dan hanya di negara yang mengizinkan) |
| Tiga arena (aspal Berlin, pasir Giza, marmer Vegas), tiga karakter (NEO, MAYA, BO), lawan AI lokal | Multiplayer online, turnamen, kru kota |
| Chat masukan dengan reward, Program kreator dengan tautan pelacakan, buletin | Founder Mint di mainnet (alur lengkap telah dilatih di Solana devnet, lihat bagian 6) |
| Server Discord dengan bot Schallern Rewards | Penautan dompet di dalam game |

Poin demo tidak bernilai tunai. Tidak ada NFT, token, atau pembayaran yang dibuat dengan memainkan demo.

## 4. Founder Collection

- **Suplai:** 10.000 collectible, bernomor.
- **Subjek:** koin Schallern (material, finishing, tepi, ukiran, patina) dan karakter bergaya figur milik game sendiri; tema arena opsional dari katalog 48 tembok terkenal.
- **Standar:** Metaplex Core di Solana; setiap collectible adalah satu aset on-chain dalam koleksi terverifikasi dengan informasi royalti on-chain.
- **Kelangkaan:** sistem trait (sekitar 8 hingga 12 kategori trait, 200 hingga 300 varian) memberi setiap karya peringkat kelangkaannya sendiri dari 1 hingga 10.000, ditambah lima tingkat pemasaran dan sejumlah kecil spesial 1/1. Kelangkaan hanya soal prestise.
- **Reveal:** apakah pembeli memilih tingkatnya tanpa reveal acak, atau karya seni diungkap pada hari reveal, adalah keputusan produk yang masih terbuka; ini dipublikasikan sebelum mint dibuka.
- **Hak karya seni:** holder menerima lisensi personal non-eksklusif atas karya seni mereka; merek kata SCHALLERN tetap milik operator. Teks lisensi final dipublikasikan bersama ketentuan mint.

## 5. Apa yang didapat seorang founder, dan apa yang tidak

**Didapat:** collectible sebagai skin lempar di dalam game begitu penautan dompet aktif; lencana Founder dengan nomor collectible di profil pemain; peran Founder dan kanal holder di Discord; hak suara untuk menentukan arena dan desain koin berikutnya; akses awal ke arena baru dalam mode uang mainan.

**Tidak didapat:** saham perusahaan, klaim atas laba, pembagian keuntungan, buy-back, atau kenaikan nilai, maupun keunggulan gameplay apa pun. Founder Collection adalah koleksi, bukan produk investasi. Pendanaan perusahaan apa pun adalah penawaran terpisah dengan struktur tersendiri (lihat bagian 10).

## 6. Mekanisme mint

| Hal | Rencana |
|---|---|
| Chain dan standar | Solana, Metaplex Core, Core Candy Machine dengan Candy Guard |
| Tingkat dan harga | #1–4.000 seharga 0,5 SOL · #4.001–7.000 seharga 1 SOL · #7.001–9.000 seharga 1,5 SOL · #9.001–10.000 seharga 2 SOL (model terencana; ketentuan final dipublikasikan sebelum mulai) |
| Fase | tim dan OG → allowlist (terjamin, dibatasi per dompet) → undian waitlist → publik; tanggal diumumkan hanya di schallern.io dan di kanal pengumuman Discord |
| Batas | batas mint per dompet per fase; pajak bot; setiap transaksi mint dibangun dan ditandatangani bersama oleh backend Schallern setelah captcha dan pemeriksaan laju |
| Di mana | hanya di schallern.io; tim tidak pernah mengirim pesan lebih dulu dan tidak pernah meminta seed phrase |
| Treasury | hasil mint langsung masuk ke treasury multi-tanda tangan (2-dari-3) |
| Royalti | royalti sekunder 5 %, tertulis di dalam koleksi |
| Penyimpanan | karya seni dan metadata di Arweave (permanen) |
| Gladi | alur lengkap (koleksi, empat mesin tingkat dengan grup fase, bukti allowlist, penanda tangan backend, uji bot dan beban, unggahan Arweave, pembaruan reveal) telah dijalankan dan diverifikasi di Solana devnet pada Oktober 2026 |

Biaya mint bagi pembeli adalah harga tingkat ditambah biaya jaringan Solana (sekitar 0,003 SOL per mint).

## 7. Penggunaan dana

Hasil mint mendanai tahap pengembangan Schallern berikutnya. Alokasi yang direncanakan mencakup: pengembangan game (multiplayer, turnamen, akun), seni dan animasi (produksi koleksi, arena baru), infrastruktur dan keamanan (server, RPC, audit), komunitas dan pemasaran (Program kreator, acara), serta cadangan operasional. Pembagian persentase serta skenario pendanaan minimum, target, dan lanjutan dipublikasikan sebelum mint dibuka. Royalti sekunder bukan bagian dari anggaran dasar.

## 8. Peta jalan

1. **Bisa dimainkan sekarang:** demo 3D, tiga arena, penyempurnaan dengan masukan pemain, Program kreator, reward demo.
2. **Berikutnya:** Founder Collection, pertumbuhan komunitas, konsep mint final, dan mint itu sendiri.
3. **Direncanakan:** pertandingan online, kru kota, turnamen, akun pemain dengan reward dan dasbor afiliasi.
4. **Visi:** figur fisik personal, tembok sungguhan, acara langsung.

Tanggal tidak dijanjikan. Setiap langkah diumumkan saat sudah siap.

## 9. Ekonomi game (mode uang asli yang direncanakan)

Permainan uang asli adalah tahap selanjutnya yang berlisensi terpisah. Model yang direncanakan: sebuah meja menetapkan taruhan (misalnya enam pemain, tiga ronde, 1 USDC masing-masing); pemenang mengambil pot dikurangi **biaya bandar 10 % atas kemenangan positif**; taruhan dan biaya bandar dipisahkan secara ketat. Kreator yang membawa pemain menerima **10 % dari biaya bandar yang disesuaikan** dari pemain mereka selama 36 bulan (lihat schallern.io/partners.html). Founder Collectibles tidak berperan dalam ekonomi ini selain sebagai skin yang dipakai pemain untuk melempar.

## 10. Pendanaan perusahaan (terpisah dari koleksi)

Schallern juga berbicara dengan investor privat tentang pendanaan perusahaan (minimum yang direncanakan EUR 20.000). Itu adalah penawaran privat terpisah dengan ketentuan dan dokumen tersendiri, hanya tersedia setelah pengajuan dan peninjauan. Penawaran ini tidak pernah digabungkan dengan Founder Collection, dan tidak ada bagian dari whitepaper ini yang menjadi bagian darinya.

## 11. Tim dan operator

Operator sampai perusahaan game didirikan: **Culturetek Pte. Ltd., 6 Raffles Quay, #14-02, Singapore 048580, UEN 202411392W**. Direktur: Kai Zimmer (founder). Tim: Kai (founder), Pallavi (keuangan), Riya (operasional), Arsh (pengembangan), Raj (pengembangan). Kontak: mint@schallern.io.

## 12. Teknologi

- **Game:** 3D real-time Three.js, fisika koin deterministik buatan sendiri, karakter ber-rig dengan animasi wajah, telemetri untuk penyeimbangan. Hasil dalam mode kompetitif akan dihitung di sisi server.
- **Stack mint:** Metaplex Core, Core Candy Machine, Umi SDK, Arweave via Irys, Helius RPC, penanda tangan backend Node, multisig Squads.
- **Situs web:** schallern.io (bahasa Inggris lebih dulu, Jerman), halaman legal di schallern.io/legal.html.

## 13. Komunitas dan reward

Discord: https://discord.gg/FpZ5zDjV4. Penguji demo mendapat voucher kredit bermain untuk masukan berkualitas, untuk bergabung ke Discord, dan untuk level komunitas (dibatasi per orang; hanya dapat ditukar saat peluncuran uang asli; tidak dapat dicairkan). Kreator mendapat penghasilan lewat Program kreator. Aturan: schallern.io/legal.html#rewards dan #partners.

## 14. Risiko

Schallern sedang dikembangkan. Demo dapat berubah, koleksi dapat tertunda, jaringan blockchain dan dompet dapat gagal, koleksi digital dapat kehilangan nilai, dan permainan uang asli bergantung pada lisensi yang belum ada. Belilah hanya apa yang mampu kamu simpan demi dirinya sendiri.

## 15. Pemberitahuan hukum dan versi

Kerangka hukum, ketentuan, privasi, dan disclaimer dikelola oleh Culturetek Pte. Ltd. dan dipublikasikan di https://schallern.io/legal.html. Dokumen ini bersifat informatif, bukan penawaran penjualan sekuritas, dan bukan nasihat investasi. Versi whitepaper ini dipublikasikan beserta tanggalnya di schallern.io/whitepaper/ dan di repositori publik yang ditautkan di sana.

- v0.1 · 16 Oktober 2026 · draf kerja pertama
