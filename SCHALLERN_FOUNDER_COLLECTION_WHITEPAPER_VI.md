# Schallern — Whitepaper Founder Collection

**Phiên bản 0.2 · Bản thảo đang làm việc · 18 tháng 10 năm 2026 · Culturetek Pte. Ltd., Singapore**

> Flip the World. Một cú ném. Một bức tường. Từng milimét quyết định.

## 1. Tóm tắt

Schallern là game ném xu được hiệu chỉnh vật lý, chơi trên trình duyệt: ném một đồng xu về phía tường; đồng xu có mép gần nhất dừng lại sát tường nhất sẽ thắng. Trò chơi là phiên bản hiện đại của một trò chơi sân trường chơi bằng tiền mua sữa ở nước Đức thập niên 1980. Một bản demo miễn phí, chơi được với ba đấu trường và ba nhân vật đang hoạt động tại https://schallern.io/play/.

**Founder Collection** là một loạt dự kiến gồm **10.000 vật phẩm sưu tầm kỹ thuật số trên Solana** (đồng xu và nhân vật). Founder Collectibles mang tính trang trí: chúng thay đổi diện mạo đồng xu và avatar của người chơi, không bao giờ thay đổi vật lý, hình học hay tỷ lệ thắng. Đợt mint tài trợ cho giai đoạn phát triển tiếp theo của game. Whitepaper này mô tả trò chơi, bộ sưu tập, cơ chế mint, việc sử dụng tiền thu được, lộ trình và đội ngũ, đồng thời tách bạch những gì đang hoạt động hôm nay với những gì đang dự kiến.

## 2. Trò chơi

**Luật.** Một bức tường, một đồng xu mỗi cú ném, ba vòng mỗi trận; tổng nhỏ nhất thắng. Mỗi cú ném được tính bằng khoảng cách tính theo milimét từ mép gần nhất của đồng xu đến tường, sau khi đồng xu dừng hẳn. Đồng xu **không** cần chạm tường. Đồng xu dừng lại tựa tường (leaner) được tính 0 mm. Góc máy, bóng đổ và hình ảnh không bao giờ quyết định người thắng; kết quả vật lý mới quyết định.

**Phạm lỗi và cú ném không hợp lệ.** Lỗi duy nhất là đồng xu bay qua tường. Cú ném không hợp lệ nếu điểm chạm đất đầu tiên của đồng xu cách vạch ném chưa tới 2 m (chạm đất đúng trên vạch 2 m vẫn hợp lệ). Cú ném phạm lỗi hoặc không hợp lệ được tính bằng khoảng cách ném của vòng đó; không cú ném hợp lệ nào có thể bị tính tệ hơn mức này.

**Thẻ vòng.** Trước mỗi vòng, một thẻ hiển thị các điều kiện, giống nhau cho mọi người chơi: khoảng cách ném từ 6 đến 10 m với số đo lẻ (ví dụ 7,43 m), đồng xu của vòng lấy từ danh mục các đồng xu thật với kích thước thật, các mảng nền và tường nhìn thấy được (ví dụ vết nứt, sỏi, chỗ trơn nhẵn hay tấm kim loại) và độ dốc.

**Vật lý.** Đồng xu là một đĩa mỏng mang dữ liệu của đồng xu thật, được mô phỏng với ma sát, lực cản lăn và độ nảy theo từng bề mặt (nhựa đường, cát, cẩm thạch) và theo từng vật liệu tường. Mô hình được hiệu chỉnh vật lý dựa trên các số đo đã công bố; việc hiệu chỉnh đối chiếu với các cú ném thật được quay phim vẫn chưa thực hiện, nên chúng tôi chưa gọi đó là vật lý thật. Mô phỏng là tất định: cùng một đầu vào cho cùng một kết quả trên mọi thiết bị.

**Điều khiển.** Bốn kiểu ném: Trượt (thấp và phẳng), Nửa vòng cung, Lốp bổng và Đập tường, mỗi kiểu có dải tốc độ và vòng cung riêng. Nhấn và kéo lùi để chọn lực và hướng, uốn cong cử chỉ để tạo xoáy ngang, và thả tay khi vòng thả đang thu nhỏ khép lại; thời điểm và bàn tay vững quyết định chất lượng cú thả. Chuột và cảm ứng dùng chung đầu vào đã chuẩn hóa.

