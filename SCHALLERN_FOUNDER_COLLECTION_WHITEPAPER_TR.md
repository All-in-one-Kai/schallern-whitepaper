# Schallern — Founder Collection Whitepaper

**Sürüm 0.1 · Çalışma taslağı · 16 Ekim 2026 · Culturetek Pte. Ltd., Singapur**

> Flip the World. Bir atış. Bir duvar. Milimetreler belirler.

## 1. Özet

Schallern, tarayıcıda oynanan gerçek fizikli bir para atma oyunudur: bir parayı duvara doğru at, kenarı duvara en yakın duran para kazanır. Oyun, 1980'ler Almanya'sında süt parasıyla oynanan bir okul bahçesi oyununun modern versiyonudur. Üç arena ve üç karakterli ücretsiz, oynanabilir bir demo https://schallern.io/play/ adresinde yayında.

**Founder Collection**, **Solana üzerinde 10.000 dijital koleksiyon parçasından** (coin'ler ve karakterler) oluşan planlanmış bir seridir. Founder Collectibles kozmetiktir: oyuncunun coin'inin ve avatarının görünümünü değiştirir, fiziği, geometriyi veya olasılıkları asla değiştirmez. Mint, oyunun bir sonraki geliştirme aşamasını finanse eder. Bu whitepaper oyunu, koleksiyonu, mint mekaniğini, gelirin kullanımını, yol haritasını ve ekibi anlatır; bugün yayında olanı planlanandan ayırır.

## 2. Oyun

**Kural.** Bir duvar, atış başına bir para, maç başına üç tur. Üç turun sonunda en küçük mesafe toplamı kazanır. Duvara hiç değmeyen, kulvardan çıkan, duvarın üzerinden geçen veya 150 cm'den fazla geri seken bir atış fauldür ve yayımlanan maksimum mesafe olarak sayılır.

**Ölçüm.** Mesafe, para durduktan sonra paranın en yakın kenarından duvara kadar ölçülür ve yayımlanan bir milimetre ızgarasına yuvarlanır. Kamera, gölgeler ve görseller asla kazananı belirlemez; fizik sonucu belirler.

**Fizik.** Para, sabit 240 Hz adımda simüle edilen rijit ince bir disktir; hıza bağlı esneklik katsayısı, yüzeye göre yuvarlanma sürtünmesi (asfalt, kum, mermer) ve duvar malzemeleri (beton, kumtaşı, lake) içerir. Bir turdaki her oyuncu aynı mesafe, yüzey ve duvarla atar. Aynı girdi için atışlar deterministiktir.

**Kontroller.** Güç için aşağı sürükle, yön için yana sürükle, yay için bir kaydırıcı; fare ve dokunmatik aynı normalize edilmiş girdi sınırlarını paylaşır. Bırakma, beş parmaklı bir el ve başparmak fiskesiyle ağır çekimde gösterilir.

**Adalet.** Bir oyuncunun satın alabileceği hiçbir şey kütleyi, çapı, sürtünmeyi, sekmeyi veya hassasiyeti değiştirmez. Nadirlik görseldir. Bu, projenin kurucu kuralıdır ve burada anlatılan her koleksiyon parçası için geçerlidir.

## 3. Bugünkü durum (ne yayında, ne değil)

| Bugün yayında | Henüz değil |
|---|---|
| schallern.io/play/ adresinde ücretsiz tarayıcı demosu, masaüstü ve mobil, cüzdansız | Gerçek para masaları (yalnızca lisans, denetim ve onaydan sonra ve yalnızca izin verilen ülkelerde) |
| Üç arena (Berlin asfalt, Gize kum, Vegas mermer), üç karakter (NEO, MAYA, BO), yerel yapay zekâ rakipler | Çevrimiçi çok oyunculu, turnuvalar, şehir ekipleri |
| Ödüllü geri bildirim sohbeti, takip bağlantılı içerik üretici programı, bülten | Mainnet üzerinde Founder Mint (tam akış Solana devnet üzerinde prova edildi, bkz. bölüm 6) |
| Schallern Rewards botlu Discord sunucusu | Oyunda cüzdan bağlantısı |

Demo puanlarının nakit değeri yoktur. Demoyu oynayarak hiçbir NFT, token veya ödeme oluşturulmaz.

## 4. Founder Collection

- **Arz:** 10.000 koleksiyon parçası, numaralı.
- **Konular:** Schallern coin'leri (malzemeler, kaplamalar, kenarlar, gravürler, patina) ve oyunun kendi figürlerinin tarzında karakterler; 48 ünlü duvardan oluşan bir katalogdan isteğe bağlı arena temaları.
- **Standart:** Solana üzerinde Metaplex Core; her koleksiyon parçası, zincir üstü telif bilgisi içeren doğrulanmış bir koleksiyondaki tek bir zincir üstü varlıktır.
- **Nadirlik:** bir özellik sistemi (yaklaşık 8 ila 12 özellik kategorisi, 200 ila 300 varyant) her parçaya 1'den 10.000'e kadar kendi nadirlik sırasını verir; ayrıca beş pazarlama kademesi ve az sayıda 1/1 özel parça. Nadirlik yalnızca prestijdir.
- **Reveal:** alıcıların rastgele bir reveal olmadan kademelerini seçmesi mi, yoksa çizimlerin bir reveal gününde açıklanması mı, açık bir ürün kararıdır; mint açılmadan önce yayımlanır.
- **Çizim hakları:** holder'lar çizimleri için kişisel, münhasır olmayan bir lisans alır; SCHALLERN kelime markası operatörde kalır. Nihai lisans metni mint şartlarıyla birlikte yayımlanır.

## 5. Bir founder ne alır, ne almaz

**Alır:** cüzdan bağlantısı yayına girdiğinde koleksiyon parçasını oyunda atış skini olarak; oyuncu profilinde koleksiyon parçası numarasını taşıyan bir Founder rozeti; Discord'da Founder rolü ve holder kanalları; sıradaki arenalar ve coin tasarımları için oy hakkı; oyun parası modunda yeni arenalara erken erişim.

**Almaz:** şirkette pay, kâr, dağıtım, geri alım veya değer artışı üzerinde hak ya da herhangi bir oynanış avantajı. Founder Collection bir koleksiyon parçasıdır, yatırım ürünü değil. Her türlü şirket finansmanı ayrı, ayrıca yapılandırılmış bir tekliftir (bkz. bölüm 10).

## 6. Mint mekaniği

| Konu | Plan |
|---|---|
| Zincir ve standart | Solana, Metaplex Core, Candy Guard ile Core Candy Machine |
| Kademeler ve fiyatlar | #1–4.000: 0,5 SOL · #4.001–7.000: 1 SOL · #7.001–9.000: 1,5 SOL · #9.001–10.000: 2 SOL (planlanan model; nihai şartlar başlangıçtan önce yayımlanır) |
| Aşamalar | ekip ve OG → Allowlist (garantili, cüzdan başına sınırlı) → bekleme listesi çekilişi → herkese açık; tarihler yalnızca schallern.io üzerinde ve Discord duyurular kanalında açıklanır |
| Sınırlar | aşama başına cüzdan başına mint sınırları; bot vergisi; her mint işlemi captcha ve hız kontrollerinden sonra Schallern arka ucu tarafından oluşturulur ve ortak imzalanır |
| Nerede | yalnızca schallern.io üzerinde; ekip asla önce yazmaz ve asla seed cümlesi sormaz |
| Hazine | mint geliri doğrudan çok imzalı bir hazineye (2/3) gider |
| Telifler | koleksiyona yazılmış %5 ikincil telif |
| Depolama | çizimler ve meta veriler Arweave üzerinde (kalıcı) |
| Prova | tam akış (koleksiyon, aşama gruplu dört kademe makinesi, Allowlist kanıtları, arka uç imzalayıcı, bot ve yük testleri, Arweave yüklemesi, reveal güncellemesi) Ekim 2026'da Solana devnet üzerinde çalıştırıldı ve doğrulandı |

Alıcılar için mint maliyeti, kademe fiyatı artı Solana ağ ücretleridir (mint başına yaklaşık 0,003 SOL).

## 7. Gelirin kullanımı

Gelir, Schallern'in bir sonraki geliştirme aşamasını finanse eder. Planlanan dağılım şunları kapsar: oyun geliştirme (çok oyunculu, turnuvalar, hesaplar), sanat ve animasyon (koleksiyon üretimi, yeni arenalar), altyapı ve güvenlik (sunucular, RPC, denetimler), topluluk ve pazarlama (içerik üretici programı, etkinlikler) ve bir işletme rezervi. Yüzde dağılımı ile asgari, hedef ve genişletilmiş finansman senaryoları mint açılmadan önce yayımlanır. İkincil telifler temel bütçenin parçası değildir.

## 8. Yol haritası

1. **Şimdi oynanabilir:** 3D demo, üç arena, oyuncu geri bildirimiyle ince ayar, içerik üretici programı, demo ödülleri.
2. **Sırada:** Founder Collection, topluluk büyümesi, nihai mint konsepti ve mint.
3. **Planlanan:** çevrimiçi maçlar, şehir ekipleri, turnuvalar, ödüllü oyuncu hesapları ve affiliate panelleri.
4. **Vizyon:** kişisel fiziksel figürler, gerçek duvarlar, canlı etkinlikler.

Tarihler vaat edilmez. Her adım hazır olduğunda duyurulur.

## 9. Oyun ekonomisi (planlanan gerçek para modu)

Gerçek parayla oyun, sonraki ve ayrıca lisanslanan bir aşamadır. Planlanan model: bir masa bahsi belirler (örneğin altı oyuncu, üç tur, her biri 1 USDC); kazanan potu **pozitif kazanç üzerinden %10 kasa komisyonu** düşülerek alır; bahisler ve kasa komisyonları kesinlikle ayrı tutulur. Oyuncu getiren içerik üreticiler, oyuncularının **düzeltilmiş kasa komisyonlarının %10'unu** 36 ay boyunca alır (bkz. schallern.io/partners.html). Founder Collectibles bu ekonomide, oyuncunun atış yaptığı skin olmanın dışında bir rol oynamaz.

## 10. Şirket finansmanı (koleksiyondan ayrı)

Schallern ayrıca şirketin finansmanı için özel yatırımcılarla görüşmektedir (planlanan asgari 20.000 EUR). Bu, kendi şartları ve belgeleri olan, yalnızca başvuru ve incelemeden sonra erişilebilen ayrı, özel bir tekliftir. Founder Collection ile asla birlikte sunulmaz ve bu whitepaper'daki hiçbir şey onun parçası değildir.

## 11. Ekip ve operatör

Oyun şirketi kurulana kadar operatör: **Culturetek Pte. Ltd., 6 Raffles Quay, #14-02, Singapore 048580, UEN 202411392W**. Direktör: Kai Zimmer (kurucu). Ekip: Kai (kurucu), Pallavi (finans), Riya (operasyon), Arsh (geliştirme), Raj (geliştirme). İletişim: mint@schallern.io.

## 12. Teknoloji

- **Oyun:** Three.js gerçek zamanlı 3D, özel deterministik para fiziği, yüz animasyonlu riglenmiş karakterler, dengeleme için telemetri. Rekabetçi modlardaki sonuçlar sunucu tarafında hesaplanacaktır.
- **Mint yığını:** Metaplex Core, Core Candy Machine, Umi SDK, Irys üzerinden Arweave, Helius RPC, bir Node arka uç imzalayıcı, Squads multisig.
- **Web sitesi:** schallern.io (önce İngilizce, Almanca), yasal sayfalar schallern.io/legal.html adresinde.

## 13. Topluluk ve ödüller

Discord: https://discord.gg/FpZ5zDjV4. Demo test kullanıcıları nitelikli geri bildirim, Discord'a katılım ve topluluk seviyeleri için oyun kredisi kuponları kazanır (kişi başı üst sınırlı; yalnızca gerçek para lansmanında kullanılabilir; nakde çevrilemez). İçerik üreticiler içerik üretici programı üzerinden kazanır. Kurallar: schallern.io/legal.html#rewards ve #partners.

## 14. Riskler

Schallern geliştirme aşamasındadır. Demo değişebilir, koleksiyon gecikebilir, blokzincir ağları ve cüzdanlar arızalanabilir, dijital koleksiyon parçaları değer kaybedebilir ve gerçek parayla oyun henüz mevcut olmayan lisanslara bağlıdır. Yalnızca kendisi için tutmayı göze alabileceğin şeyi satın al.

## 15. Yasal uyarı ve sürümler

Yasal çerçeve, şartlar, gizlilik ve sorumluluk reddi Culturetek Pte. Ltd. tarafından yönetilir ve https://schallern.io/legal.html adresinde yayımlanır. Bu belge bilgilendirme amaçlıdır, menkul kıymet satış teklifi ve yatırım tavsiyesi değildir. Bu whitepaper'ın sürümleri tarihleriyle birlikte schallern.io/whitepaper/ adresinde ve orada bağlantısı verilen herkese açık depoda yayımlanır.

- v0.1 · 16 Ekim 2026 · ilk çalışma taslağı
