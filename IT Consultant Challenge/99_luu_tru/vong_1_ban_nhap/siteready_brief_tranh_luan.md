# Vì sao chọn SiteReady – brief tranh luận nhóm

Ta chọn lớp AI xử lý đơn hàng B2B (SiteReady) vì đây là phương án duy nhất đạt cùng lúc ba điều đề bài chấm: tác động lớn, dùng được cho cả ba nước, và ra mắt trong một quý.

## Pain point của Company A

Company A mất tiền và mất khách vì đơn hàng B2B được xử lý thủ công, mỗi nước một kiểu.

| Nước | Pain point chính | Ai chịu | Hệ quả |
| --- | --- | --- | --- |
| Đan Mạch | Nhập tay: đơn qua email, PDF, điện thoại bị gõ lại vào ERP, ~12 phút/đơn | Nhân viên trade desk, khách chờ xác nhận (~3 giờ) | Chi phí phục vụ cao, trả lời chậm nên mất đơn |
| Na Uy | Vận hành cửa hàng không đồng đều: mỗi cửa hàng chuẩn bị đơn một kiểu | Nhân viên cửa hàng và bãi hàng, khách đến lấy hàng | Đơn không sẵn đúng giờ, xếp hàng chờ, trải nghiệm thất thường |
| Thụy Điển | Giao hàng trễ, thiếu hàng, phải giao lại | Chỉ huy công trình, điều phối, tài xế | Thợ chờ vật tư (~€400/lần cho khách), mất khách thầu |
| Cả ba nước | Hệ thống phân mảnh: 3 ERP, không có mô hình đơn hàng chung | Ban lãnh đạo, IT | Cải tiến ở nước này không dùng lại được ở nước khác |

Tất cả quy về một điểm: khoảng 5% đơn nhập tay có lỗi (khoảng €120 mỗi lỗi), trong một thị trường cạnh tranh gay gắt, nơi khách thầu đổi nhà cung cấp chỉ sau vài lần giao hỏng. Các con số trên là giả định có nêu rõ, sẽ kiểm chứng ở giai đoạn discovery.

## SiteReady là gì — và không là gì

- **Là:** một lớp AI tiếp nhận và chuẩn hoá **đơn đặt hàng** của khách thầu xây dựng (B2B), chạy trên ERP sẵn có của cả ba nước.
- **Làm gì:** đọc đơn từ email, PDF, Excel hoặc ảnh → khớp từng dòng với mã sản phẩm (SKU) → kiểm tra lỗi (sai đơn vị, số lượng bất thường, thiếu địa chỉ công trình) → nhân viên duyệt dòng AI chưa chắc và bấm xác nhận → đơn đi thẳng vào ERP.
- **Không phải hệ thống kiểm kê hay quản lý kho:** SiteReady không đếm hàng. Nó chỉ đọc số tồn kho để báo cho khách biết còn hàng hay không.
- **Không phải ERP mới, cũng không phải portal bắt khách học cách dùng:** khách vẫn gửi đơn như hiện nay.
- **"Chuẩn hoá" nghĩa là:** đơn ở cả ba nước được đưa về cùng một định dạng, nên cải tiến làm ở Đan Mạch dùng lại được ở Na Uy và Thụy Điển.

## Bốn lập luận chính

1. **Đánh vào gốc rễ, không vào triệu chứng.** Nỗi đau của cả ba nước (nhập tay ở DK, cửa hàng ở NO, giao hàng ở SE) đều bắt nguồn từ khâu nhận đơn. Sửa khâu đầu thì lỗi giảm cho cả chuỗi (quy tắc 1-10-100). Đây đúng là tiêu chí "go beyond the surface".
2. **Bám sát ba ràng buộc của đề.** Đề yêu cầu "one digital solution", "time to market is critical" và "one strategic solution ≠ one identical implementation". Mô hình một lõi chung + module riêng từng nước trả lời thẳng cả ba.
3. **Dễ chứng minh giá trị nhất.** KPI đo được ngay từ tuần 9 (phút/đơn, tỷ lệ lỗi), MVP có nhóm cửa hàng đối chứng, và business case vẫn có lãi khi lợi ích chỉ đạt 50%.
4. **AI có vai trò thật, đúng gu giám khảo.** AI làm phần khó nhất (đọc đơn ba thứ tiếng, khớp SKU), chạy trên hạ tầng EU — khớp thông điệp "European sovereignty for the age of AI" của Netcompany, đơn vị ra đề và chấm bài.

## Vì sao không chọn các phương án khác

Mỗi phương án dưới đây đều có lý lẽ mạnh. Cách thuyết phục tốt nhất là công nhận điểm mạnh đó trước, rồi chỉ ra vì sao nó thua ở tiêu chí chấm điểm.

