---
name: doi-soat-san-meinvoice-misa
description: Đối soát doanh thu và tiền về từ Shopee, TikTok Shop với hoá đơn MISA meInvoice và sổ MISA AMIS theo tháng – tách doanh thu, voucher, phí sàn, hoàn trả; tìm chênh lệch; đề xuất bút toán điều chỉnh. Dùng khi kế toán khoá sổ tháng, khi tiền sàn về không khớp, hoặc trước khi lập báo cáo tháng cho Giám đốc.
---

# Đối soát sàn – meInvoice – MISA AMIS

Nguyên tắc: **ba nguồn phải kể cùng một câu chuyện** – sàn nói bán bao nhiêu và trả bao nhiêu, meInvoice nói đã xuất hoá đơn bao nhiêu, MISA nói đã ghi sổ bao nhiêu. Mọi chênh lệch phải có lý do.

MISA AMIS là sổ sách chính thức. Skill này chỉ chỉ ra chênh lệch và đề xuất điều chỉnh; **người hạch toán quyết định**. Kết quả là tài liệu nội bộ.

## Bước 1. Yêu cầu file (dừng nếu thiếu file bắt buộc)

| File | Lấy ở đâu | Bắt buộc |
|---|---|---|
| Báo cáo thanh toán / Income theo đơn – Shopee | Kênh Người Bán → Tài chính → Doanh thu → Xuất | ✅ |
| Báo cáo thanh toán / settlement theo đơn – TikTok Shop | Seller Center → Tài chính → Xuất báo cáo | ✅ |
| File đơn hàng (tất cả trạng thái) của tháng | Mỗi sàn | ✅ |
| Bảng kê hoá đơn đã xuất trong tháng | MISA meInvoice → Bảng kê | ✅ |
| Sổ chi tiết TK 131 (theo đối tượng sàn), 511, 521 (nếu dùng), 641/6421 | MISA AMIS | ✅ |
| Sao kê ngân hàng nhận tiền sàn | Ngân hàng | ✅ |
| Hoá đơn phí sàn, phí quảng cáo do sàn xuất | Email/Portal sàn | Nên có |

Hỏi thêm: chế độ kế toán (TT133/TT200), công ty ghi doanh thu sàn theo **giá trước voucher sàn** hay **sau**, xuất hoá đơn theo từng đơn hay tổng hợp.

## Bước 2. Chuẩn hoá dữ liệu sàn

Với mỗi sàn, gom theo **mã đơn** và tách thành các cột:

| Cột | Ghi chú |
|---|---|
| Giá bán sản phẩm (trước mọi giảm giá) | |
| Giảm giá / voucher do **shop** tài trợ | Giảm trừ doanh thu của shop |
| Voucher / trợ giá do **sàn** tài trợ | Sàn bù lại → thường không giảm doanh thu của shop; kiểm tra cách sàn thể hiện |
| Phí cố định, phí thanh toán/giao dịch, phí dịch vụ (Voucher Xtra, Freeship Xtra), phí khác | Chi phí bán hàng – cần hoá đơn từ sàn |
| Phí vận chuyển người mua trả / sàn trợ giá / shop chịu | Tách riêng |
| Phí quảng cáo trừ vào doanh thu (nếu có) | Có thể được nạp riêng – tránh tính hai lần |
| Hoàn tiền / trả hàng | Ghi nhận giảm doanh thu đúng kỳ |
| Số tiền sàn thanh toán | = cột cuối của file Income |
| Ngày đơn hoàn thành, ngày sàn thanh toán | Để tìm chênh lệch thời điểm |

Thuế do sàn khấu trừ: quy định sàn khấu trừ, nộp thay áp dụng cho **hộ kinh doanh, cá nhân** – HDP là công ty; nếu file có dòng thuế khấu trừ thì báo ngay để kiểm tra cài đặt tài khoản.

## Bước 3. Đối soát ba chiều

### 3a. Sàn ↔ meInvoice (đã xuất đủ hoá đơn chưa?)
- Mọi đơn **hoàn thành** trong tháng đã có hoá đơn (hoặc nằm trong hoá đơn tổng hợp) chưa?
- Đơn huỷ/hoàn nhưng đã xuất hoá đơn → cần hoá đơn điều chỉnh/thay thế theo quy định hoá đơn điện tử hiện hành.
- Giá trên hoá đơn khớp giá bán sau voucher shop?

### 3b. meInvoice ↔ MISA AMIS (đã ghi sổ đủ chưa?)
- Tổng tiền hàng, thuế GTGT trên bảng kê = phát sinh Có 511, Có 3331 trong tháng?

### 3c. Sàn ↔ ngân hàng ↔ TK 131 (tiền về đủ chưa?)
- Tổng số tiền sàn thanh toán theo file = tổng tiền nhận trên sao kê (theo ngày thanh toán)?
- Số dư 131 chi tiết sàn cuối tháng = đơn đã hoàn thành nhưng sàn chưa trả + chênh lệch đã giải thích.

## Bước 4. Nguyên nhân chênh lệch hay gặp

| Hiện tượng | Nguyên nhân thường gặp |
|---|---|
| Sàn > meInvoice | Đơn hoàn thành chưa xuất hoá đơn; đơn cuối tháng hoàn thành đầu tháng sau |
| meInvoice > sàn | Xuất hoá đơn cho đơn sau đó bị huỷ/hoàn |
| Tiền về < doanh thu – phí | Phí quảng cáo/phạt trừ thẳng; đơn hoàn sau khi đã thanh toán; sàn giữ tiền |
| 131 sàn âm | Ghi tiền về nhưng chưa ghi doanh thu; ghi trùng phiếu thu |
| Phí sàn trong sổ ≠ file Income | Thiếu hoá đơn phí; ghi theo hoá đơn tháng khác |
| Voucher sàn bị trừ vào doanh thu | Hiểu sai voucher sàn là giảm giá của shop |

## Bước 5. Đầu ra

```
ĐỐI SOÁT [SÀN] – THÁNG [mm/yyyy] – nguồn: [tên file]

| Chỉ tiêu | File sàn | meInvoice | MISA AMIS | Ngân hàng | Chênh lệch | Giải thích |
|---|---|---|---|---|---|---|
| Số đơn hoàn thành | | | | – | | |
| Doanh thu theo giá bán | | | | – | | |
| Voucher shop | | | | – | | |
| Phí sàn | | – | | – | | |
| Phí quảng cáo | | – | | – | | |
| Hoàn trả | | | | – | | |
| Tiền sàn thanh toán | | – | | | | |
| Số hoá đơn đã xuất | – | | – | – | | |

Danh sách đơn lệch: [mã đơn – loại lệch – số tiền – việc cần làm]
Đề xuất bút toán điều chỉnh: [Nợ … / Có … – số tiền – lý do] (người hạch toán duyệt)
Hoá đơn cần xử lý: [xuất bổ sung / điều chỉnh / thay thế – mã đơn]
Việc cho tháng sau: [..]
```

Mọi số ghi rõ nguồn (file, sheet, cột). Chênh lệch ≠ 0 phải có giải thích hoặc `[cần kiểm tra]`.

## Lỗi hay gặp

- Đối soát theo **ngày đặt đơn** thay vì ngày hoàn thành/ghi nhận doanh thu → lệch kỳ.
- Cộng cả đơn huỷ (file "tất cả đơn") vào doanh thu.
- Ghi phí quảng cáo hai lần: một lần khi nạp tiền, một lần khi sàn trừ.
- Gộp Shopee và TikTok vào một đối tượng 131 → không truy được lệch.
