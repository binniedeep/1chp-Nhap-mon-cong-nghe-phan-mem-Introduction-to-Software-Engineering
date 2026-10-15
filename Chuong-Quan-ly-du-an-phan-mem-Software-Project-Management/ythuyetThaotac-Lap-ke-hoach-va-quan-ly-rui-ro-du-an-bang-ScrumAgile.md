<details id="tai-lieu" open>
<summary><strong>🔍LythuyetThaotac: Lập kế hoạch và quản lý rủi ro dự án bằng Scrum/Agile</strong></summary>

Tên công cụ cần học: **Project Charter, WBS sản phẩm/Scrum, Product Backlog, Sprint Backlog, Sprint Goal, Increment, Definition of Done, Gantt theo Sprint và quản lý rủi ro**. Tool thao tác: **MYTOOL-kehoachvaruiroduan**. Bộ hiện hành chỉ dùng Scrum/Agile.

Bài toán mẫu: xây dựng phần mềm quản lý và thu phí ở chung cư **Blue Moon**, gồm module thu phí, người dùng và hộ gia đình. Mỗi Sprint tạo Increment dùng được, kiểm chứng theo AC/DoD; các file của tool là kế hoạch xây dựng phần mềm đó.

Các đường dẫn bạn gửi:

```text
C:\Users\admin\Desktop\hp_cong_nghe_phan_mem\MYTOOL_kehoachvaruiroduan\input-docs\Huong dan xay dung Ke hoach du an.pdf
C:\Users\admin\Desktop\hp_cong_nghe_phan_mem\MYTOOL_kehoachvaruiroduan\input-docs
C:\Users\admin\Desktop\hp_cong_nghe_phan_mem\MYTOOL_kehoachvaruiroduan\1. Thu thập yêu cầu thô
C:\Users\admin\Desktop\hp_cong_nghe_phan_mem\MYTOOL_kehoachvaruiroduan\2. Ghi nhận yêu cầu
```