| Phương án | Lý lẽ mạnh nhất của phe ủng hộ | Phản biện của ta | Điểm (/5) |
| --- | --- | --- | --- |
| Hợp nhất / thay ERP | Giải quyết tận gốc "fragmented systems" | Đúng đích đến, sai bước đi: 2–3 năm mới có giá trị, trái với "time to market". Không thể làm MVP là "một ERP". SiteReady xây sẵn mô hình đơn hàng chung, tức viên gạch đầu tiên của việc hợp nhất. | 3.40 |
| App vận hành cửa hàng (Na Uy) | Chuẩn hoá quy trình, làm nhanh | Chỉ giúp một nước, giá trị khó quy ra tiền. Phần lớn hỗn loạn ở cửa hàng đến từ đơn thiếu hoặc sai từ đầu. Module "Prepare" vẫn có trong lộ trình. | 3.30 |
| RPA back-office (Đan Mạch) | Rẻ, nhanh, ít rủi ro | Tự động hoá một quy trình đang lỗi, dễ gãy khi giao diện đổi, không giúp gì cho khách hàng, gần như không có AI nên yếu ở tiêu chí Innovation. | 3.00 |
| Hệ thống giao hàng / tối ưu tuyến (Thụy Điển) | Giao hàng là thứ khách thấy rõ nhất | Phần mềm tối ưu tuyến mua sẵn được nên ít điểm sáng tạo. Chỉ giúp một nước, và chỉ tối ưu việc giao những đơn vốn đã sai. Module "Deliver" vẫn vào ngay đợt 1. | 2.95 |
| Portal / app đặt hàng cho khách B2B | Số hoá từ phía khách | Bắt thầu thợ đổi thói quen, rủi ro ít người dùng. Ta làm ngược lại: khách gửi kiểu gì, AI cũng đọc được. Portal để dành cho đợt 3. | — |

SiteReady đạt 4.20 điểm và vẫn đứng đầu khi giảm một nửa trọng số time to market (4.20 so với 3.90 của phương án ERP).

## Câu hỏi khó dự kiến

- **"Mỗi nước ưu tiên một thứ, sao lại chọn vấn đề của Đan Mạch?"** — Ta không chọn vấn đề riêng của Đan Mạch mà chọn khâu chung của cả ba nước. Đan Mạch chỉ là nơi pilot, vì nỗi đau nhập tay lớn nhất và gần trụ sở chính.
- **"Nhận đơn nghe nhỏ quá, có đủ impact không?"** — Khoảng 1.1 triệu đơn mỗi năm, giá trị ~€11.9M/năm (trong đó €5.9M là tiền cứng). Đơn hàng là đầu vào của mọi khâu phía sau.
- **"AI đọc sai thì sao?"** — Trong MVP, con người duyệt mọi đơn và có ngưỡng tin cậy. Chỉ tự động xác nhận sau khi pilot chứng minh độ chính xác ≥ 98%.
- **"Số liệu toàn giả định, giám khảo có bắt bẻ không?"** — Đề cho phép giả định nếu nêu rõ. Ta gắn mã A1–A8 cho từng con số và có phân tích độ nhạy ở mức 50%.
- **"Thế khác gì OCR bình thường?"** — OCR chỉ đọc chữ. Phần khó là khớp từ chuyên ngành ba thứ tiếng ("lægte", "läkt", "lekt") với khoảng 100.000 SKU và kiểm tra logic đơn hàng, việc này cần LLM kết hợp semantic search.

## Nhượng bộ và cách dẫn buổi thảo luận

Giữ chắc hướng giải, nhưng nhường những điểm không ảnh hưởng đến lập luận chính, để cả nhóm thấy ý kiến của mình được dùng.

**Sẵn sàng nhượng bộ:**

- Tên giải pháp, bố cục và thiết kế slide.
- Trọng số chấm điểm: mời mọi người tự chấm lại theo trọng số của họ.
- Số liệu: ai có benchmark hoặc nguồn tốt hơn thì thay vào giả định.
- Mức nhấn mạnh từng nước: có thể đẩy module "Deliver" (Thụy Điển) lên nổi bật hơn ở slide 9.

**Cách dẫn buổi thảo luận:**

1. Mở đầu bằng 5 tiêu chí chấm điểm của đề, không bằng ý kiến cá nhân: "Phương án nào đạt nhiều tiêu chí nhất?"
2. Để mọi người tự điền bảng chấm điểm, để con số nói thay mình.
3. Ghi nhận ý tưởng của từng người vào lộ trình (Deliver, Prepare, portal, ERP), để không ai thấy mình bị gạt bỏ.
4. Chốt hướng ngay trong buổi này: chỉ còn 3 ngày đến hạn nộp lúc 22:00 ngày 26/10/2026.
