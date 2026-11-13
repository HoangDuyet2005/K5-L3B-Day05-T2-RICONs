# Kế hoạch tự hoàn thành LAB5 — T2 Giáo dục

Kế hoạch này đi theo quy trình đầu-cuối của buổi lab: chuẩn bị bài và repo → thiết kế → prototype → rà soát → demo → nộp. Nó dựa trên `01-challenge-brief.md`, `02-guide.md`, `03-spec-template.md`, `04-rubric.md` và `tracks/t2-education.md`. Đây là lộ trình làm bài, không phải câu trả lời điền sẵn. Bạn tự quyết định nội dung; đánh dấu checklist khi hoàn thành.

## Quy trình tổng thể

1. **Xác nhận bối cảnh:** L3B, track T2; làm cá nhân. Ghi đúng thông tin cá nhân và việc bạn thực hiện. Nếu chưa rõ cách ghi thành viên/nộp bài cá nhân, hỏi TA, nhưng tiếp tục làm bài trong lúc chờ.
2. **Không fork repo đề bài.** Đề yêu cầu tạo một repo GitHub mới và trống; repo nộp chỉ chứa bài của bạn. Không clone/fork toàn bộ repo lab để nộp.
3. **Đặt tên repo:** `K5-L3B-Day05-T2-<ten-nhom>`. Vì làm cá nhân, chọn một hậu tố ngắn, liền không dấu, không khoảng trắng (chẳng hạn tên riêng viết liền); đừng tự nhận là một nhóm nếu chưa có tên nhóm.
4. **Tạo repo mới trên GitHub:** chọn New repository, nhập tên đúng, đặt Public. Theo hướng dẫn, để repo trống lúc tạo (không khởi tạo README/license nếu muốn giữ đúng yêu cầu repo trống). Chưa cần gửi link cho ai.
5. **Làm bài trong workspace/thư mục riêng:** dùng `03-spec-template.md` làm nguồn để tạo `spec.md`; không đưa các file hướng dẫn khác vào repo bài nộp. Tạo `prototype/` cho file/link prototype và 1–2 ảnh có đánh số.
6. **Hoàn tất và rà rubric** theo các chặng dưới đây. Giữ dữ liệu dựng, không thêm dữ liệu cá nhân thật.
7. **Đưa đúng deliverable lên repo mới:** `spec.md` và `prototype/` là cấu trúc tối thiểu. Commit/push các thay đổi lên repo GitHub mới; không đưa toàn bộ tài liệu lab vào repo nộp.
8. **Kiểm tra như người chấm:** mở repo ở cửa sổ ẩn danh để chắc chắn Public; mở `spec.md`, prototype, ảnh và link; kiểm tra tên repo, lớp/track, mã học viên, link không hỏng.
9. **Demo rồi nộp:** trình bày ca khó, tự chủ và phản ứng với ca lạ; gửi link repo qua đúng kênh giảng viên thông báo, trước 23:59 ngày 13/11/2026. Nếu TA đưa ca lạ hoặc góp ý, ghi lại kết quả thật trong §7 rồi cập nhật/push trước khi nộp nếu còn thời gian.

> Nếu đã lỡ fork repo lab, đừng dùng fork đó làm repo nộp. Tạo repo mới, trống theo các bước trên rồi chỉ chuyển `spec.md` và thư mục `prototype/` sang repo mới.

## Mục tiêu và yêu cầu nộp

- Hoàn thành `spec.md` theo template, từ §1 đến §7, có bảng thành viên/việc làm ghi đúng thực tế cá nhân.
- Dựng prototype 1–2 màn hình bấm được cho một ca khó; kèm 1–2 ảnh đánh số và chú thích.
- Tạo repo GitHub mới, công khai, tên dạng `K5-L3B-Day05-T2-<ten-nhom>`; nộp link theo kênh lớp trước 23:59 ngày 13/11/2026. Không fork repo đề bài.
- Đề ghi nhóm đúng 3 người nhưng bạn làm cá nhân. Không bịa thành viên hay phần việc; hỏi TA/giảng viên cách ghi bảng nếu cần, đồng thời vẫn tiếp tục làm bài.
- Chỉ dùng dữ liệu dựng trong track. Không cần API hay lời gọi AI thật.

## Kế hoạch 240 phút


