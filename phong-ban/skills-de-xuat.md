# Skill đề xuất cho 7 phòng ban

Nguồn: *Claude Skills Ultimate Bundle* (khoảng 500 skill, 20 nhóm, tiếng Anh). Đánh giá ngày 25/10/2026.

## Nhận xét chung về bộ skill

- Mỗi skill là một file `SKILL.md`: quy trình nhiều bước, có điểm dừng để hỏi thông tin (GATE), mẫu đầu ra và lỗi hay gặp. Không có script chạy được. Mình đã rà và không thấy lệnh tải hay chạy gì từ bên ngoài.
- **Viết cho thị trường Mỹ**: ví dụ dùng Amazon/Etsy/Shopify, tiền $, luật FDA/FTC/IRS. Phần cấu trúc dùng được, còn phần **luật và thuế thì không áp dụng** cho Việt Nam.
- Khoảng 20 skill yêu cầu Notion/Canva (`content-calendar`, `sop-builder`, `kpi-dashboard`, `expense-tracker`…). HDP làm việc trên Drive và Zalo nên **không ưu tiên** các skill này.
- Khi skill và agent mâu thuẫn, **agent thắng**: quy tắc chung, điều cấm nói khi quảng cáo, ROAS hoà vốn, brand guideline Dodie luôn được ưu tiên hơn ví dụ trong skill.

Ký hiệu: ✅ dùng ngay · 🔧 dùng được nhưng phải bỏ phần nước ngoài · ⛔ không dùng

## 01 · Vận hành sàn Dodie

| Skill | Mức | Dùng cho |
|---|---|---|
| `discount-strategy` | ✅ | Kiểm giá Spike/Minispike: có "sàn biên lợi nhuận" và lượng bán cần thêm để hoà vốn; khuyên combo/quà thay vì giảm sâu, khớp brand guideline |
| `bundle-creator` | ✅ | Thiết kế combo (bình + núm, bộ FIRST CARE), giá combo, kiểm lãi |
| `flash-sale-campaign` | 🔧 | Kế hoạch FS/LIVE ngày đôi; bỏ phần email, giữ lịch đếm ngược và phối hợp kênh |
| `seasonal-campaign` | 🔧 | Lịch 11.11, 12.12, Tết; thay lịch lễ Mỹ bằng lịch sale sàn |
| `product-listing-optimizer` | 🔧 | Tên, mô tả, ảnh listing; thay quy tắc Amazon bằng giới hạn ký tự Shopee/TikTok |
| `product-faq` | ✅ | Bộ câu hỏi trước khi mua (núm mức mấy, PP hay thuỷ tinh…) |
| `support-response-templates` | ✅ | Mẫu trả lời chat theo tình huống, có lúc nào cần chuyển quản lý |
| `complaint-resolution` | ✅ | Xử lý khiếu nại, đánh giá 1–2 sao, phương án bù đắp |
| `review-response` | ✅ | Trả lời đánh giá trên sàn |
| `exchange-policy` | ✅ | Viết chính sách đổi trả của shop (phần còn trống ở mẫu lịch sale) |
| `seasonal-inventory-plan` | ✅ | Dự báo hàng trước đợt sale lớn, xả hàng cận date |
| `return-policy` | ⛔ | Nặng luật Mỹ; dùng `exchange-policy` |
| `marketplace-listing` | ⛔ | Chỉ cho Etsy/Amazon/eBay |

## 02 · Marketing & nội dung Dodie

| Skill | Mức | Dùng cho |
|---|---|---|
| `tiktok-script` | ✅ | Kịch bản video 15–90s: hook, text, cảnh quay (dùng cùng `mau/kich-ban-video.md`) |
| `hook-generator` | ✅ | Tạo 10–20 hook từ câu hỏi hay gặp của mẹ |
| `short-form-video-plan` | ✅ | Kế hoạch 30 ngày video TikTok, giải quyết vấn đề "2–5 bài/tháng" |
| `caption-writer` | ✅ | Caption TikTok/Facebook/Shopee Feed |
| `social-media-calendar` | ✅ | Lịch nội dung tuần/tháng (không cần Notion) |
| `content-pillar-strategy` | ✅ | Trụ cột nội dung theo FIRST FEED / SOOTHE / CARE / MOM |
| `customer-persona` | ✅ | Hoàn thiện chân dung khách mẹ 25–35 và người mua quà |
| `product-photography-brief` | 🔧 | Danh sách cảnh chụp sản phẩm; thêm quy chuẩn 1200×1200, gradient nền |
| `brand-voice-guide` | ✅ | Viết đầy đủ bộ quy tắc giọng văn Dodie từ brand guideline |
| `user-generated-content` | ✅ | Chiến dịch mẹ gửi ảnh/video dùng thật |
| `competitor-analysis` | 🔧 | Phân tích đối thủ để định vị nội bộ; **không** đưa tên đối thủ vào nội dung đăng |
| `crisis-comms` | ✅ | Khủng hoảng (khách tố lỗi sản phẩm, video tiêu cực) |
| `content-calendar` | ⛔ | Bắt buộc Notion + Canva |