PDF: bài 4.1 trang 1–4 (Charter), bài 4.2 trang 4–6 (**dùng hình 4-3 Scrum trang 6**), bài 4.3 trang 6–9 (rủi ro). Mẫu Excel chỉ tham khảo trường dữ liệu. Đối chiếu [Scrum Guide 2020](https://scrumguides.org/scrum-guide.html): PO quản lý giá trị/Backlog, SM hỗ trợ thực hành Scrum, Developers tự quản tạo Increment; Sprint nhất quán tối đa một tháng, có Planning, Daily, Review, Retrospective và DoD.

Nguồn bài trước:

| Workbook | Dữ liệu sử dụng |
| --- | --- |
| `Epic_and_Feature_BlueMoon.xlsx` | 5 Epic, 17 Feature xác định phạm vi sản phẩm |
| `User_Story_BlueMoon_.xlsx`, sheet `User Story`/`Acceptance Criteria (AC)` | 23 Story, liên kết Feature/RAW và AC |
| `Product_Backlog_BlueMoon.xlsx` | MoSCoW/Sprint dự kiến, cần PO/Developers xác nhận |
| `05_NFR-List_tho_BlueMoon.xlsx` | 10 NFR áp dụng/kiểm chứng trong Increment |

Đối chiếu thêm Traceability Matrix, scenario và yêu cầu thô. US-05/US-20 cùng liên quan Audit Log/điều chỉnh: mẫu đề xuất nền tảng Audit Log ở US-05 và luồng điều chỉnh dùng lại nền tảng ở US-20, chờ PO xác nhận để tránh tính trùng.

Luồng **01 → 02 → 03 → 04 → 05 → 06 → 07 → 08**, một lệnh tạo một sản phẩm. `src/scrum_plan.py` tạo WBS/Backlog/Sprint/Gantt thống nhất; `src/products.py` tạo Charter/rủi ro/Dashboard; `src/sample_plan.py` điền nội dung/giả định; `src/validation.py` kiểm tra. Không có lệnh chạy hết kết quả trong `src`.

Bộ mẫu có **6 Sprint, 46 PBI, 110 task, 17 rủi ro**. 46 PBI gồm 23 Story, 10 NFR, 10 bàn giao/tài liệu, 1 mục môi trường và 2 mục phản hồi dự kiến. Sprint tương lai/FB-05/FB-06 là forecast; chưa có phản hồi thực tế được chốt. Chữ ký/approval, bằng chứng DoD và số liệu thực hiện không tự tạo.

Trong Excel chọn tab sheet ở dưới; giữ tên sheet/cột dòng 4, nhập từ dòng 5. ID là văn bản, liên kết nhiều ID dùng `;`, ngày là ô ngày hoặc ISO. Không dùng công thức ở cột nguồn như ngày công/chi phí/P/I. Ctrl+S, đóng workbook rồi chạy Python. Mở Excel để tính lại công thức/Gantt.

`create --step NN --draft --sample` tạo riêng bản mẫu từ dự thảo trước; có file rồi thêm `--replace` để sao lưu/tạo lại. `check --draft` kiểm tra dữ liệu/liên kết; `check`/`approve` thông thường yêu cầu bước trước đã xác nhận và từng dòng được rà soát. Sửa file đã xác nhận làm xác nhận cũ hết hiệu lực; nguồn đổi thì cập nhật sản phẩm phụ thuộc theo thứ tự.

<details id="tong-quan-ket-qua">
<summary><strong>Bộ kết quả BlueMoon — chỉ dùng Scrum/Agile</strong></summary>

8 workbook dùng một kế hoạch Scrum thống nhất. Hai WBS là **theo sản phẩm** và **theo Scrum: Sprint → PBI → task**. Sprint Plan là bước chính; Gantt đọc đúng calendar/PBI/task đó.

| Bước | Kết quả | Nội dung |
| --- | --- | --- |
| 01 | [Project Charter](result/01-khoi-tao-du-an/Project_Charter.xlsx) | Product Goal, PO/SM/Developers, phạm vi, mốc, ngân sách và giả định |
| 02 | [WBS và Product Backlog](result/02-cau-truc-phan-chia-cong-viec/WBS.xlsx) | Hai cây, 46 PBI, 110 task, nguồn Feature/NFR, Sprint và dự toán |
| 03 | [Scrum/Sprint Plan](result/03-ke-hoach-scrum-sprint/Scrum_Sprint_Plan.xlsx) | 6 Sprint, Goal/Increment, AC/DoD, Planning/Daily/Review/Retro và capacity |
| 04 | [Gantt/Timeline theo Sprint](result/04-lich-trinh-sprint-gantt/Gantt_Timeline.xlsx) | Cùng lịch Sprint/PBI/task; kiểm tra timebox, nguồn lực, FS và mốc |
| 05 | [Rủi ro Scrum](result/05-nhan-dien-danh-gia-rui-ro/Risk_Register.xlsx) | 17 rủi ro Goal/capacity/DoD, nghiệp vụ và kỹ thuật |
| 06 | [Ma trận ưu tiên](result/06-ma-tran-uu-tien-rui-ro/Risk_Matrix.xlsx) | 3×3 theo PDF trang 9, ưu tiên bảo vệ Goal/Increment |
| 07 | [Ứng phó/theo dõi](result/07-theo-doi-ung-pho-rui-ro/Risk_Tracking.xlsx) | Người/hạn/chi phí, Daily/Review/Retro, tiêu chí đóng |
| 08 | [Dashboard Scrum](result/08-dashboard-bao-cao/Dashboard.xlsx) | Done PBI/SP, tiến độ Sprint, rủi ro, dự toán, Burndown |

46 PBI: **23 Story, 10 NFR, 10 bàn giao/tài liệu, 1 mục môi trường, 2 mục phản hồi dự kiến**. FB-05/FB-06 chưa phải yêu cầu/phản hồi thực tế được chốt. NFR/tài liệu áp dụng/cập nhật cùng DoD mỗi Sprint; task ghi phần kiểm chứng/snapshot dự kiến.

| Sprint | Timebox | Review | Mục tiêu chính |
| --- | --- | --- | --- |
| 1 | 02–15/10/2023 | 13/10 | Đăng nhập, quyền, căn hộ/chủ hộ |
| 2 | 16–29/10/2023 | 27/10 | Cư dân, khoản thu, nền tảng Audit Log |
| 3 | 30/10–12/11/2023 | 10/11 | Tra cứu, đóng góp, thanh toán |
| 4 | 13–26/11/2023 | 24/11 | Đối soát, phiếu thu, điều chỉnh, báo cáo, restore |
| 5 | 27/11–10/12/2023 | 08/12 | Cải tiến được PO chọn từ phản hồi/Review/UAT |
| 6 | 11–24/12/2023 | 22/12 | Increment bàn giao/cải tiến cuối được PO chọn |

UAT 30/11 và 15/12 là checkpoint trong Sprint 5/6, không thay Review từng Sprint. Bàn giao dự kiến trong Sprint 6; 25–30/12 là khoảng đệm hành chính trước hạn hợp đồng.

Dự toán mẫu:

- Trần: **100.000.000 VND**.
- Task: **53.750.000 VND**; Developers events/refinement: **27.000.000 VND**.
- Dự phòng: **10.000.000 VND**; tổng cơ sở + dự phòng: **90.750.000 VND**.
- Trong trần chưa phân bổ: **9.250.000 VND**.
- Ứng phó dự kiến **8.600.000 VND** nằm trong dự phòng, không cộng lại.

PO/SM/Developers, khả dụng, SP, ngày công, đơn giá, điểm rủi ro và timebox sự kiện mẫu cần nhóm xác nhận. Mọi task/PBI/Increment/hành động đang Chưa bắt đầu, %/Done SP là 0. Chữ ký/approval, bằng chứng DoD, mức còn lại và Burndown thực tế để trống khi chưa có dữ liệu.

Sửa Excel từ dòng 5 và đọc `Gia_dinh_mau`; xem [lý thuyết/thao tác](#tai-lieu). Bộ trước khi đổi phương pháp được bảo quản trong `_backup` để đối chiếu, không dùng làm bộ hiện hành.

```powershell
Set-Location -LiteralPath 'C:\Users\admin\Desktop\hp_cong_nghe_phan_mem\MYTOOL_kehoachvaruiroduan'
& '.\.venv\Scripts\python.exe' .\src\tool.py check --step 03 --draft
& '.\.venv\Scripts\python.exe' .\src\tool.py check --step 04 --draft
& '.\.venv\Scripts\python.exe' .\src\tool.py status
```

</details>

<details id="san-pham-01">
<summary><strong>Sản phẩm 01 — Project Charter, Product Goal và vai trò Scrum; các thao tác</strong></summary>

**Lý thuyết.** Charter là hồ sơ khởi tạo theo bài học: bối cảnh, mục tiêu, phạm vi, bàn giao, nguồn lực, ngân sách, mốc, giả định, truyền thông và phê duyệt. Bổ sung Product Goal và phối hợp Scrum; nhóm cập nhật Backlog và thích nghi mỗi Sprint.

**Nguyên liệu.** PDF trang 1–4, mẫu Charter, nhu cầu bài trước và thông tin thật của nhà tài trợ/PO/SM/Developers. PDF cho 100 triệu VND, quý IV/2023, UAT 30/11 và 15/12, hạn 30/12. Ngày bắt đầu 02/10, dự phòng 10 triệu, đơn giá và ngày công của mẫu là giả định.

**File:** `result/01-khoi-tao-du-an/Project_Charter.xlsx`.

1. Mở JSON `input-docs/thong-tin-du-an.json` bằng Notepad/VS Code; điền tên người phối hợp hồ sơ, tài trợ, ngân sách và ngày/mốc. Giữ cú pháp JSON; số không có dấu phân cách nghìn, đường dẫn dùng `/` hoặc `\\`. Cấu hình Sprint:

```json
"sprint_days": 10,
"sprint_capacity_points": 20
```

10 ngày làm việc tương ứng Sprint hai tuần có cả cuối tuần. SP là dự báo tương đối; không đổi tự động ra ngày công. Tool cần ngày đầu thứ Hai, Sprint 5/10/15/20 ngày làm việc; đổi lịch thật phải đổi đồng bộ mốc.

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py create --step 01 --draft --sample
Invoke-Item -LiteralPath '.\result\01-khoi-tao-du-an\Project_Charter.xlsx'
```

2. `Thong_tin`: B6 phối hợp/quản lý hồ sơ, B7 tài trợ, B10 ngân sách, B11 dự phòng, B12/B13 ngày. Đọc Phương pháp, PO, SM phía cuối. Mục quản lý dự án giữ để đối chiếu Charter PDF; SM trong mẫu phối hợp hồ sơ, Developers vẫn tự quản phân công.
3. `Nhom_du_an`: điền họ tên/nơi công tác/liên hệ, xác định một PO, một SM và Developers đa năng. Nghiệp vụ/thiết kế/lập trình/kiểm thử là năng lực trong Developers. `Ben_lien_quan` có đại diện theo bài toán mẫu, cần xác nhận thực tế.
4. `Pham_vi`: chốt Product Goal, ba module, ngoài phạm vi và phụ thuộc BQT. Mobile/QR v2.0 và nhập liệu thay BQT chưa vào phạm vi. PO cập nhật Backlog, còn trần ngân sách/thời hạn cần các bên thống nhất khi thay đổi.
5. `Ban_giao`: cột D viết tiêu chí DL-01…DL-10; tài liệu/mã/bộ cài cập nhật cùng DoD từng Sprint. `Moc_thoi_gian`: cột C tiêu chí UAT/bàn giao; checkpoint không thay Review mỗi Sprint. `Truyen_thong`: chốt Planning/Daily/Review/Retro/refinement. `Gia_dinh`/`Gia_dinh_mau`: rà người, thiết bị, lịch và tiền.
6. `Phe_duyet`: các bên tự ký/tham chiếu biên bản khi thực sự phê duyệt. Lưu/đóng Excel:

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py check --step 01 --draft
# Chỉ sau khi đã thực sự kiểm chứng:
& '.\.venv\Scripts\python.exe' .\src\tool.py approve --step 01 --by 'Họ tên người kiểm chứng' --note 'Đã kiểm tra Charter, Scrum Team, Goal, trần, mốc và giả định'
```

**Điều kiện:** thông tin chính/người/giả định/truyền thông được bổ sung, bàn giao có tiêu chí, ngày/mốc hợp lệ và không quá 4 tháng, dự phòng trong ngân sách. Phê duyệt chính thức khác nhật ký tool.

<details>
<summary><strong>Thao tác nhanh và bước phụ thuộc</strong></summary>

Sản phẩm: `Project_Charter.xlsx`. Bước phụ thuộc: không có.

Bộ hiện hành chỉ dùng Scrum/Agile. Mở file đã có, đọc Gia_dinh_mau và kiểm chứng nội dung trước khi cam kết. [Lý thuyết và thao tác đầy đủ](#tai-lieu).

Từ thư mục gốc, tạo lại riêng sản phẩm với sao lưu file cũ:

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py create --step 01 --draft --sample --replace
& '.\.venv\Scripts\python.exe' .\src\tool.py check --step 01 --draft
```

Mỗi lệnh chỉ tạo file này; kiểm tra dự thảo không tạo phê duyệt con người. Lưu/đóng Excel sau khi sửa; dùng check/approve thông thường theo thứ tự khi thực sự kiểm chứng.

</details>

</details>

<details id="san-pham-02">
<summary><strong>Sản phẩm 02 — WBS sản phẩm, WBS Scrum và Product Backlog; các thao tác</strong></summary>

**Lý thuyết.** WBS sản phẩm: BlueMoon → module → Feature/sản phẩm chung. WBS Scrum: BlueMoon → **Sprint → PBI/sự kiện Scrum → task**. Quy tắc 100% là đủ công việc tạo kết quả trong phạm vi, không tính trùng. Hai cây là cách nhìn của cùng danh sách task; WBS hỗ trợ trình bày kế hoạch, không thay Backlog chính thức của Scrum Team.

**Nguyên liệu.** Charter, Feature/NFR/Story/AC/Backlog, bàn giao, PDF hình Scrum trang 6 và mẫu WBS. Các công việc làm rõ AC, thiết kế, hiện thực, tích hợp và kiểm chứng được làm cho Increment trong Sprint tương ứng.

**File:** `result/02-cau-truc-phan-chia-cong-viec/WBS.xlsx`.

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py create --step 02 --draft --sample
Invoke-Item -LiteralPath '.\result\02-cau-truc-phan-chia-cong-viec\WBS.xlsx'
```

1. `Danh_muc_pham_vi`: A ID, B Epic, C/D tên/mô tả, E Có/Không, F lý do, G WBS. Loại mục phải giữ dấu vết/quyết định, cập nhật PBI/task/cây liên quan. `WBS_San_pham`: A mã, B cha, C mức, D sản phẩm, E loại, F nguồn; kiểm tra nhóm 3 module và sản phẩm chung.
2. `Product_Backlog`: A PBI ID, B nguồn, C loại, D nội dung, E Epic, F Sprint forecast, G SP, H ưu tiên, I AC, J kiểm chứng, K ghi chú. PO sắp ưu tiên; Developers chọn lượng Done tại Planning. FB-05/FB-06 cần thay bằng phản hồi đã refine trước khi chọn.
3. `Lich_Sprint`: kiểm tra timebox/Review/Goal/Increment. Mẫu 6 Sprint liên tiếp hai tuần, Review/Retro thứ Sáu cuối, Sprint kết thúc Chủ nhật. Từ 25–30/12 là khoảng đệm hành chính trước hạn.
4. `Cong_viec`, từ dòng 5:

| Cột | Nội dung |
| --- | --- |
| A/B | Task ID duy nhất / WBS sản phẩm |
| C/D | Hoạt động trong Sprint / ID nguồn |
| E/F | Công việc / sản phẩm hoặc bằng chứng |
| G/H/I | Người / ngày công / chi phí VND |
| J | Tiền nhiệm bằng `;`, không có chu trình |
| K/L | Kiểm chứng / cơ sở ước lượng và ghi chú |
| M/N/O | Không trước / Sprint / PBI ID |

Ví dụ trong **cùng Sprint 1**:

```text
US-01-AC  : Làm rõ AC/thiết kế cần cho đăng nhập
US-01-DO  : Hiện thực/tích hợp đăng nhập; tiền nhiệm US-01-AC; TECH-ENV
US-01-DOD : Kiểm chứng AC/DoD; tiền nhiệm US-01-DO
```

Developers có thể thay cách chia task/người; ba task là gợi ý của tool, không phải ba pha bắt buộc của Scrum. Ngày công/đơn giá/tiền nhiệm đều cần nhóm kiểm chứng.

5. `WBS_Scrum`: A mã, B cha, C mức, D nội dung, E Task ID, F nguồn, G Sprint. Mức 1 Sprint, mức 2 PBI/nhóm sự kiện, mức 3 task; mỗi task đúng một lần, khớp bảng chính. EV-xx là nhóm sự kiện/hỗ trợ Sprint, không phải User Story khách hàng.
6. `Kiem_tra_100`: C đủ task cho từng Feature/NFR. Feature có nhiều Story/Sprint chỉ xong khi đủ phạm vi. `Nguon_luc`: kiểm tra ngày/đơn giá/chi phí; Developers dành riêng 2 ngày/Sprint cho events/refinement; SM facilitation đã có trong task.
7. Dự toán = task + Developers events/refinement + dự phòng, trong trần. Không cộng hai cây WBS hai lần. Lưu/đóng và kiểm tra:

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py check --step 02 --draft
& '.\.venv\Scripts\python.exe' .\src\tool.py approve --step 02 --by 'Họ tên người kiểm chứng' --note 'Đã kiểm tra 100%, Product Backlog, cây Scrum, task/Sprint/PBI và dự toán'
```

**Điều kiện:** bao phủ nguồn/bàn giao, cây và ID đúng, task thuộc Sprint/PBI, tiền nhiệm hợp lệ, AC và ước lượng đã rà soát, chi phí trong trần.

<details>
<summary><strong>Thao tác nhanh và bước phụ thuộc</strong></summary>

Sản phẩm: `WBS.xlsx`. Bước phụ thuộc: 01.

Bộ hiện hành chỉ dùng Scrum/Agile. Mở file đã có, đọc Gia_dinh_mau và kiểm chứng nội dung trước khi cam kết. [Lý thuyết và thao tác đầy đủ](#tai-lieu).

Từ thư mục gốc, tạo lại riêng sản phẩm với sao lưu file cũ:

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py create --step 02 --draft --sample --replace
& '.\.venv\Scripts\python.exe' .\src\tool.py check --step 02 --draft
```

Mỗi lệnh chỉ tạo file này; kiểm tra dự thảo không tạo phê duyệt con người. Lưu/đóng Excel sau khi sửa; dùng check/approve thông thường theo thứ tự khi thực sự kiểm chứng.

</details>

</details>

<details id="san-pham-03">
<summary><strong>Sản phẩm 03 — Scrum/Sprint Plan, Goal, DoD, events, capacity và Increment; các thao tác</strong></summary>

**Lý thuyết.** Product Backlog là nhu cầu có thứ tự; Sprint Backlog gồm Sprint Goal, PBI chọn và kế hoạch tạo Increment. DoD là chuẩn chung; AC là điều kiện từng PBI. SP đo tương đối, capacity ngày công kiểm tra khả dụng. Sprint tương lai là forecast có thể thích nghi sau Review.

**Nguyên liệu.** WBS/Backlog/calendar/task, mẫu Agile, AC và thỏa thuận PO/Developers. Đây là bước chính; Gantt đọc đúng kế hoạch này.

**File:** `result/03-ke-hoach-scrum-sprint/Scrum_Sprint_Plan.xlsx`.

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py create --step 03 --draft --sample
Invoke-Item -LiteralPath '.\result\03-ke-hoach-scrum-sprint\Scrum_Sprint_Plan.xlsx'
```

1. `Sprint_Backlog`: A PBI, B nội dung, C nguồn, D ưu tiên, E Sprint, F SP, G người, H trạng thái, I AC, J kiểm chứng, **K bằng chứng DoD**. Đổi Sprint/SP thì sửa canonical ở WBS trước; trạng thái/bằng chứng thực hiện cập nhật tại 03.
2. `Sprint`: A tên, B/C ngày, D capacity SP, E tổng SP công thức, F Goal, G Increment dự kiến, H Review, I kiểm chứng. Kiểm tra lượng PBI/capacity/mục tiêu; 20 SP/Sprint là giả định, chưa phải velocity đã đo.
3. `Definition_of_Done`: chốt chuẩn và cách lưu bằng chứng. `Increment`: ghi trạng thái/bằng chứng thực tế; PBI chưa đạt DoD về Backlog để PO sắp lại. Không ghi Done chỉ vì code xong.
4. `Scrum_Events`: Planning đầu Sprint (2 giờ mẫu), Daily 15 phút/ngày làm việc, Review cuối Sprint (2 giờ mẫu), Retrospective sau Review (1 giờ mẫu). 2/2/1 giờ là giả định của bộ này. Review là kiểm tra và thích nghi với stakeholders, Daily để Developers điều chỉnh kế hoạch đạt Goal.
5. `Capacity`: so ngày khả dụng trừ 2 ngày events/refinement với ngày task; chỉnh lịch nghỉ/mức huy động/lượng công việc, không hạ DoD. `Quy_tac_Scrum`: đọc trách nhiệm, refinement liên tục, forecast và UAT. AC/NFR/tài liệu cập nhật cùng Increment.

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py check --step 03 --draft
& '.\.venv\Scripts\python.exe' .\src\tool.py approve --step 03 --by 'Họ tên người kiểm chứng' --note 'Đã rà Goal, Increment, Backlog/AC, capacity, DoD và events'
```

**Điều kiện:** Backlog/Sprint/SP khớp WBS, Goal/Increment rõ, timebox nhất quán/nối tiếp, đủ events/DoD, không vượt capacity. Done PBI/Increment phải có bằng chứng. Chỉ coi Sprint đã thực sự Planning là kế hoạch nhóm đã chốt.

<details>
<summary><strong>Thao tác nhanh và bước phụ thuộc</strong></summary>

Sản phẩm: `Scrum_Sprint_Plan.xlsx`. Bước phụ thuộc: 01, 02.

Bộ hiện hành chỉ dùng Scrum/Agile. Mở file đã có, đọc Gia_dinh_mau và kiểm chứng nội dung trước khi cam kết. [Lý thuyết và thao tác đầy đủ](#tai-lieu).

Từ thư mục gốc, tạo lại riêng sản phẩm với sao lưu file cũ:

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py create --step 03 --draft --sample --replace
& '.\.venv\Scripts\python.exe' .\src\tool.py check --step 03 --draft
```

Mỗi lệnh chỉ tạo file này; kiểm tra dự thảo không tạo phê duyệt con người. Lưu/đóng Excel sau khi sửa; dùng check/approve thông thường theo thứ tự khi thực sự kiểm chứng.

</details>

</details>

<details id="san-pham-04">
<summary><strong>Sản phẩm 04 — Gantt/Timeline của cùng kế hoạch Scrum; các thao tác</strong></summary>

**Lý thuyết.** Gantt hiển thị task theo thời gian, Timeline nhấn mốc. Chúng dùng cùng Sprint/PBI/Goal ở 03; tiền nhiệm là nhu cầu kỹ thuật của công việc. Task phải trong timebox/Review của Sprint đã gán.

**Nguyên liệu.** Charter, WBS, Scrum/Sprint Plan, mẫu Gantt/Timeline. Lịch dùng thứ Hai–thứ Sáu, FS, Không trước và một người một task/ngày; chưa loại ngày lễ/lịch cá nhân.

**File:** `result/04-lich-trinh-sprint-gantt/Gantt_Timeline.xlsx`.

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py create --step 04 --draft --sample
Invoke-Item -LiteralPath '.\result\04-lich-trinh-sprint-gantt\Gantt_Timeline.xlsx'
```

1. `Lich_trinh`: A:D ID/WBS/nội dung/người; E/F ngày; G/H ngày công/tiền nhiệm; I/J phần trăm task/trạng thái; K chi phí; L ghi chú; **M/N Sprint/PBI**. Đổi người/ngày công/tiền/tiền nhiệm/Sprint/PBI phải cập nhật WBS trước.
2. Điều chỉnh E/F trong Sprint: đủ ngày làm việc, không chồng người/vi phạm FS/Không trước. Thiếu capacity thì Developers/PO thương lượng PBI và cập nhật forecast; không kéo task qua Sprint để che chưa Done.
3. `Gantt_Sprint`: B là Sprint, D trở đi là tuần; thanh đọc `Lich_trinh`. Nếu dời ngoài vùng tuần thì bổ sung cột/công thức hoặc tạo lại. `Lich_Sprint` phải khớp 03.
4. `Timeline`/`Doi_chieu_moc`: UAT 30/11, 15/12 và hạn 30/12; sản phẩm dự kiến bàn giao trong Sprint 6. `Kiem_tra`: task/events/dự phòng/kết thúc/khoảng đệm.
5. I nhập 0–100, J theo thực tế; Hoàn thành task phải 100%. Done PBI vẫn cần bằng chứng DoD ở 03, không tự suy ra từ % task.

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py check --step 04 --draft
& '.\.venv\Scripts\python.exe' .\src\tool.py approve --step 04 --by 'Họ tên người kiểm chứng' --note 'Đã kiểm tra timebox Sprint, task/source, lịch người, FS, capacity và mốc'
```

**Điều kiện:** task/source khớp, ngày trong Sprint/Charter, đủ ngày công, không trùng người/vi phạm FS, UAT đúng mốc; tiến độ có căn cứ.

<details>
<summary><strong>Thao tác nhanh và bước phụ thuộc</strong></summary>

Sản phẩm: `Gantt_Timeline.xlsx`. Bước phụ thuộc: 01, 02, 03.

Bộ hiện hành chỉ dùng Scrum/Agile. Mở file đã có, đọc Gia_dinh_mau và kiểm chứng nội dung trước khi cam kết. [Lý thuyết và thao tác đầy đủ](#tai-lieu).

Từ thư mục gốc, tạo lại riêng sản phẩm với sao lưu file cũ:

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py create --step 04 --draft --sample --replace
& '.\.venv\Scripts\python.exe' .\src\tool.py check --step 04 --draft
```

Mỗi lệnh chỉ tạo file này; kiểm tra dự thảo không tạo phê duyệt con người. Lưu/đóng Excel sau khi sửa; dùng check/approve thông thường theo thứ tự khi thực sự kiểm chứng.

</details>

</details>

<details id="san-pham-05">
<summary><strong>Sản phẩm 05 — Nhận diện/đánh giá rủi ro Scrum; các thao tác</strong></summary>

**Lý thuyết.** Rủi ro là sự kiện chưa chắc xảy ra tác động Product/Sprint Goal, DoD, lịch hoặc chi phí. Viết nguyên nhân → sự kiện → hậu quả, task/PBI liên quan, chủ, dấu hiệu, phòng ngừa. Thay đổi Backlog là bình thường; rủi ro là thay đổi không thương lượng làm hại Goal/chất lượng/trần đã thống nhất.

**Nguyên liệu.** Charter/WBS/Sprint/lịch, PDF trang 6–9 và NFR. Mẫu có 9 rủi ro từ ví dụ áp dụng vào Scrum, 7 rủi ro BlueMoon và 1 rủi ro quá capacity/ghi Done sai DoD: tổng 17.

**File:** `result/05-nhan-dien-danh-gia-rui-ro/Risk_Register.xlsx`.

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py create --step 05 --draft --sample
Invoke-Item -LiteralPath '.\result\05-nhan-dien-danh-gia-rui-ro\Risk_Register.xlsx'
```

1. `Rui_ro`: A ID, B sự kiện, C nguyên nhân/hậu quả, D Task ID dùng `;` hoặc TOAN-DU-AN, E/F P/I 1–3, G/H điểm/mức, I phòng ngừa, J chủ, K dấu hiệu, L trạng thái, M nguồn, N kiểm chứng. Điểm mẫu cần nhóm đánh giá lại.
2. PDF trang 7 dùng P×I; bảng 3×3 trang 9 dùng mức 1–5 tương đương P+I−1. Giữ cả hai: P=2/I=2 có điểm nhân 4 nhưng mức 3. Trang 8 lỗi nhãn lặp Mức 4/5 và dấu hiệu sao chép mô tả chi phí; `Thang_do` giữ dấu vết, cần đối chiếu giảng viên.
3. `Boi_canh` đối chiếu task/người/lịch/tiền; bổ sung nguy cơ giao dịch trùng, tính phí, quyền, restore, hiệu năng, triển khai và Goal/DoD. Thêm dòng thì sao chép G/H:

```excel
=E5*F5
=E5+F5-1
```

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py check --step 05 --draft
& '.\.venv\Scripts\python.exe' .\src\tool.py approve --step 05 --by 'Họ tên người kiểm chứng' --note 'Đã rà rủi ro Scrum/BlueMoon, thang điểm, task, chủ và dấu hiệu'
```

**Điều kiện:** ID/task đúng, P/I 1–3, mô tả/nguồn/người/dấu hiệu rõ; từng dòng được rà. Đổi trạng thái không tự chứng minh đã xử lý.

<details>
<summary><strong>Thao tác nhanh và bước phụ thuộc</strong></summary>

Sản phẩm: `Risk_Register.xlsx`. Bước phụ thuộc: 01, 02, 03, 04.

Bộ hiện hành chỉ dùng Scrum/Agile. Mở file đã có, đọc Gia_dinh_mau và kiểm chứng nội dung trước khi cam kết. [Lý thuyết và thao tác đầy đủ](#tai-lieu).

Từ thư mục gốc, tạo lại riêng sản phẩm với sao lưu file cũ:

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py create --step 05 --draft --sample --replace
& '.\.venv\Scripts\python.exe' .\src\tool.py check --step 05 --draft
```

Mỗi lệnh chỉ tạo file này; kiểm tra dự thảo không tạo phê duyệt con người. Lưu/đóng Excel sau khi sửa; dùng check/approve thông thường theo thứ tự khi thực sự kiểm chứng.

</details>

</details>

<details id="san-pham-06">
<summary><strong>Sản phẩm 06 — Ma trận 3×3 và ưu tiên rủi ro; các thao tác</strong></summary>

**Lý thuyết.** Ma trận giúp ưu tiên theo P/I tác động Goal/chất lượng. Mức bài là P+I−1; P×I là cột tham khảo riêng. Nguồn: Risk Register kiểm chứng, PDF trang 9; mẫu Excel 5×5 chỉ tham khảo trường.

| P \ I | 1 | 2 | 3 |
| --- | --- | --- | --- |
| 3 | 3 | 4 | 5 |
| 2 | 2 | 3 | 4 |
| 1 | 1 | 2 | 3 |

**File:** `result/06-ma-tran-uu-tien-rui-ro/Risk_Matrix.xlsx`.

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py create --step 06 --draft --sample
Invoke-Item -LiteralPath '.\result\06-ma-tran-uu-tien-rui-ro\Risk_Matrix.xlsx'
```

1. `Ma_tran_3x3`: kiểm tra cả 9 ô/ID đúng nguồn. `Uu_tien`: mức giảm dần, tác động giảm dần, rồi ID; I viết quyết định bảo vệ Goal/Increment. `Chu_giai` giải thích mức/lỗi nhãn.
2. Đổi P/I phải sửa 05, kiểm chứng và tạo lại 06. Không sửa riêng ma trận để khác nguồn.

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py check --step 06 --draft
& '.\.venv\Scripts\python.exe' .\src\tool.py approve --step 06 --by 'Họ tên người kiểm chứng' --note 'Đã đối chiếu ma trận và quyết định ưu tiên'
```

**Điều kiện:** đủ ID, điểm/mức/ô/thứ tự khớp; quyết định ưu tiên được nhóm xác nhận.

<details>
<summary><strong>Thao tác nhanh và bước phụ thuộc</strong></summary>

Sản phẩm: `Risk_Matrix.xlsx`. Bước phụ thuộc: 05.

Bộ hiện hành chỉ dùng Scrum/Agile. Mở file đã có, đọc Gia_dinh_mau và kiểm chứng nội dung trước khi cam kết. [Lý thuyết và thao tác đầy đủ](#tai-lieu).

Từ thư mục gốc, tạo lại riêng sản phẩm với sao lưu file cũ:

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py create --step 06 --draft --sample --replace
& '.\.venv\Scripts\python.exe' .\src\tool.py check --step 06 --draft
```

Mỗi lệnh chỉ tạo file này; kiểm tra dự thảo không tạo phê duyệt con người. Lưu/đóng Excel sau khi sửa; dùng check/approve thông thường theo thứ tự khi thực sự kiểm chứng.

</details>

</details>

<details id="san-pham-07">
<summary><strong>Sản phẩm 07 — Ứng phó và theo dõi trong Sprint; các thao tác</strong></summary>

**Lý thuyết.** Ứng phó có chiến lược, người, hạn, dấu hiệu, nguồn lực và tiêu chí đóng. Developers/PO thương lượng kế hoạch/phạm vi; SM hỗ trợ Scrum/giải trở ngại. Rủi ro còn lại chỉ đánh giá khi có bằng chứng.

**Nguyên liệu.** Charter, danh mục/ma trận, mẫu theo dõi, quyết định tại Daily/Review/Retro.

**File:** `result/07-theo-doi-ung-pho-rui-ro/Risk_Tracking.xlsx`.

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py create --step 07 --draft --sample
Invoke-Item -LiteralPath '.\result\07-theo-doi-ung-pho-rui-ro\Risk_Tracking.xlsx'
```

1. `Ung_pho`: A/B Action/Risk ID, C mức, D chiến lược; E/F/G phòng ngừa/kích hoạt/dự phòng; H/I/J người/hạn/tiền; K trạng thái; L/M/N P/I/mức còn lại; O tiêu chí/bằng chứng; P kiểm chứng.
2. Hạn phù hợp Sprint/PBI cần bảo vệ, chi phí tăng thêm trong dự phòng. Test/phòng ngừa đã ở task hoặc DoD không tính lại. Nếu cần task ứng phó, đưa vào Backlog/Planning hoặc thương lượng khi rủi ro xảy ra; không hạ DoD vì thiếu capacity.
3. L/M để trống khi chưa đánh giá. Chỉ chọn Hoàn thành khi có bằng chứng/đánh giá còn lại. `Lich_ra_soat`: Daily/Review/Retro và dấu hiệu; `Doi_chieu_du_phong`: kiểm tra phân bổ/chưa phân bổ.

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py check --step 07 --draft
& '.\.venv\Scripts\python.exe' .\src\tool.py approve --step 07 --by 'Họ tên người kiểm chứng' --note 'Đã rà hành động, người/hạn, dự phòng, dấu hiệu và tiêu chí đóng'
```

**Điều kiện:** mọi Risk có hành động, liên kết/chiến lược/người/hạn hợp lệ, tổng trong dự phòng; kiểm chứng kế hoạch không đồng nghĩa đã thực hiện.

<details>
<summary><strong>Thao tác nhanh và bước phụ thuộc</strong></summary>

Sản phẩm: `Risk_Tracking.xlsx`. Bước phụ thuộc: 01, 05, 06.

Bộ hiện hành chỉ dùng Scrum/Agile. Mở file đã có, đọc Gia_dinh_mau và kiểm chứng nội dung trước khi cam kết. [Lý thuyết và thao tác đầy đủ](#tai-lieu).

Từ thư mục gốc, tạo lại riêng sản phẩm với sao lưu file cũ:

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py create --step 07 --draft --sample --replace
& '.\.venv\Scripts\python.exe' .\src\tool.py check --step 07 --draft
```

Mỗi lệnh chỉ tạo file này; kiểm tra dự thảo không tạo phê duyệt con người. Lưu/đóng Excel sau khi sửa; dùng check/approve thông thường theo thứ tự khi thực sự kiểm chứng.

</details>

</details>

<details id="san-pham-08">
<summary><strong>Sản phẩm 08 — Dashboard Scrum, Done SP và Burndown; các thao tác</strong></summary>

**Lý thuyết.** Theo dõi Goal bằng Increment/PBI đạt DoD; % task chỉ hỗ trợ. SP còn lại thực tế phải lấy từ PBI có bằng chứng, không suy diễn lịch sử. Nguyên liệu: 01–07 kiểm chứng, trạng thái PBI tại 03, task tại 04, rủi ro/hành động tại 05/07, mẫu Dashboard.

**File:** `result/08-dashboard-bao-cao/Dashboard.xlsx`.

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py create --step 08 --draft --sample
Invoke-Item -LiteralPath '.\result\08-dashboard-bao-cao\Dashboard.xlsx'
```

1. `Tong_quan`: tiến độ = SP Done/SP forecast, số Sprint/PBI Done, SP, task, chi phí task/events và rủi ro. `Tiến độ task %` theo ngày công không thay Done. `Tien_do_Sprint` đối chiếu SP/PBI và Goal; `Thong_ke_task`/`Thong_ke_rui_ro` đối chiếu biểu đồ/số đếm.
2. `Burndown`: đọc đường lý tưởng minh họa từ forecast; E SP còn lại thực tế để trống khi chưa có số liệu. Khi Sprint đã Planning, cập nhật baseline/lịch sử từ PBI đạt DoD, không tự bịa velocity.
3. `Doi_chieu_ngan_sach`: task + Developers events/refinement + dự phòng so trần. Ứng phó là phân bổ trong dự phòng; SM facilitation đã ở task. Đây là dự toán, chưa phải chi tiêu thực tế.
4. `Bao_cao`: B5 ngày chốt, B6 kết quả, B7 quyết định cần xin, B8 kế hoạch tiếp, B9 người phối hợp. Mẫu dùng kỳ lập kế hoạch giả định 02/10/2023, tiến độ/Done 0. Nguồn đổi phải tạo lại Dashboard.

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py check --step 08 --draft
& '.\.venv\Scripts\python.exe' .\src\tool.py approve --step 08 --by 'Họ tên người kiểm chứng' --note 'Đã kiểm tra nguồn, Goal/Done/DoD, rủi ro và dự toán kỳ báo cáo'
```

**Điều kiện:** chỉ số khớp nguồn, ngày/nội dung kỳ rõ; bằng chứng được rà soát, không giả lập hoàn thành/Burndown thực tế.

<details>
<summary><strong>Thao tác nhanh và bước phụ thuộc</strong></summary>

Sản phẩm: `Dashboard.xlsx`. Bước phụ thuộc: 01, 02, 03, 04, 05, 06, 07.

Bộ hiện hành chỉ dùng Scrum/Agile. Mở file đã có, đọc Gia_dinh_mau và kiểm chứng nội dung trước khi cam kết. [Lý thuyết và thao tác đầy đủ](#tai-lieu).

Từ thư mục gốc, tạo lại riêng sản phẩm với sao lưu file cũ:

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py create --step 08 --draft --sample --replace
& '.\.venv\Scripts\python.exe' .\src\tool.py check --step 08 --draft
```

Mỗi lệnh chỉ tạo file này; kiểm tra dự thảo không tạo phê duyệt con người. Lưu/đóng Excel sau khi sửa; dùng check/approve thông thường theo thứ tự khi thực sự kiểm chứng.

</details>

</details>

<details id="cap-nhat-sao-luu-kiem-tra">
<summary><strong>Cập nhật, sao lưu và kiểm tra</strong></summary>

Đổi Backlog/Goal/AC/ước lượng/capacity thì cập nhật từ 02, tạo lại từng sản phẩm phụ thuộc theo thứ tự. Trạng thái/bằng chứng thực hiện ở 03/04/05/07 cần rà soát nguồn bị ảnh hưởng và tạo lại Dashboard. `--replace` giữ bản cũ ở `_backup` của sản phẩm; đối chiếu/chuyển lại nội dung bổ sung còn phù hợp.

`result/_backup` chứa bộ trước khi chuyển Scrum để đối chiếu; workbook trực tiếp trong 01–08 là bộ hiện hành. PDF/mẫu và dữ liệu bài trước giữ nguyên. SHA-256 phát hiện nguồn đổi; nhật ký UTC là kỹ thuật, ngày bài toán vẫn theo tài liệu.

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py status
& '.\.venv\Scripts\python.exe' -m unittest discover -s .\tests -v
& '.\.venv\Scripts\python.exe' .\tests\verify_results.py
```

Muốn sửa mã: chỉnh `sprint_calendar`, `product_backlog`, `tasks_for_backlog`, `build_wbs`, `build_sprints`, `build_gantt` trong `src/scrum_plan.py`; `DOD` là chuẩn mẫu. Cập nhật `src/validation.py` và tài liệu, chạy kiểm tra rồi tạo lại sản phẩm bị ảnh hưởng. Lỗi ghi file thì đóng Excel; thiếu nguồn thì chép vào `input-docs` và sửa JSON; thiếu thư viện thì cài `src/requirements.txt`.

</details>

</details>