| Chặng            | Phút | Đầu ra                                                                                   | Mốc kiểm soát                                       |
| ---------------- | ----: | ---------------------------------------------------------------------------------------- | --------------------------------------------------- |
| 0. Chuẩn bị      | 10   | Xác nhận thông tin, tạo repo mới trống/Public đúng tên, tạo nháp `spec.md`, chọn công cụ | Repo cá nhân sẵn sàng, không fork repo lab          |
| 1. Đọc đề        | 10   | §1: lát cắt và 3 điều tính năng không làm                                                | Nói rõ người dùng, việc, quyết định AI, hậu quả sai |
| 2. Kịch bản      | 35   | §2: ≥8 ca, đủ 4 lớp, chọn 2 ca đắt nhất                                                  | **M1:** bằng chứng cụ thể cho mỗi ca                |
| 3. UX khi AI sai | 45   | §3: thiết kế phản hồi đầy đủ cho 2 ca đắt nhất                                           | Có câu AI nguyên văn, bước tiếp, căn cứ, đường lui  |
| 4. Mức tự chủ    | 35   | §4: xếp mức tất cả tool, thử 3 ca                                                        | **M2:** lý do cost-of-error và tool khó xếp         |
| Nghỉ             | 15   | Lưu bản nháp, nghỉ mắt                                                                   | Nội dung đã lưu                                     |
| 5. Prototype     | 60   | §5 và prototype 1–2 màn hình                                                             | **M3:** bấm hết ca khó, thấy ≥2 mức tự chủ          |
| 6. Tiêu chí đạt  | 10   | §6: 3 tiêu chí Pass/Fail, chấm trên 2 ca                                                 | Tiêu chí quan sát/chấm được                         |
| 7. Demo và nộp   | 20   | §7, ảnh, kiểm tra repo và link                                                           | Mọi thứ mở được, demo nhất quán với spec            |


Tổng 240 phút. Nếu thiếu giờ, rút gọn §6 trước; giữ thời gian cho §3–§5 vì chúng chiếm phần lớn điểm. Chặng cuối gồm cả demo và thao tác commit/push, nên chuẩn bị repo từ đầu.

## Chặng 0 — Chuẩn bị (10 phút)

1. Mở `tracks/t2-education.md`, `03-spec-template.md`, `04-rubric.md`.
2. Tạo repo GitHub **mới và trống**, không fork repo bài lab; đặt tên theo mẫu `K5-L3B-Day05-T2-<ten-nhom>`, chọn Public.
3. Tạo bản nháp `spec.md` theo template, để trống các phần chưa làm.
4. Chọn công cụ prototype sẵn dùng (HTML, Figma hoặc công cụ đã đăng ký).

**Đạt khi:** repo mới đúng tên/Public, có nháp §1–§7 và biết sẽ dựng prototype bằng gì.

## Chặng 1 — Đọc đề (10 phút)

1. Đọc lát cắt, tool, dữ liệu dựng, tin mồi và Hard tests của T2.
2. Tự viết lại lát cắt theo khung: một người dùng · một việc · một quyết định AI · một kết quả.
3. Ghi 3 việc tính năng không làm; mỗi việc kèm lý do theo thẩm quyền, dữ liệu hoặc hậu quả khi sai.
4. Ghi các bằng chứng có thể cần trích về sau: tài liệu buổi 3 có mục §3.1–§3.5 (không có slide đánh số); lịch khóa học, giờ TA và trạng thái/hạn bài tập; bảng tool.

**Đạt khi:** §1 đúng phạm vi T2, không biến thành trợ lý học tập không giới hạn.

## Chặng 2 — Kịch bản rủi ro (35 phút, M1)

1. Dùng ba tin mồi và Hard tests để viết tin nhắn tự nhiên: thiếu thông tin, hiểu nhầm, hoặc gộp nhiều câu hỏi.
2. Tạo ít nhất 8 dòng trong §2; mỗi dòng có: tin nhắn · lớp · AI có thể sai thế nào · sản phẩm tốt nên làm gì · nhãn mức hại.
3. Phủ bốn lớp: ① nguồn sự thật (tài liệu không nói) · ② mơ hồ/thiếu dữ kiện · ③ ngoài phạm vi/thẩm quyền · ④ rủi ro học sai, chép đáp án hoặc ảnh hưởng cả lớp.
4. Mỗi lỗi phải gắn với tool/dữ kiện cụ thể hoặc nói rõ dữ liệu nào không có. Tránh câu chung như “AI có thể sai”.
5. Chọn 2 ca đắt nhất, giải thích vì sao đắt hơn các ca còn lại; ghi một ca suýt chọn và lý do loại.

