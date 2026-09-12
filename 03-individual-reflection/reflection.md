# 03 — Individual Reflection

> Viết bằng lời của bạn (Phase 7 trong `01-worksheet.md`). Có thể dùng AI gợi ý câu hỏi tự soi, không dùng AI viết thay. 8-12 câu, có chuyện cụ thể.

## Thông tin cá nhân

- Họ và tên: Phạm Thanh Sơn
- Mã học viên: 2A202602794
- Nhóm: A-04
- Candidate problem nhóm chọn: Chuẩn hóa và cào dữ liệu từ nhiều nguồn (iPOS, Ads Nyna, Định biên nhân sự) để làm weekly report — Data Analyst mất ~2h/lần vì chờ HR gửi số và phải copy-paste thủ công từ 3 nguồn lệch format.

---

## 1. Tôi đã tham gia vào phần nào?

Ghi việc cụ thể + kết quả cụ thể. Không ghi chung chung kiểu "tham gia thảo luận".

| Hoạt động | Tôi đã làm gì? (việc cụ thể) | Kết quả / ảnh hưởng tới nhóm |
|---|---|---|
| Scan cá nhân | Scan 10 problems từ công việc DA thực tế (IPOS, KPI, Ads, data cleaning Shopee/Lazada/TikTok), dùng đủ 4 lăng kính | Nhóm có 3 candidates chất lượng cao từ domain e-commerce DA — Cluster A (gom/chuẩn hóa data) hình thành từ đây |
| Pitch Problem Card | Pitch Card #1 (tổng hợp báo cáo từ iPOS/Ads/định biên): trình bày workflow 7 bước, chứng minh ~2h/lần bằng ví dụ cụ thể từng bước | Card được nhóm đánh giá 35/35 điểm và chọn làm candidate chính của nhóm |
| Challenge bài của bạn khác | Hỏi Võ Đức Tài: "Paper analysis bottleneck nặng nhưng cả nhóm có đủ context để validate và research tool không?" | Nhóm thống nhất loại bài paper analysis vì domain riêng, chỉ 1 người có pain — tránh phụ thuộc |
| Gom trùng / cluster | Gom Card #1 (báo cáo dashboard), Card #2 (data cleaning Shopee/Lazada), Card Phan Duy Thành #2 (thu chi Grab) vào Cluster A: "gom/nối data từ nhiều nguồn rồi chuẩn hóa thủ công" | Nhóm thấy pattern chung: pain không nằm ở phân tích mà ở bước kéo + chuẩn hóa data thủ công |
| Chọn candidate problem | Lập luận chọn Card #1 thay vì Card #2 (Shopee/Lazada): Card #1 có impact cao hơn (~10h/tuần vs ~3h/tuần), workflow chi tiết hơn, và có API để pilot ngay | Nhóm chốt Card #1 và thu hẹp scope: chỉ làm bước cào + chuẩn hóa, không làm phân tích hay dashboard |
| Validation / research | Dẫn ra case "API iPOS cần kiểm tra phân quyền trước khi build" và đề xuất dùng Power Query làm non-AI alternative | Nhóm thêm non-AI alternative rõ ràng và note "giả định API accessible" vào field Boundary của PS |
| Workflow nhóm | Vẽ current state 7 bước (có thời gian từng bước), tách bottleneck thành 2 loại riêng: (1) chờ HR và (2) copy-paste/chuẩn hóa | Nhóm dùng làm workflow bản cuối; future workflow 5 bước rõ boundary tại bước DA duyệt |
| Problem Statement | Đóng góp field Bottleneck (tách "chờ người" khác hẳn "chuẩn hóa thủ công" về giải pháp) và field Boundary ("chỉ làm bước cào + chuẩn hóa, không làm insight, không build dashboard") | PS v1 rõ hơn về phạm vi — tránh scope creep sang phân tích và dashboard |
| Rule / Workflow / Agent | Lập luận chọn Workflow (Rule đủ cho phần lớn nhưng không đủ cho tên lạ; Agent quá rộng); AI chỉ hỗ trợ bước gợi ý khớp tên lạ | Nhóm thống nhất Workflow, không bị kéo sang Agent |
| Decision | Đề xuất pilot 3 số đo cụ thể: precision extract, recall extract, và thời gian đọc digest vs làm tay | Nhóm có exit condition rõ: nếu AI gợi ý sai ≥2 lần trong 2 tuần → rollback về Rule/mapping thuần |