**Công bằng.** Không thứ gì người chơi có thể mua làm thay đổi khối lượng, đường kính, ma sát, độ nảy hay độ chính xác. Độ hiếm là thị giác. Đây là nguyên tắc nền tảng của dự án và áp dụng cho mọi vật phẩm sưu tầm được mô tả ở đây.

## 3. Trạng thái hôm nay (đang hoạt động, chưa có)

| Đang hoạt động | Chưa có |
|---|---|
| Demo miễn phí trên trình duyệt tại schallern.io/play/, máy tính và di động, không cần ví | Bàn chơi tiền thật (chỉ sau khi có giấy phép, kiểm toán và phê duyệt, và chỉ ở các quốc gia được phép) |
| Ba đấu trường (nhựa đường Berlin, cát Giza, cẩm thạch Vegas), ba nhân vật (NEO, MAYA, BO), đối thủ AI cục bộ | Nhiều người chơi online, giải đấu, băng nhóm thành phố |
| Chat góp ý có thưởng, Chương trình nhà sáng tạo với link theo dõi, bản tin | Founder Mint trên mainnet (toàn bộ quy trình đã được diễn tập trên Solana devnet, xem mục 6) |
| Máy chủ Discord với bot Schallern Rewards | Liên kết ví trong game |

Điểm demo không có giá trị tiền mặt. Không NFT, token hay khoản thanh toán nào được tạo ra khi chơi demo.

## 4. Founder Collection

- **Tổng cung:** 10.000 vật phẩm sưu tầm, được đánh số.
- **Chủ đề:** đồng xu Schallern với tám nhóm thuộc tính nhìn thấy được: bậc, chất liệu, lớp hoàn thiện, viền, họa tiết (bao gồm các nhân vật của game), dòng chữ khắc, phông nền (bao gồm 48 bức tường nổi tiếng) và hiệu ứng.
- **Tiêu chuẩn:** Metaplex Core trên Solana; mỗi vật phẩm là một tài sản on-chain trong một bộ sưu tập đã xác minh với thông tin tiền bản quyền on-chain.
- **Độ hiếm:** 8 nhóm thuộc tính với 129 giá trị; mỗi vật phẩm đều có đủ mọi nhóm và có thứ hạng độ hiếm riêng. Các bậc: 11 vật phẩm độc bản (1/1), 89 Legendary, 500 Epic, 1.400 Rare, 3.000 Uncommon và 5.000 Common. Độ hiếm chỉ là uy tín về mặt thị giác.
- **Phân bổ ngẫu nhiên và reveal:** người mua không chọn artwork, độ hiếm hay bậc. Cho đến khi bán hết, mọi vật phẩm sưu tầm đều hiển thị cùng một hình giữ chỗ. Trước khi mint mở, mã băm provenance của toàn bộ bộ sưu tập theo đúng thứ tự được công bố và lưu on-chain. Sau khi bán hết, điểm bắt đầu (offset) được lấy từ một slot Solana trong tương lai đã thông báo trước, nên không ai, kể cả đội ngũ, có thể điều khiển ai nhận được vật phẩm nào. Bất kỳ ai cũng có thể đối chiếu kết quả với mã băm đã công bố.
- **Quyền với artwork:** holder được sử dụng artwork của vật phẩm sưu tầm của mình cho mục đích thương mại. Thương hiệu SCHALLERN (tên và logo) không nằm trong quyền này và vẫn thuộc đơn vị vận hành. Văn bản giấy phép cuối cùng được công bố cùng điều khoản mint.

## 5. Founder nhận được gì, và không nhận được gì

**Nhận được:** vật phẩm làm skin ném trong game khi liên kết ví đi vào hoạt động; huy hiệu Founder kèm số vật phẩm trên hồ sơ người chơi; vai trò Founder và kênh dành cho holder trên Discord; một phiếu bầu chọn đấu trường và thiết kế xu tiếp theo; truy cập sớm các đấu trường mới ở chế độ tiền ảo; quyền sử dụng artwork cho mục đích thương mại (trừ thương hiệu SCHALLERN).

**Không nhận được:** cổ phần công ty, quyền đòi lợi nhuận, chia cổ tức, mua lại hay tăng giá trị, hoặc bất kỳ lợi thế nào trong gameplay. Founder Collection là vật phẩm sưu tầm, không phải sản phẩm đầu tư. Mọi khoản tài trợ cho công ty là một đề nghị riêng, được cấu trúc riêng (xem mục 10).