**M1 đạt khi:** ≥8 ca, đủ 4 lớp, mỗi ca có bằng chứng và phản ứng tốt; 2 ca đắt nhất có lý do.

## Chặng 3 — UX khi AI sai (45 phút)

Chỉ làm sâu 2 ca đắt nhất.

1. Với từng ca, cân nhắc: hỏi lại · trả lời có giới hạn/căn cứ · dừng và chuyển TA/hướng dẫn hỏi giảng viên. Chọn một hướng và giải thích vì sao loại hai hướng kia.
2. Viết nguyên văn câu AI sẽ nói. Nêu căn cứ, điều chưa biết và giới hạn; không bịa nguồn.
3. Ghi người học thấy gì ngoài câu chữ: mục tài liệu, trạng thái thiếu căn cứ/độ chắc, lựa chọn tiếp theo.
4. Ghi người học làm gì tiếp: bổ sung câu hỏi, xem nguồn, sửa phản hồi, chờ TA hoặc dừng.
5. Nếu chuyển TA: ai nhận, nhận thông tin nào, thời gian/giờ phản hồi và chuyện gì khi ngoài giờ.
6. Phân loại lỗi hệ thống / người dùng / ngữ cảnh; nêu cách xin lỗi và khắc phục tương ứng.
7. Chọn 2–3 nguyên tắc HAX/PAIR. Mỗi nguyên tắc phải chỉ vào câu hoặc thành phần giao diện cụ thể.
8. Nêu lỗi mà câu chữ không thể cứu và cơ chế thiết kế giúp ngăn/giảm lỗi.

**Đạt khi:** hai ca có câu AI nguyên văn, căn cứ, bước tiếp, người được báo nếu có, phương án bị loại và lý do.

## Chặng 4 — Mức tự chủ (35 phút, M2)

1. Liệt kê đủ tool T2: `tra_cuu_tai_lieu`, `goi_y_bai_tap`, `chuyen_TA`, `dang_FAQ`.
2. Đặt mỗi tool một mức: **tự làm / cần người duyệt / cấm**.
3. Với mỗi tool, ghi ai chịu hậu quả, có đảo ngược được không, chờ duyệt gây thiệt hại gì, đã cân nhắc mức nào khác và vì sao loại.
4. Với tool cần duyệt, ghi ai duyệt, họ thấy gì trước khi bấm, quá hạn thì sao.
5. Chọn tool khó xếp nhất. Vì làm cá nhân, ghi các phương án bạn tự cân nhắc và cái giá của mỗi phương án; không dựng ý kiến thành viên khác.
6. Thử mức đã chọn trên hai ca đắt nhất và một ca bình thường. Trả lời: sai có bị chặn không? AI còn làm khi đáng ra phải hỏi không? Người dùng thường có phải chờ vô ích không?
7. Ghi một mức tự chủ đã làm thay đổi lời hứa với học viên như thế nào.

**M2 đạt khi:** mọi tool có mức/lý do; có phân tích tool khó xếp; đã thử 3 ca theo đủ ba câu hỏi.

## Nghỉ (15 phút)

Lưu nháp, nghỉ mắt và bảo đảm còn đủ 60 phút cho prototype. Không mở rộng phạm vi.

## Chặng 5 — Prototype (60 phút, M3)

1. Chọn một ca đắt nhất làm luồng prototype; phác các trạng thái: câu hỏi → căn cứ/thiếu căn cứ → quyết định AI → hành động tiếp.
2. Dựng 1–2 màn hình bấm được, dùng dữ liệu giả từ track. Không cần backend hay AI thật.
3. Hiện căn cứ cụ thể, chẳng hạn tên tài liệu và mục §3.x nếu đó là căn cứ. Không bịa số trang/slide.
4. Thể hiện mức tự chủ đã chốt: xác nhận trước hành động cần duyệt; đường chuyển TA; không đặt nút cho hành động bị cấm; có sửa/hoàn tác nếu thiết kế yêu cầu.
5. Đánh số 1–2 chỗ thể hiện nguyên tắc HAX/PAIR; chụp ảnh và ghi chú trong §5.
6. Bấm luồng từ đầu tới cuối; sửa nếu giao diện cho phép hành động trái §3–§4.
7. Trong §5 ghi link/file, công cụ, phần mock và có/không có lời gọi AI thật.

