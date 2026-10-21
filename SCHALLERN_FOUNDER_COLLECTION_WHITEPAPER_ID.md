# Schallern — Whitepaper Founder Collection

**Versi 0.2 · Draf kerja · 18 Oktober 2026 · Culturetek Pte. Ltd., Singapura**

> Flip the World. Satu lemparan. Satu tembok. Milimeter yang menentukan.

## 1. Abstrak

Schallern adalah game lempar koin yang dikalibrasi secara fisik dan dimainkan di browser: lempar koin ke arah tembok; koin yang tepi terdekatnya berhenti paling dekat ke tembok menang. Game ini adalah versi modern dari permainan halaman sekolah yang dimainkan dengan uang susu di Jerman era 1980-an. Demo gratis yang bisa dimainkan dengan tiga arena dan tiga karakter sudah tersedia di https://schallern.io/play/.

**Founder Collection** adalah seri terencana berisi **10.000 koleksi digital di Solana** (koin dan karakter). Founder Collectibles bersifat kosmetik: mereka mengubah tampilan koin dan avatar pemain, tetapi tidak pernah mengubah fisika, geometri, atau peluang. Mint ini mendanai tahap pengembangan game berikutnya. Whitepaper ini menjelaskan game, koleksi, mekanisme mint, penggunaan dana, peta jalan, dan tim, serta memisahkan apa yang sudah aktif hari ini dari apa yang direncanakan.

## 2. Game

**Aturan.** Satu tembok, satu koin per lemparan, tiga ronde per pertandingan; total terkecil menang. Skor sebuah lemparan adalah jarak dalam milimeter dari tepi koin terdekat ke tembok setelah koin berhenti. Koin **tidak** harus menyentuh tembok. Koin yang tetap bersandar di tembok (leaner) mendapat skor 0 mm. Kamera, bayangan, dan visual tidak pernah menentukan pemenang; hasil fisikalah yang menentukan.

**Pelanggaran dan lemparan tidak sah.** Satu-satunya pelanggaran adalah koin yang terbang melewati tembok. Lemparan tidak sah jika sentuhan pertama koin dengan tanah kurang dari 2 m di depan garis lempar (mendarat tepat di garis 2 m tetap sah). Pelanggaran atau lemparan tidak sah dihitung dengan jarak ronde; tidak ada lemparan sah yang bisa mendapat skor lebih buruk dari itu.

**Kartu ronde.** Sebelum setiap ronde, sebuah kartu menampilkan kondisi yang sama untuk setiap pemain: jarak lempar antara 6 dan 10 m dengan angka tidak bulat (misalnya 7,43 m), koin ronde dari katalog koin asli dalam ukuran aslinya, serta bidang tanah dan tembok yang terlihat (misalnya retakan, kerikil, bagian licin, atau pelat logam) dan kemiringannya.

**Fisika.** Koin adalah cakram tipis dengan data koin asli, disimulasikan dengan gesekan, hambatan gelinding, dan pantulan per permukaan (aspal, pasir, marmer) dan per material tembok. Model ini dikalibrasi secara fisik berdasarkan hasil pengukuran yang telah dipublikasikan; kalibrasi terhadap rekaman lemparan nyata masih menunggu, jadi kami belum menyebutnya fisika nyata. Simulasinya deterministik: input yang sama memberikan hasil yang sama di setiap perangkat.

**Kontrol.** Empat gaya lempar: Peluncur (rendah dan datar), Setengah busur, Lob tinggi, dan Tampar dinding, masing-masing dengan rentang kecepatan dan lengkungnya sendiri. Tekan dan tarik ke belakang untuk tenaga dan arah, lengkungkan gerakan untuk putaran samping, lalu lepaskan saat cincin pelepasan yang menyusut menutup; timing dan tangan yang stabil menentukan kualitas pelepasan. Mouse dan sentuhan menggunakan input ternormalisasi yang sama.

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
- **Subjek:** koin Schallern dalam delapan kategori trait yang terlihat: tingkat, material, finishing, tepi, motif (termasuk karakter game), inskripsi, latar (termasuk 48 tembok terkenal), dan efek.
- **Standar:** Metaplex Core di Solana; setiap collectible adalah satu aset on-chain dalam koleksi terverifikasi dengan informasi royalti on-chain.
- **Kelangkaan:** 8 kategori trait dengan 129 nilai; setiap karya memiliki semua kategori dan peringkat kelangkaannya sendiri. Tingkat: 11 karya satu-satunya (1/1), 89 Legendary, 500 Epic, 1.400 Rare, 3.000 Uncommon, dan 5.000 Common. Kelangkaan hanya soal prestise visual.
- **Pembagian acak dan reveal:** pembeli tidak memilih karya seni, kelangkaan, atau tingkat. Sampai sold out, setiap collectible menampilkan placeholder yang sama. Sebelum mint dibuka, hash provenance dari seluruh koleksi dalam urutan finalnya dipublikasikan dan disimpan on-chain. Setelah sold out, offset awal diambil dari slot Solana di masa depan yang sudah diumumkan sebelumnya, sehingga tidak ada seorang pun, termasuk tim, yang bisa mengatur siapa mendapat karya yang mana. Siapa pun dapat mencocokkan hasilnya dengan hash yang dipublikasikan.
- **Hak karya seni:** holder boleh menggunakan karya seni collectible mereka secara komersial. Merek SCHALLERN (nama dan logo) dikecualikan dan tetap milik operator. Teks lisensi final dipublikasikan bersama ketentuan mint.