## 6. Cơ chế mint

| Hạng mục | Kế hoạch |
|---|---|
| Chain và tiêu chuẩn | Solana, Metaplex Core, một Core Candy Machine với Candy Guard |
| Bậc giá | do số lượng đã bán quyết định, người mua không tự chọn: #1–4.000 ở 0,5 SOL · #4.001–7.000 ở 1 SOL · #7.001–9.000 ở 1,5 SOL · #9.001–10.000 ở 2 SOL. Người mua sớm trả ít hơn; giao dịch mua vượt qua một bậc được tính giá theo từng vật phẩm (mô hình dự kiến; điều khoản cuối cùng được công bố trước khi bắt đầu) |
| Phân bổ | artwork và độ hiếm ngẫu nhiên cho cả 10.000 vật phẩm từ một Candy Machine, reveal sau khi bán hết (xem mục 4) |
| Giai đoạn | OG → Allowlist → công khai; Allowlist nghĩa là được truy cập sớm hơn. Ngày chỉ được thông báo trên schallern.io và trong các kênh Discord và Telegram chính thức |
| Giới hạn | không giới hạn mỗi ví ở bất kỳ giai đoạn nào; chống bot bằng captcha, kiểm tra tần suất và thuế bot; mọi giao dịch mint được backend Schallern xây dựng và đồng ký |
| Ở đâu | chỉ trên schallern.io; đội ngũ không bao giờ nhắn tin trước và không bao giờ hỏi seed phrase |
| Khả dụng | đợt mint chỉ bị giới hạn theo khu vực địa lý ở những nơi điều khoản của các nhà cung cấp dịch vụ của chúng tôi yêu cầu |
| Kho bạc | tiền thu từ mint được thanh toán on-chain thẳng vào ví kho bạc của đơn vị vận hành |
| Tiền bản quyền | 5 % tiền bản quyền thứ cấp, ghi vào bộ sưu tập |
| Lưu trữ | artwork và metadata trên Arweave (vĩnh viễn); artwork cuối cùng được tải lên khi reveal |
| Diễn tập | toàn bộ quy trình (bộ sưu tập, một Candy Machine với hình giữ chỗ và mã băm provenance on-chain, các nhóm theo giai đoạn và bậc giá, bộ ký backend, kiểm tra địa lý và lệnh trừng phạt, kiểm thử bot và tải, reveal từ một slot Solana, xác minh công khai) đã được chạy và xác minh trên Solana devnet vào tháng 10 năm 2026 |

Chi phí mint cho người mua là giá của bậc đang mở cộng phí mạng Solana (khoảng 0,003 SOL mỗi lượt mint).

## 7. Sử dụng tiền thu được

Tiền thu được tài trợ cho giai đoạn phát triển tiếp theo của Schallern. Phân bổ dự kiến gồm: phát triển game (nhiều người chơi, giải đấu, tài khoản), nghệ thuật và hoạt hình (sản xuất bộ sưu tập, đấu trường mới), hạ tầng và bảo mật (máy chủ, RPC, kiểm toán), cộng đồng và marketing (Chương trình nhà sáng tạo, sự kiện) và một khoản dự phòng vận hành. Tỷ lệ phân chia và các kịch bản tài trợ tối thiểu, mục tiêu và mở rộng được công bố trước khi mint mở. Tiền bản quyền thứ cấp không thuộc ngân sách cơ sở.

## 8. Lộ trình

1. **Chơi được ngay:** demo 3D, ba đấu trường, tinh chỉnh bằng góp ý người chơi, Chương trình nhà sáng tạo, phần thưởng demo.
2. **Tiếp theo:** Founder Collection, tăng trưởng cộng đồng, ý tưởng mint cuối cùng và đợt mint.
3. **Dự kiến:** đấu online, băng nhóm thành phố, giải đấu, tài khoản người chơi với phần thưởng và bảng điều khiển affiliate.
4. **Tầm nhìn:** mô hình vật lý cá nhân, tường thật, sự kiện trực tiếp.

Ngày tháng không được cam kết. Mỗi bước được thông báo khi sẵn sàng.

## 9. Kinh tế game (chế độ tiền thật dự kiến)