**M3 đạt khi:** ca khó bấm hết được, căn cứ hiển thị, ít nhất hai mức tự chủ hiện rõ và HAX/PAIR trỏ được vào vị trí cụ thể.

## Chặng 6 — Tiêu chí tốt (10 phút)

1. Viết 3 tiêu chí Pass/Fail có thể quan sát, không dùng tiêu chí cảm tính.
2. Chấm thiết kế trên 2 ca đắt nhất.
3. Ghi lỗi còn lại/điều kiện chưa đạt.

**Đạt khi:** người khác có thể chấm tiêu chí mà không phải đoán ý bạn.

## Chặng 7 — Demo và nộp (25 phút)

1. Chuẩn bị mở đầu 30 giây: lát cắt, người dùng, lỗi đắt nhất.
2. Bấm prototype qua ca khó; chỉ rõ căn cứ, mức tự chủ, đường sửa/chuyển người.
3. Thử trả lời một ca lạ theo chính sách §3–§4; không tuyên bố demo đã diễn ra nếu chưa demo.
4. Hoàn thiện §7, bảng thành viên và việc làm đúng thực tế.
5. Đưa `spec.md` và `prototype/` (file/link cùng ảnh đánh số) lên repo mới; commit/push.
6. Kiểm tra repo đúng tên/công khai; mở được bằng cửa sổ ẩn danh; kiểm tra `spec.md`, prototype, ảnh, link, lớp/track và mã học viên.
7. Gửi link repo qua đúng kênh giảng viên thông báo, trước hạn.

## Checklist theo tiến độ

- [ ] Repo GitHub mới, trống lúc tạo, Public, đúng tên; không dùng fork repo lab.
- [ ] Có bản nháp `spec.md` và chọn công cụ.
- [ ] §1: lát cắt, phạm vi, 3 điều không làm.
- [ ] §2: ≥8 kịch bản, đủ 4 lớp, 2 ca đắt nhất (**M1**).
- [ ] §3: phản hồi chi tiết cho hai ca; HAX/PAIR gắn với chỗ cụ thể.
- [ ] §4: mức cho mọi tool; thử 3 ca; phân tích tool khó xếp (**M2**).
- [ ] §5: prototype bấm được, căn cứ và ≥2 mức tự chủ (**M3**).
- [ ] §6: ba Pass/Fail và chấm thử hai ca.
- [ ] §7: demo/ca lạ được chuẩn bị trung thực.
- [ ] Bảng thành viên ghi đúng thực tế; cách nộp cá nhân được làm rõ nếu cần.
- [ ] `spec.md` và `prototype/` đã commit/push lên repo nộp; repo mở được ở cửa sổ ẩn danh.
- [ ] Link repo đã gửi đúng kênh trước hạn.

## Rà soát nhanh theo rubric


| Khối                 | Tự kiểm                                                                                        |
| -------------------- | ---------------------------------------------------------------------------------------------- |
| R1 · Phạm vi (5)     | Đúng lát cắt T2 và có ≥3 việc không làm kèm lý do?                                             |
| R2 · Rủi ro (10)     | ≥8 ca, đủ lớp, bằng chứng cụ thể, có hai ca đắt nhất và ca suýt chọn?                          |
| R3 · UX khi sai (25) | Hai ca có câu nguyên văn, căn cứ, bước tiếp, loại lỗi, đường lui và lý do loại phương án khác? |
| R4 · Tự chủ (25)     | Mọi tool có mức/lý do theo hậu quả, khả năng đảo và chi phí chờ; đã thử 3 ca?                  |
| R5 · Prototype (25)  | Bấm được, có căn cứ, mức tự chủ rõ, ảnh chú thích trỏ được HAX/PAIR?                           |
| R6 · Tiêu chí (5)    | Ba tiêu chí Pass/Fail và kết quả trên hai ca đắt nhất?                                         |
| R7 · Demo (5)        | Demo/ca lạ nhất quán với chính sách; giải thích được phần mình làm?                            |