## 5. Apa yang didapat seorang founder, dan apa yang tidak

**Didapat:** collectible sebagai skin lempar di dalam game begitu penautan dompet aktif; lencana Founder dengan nomor collectible di profil pemain; peran Founder dan kanal holder di Discord; hak suara untuk menentukan arena dan desain koin berikutnya; akses awal ke arena baru dalam mode uang mainan; hak menggunakan karya seni secara komersial (kecuali merek SCHALLERN).

**Tidak didapat:** saham perusahaan, klaim atas laba, pembagian keuntungan, buy-back, atau kenaikan nilai, maupun keunggulan gameplay apa pun. Founder Collection adalah koleksi, bukan produk investasi. Pendanaan perusahaan apa pun adalah penawaran terpisah dengan struktur tersendiri (lihat bagian 10).

## 6. Mekanisme mint

| Hal | Rencana |
|---|---|
| Chain dan standar | Solana, Metaplex Core, satu Core Candy Machine dengan Candy Guard |
| Tahap harga | ditentukan oleh jumlah yang terjual, bukan dipilih pembeli: #1–4.000 seharga 0,5 SOL · #4.001–7.000 seharga 1 SOL · #7.001–9.000 seharga 1,5 SOL · #9.001–10.000 seharga 2 SOL. Pembeli awal membayar lebih murah; pembelian yang melewati batas tahap dihargai per karya (model terencana; ketentuan final dipublikasikan sebelum mulai) |
| Pembagian | karya seni dan kelangkaan acak untuk seluruh 10.000 dari satu Candy Machine, diungkap setelah sold out (lihat bagian 4) |
| Fase | mulai **11 November 2026, 11.11 CET Berlin (10.11 UTC)**; OG → allowlist → publik; allowlist berarti akses lebih awal. Tanggal dan perubahan apa pun diumumkan hanya di schallern.io serta di kanal resmi Discord dan Telegram |
| Batas | tidak ada batas per dompet di fase mana pun; perlindungan bot lewat captcha, pemeriksaan laju, dan pajak bot; setiap transaksi mint dibangun dan ditandatangani bersama oleh backend Schallern |
| Di mana | hanya di schallern.io; tim tidak pernah mengirim pesan lebih dulu dan tidak pernah meminta seed phrase |
| Ketersediaan | mint dibatasi secara geografis hanya jika ketentuan penyedia layanan kami mewajibkannya |
| Treasury | hasil mint dibayarkan on-chain ke brankas multisig 2-dari-3 (Squads v4) milik operator; tidak ada satu kunci pun yang bisa memindahkan dana sendirian |
| Royalti | royalti sekunder 5 %, tertulis di dalam koleksi |
| Penyimpanan | karya seni dan metadata di Arweave (permanen); karya seni final diunggah saat reveal |
| Gladi | alur lengkap (koleksi, satu Candy Machine dengan placeholder dan hash provenance on-chain, grup fase dan tahap harga, penanda tangan backend, pemeriksaan geo dan sanksi, uji bot dan beban, reveal dari slot Solana, verifikasi publik) telah dijalankan dan diverifikasi di Solana devnet pada Oktober 2026 |

Biaya mint bagi pembeli adalah harga tahap yang sedang berlaku ditambah biaya jaringan Solana (sekitar 0,003 SOL per mint).

## 7. Penggunaan dana

Hasil mint mendanai tahap pengembangan Schallern berikutnya. Alokasi yang direncanakan mencakup: pengembangan game (multiplayer, turnamen, akun), seni dan animasi (produksi koleksi, arena baru), infrastruktur dan keamanan (server, RPC, audit), komunitas dan pemasaran (Program kreator, acara), serta cadangan operasional. Pembagian persentase serta skenario pendanaan minimum, target, dan lanjutan dipublikasikan sebelum mint dibuka. Royalti sekunder bukan bagian dari anggaran dasar.

## 8. Peta jalan