Chơi tiền thật là một giai đoạn sau, được cấp phép riêng. Mô hình dự kiến: một bàn đặt mức cược (ví dụ sáu người chơi, ba vòng, mỗi người 1 USDC); người thắng nhận pot trừ **phí nhà cái 10 % trên phần thắng dương**; tiền cược và phí nhà cái được tách bạch nghiêm ngặt. Nhà sáng tạo mang người chơi đến nhận **10 % phí nhà cái đã điều chỉnh** của người chơi của họ trong 36 tháng (xem schallern.io/partners.html). Founder Collectibles không có vai trò nào trong nền kinh tế này ngoài việc là skin mà người chơi dùng để ném.

## 10. Tài trợ công ty (tách biệt với bộ sưu tập)

Schallern cũng trao đổi với các nhà đầu tư cá nhân về việc tài trợ cho công ty (tối thiểu dự kiến 20.000 EUR). Đó là một đề nghị riêng, không công khai, với điều khoản và tài liệu riêng, chỉ có sau khi đăng ký và xem xét. Nó không bao giờ được gộp với Founder Collection, và không nội dung nào trong whitepaper này thuộc về đề nghị đó.

## 11. Đội ngũ và đơn vị vận hành

Đơn vị vận hành cho đến khi công ty game được thành lập: **Culturetek Pte. Ltd., 6 Raffles Quay, #14-02, Singapore 048580, UEN 202411392W**. Giám đốc: Kai Zimmer (nhà sáng lập). Đội ngũ: Kai (nhà sáng lập), Pallavi (tài chính), Riya (vận hành), Arsh (phát triển), Raj (phát triển). Liên hệ: mint@schallern.io.

## 12. Công nghệ

- **Game:** 3D thời gian thực Three.js, vật lý xu tự xây dựng, tất định và được hiệu chỉnh vật lý, nhân vật có khung xương với hoạt hình khuôn mặt, telemetry để cân bằng. Kết quả ở các chế độ thi đấu sẽ được tính phía máy chủ.
- **Ngăn xếp mint:** Metaplex Core, Core Candy Machine, Umi SDK, Arweave, Helius RPC, bộ ký backend Node.
- **Website:** schallern.io (tiếng Anh trước, tiếng Đức), trang pháp lý tại schallern.io/legal.html.

## 13. Cộng đồng và phần thưởng

Discord: https://discord.gg/FpZ5zDjV4. Người thử demo nhận voucher tín dụng chơi cho góp ý đạt chuẩn, cho việc tham gia Discord và cho các cấp cộng đồng (giới hạn mỗi người; chỉ đổi được khi ra mắt tiền thật; không quy đổi thành tiền mặt). Nhà sáng tạo kiếm thu nhập qua Chương trình nhà sáng tạo. Quy tắc: schallern.io/legal.html#rewards và #partners.

## 14. Rủi ro

Schallern đang trong giai đoạn phát triển. Demo có thể thay đổi, bộ sưu tập có thể bị trì hoãn, mạng blockchain và ví có thể gặp sự cố, vật phẩm sưu tầm kỹ thuật số có thể mất giá trị, và chơi tiền thật phụ thuộc vào giấy phép chưa có. Chỉ mua những gì bạn có thể giữ vì chính giá trị sưu tầm của nó.

## 15. Thông báo pháp lý và các phiên bản

Khung pháp lý, điều khoản, quyền riêng tư và miễn trừ trách nhiệm do Culturetek Pte. Ltd. duy trì và công bố tại https://schallern.io/legal.html. Tài liệu này mang tính thông tin, không phải lời chào bán chứng khoán và không phải tư vấn đầu tư. Các phiên bản của whitepaper này được công bố kèm ngày tại schallern.io/whitepaper/ và trong kho lưu trữ công khai được liên kết ở đó.

- v0.1 · 16 tháng 10 năm 2026 · bản thảo làm việc đầu tiên
- v0.2 · 18 tháng 10 năm 2026 · luật chơi của demo V04 (không cần chạm tường, lỗi duy nhất là bay qua tường, vạch chạm đất 2 m, thẻ vòng, bốn kiểu ném), cách diễn đạt “được hiệu chỉnh vật lý”, phân bổ ngẫu nhiên với độ hiếm và reveal sau khi bán hết, một Candy Machine, bậc giá theo số lượng đã bán, không giới hạn mỗi ví, hệ thống thuộc tính và số lượng theo bậc, sử dụng artwork cho mục đích thương mại, giới hạn theo khu vực địa lý
