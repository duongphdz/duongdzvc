# HDP AI Agents – 7 phòng ban

Bộ AI agent cho **Công ty TNHH Dược Phẩm Hoàng Dương (HDP)**, chia theo 7 phòng ban giống kế hoạch "7 Claude Project" đã tư vấn (thư mục Drive *Claude Projects - Hoang Duong*, cập nhật 21/10/2026).

Mỗi phòng ban có:

| Thành phần | Vị trí | Dùng để |
|---|---|---|
| Hướng dẫn agent (system prompt) | `.claude/agents/<phong-ban>.md` | Dán vào **Custom Instructions** của Claude Project, hoặc dùng trực tiếp làm subagent trong Claude Code |
| Mô tả phòng ban + danh sách tài liệu | `phong-ban/<nn>-<ten>/README.md` | Biết cần nạp file nào vào Project Knowledge |
| Mẫu (template) | `phong-ban/<nn>-<ten>/mau/` | Báo giá, brief, báo cáo… agent điền vào |
| Quy tắc dùng chung | `phong-ban/00-chung/` | Hồ sơ công ty, điều cấm nói khi quảng cáo, quy tắc bảo mật – nạp vào **cả 7** Project |

## Sơ đồ tổ chức

```
                     Quản lý (Phạm Hoàng Dương)
                     └─ CLAUDE.md  ← "điều phối": nhận việc, chuyển đúng phòng
                                │
 ┌──────────────┬───────────────┼───────────────┬──────────────┬──────────────┬──────────────┐
 01 Vận hành    02 Marketing    03 MBP &        04 Kế toán,    05 Điều hành,  06 Quảng cáo   07 Booking
 sàn Dodie      & nội dung      Lentin bán hàng kho & quỹ      admin, pháp lý & dữ liệu      KOC Dodie
 (Shopee,       Dodie           (nhà thuốc,     (MISA AMIS,    (hợp đồng,     (ROAS, ngân    (tiếp cận,
 TikTok Shop)                   đại lý, bác sĩ) meInvoice)     nội quy, KH)   sách ads)      brief, HĐ)
```

| # | Agent | Người nhận việc (thực hiện) | Việc chính |
|---|---|---|---|
| 01 | [`dodie-van-hanh-san`](.claude/agents/dodie-van-hanh-san.md) | NV vận hành sàn | Lịch sale, giá campaign, listing, đổi trả, trả lời khách |
| 02 | [`dodie-marketing-noi-dung`](.claude/agents/dodie-marketing-noi-dung.md) | Content & Design | Kịch bản video, caption, brief ảnh, kịch bản LIVE |
| 03 | [`mbp-lentin-ban-hang`](.claude/agents/mbp-lentin-ban-hang.md) | Field sale | Báo giá, kịch bản gặp nhà thuốc/bác sĩ, theo dõi công nợ |
| 04 | [`ke-toan-kho-quy`](.claude/agents/ke-toan-kho-quy.md) | Quản lý, thủ kho | Đối soát sàn, xuất nhập tồn, quỹ, báo cáo tháng |
| 05 | [`dieu-hanh-phap-ly`](.claude/agents/dieu-hanh-phap-ly.md) | Quản lý, Giám đốc | Hợp đồng, nội quy, kế hoạch năm, hồ sơ pháp lý |
| 06 | [`dodie-quang-cao-du-lieu`](.claude/agents/dodie-quang-cao-du-lieu.md) | Quản lý | Phân tích ROAS, xếp nhóm chiến dịch, báo cáo tuần |
| 07 | [`dodie-booking-koc`](.claude/agents/dodie-booking-koc.md) | Quản lý / CTV | Tìm, tiếp cận, brief, thoả thuận, theo dõi KOC |

> Nhân viên không dùng Claude. Quản lý dùng agent soạn brief/checklist/báo cáo, rồi giao việc qua Zalo hoặc Google Drive.

## Cách dùng

### A. Trên claude.ai (Claude Projects)

1. Tạo 7 Project, đặt tên theo bảng trên (ví dụ `01 · Dodie – Vận hành sàn`).
2. Mở file `.claude/agents/<phong-ban>.md`, copy **phần nội dung bên dưới dòng `---` thứ hai** vào ô *Custom instructions* của Project.
3. Ở *Project knowledge*: thêm các file trong `phong-ban/00-chung/` + các file được liệt kê trong `phong-ban/<nn>-<ten>/README.md` (chọn "Google Drive" rồi tìm theo tên).
4. Dữ liệu theo tháng (tồn kho, đơn hàng, lương…) **không** lưu vào Project – đính kèm vào từng hội thoại.

### B. Trong Claude Code (repo này)

Mở repo bằng Claude Code. File `CLAUDE.md` tự chuyển việc cho đúng subagent, hoặc gọi trực tiếp:

```
> Dùng agent dodie-booking-koc soạn tin nhắn tiếp cận cho 5 KOC mẹ bé tháng 11
> Dùng agent ke-toan-kho-quy đối soát file Income Shopee tháng 10 đính kèm
```

## Skill cho từng phòng

Xem [`phong-ban/skills-de-xuat.md`](phong-ban/skills-de-xuat.md): chọn từ *Claude Skills Ultimate Bundle*, chia theo phòng, đánh dấu dùng ngay / cần chỉnh / không dùng, kèm 10 skill nên cài trước.

## Bảo mật – repo này đang PUBLIC

Theo nội quy (bảo mật giá vốn, công thức tính lãi, danh sách khách hàng, tài khoản sàn), repo này **chỉ chứa hướng dẫn và mẫu trống**. Các số liệu sau nằm trên Drive, không đưa lên GitHub:

- Giá vốn, lãi gộp, ROAS hoà vốn từng nhóm (file *ALL ABOUT DODIE*)
- Bảng giá sỉ, chiết khấu, công nợ, danh sách khách hàng
- Hợp đồng đã ký, CCCD, số điện thoại, bảng lương

Nếu muốn lưu cả số liệu vào GitHub, hãy chuyển repo sang **Private** trước (Settings → General → Danger Zone → Change visibility).

## Việc còn thiếu (từ danh sách tài liệu 21/10/2026)

- [ ] `Dieu_cam_noi_khi_quang_cao` chưa có trên Drive → bản nháp ở [`phong-ban/00-chung/dieu-cam-noi-khi-quang-cao.md`](phong-ban/00-chung/dieu-cam-noi-khi-quang-cao.md), cần luật sư/quản lý duyệt
- [ ] Hệ thống tài khoản MISA AMIS, văn bản thuế mới nhất (04)
- [ ] Danh sách khách hàng MBP/Lentin, giấy xác nhận nội dung quảng cáo TPBVSK (03)
- [ ] Hồ sơ công bố Dodie và Lentin (05)
- [ ] Bản mẫu hợp đồng đã xoá thông tin cá nhân (05)
- [ ] 5–10 nội dung hiệu quả nhất (02), hạn đăng ký lịch sale (01), KPI tháng 11 (06)

---
*`person_map_website (1).html` là dự án cũ (PersonMap), không liên quan bộ agent.*