1. **Bisa dimainkan sekarang:** demo 3D, tiga arena, penyempurnaan dengan masukan pemain, Program kreator, reward demo.
2. **Berikutnya:** Founder Collection, pertumbuhan komunitas, konsep mint final, dan mint itu sendiri.
3. **Direncanakan:** pertandingan online, kru kota, turnamen, akun pemain dengan reward dan dasbor afiliasi.
4. **Visi:** figur fisik personal, tembok sungguhan, acara langsung.

Selain dimulainya Founder Mint (11 November 2026, 11.11 CET Berlin), tanggal tidak dijanjikan. Setiap langkah diumumkan saat sudah siap.

## 9. Ekonomi game (mode uang asli yang direncanakan)

Permainan uang asli adalah tahap selanjutnya yang berlisensi terpisah. Model yang direncanakan: sebuah meja menetapkan taruhan (misalnya enam pemain, tiga ronde, 1 USDC masing-masing); pemenang mengambil pot dikurangi **biaya bandar 10 % atas kemenangan positif**; taruhan dan biaya bandar dipisahkan secara ketat. Kreator yang membawa pemain menerima **10 % dari biaya bandar yang disesuaikan** dari pemain mereka selama 36 bulan (lihat schallern.io/partners.html). Founder Collectibles tidak berperan dalam ekonomi ini selain sebagai skin yang dipakai pemain untuk melempar.

## 10. Pendanaan perusahaan (terpisah dari koleksi)

Schallern juga berbicara dengan investor privat tentang pendanaan perusahaan (minimum yang direncanakan EUR 20.000). Itu adalah penawaran privat terpisah dengan ketentuan dan dokumen tersendiri, hanya tersedia setelah pengajuan dan peninjauan. Penawaran ini tidak pernah digabungkan dengan Founder Collection, dan tidak ada bagian dari whitepaper ini yang menjadi bagian darinya.

## 11. Tim dan operator

Operator sampai perusahaan game didirikan: **Culturetek Pte. Ltd., 6 Raffles Quay, #14-02, Singapore 048580, UEN 202411392W**. Direktur: Kai Zimmer (founder). Tim: Kai (founder), Pallavi (keuangan), Riya (operasional), Arsh (pengembangan), Raj (pengembangan). Kontak: mint@schallern.io.

## 12. Teknologi

- **Game:** 3D real-time Three.js, fisika koin buatan sendiri yang deterministik dan dikalibrasi secara fisik, karakter ber-rig dengan animasi wajah, telemetri untuk penyeimbangan. Hasil dalam mode kompetitif akan dihitung di sisi server.
- **Stack mint:** Metaplex Core, Core Candy Machine, Umi SDK, Arweave, Helius RPC, penanda tangan backend Node, brankas multisig Squads v4 untuk hasil mint.
- **Situs web:** schallern.io (bahasa Inggris lebih dulu, Jerman), halaman legal di schallern.io/legal.html.

## 13. Komunitas dan reward

Discord: https://discord.gg/FpZ5zDjV4. Penguji demo mendapat voucher kredit bermain untuk masukan berkualitas, untuk bergabung ke Discord, dan untuk level komunitas (dibatasi per orang; hanya dapat ditukar saat peluncuran uang asli; tidak dapat dicairkan). Kreator mendapat penghasilan lewat Program kreator. Aturan: schallern.io/legal.html#rewards dan #partners.

## 14. Risiko

Schallern sedang dikembangkan. Demo dapat berubah, koleksi dapat tertunda, jaringan blockchain dan dompet dapat gagal, koleksi digital dapat kehilangan nilai, dan permainan uang asli bergantung pada lisensi yang belum ada. Belilah hanya apa yang mampu kamu simpan demi dirinya sendiri.

## 15. Pemberitahuan hukum dan versi

Kerangka hukum, ketentuan, privasi, dan disclaimer dikelola oleh Culturetek Pte. Ltd. dan dipublikasikan di https://schallern.io/legal.html. Dokumen ini bersifat informatif, bukan penawaran penjualan sekuritas, dan bukan nasihat investasi. Versi whitepaper ini dipublikasikan beserta tanggalnya di schallern.io/whitepaper/ dan di repositori publik yang ditautkan di sana.

- v0.1 · 16 Oktober 2026 · draf kerja pertama
- v0.2 · 18 Oktober 2026 · aturan game demo V04 (tidak wajib menyentuh tembok, satu-satunya pelanggaran = melewati tembok, garis pendaratan 2 m, kartu ronde, empat gaya lempar), istilah “dikalibrasi secara fisik”, pembagian acak dengan kelangkaan dan reveal setelah sold out, satu Candy Machine, tahap harga berdasarkan jumlah terjual, tanpa batas per dompet, sistem trait dan jumlah per tingkat, penggunaan komersial karya seni, pembatasan geografis