## 03 · MBP & Lentin – Bán hàng

| Skill | Mức | Dùng cho |
|---|---|---|
| `sales-script` | ✅ | Kịch bản gặp nhà thuốc, gọi điện, nhắn Zalo |
| `discovery-call-script` | ✅ | Câu hỏi khai thác nhu cầu nhà thuốc/đại lý |
| `objection-handler` | ✅ | Xử lý từ chối: "giá cao", "khách không hỏi", "đang bán hãng khác" |
| `sales-battlecard` | ✅ | Thẻ so sánh MBP với sản phẩm canxi khác (chỉ dùng nội bộ cho sale) |
| `wholesale-catalog` | ✅ | Catalogue sỉ: bậc giá, số lượng tối thiểu, chiết khấu |
| `customer-segmentation` | ✅ | Chia nhà thuốc/đại lý/bác sĩ theo doanh số, tần suất |
| `payment-terms-policy` | ✅ | Chính sách công nợ, nhắc nợ quá hạn |
| `commission-structure` | ✅ | Hoa hồng cho field sale, đại lý |
| `supplement-disclaimer` | ⛔ | Viết theo FDA Mỹ; ở Việt Nam dùng `dieu-cam-noi-khi-quang-cao.md` và giấy xác nhận nội dung quảng cáo |
| `health-disclaimer` | ⛔ | Cho phòng gym/thể hình ở Mỹ |

## 04 · Kế toán, kho & quỹ

| Skill | Mức | Dùng cho |
|---|---|---|
| `inventory-management` | ✅ | Điểm đặt hàng lại, phân loại ABC, cảnh báo hết hàng/cận date |
| `cash-flow-forecast` | ✅ | Dự báo dòng tiền 3–12 tháng (tiền sàn về chậm, nhập hàng theo lô) |
| `profit-loss-report` | 🔧 | Lãi lỗ theo nhãn/kênh; thay mẫu Mỹ bằng TK 511/632/641 |
| `cost-analysis` | ✅ | Giá vốn từng đơn vị gồm nhập khẩu, thuế, vận chuyển |
| `unit-economics` | ✅ | Lãi trên mỗi đơn sàn sau phí, voucher, hoa hồng KOC |
| `breakeven-analysis` | ✅ | Hoà vốn theo nhãn, theo tháng (chi phí cố định) |
| `budget-planner` | ✅ | Ngân sách năm/tháng, theo dõi chênh lệch |
| `financial-dashboard` | ✅ | Khung báo cáo 1 trang cho Giám đốc |
| `bookkeeping-setup` | ⛔ | Hệ tài khoản Mỹ; HDP dùng MISA AMIS theo TT133/TT200 |
| `tax-prep-checklist`, `expense-tracker`, `invoice-template` | ⛔ | Thuế Mỹ / Notion; hoá đơn dùng MISA meInvoice |

## 05 · Điều hành, admin & pháp lý

| Skill | Mức | Dùng cho |
|---|---|---|
| `annual-planning` | ✅ | Kế hoạch năm 2027 (khớp mẫu kế hoạch năm) |
| `okr-builder` | ✅ | Mục tiêu quý cho từng vị trí |
| `employee-handbook` | 🔧 | Sổ tay nhân viên; bỏ quy định Mỹ, căn cứ Bộ luật Lao động 2019 |
| `job-posting`, `interview-question-bank`, `hiring-scorecard` | ✅ | Tuyển NV sàn, content, sale |
| `onboarding-checklist` | 🔧 | Ngày đầu đi làm; bỏ phần phúc lợi Mỹ |
| `performance-review` | ✅ | Đánh giá nhân viên theo quý/năm |
| `training-manual` | ✅ | Sổ tay đào tạo NV sàn, CTV livestream |
| `delegation-framework` | ✅ | Ma trận giao việc Quản lý → nhân viên |
| `weekly-report` | ✅ | Gộp báo cáo cuối ngày thành báo cáo tuần cho Giám đốc |
| `risk-assessment` | ✅ | Rủi ro: hàng cận date, phụ thuộc sàn, vi phạm quảng cáo |
| `nda-template` | 🔧 | Thoả thuận bảo mật với CTV, đối tác (cần đối chiếu luật VN) |
| `contract-writer`, `independent-contractor-agreement` | 🔧 | Chỉ lấy danh sách điều khoản cần có; văn bản dùng mẫu HĐ Việt Nam hiện có |
| `vendor-evaluation` | 🔧 | So sánh đối tác gửi bán, đơn vị vận chuyển |
| `compliance-checklist`, `offer-letter`, `workplace-policy` | ⛔ | Luật lao động/quy định Mỹ |

## 06 · Phân tích quảng cáo & dữ liệu

