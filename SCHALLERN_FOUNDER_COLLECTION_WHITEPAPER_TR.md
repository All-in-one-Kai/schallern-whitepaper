# Schallern — Founder Collection Whitepaper

**Sürüm 0.2 · Çalışma taslağı · 18 Ekim 2026 · Culturetek Pte. Ltd., Singapur**

> Flip the World. Bir atış. Bir duvar. Milimetreler belirler.

## 1. Özet

Schallern, tarayıcıda oynanan ve fiziksel olarak kalibre edilmiş bir para atma oyunudur: bir parayı duvara doğru at; durduğunda en yakın kenarı duvara en yakın olan para kazanır. Oyun, 1980'ler Almanya'sında süt parasıyla oynanan bir okul bahçesi oyununun modern versiyonudur. Üç arena ve üç karakterli ücretsiz, oynanabilir bir demo https://schallern.io/play/ adresinde yayında.

**Founder Collection**, **Solana üzerinde 10.000 dijital koleksiyon parçasından** (coin'ler ve karakterler) oluşan planlanmış bir seridir. Founder Collectibles kozmetiktir: oyuncunun coin'inin ve avatarının görünümünü değiştirir, fiziği, geometriyi veya olasılıkları asla değiştirmez. Mint, oyunun bir sonraki geliştirme aşamasını finanse eder. Bu whitepaper oyunu, koleksiyonu, mint mekaniğini, gelirin kullanımını, yol haritasını ve ekibi anlatır; bugün yayında olanı planlanandan ayırır.

## 2. Oyun

**Kural.** Bir duvar, atış başına bir para, maç başına üç tur; en küçük toplam kazanır. Bir atışın puanı, para durduktan sonra paranın en yakın kenarından duvara olan milimetre cinsinden mesafedir. Paranın duvara değmesi **gerekmez**. Duvara yaslanan para (leaner) 0 mm sayılır. Kamera, gölgeler ve görseller asla kazananı belirlemez; fizik sonucu belirler.

**Faul ve geçersiz atışlar.** Tek faul, duvarın üzerinden uçan paradır. Paranın yere ilk değdiği nokta atış çizgisinin 2 m'den daha az ötesindeyse atış geçersizdir (tam 2 m çizgisine düşmek geçerlidir). Faul veya geçersiz atış tur mesafesi olarak sayılır; hiçbir geçerli atış bundan daha kötü puan alamaz.

**Tur kartı.** Her turdan önce bir kart, tüm oyuncular için aynı olan koşulları gösterir: 6 ile 10 m arasında küsuratlı değerlerde atış mesafesi (örneğin 7,43 m), gerçek boyutlarıyla gerçek paralardan oluşan bir katalogdan seçilen tur parası, görünür zemin ve duvar bölgeleri (örneğin çatlaklar, çakıl, pürüzsüz noktalar veya metal plakalar) ve eğim.

**Fizik.** Para, gerçek para verilerine sahip ince bir disktir; her yüzey (asfalt, kum, mermer) ve her duvar malzemesi için sürtünme, yuvarlanma direnci ve sekmeyle simüle edilir. Model, yayımlanmış ölçümlere dayanarak fiziksel olarak kalibre edilmiştir; filme alınmış gerçek atışlarla kalibrasyon henüz tamamlanmadığından buna şimdilik gerçek fizik demiyoruz. Simülasyon deterministiktir: aynı girdi her cihazda aynı sonucu verir.

**Kontroller.** Dört atış stili: Kaydırma (alçak ve düz), Yarım yay, Yüksek lob ve Duvara tokat; her birinin kendi hız ve yay aralığı vardır. Güç ve yön için bas ve geri çek, yan dönüş için hareketi kavisli yap ve küçülen bırakma halkası kapanırken bırak; bırakışın kalitesini zamanlama ve sabit bir el belirler. Fare ve dokunmatik aynı normalize edilmiş girdiyi kullanır.

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
- **Konular:** sekiz görünür özellik kategorisinde Schallern coin'leri: kademe, malzeme, kaplama, kenar, motif (oyunun karakterleri dahil), yazı, arka plan (48 ünlü duvar dahil) ve efekt.
- **Standart:** Solana üzerinde Metaplex Core; her koleksiyon parçası, zincir üstü telif bilgisi içeren doğrulanmış bir koleksiyondaki tek bir zincir üstü varlıktır.
- **Nadirlik:** 129 değerli 8 özellik kategorisi; her parça her kategoriye ve kendi nadirlik sırasına sahiptir. Kademeler: 11 tek parça (1/1), 89 Legendary, 500 Epic, 1.400 Rare, 3.000 Uncommon ve 5.000 Common. Nadirlik yalnızca görsel prestijdir.
- **Rastgele dağıtım ve reveal:** alıcılar çizimi, nadirliği veya kademeyi seçmez. Tamamı satılana kadar her koleksiyon parçası aynı yer tutucu görseli gösterir. Mint açılmadan önce koleksiyonun tamamının sıralı hâline ait bir provenance hash'i yayımlanır ve zincir üstünde saklanır. Tamamı satıldıktan sonra başlangıç kaydırması, önceden duyurulmuş ileri tarihli bir Solana slot'undan alınır; böylece ekip dahil hiç kimse kimin hangi parçayı alacağını yönlendiremez. Herkes sonucu yayımlanan hash ile karşılaştırarak kontrol edebilir.
- **Çizim hakları:** holder'lar koleksiyon parçalarının çizimini ticari olarak kullanabilir. SCHALLERN markası (isim ve logo) bunun dışındadır ve operatörde kalır. Nihai lisans metni mint şartlarıyla birlikte yayımlanır.

## 5. Bir founder ne alır, ne almaz

**Alır:** cüzdan bağlantısı yayına girdiğinde koleksiyon parçasını oyunda atış skini olarak; oyuncu profilinde koleksiyon parçası numarasını taşıyan bir Founder rozeti; Discord'da Founder rolü ve holder kanalları; sıradaki arenalar ve coin tasarımları için oy hakkı; oyun parası modunda yeni arenalara erken erişim; çizimi ticari olarak kullanma hakkı (SCHALLERN markası hariç).

**Almaz:** şirkette pay, kâr, dağıtım, geri alım veya değer artışı üzerinde hak ya da herhangi bir oynanış avantajı. Founder Collection bir koleksiyon parçasıdır, yatırım ürünü değil. Her türlü şirket finansmanı ayrı, ayrıca yapılandırılmış bir tekliftir (bkz. bölüm 10).

## 6. Mint mekaniği

| Konu | Plan |
|---|---|
| Zincir ve standart | Solana, Metaplex Core, Candy Guard ile tek bir Core Candy Machine |
| Fiyat basamakları | alıcı tarafından seçilmez, satılan adede göre belirlenir: #1–4.000: 0,5 SOL · #4.001–7.000: 1 SOL · #7.001–9.000: 1,5 SOL · #9.001–10.000: 2 SOL. Erken alıcılar daha az öder; bir basamağı aşan satın alma parça başına fiyatlandırılır (planlanan model; nihai şartlar başlangıçtan önce yayımlanır) |
| Dağıtım | 10.000 parçanın tamamı için tek bir Candy Machine'den rastgele çizim ve nadirlik; tamamı satıldıktan sonra açıklanır (bkz. bölüm 4) |
| Aşamalar | OG → Allowlist → herkese açık; Allowlist daha erken erişim demektir. Tarihler yalnızca schallern.io üzerinde ve resmî Discord ve Telegram kanallarında duyurulur |
| Sınırlar | hiçbir aşamada cüzdan başına sınır yok; captcha, hız kontrolleri ve bot vergisiyle bot koruması; her mint işlemi Schallern arka ucu tarafından oluşturulur ve ortak imzalanır |
| Nerede | yalnızca schallern.io üzerinde; ekip asla önce yazmaz ve asla seed cümlesi sormaz |
| Erişilebilirlik | mint, yalnızca hizmet sağlayıcılarımızın şartlarının gerektirdiği yerlerde coğrafi olarak kısıtlanır |
| Hazine | mint geliri zincir üstünde doğrudan operatörün hazine cüzdanına ödenir |
| Telifler | koleksiyona yazılmış %5 ikincil telif |
| Depolama | çizimler ve meta veriler Arweave üzerinde (kalıcı); nihai çizimler reveal sırasında yüklenir |
| Prova | tam akış (koleksiyon, yer tutucu ve zincir üstü provenance hash'li tek bir Candy Machine, aşama ve fiyat basamağı grupları, arka uç imzalayıcı, coğrafya ve yaptırım kontrolleri, bot ve yük testleri, bir Solana slot'undan reveal, herkese açık doğrulama) Ekim 2026'da Solana devnet üzerinde çalıştırıldı ve doğrulandı |

Alıcılar için mint maliyeti, o anda açık olan basamağın fiyatı artı Solana ağ ücretleridir (mint başına yaklaşık 0,003 SOL).

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

- **Oyun:** Three.js gerçek zamanlı 3D, özel, deterministik ve fiziksel olarak kalibre edilmiş para fiziği, yüz animasyonlu riglenmiş karakterler, dengeleme için telemetri. Rekabetçi modlardaki sonuçlar sunucu tarafında hesaplanacaktır.
- **Mint yığını:** Metaplex Core, Core Candy Machine, Umi SDK, Arweave, Helius RPC, bir Node arka uç imzalayıcı.
- **Web sitesi:** schallern.io (önce İngilizce, Almanca), yasal sayfalar schallern.io/legal.html adresinde.

## 13. Topluluk ve ödüller

Discord: https://discord.gg/FpZ5zDjV4. Demo test kullanıcıları nitelikli geri bildirim, Discord'a katılım ve topluluk seviyeleri için oyun kredisi kuponları kazanır (kişi başı üst sınırlı; yalnızca gerçek para lansmanında kullanılabilir; nakde çevrilemez). İçerik üreticiler içerik üretici programı üzerinden kazanır. Kurallar: schallern.io/legal.html#rewards ve #partners.

## 14. Riskler

Schallern geliştirme aşamasındadır. Demo değişebilir, koleksiyon gecikebilir, blokzincir ağları ve cüzdanlar arızalanabilir, dijital koleksiyon parçaları değer kaybedebilir ve gerçek parayla oyun henüz mevcut olmayan lisanslara bağlıdır. Yalnızca kendisi için tutmayı göze alabileceğin şeyi satın al.

## 15. Yasal uyarı ve sürümler

Yasal çerçeve, şartlar, gizlilik ve sorumluluk reddi Culturetek Pte. Ltd. tarafından yönetilir ve https://schallern.io/legal.html adresinde yayımlanır. Bu belge bilgilendirme amaçlıdır, menkul kıymet satış teklifi ve yatırım tavsiyesi değildir. Bu whitepaper'ın sürümleri tarihleriyle birlikte schallern.io/whitepaper/ adresinde ve orada bağlantısı verilen herkese açık depoda yayımlanır.

- v0.1 · 16 Ekim 2026 · ilk çalışma taslağı
- v0.2 · 18 Ekim 2026 · demo V04 oyun kuralları (duvara değme şartı yok, tek faul = duvarın üzerinden geçmek, 2 m temas çizgisi, tur kartı, dört atış stili), “fiziksel olarak kalibre edilmiş” ifadesi, nadirliklerle rastgele dağıtım ve tamamı satıldıktan sonra reveal, tek Candy Machine, satılan adede göre fiyat basamakları, cüzdan başına sınır yok, özellik sistemi ve kademe adetleri, çizimin ticari kullanımı, coğrafi kısıtlama