**Dấu tay rõ nhất của tôi trong artifact cuối (1-2 câu):**

```text
Bài của tôi (Card #1) được nhóm chọn làm candidate chính. Ngoài ra tôi tách bottleneck
thành 2 loại riêng biệt: (1) chờ HR gửi số → giải pháp là SLA hoặc kết nối thẳng HR system;
(2) copy-paste/chuẩn hóa thủ công → AI + Rule giải quyết được. Phân tách này ảnh hưởng
trực tiếp đến thiết kế future workflow 5 bước và field Boundary của PS v1.
```

---

## 2. Bảng dùng AI (mỗi dòng 1 phase có dùng AI — 2 cột cuối bắt buộc)

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai / hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| Scan | Nhờ AI gợi ý thêm problems theo role DA e-commerce | Nhớ thêm "data cleaning nhiều nền tảng" và "viết comment phân tích" | Gợi ý vài ý quá chung, không bấm giờ được | Bỏ ý không có workflow thật; chỉ giữ problems tôi gặp trực tiếp |
| Problem Card | Nhờ AI phản biện Card #1 — hỏi field nào còn yếu | Chỉ ra "2h/ngày" chưa tách thời gian chờ vs làm tay; đề xuất kiểm tra API access | AI muốn build agent tự gửi báo cáo ngay từ đầu, bỏ qua bước feasibility | Giữ Workflow, không Agent; thêm "giả định API accessible" vào Boundary |
| Workflow | Nhờ AI chuyển mô tả 7 bước thành sơ đồ ASCII current/future | Format nhanh, đặt đúng vị trí bottleneck | AI gộp "chờ HR" và "copy-paste" thành 1 bottleneck | Tách thành 2 bottleneck riêng vì giải pháp khác nhau |
| Research | Tìm tool/pattern tương tự: iPOS API, Power Query, n8n | Gợi ý đúng 3 tools với link chính thức kiểm được | Có 1 claim tiết kiệm thời gian không có nguồn số liệu | Bỏ claim không verify; chỉ giữ mô tả tính năng từ trang chính thức |
| Problem Statement | Nhờ AI phản biện từng field v0 | Chỉ ra field Boundary chưa nói rõ "không làm gì"; Success Metric thiếu baseline % khớp tự động hiện tại | AI đề xuất thêm metric "satisfaction score trưởng bộ phận" mà không đo được trong lab | Giữ metric đo thời gian + % dòng khớp; bổ sung baseline "hiện 100% làm tay" |
| Rule / Workflow / Agent | Nhờ AI so sánh 3 mức trên bài toán cụ thể | Khung phân tích rõ: Rule đủ cho tên đã biết, Workflow hợp cho toàn bộ luồng, Agent thừa | Không có — AI phân tích đúng hướng | Xác nhận bằng 5 câu hỏi chốt; không sửa gì |
| Decision | Không dùng AI — tự đề xuất pilot và 3 số đo dựa trên context thực tế | — | — | — |

> Nếu phase nào không dùng AI, ghi `Không dùng` và vì sao tự làm.

---

## 3. Reflection câu hỏi mở