| Skill | Mức | Dùng cho |
|---|---|---|
| `ad-performance-report` | ✅ | Báo cáo ROAS/CPA theo sàn, nội dung tốt/kém (đổi $ → đ, dùng ROAS hoà vốn của HDP) |
| `ad-spend-calculator` | ✅ | Từ doanh thu mục tiêu → ngân sách ads cần chi |
| `metric-definition-guide` | ✅ | Bổ sung bảng định nghĩa chỉ số hiện có |
| `conversion-funnel-analysis` | ✅ | Phễu xem → click → giỏ → đơn trên Shopee/TikTok |
| `ab-test-plan` | ✅ | Thử ảnh bìa, giá, hook video |
| `tiktok-ad-script` | ✅ | Kịch bản quảng cáo kiểu UGC, Spark Ads từ video KOC |
| `ad-creative-brief` | ✅ | Brief ảnh/video quảng cáo cho phòng 02 |
| `customer-lifetime-value` | ✅ | Giá trị khách mua lại (núm thay định kỳ, hoá mỹ phẩm) |
| `roi-calculator` | ✅ | Đánh giá hiệu quả một khoản đầu tư (LIVE, KOC, booth) |
| `retargeting-strategy` | 🔧 | Bám đuổi khách đã xem; thay Facebook Pixel bằng công cụ quảng cáo của sàn |
| `kpi-dashboard` | ⛔ | Bắt buộc Notion; đã có mẫu báo cáo tuần |

## 07 · Booking KOC

| Skill | Mức | Dùng cho |
|---|---|---|
| `influencer-campaign-brief` | ✅ | Brief chiến dịch KOC: nội dung bàn giao, thông điệp, điều không nói, quy trình duyệt |
| `influencer-outreach` | ✅ | Tin nhắn tiếp cận, nhắc lại, các kiểu trả phí |
| `affiliate-recruitment` | 🔧 | Tuyển affiliate TikTok Shop số lượng lớn; bỏ phần email/landing page |
| `affiliate-terms` | 🔧 | Điều khoản affiliate (đơn huỷ/hoàn, cách làm bị cấm) |
| `collaboration-agreement` | 🔧 | Bổ sung điều khoản cho thoả thuận KOC 9 điều |
| `rate-negotiation-script` | 🔧 | Viết cho freelancer tự định giá; đảo lại thành kịch bản thương lượng phía thương hiệu |
| `user-generated-content` | ✅ | Thu thập, xin quyền dùng lại video của khách/KOC |
| `freelancer-management` | ✅ | Quản lý nhiều KOC/CTV cùng lúc: brief, góp ý, thanh toán |
| `affiliate-program` | ⛔ | Viết cho chương trình affiliate riêng của website; TikTok Shop đã có hệ thống |

## Cách cài

**claude.ai**: Customize → Skills → tải từng thư mục skill lên. Skill bật theo **tài khoản**, không theo Project; mỗi agent đã ghi rõ nên dùng skill nào.

**Claude Code** (chỉ cho repo này):

```bash
# chạy trên máy, thay <BUNDLE> bằng đường dẫn thư mục đã giải nén
for s in discount-strategy bundle-creator tiktok-script hook-generator ad-performance-report influencer-campaign-brief; do
  cp -r "<BUNDLE>"/*/"$s" .claude/skills/
done
```

> ⚠️ Repo đang public, còn bộ skill là sản phẩm có bản quyền của tác giả. **Không** commit các thư mục skill lên repo này. Hãy cài trên máy hoặc trong tài khoản claude.ai, hoặc chuyển repo sang Private.

## Nên bắt đầu với 10 skill này

1. `discount-strategy` (01) – ngay trước 11.11
2. `bundle-creator` (01)
3. `tiktok-script` (02)
4. `hook-generator` (02)
5. `objection-handler` (03)
6. `inventory-management` (04)
7. `cash-flow-forecast` (04)
8. `ad-performance-report` (06)
9. `influencer-campaign-brief` (07)
10. `influencer-outreach` (07)

## Skill tiếng Việt của công ty (đã viết, nằm trong repo)

Bộ Ultimate Bundle không có 4 skill dưới đây nên công ty tự viết, lưu ở `.claude/skills/`. Khi trùng việc với skill của bộ, ưu tiên 4 skill này.

| Skill | Phòng dùng | Thay cho / bổ sung |
|---|---|---|
| [`kiem-tra-quang-cao-vn`](../.claude/skills/kiem-tra-quang-cao-vn/SKILL.md) | 02, 03, 06, 07 (bắt buộc) | Thay `supplement-disclaimer` (luật FDA Mỹ): rà TPBVSK, bình bú/núm ti, mỹ phẩm, nội dung KOC |
| [`kich-ban-live-ban-hang`](../.claude/skills/kich-ban-live-ban-hang/SKILL.md) | 01, 02, 07 | Bộ không có skill livestream |
| [`dang-ky-campaign-san`](../.claude/skills/dang-ky-campaign-san/SKILL.md) | 01, 06 | Kết hợp với `discount-strategy`; tính lãi gộp sau phí sàn, voucher cộng dồn |
| [`doi-soat-san-meinvoice-misa`](../.claude/skills/doi-soat-san-meinvoice-misa/SKILL.md) | 04 | Thay `bookkeeping-setup` (chuẩn Mỹ) |

Cài trên claude.ai: nén từng thư mục trong `.claude/skills/` thành file .zip rồi tải lên Customize → Skills. Trong Claude Code, các skill này tự có hiệu lực khi mở repo.