Chọn 3-4 câu trong 6 câu dưới để viết thành đoạn 8-12 câu (không trả lời bullet 1 dòng):
- Tôi học được gì khi nghe top 3 problems của các bạn khác?
- Nhóm có lúc nào bị solution-first, đòi làm Agent cho ngầu không?
- Tôi có thay đổi ý kiến sau khi bị challenge không, vì sao đổi?
- Tôi đóng góp gì thật sự vào artifact cuối, phần nào có dấu tay của tôi?
- Điều khó nhất khi viết Problem Statement là gì, metric hay boundary?
- Nếu làm lại, tôi sẽ challenge nhóm mạnh hơn ở điểm nào?

**Reflection:**

```text
Điều bất ngờ nhất với tôi là bài của mình được chọn — nhưng không phải vì hay nhất, mà
vì có số đo rõ nhất. Khi tôi pitch Card #1 (tổng hợp báo cáo từ iPOS/Ads/định biên), tôi
nghĩ workflow 7 bước với "~2h/lần" là đủ. Nhưng ngay lập tức Phạm Ngọc Anh hỏi: "2h đó
bao nhiêu là chờ HR, bao nhiêu là làm tay?" — câu hỏi tôi không trả lời được chính xác.
Tôi sửa ngay: tách bottleneck thành 2 loại riêng, mỗi loại một giải pháp khác nhau, và
điều đó làm cho future workflow của nhóm rõ hơn nhiều. Đó là lúc tôi học được rằng "số rõ"
không đủ — phải "tách đúng" để biết phần nào AI giải được và phần nào cần process thay đổi.

Nhóm có một lúc bị solution-first khi bàn về Agent: "hay mình để AI tự pull data, tự chuẩn
hóa và gửi báo cáo luôn?" Tôi dừng lại và hỏi: "nếu AI gửi số sai cho trưởng bộ phận rồi
mình phát hiện sau, ai chịu trách nhiệm?" Không ai trả lời được ngay — và đó là lý do nhóm
hạ xuống Workflow với human boundary ở bước DA duyệt trước khi gửi. Tôi cũng học được từ
Võ Đức Tài: bài phân tích paper của bạn ấy có bottleneck "nặng nhất" nhưng nhóm không ai đủ
context để validate — nếu chọn thì artifact cuối sẽ phụ thuộc 1 người. Điều đó nhắc tôi:
problem tốt nhất cho nhóm không phải là khó nhất hay ảnh hưởng lớn nhất, mà là cả nhóm
hiểu domain đủ để challenge nhau chứ không chỉ gật đầu.

Điều khó nhất khi viết Problem Statement là field Boundary — không phải "AI làm gì" mà là
"AI không làm gì và tại sao". Ban đầu tôi viết chung chung "chỉ làm bước cào và chuẩn hóa"
nhưng nhóm hỏi lại "thế viết comment phân tích xu hướng có vào scope không?" — tôi phải
thêm rõ: không làm insight, không build dashboard, không sửa hệ thống nguồn. Nếu làm lại,
tôi sẽ bấm giờ tách rõ trước khi pitch — chia "thời gian chờ HR" và "thời gian làm tay"
thành 2 con số riêng để baseline chắc hơn ngay từ đầu, không phải sửa giữa chừng.
```

---

## 4. Tự kiểm cuối bài (check trước khi nộp repo)

- [x] [12đ] Cá nhân có 5+ problems + top 3 Problem Cards
- [x] [12đ] Tôi đã pitch rõ + challenge nhóm đúng trọng tâm (ghi ở bảng mục 1)
- [x] Nhóm có nhật ký hội tụ từ candidates về 1 bài
- [x] [15đ] Nhóm có workflow trước/sau
- [x] [20đ] Nhóm có PS v0/v1 với metric + boundary rõ
- [x] [15đ] Nhóm có so sánh No AI / Rule / Workflow / Agent
- [x] [10đ] Nhóm có Go / Not Yet / No-Go + lý do rõ
- [x] [10đ] Reflection này có vai trò thật + AI giúp/sai ở đâu + điều học được + nếu làm lại đổi gì
- [x] [6đ] Tôi tự giải thích được mạch problem → workflow → metric → boundary → độ phù hợp AI
