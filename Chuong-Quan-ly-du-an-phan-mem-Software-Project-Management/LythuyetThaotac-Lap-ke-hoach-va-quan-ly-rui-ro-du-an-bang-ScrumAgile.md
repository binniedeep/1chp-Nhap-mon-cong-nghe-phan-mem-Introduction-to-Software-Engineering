<details id="tong-quan-ket-qua" open>
<summary><strong>🔍LythuyetThaotac: Lập kế hoạch và quản lý rủi ro dự án bằng Scrum/Agile</strong></summary>

**Bài toán mẫu để học thao tác**

Bạn cần lập kế hoạch xây dựng phần mềm quản lý và thu phí chung cư **Blue Moon**. Phần mềm có ba mô-đun: quản lý thu phí, quản lý người dùng và quản lý hộ gia đình.

Ở bài trước, bạn đã thu thập và ghi nhận yêu cầu. Trong bài này, bạn dùng các yêu cầu đó để trả lời: dự án phải bàn giao những gì, cần làm những việc nào, dự kiến làm trong Sprint nào và phải chuẩn bị cho những rủi ro nào.

**Đường dẫn tài liệu lý thuyết bạn gửi**

`C:\Users\admin\Desktop\hp_cong_nghe_phan_mem\MYTOOL_kehoachvaruiroduan\input-docs\Huong dan xay dung Ke hoach du an.pdf`

Hướng dẫn bám Bài 4.1, 4.2 và 4.3 trong PDF; phần WBS dùng hình 4-1 và hình 4-3. Cách lập kế hoạch chỉ dùng **Scrum/Agile**.

Các mẫu Excel nằm trong `input-docs`. Dữ liệu yêu cầu của bài trước nằm ở:

- `C:\Users\admin\Desktop\hp_cong_nghe_phan_mem\MYTOOL_kehoachvaruiroduan\1. Thu thập yêu cầu thô`
- `C:\Users\admin\Desktop\hp_cong_nghe_phan_mem\MYTOOL_kehoachvaruiroduan\2. Ghi nhận yêu cầu`

Hai thư mục này là nguồn tham khảo của bài trước. Kết quả của bài này nằm trong `result`.

**Cách đọc và thực hành**

Mở lần lượt tám toggle sản phẩm bên dưới. Mỗi sản phẩm đều có bốn phần: **định nghĩa → nguyên liệu → ý nghĩa → cách hoàn thiện**.

| Thứ tự | Sản phẩm | Câu hỏi sản phẩm giúp trả lời |
| --- | --- | --- |
| 01 | Project Charter — Tuyên ngôn dự án | Dự án làm gì, trong giới hạn nào, ai xác nhận? |
| 02 | WBS — Cấu trúc phân chia công việc | Phạm vi dự án được chia thành những phần nào? |
| 03 | Kế hoạch Agile | Dự kiến chọn công việc nào cho từng Sprint? |
| 04 | Gantt | Các công việc nằm ở đâu trên lịch? |
| 05 | Timeline | Những Sprint và mốc chính diễn ra khi nào? |
| 06 | Dashboard | Tình hình công việc đang như thế nào? |
| 07 | Đánh giá và theo dõi rủi ro | Có thể gặp vấn đề gì, ai chuẩn bị ứng phó? |
| 08 | Ma trận rủi ro | Rủi ro nào cần được chú ý trước? |

Trong Excel, **sheet** là trang tính; chọn sheet bằng các tab ở đáy cửa sổ. Địa chỉ như `E4` nghĩa là ô ở cột E, dòng 4. Khi cần xuống dòng trong cùng một ô, nhấn `Alt+Enter`.

Các mã và từ viết tắt sẽ gặp:

| Ký hiệu | Cách hiểu trong bài |
| --- | --- |
| `FT-xx` — Feature | Một nhóm chức năng, ví dụ đăng nhập hoặc quản lý hộ gia đình. |
| `US-xx` — User Story | Một nhu cầu cụ thể của người sử dụng. |
| `NFR-xxx` | Yêu cầu chất lượng hoặc ràng buộc, như bảo mật, tốc độ tra cứu, công nghệ sử dụng. |
| AC | Tiêu chí chấp nhận: điều kiện để kiểm tra một yêu cầu đã được đáp ứng. |
| PO — Product Owner | Người chịu trách nhiệm về giá trị sản phẩm và quản lý Product Backlog. |
| SM — Scrum Master | Người giúp nhóm hiểu và thực hiện Scrum. |
| Developers | Những người trực tiếp tạo ra phần mềm, gồm các công việc thiết kế, lập trình, kiểm thử. |

**Chuẩn bị trước khi chạy lệnh**

Thực hiện phần cài môi trường trong [README.md](README.md) nếu chưa có Python và thư viện. Sau đó mở PowerShell và chuyển vào thư mục tool:

```powershell
Set-Location -LiteralPath 'C:\Users\admin\Desktop\hp_cong_nghe_phan_mem\MYTOOL_kehoachvaruiroduan'
& '.\.venv\Scripts\python.exe' .\src\tool.py status
```

Các lệnh trong từng sản phẩm bên dưới đều chạy tại thư mục này. `src/tool.py` chỉ tạo **một sản phẩm cho mỗi lệnh**. Tool điền dữ liệu có sẵn; bạn kiểm tra nội dung và bổ sung những thông tin nhóm chưa chốt.

Bộ mẫu dùng các mốc quý IV/2023 trong bài học, gồm UAT ngày 30/11, UAT ngày 15/12 và hoàn tất ngày 30/12. Bốn Sprint lấy từ backlog bài trước; thời lượng 21 ngày/Sprint, ngày bắt đầu 02/10 và dự phòng 10 triệu đồng là giả định cần bạn kiểm chứng. Các ô nhân sự, ước lượng và xác nhận còn thiếu được hướng dẫn cụ thể ở từng sản phẩm.

<details>
<summary><strong>Khi cần tạo lại một file đã có hoặc đổi thông tin bài toán</strong></summary>

Để tạo lại một sản phẩm, đóng file Excel đó rồi dùng `create --step` với đúng số sản phẩm. Ví dụ, tạo lại kế hoạch Agile:

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py create --step 03 --replace
```

`--replace` thay file hiện tại bằng bản mới từ nguồn; phần bạn đã điền trực tiếp trong file cũng được thay. File cũ được sao lưu tại `.tool-data/backups`.

Thông tin đầu vào chung nằm trong `input-docs/thong-tin-du-an.json`: tên dự án, nhân sự, ngân sách, ngày, các mốc, đường dẫn dữ liệu và `sprint_calendar_days`. Nếu sửa ngày trong JSON, dùng dạng `YYYY-MM-DD`; `sprint_calendar_days` hiện bằng `21`.

Thứ tự cập nhật phụ thuộc:

- Sửa Charter 01: rà soát và tạo lại các sản phẩm phụ thuộc 02, 03, 05, 07 theo thứ tự cần dùng.
- Sửa WBS hoặc backlog nguồn: tạo lại 03 sau khi đã kiểm tra phạm vi.
- Sửa kế hoạch Agile 03: tạo lại từng file 04, 05, 06.
- Sửa đánh giá rủi ro 07: tạo lại 08.

Nếu tool báo nguồn đã thay đổi, xử lý sản phẩm trước được nêu trong thông báo rồi tiếp tục. Hoàn thiện và lưu từng sản phẩm trước khi chuyển sang sản phẩm phụ thuộc.

</details>
</details>

<details id="san-pham-01">
<summary><strong>Sản phẩm 01 — Project Charter: lập tuyên ngôn dự án và xác định phạm vi</strong></summary>

**1. Sản phẩm này là gì?**

Project Charter, hay tuyên ngôn dự án, là tài liệu thống nhất những thông tin nền tảng của dự án: lý do thực hiện, mục tiêu, phạm vi, sản phẩm bàn giao, người tham gia, thời gian, ngân sách và cách xác nhận.

Trong bài Blue Moon, Charter phải làm rõ ba mô-đun cần xây dựng, các tài liệu phải bàn giao, trần ngân sách 100 triệu đồng và các mốc nghiệm thu của PDF.

**2. Cần những nguyên liệu gì?**

- Bài 4.1, trang 1–4 của PDF.
- Mẫu `input-docs/Mẫu Project Charter.xlsx` và cấu hình `input-docs/thong-tin-du-an.json`.
- Danh sách Feature trong `2. Ghi nhận yêu cầu/Epic_and_Feature_BlueMoon.xlsx`.
- Yêu cầu chất lượng trong `1. Thu thập yêu cầu thô/05_NFR-List_tho_BlueMoon.xlsx`.
- Thông tin bạn cần bổ sung: nhân sự, liên hệ, dự toán chi tiết và người có thẩm quyền xác nhận.

**3. Sản phẩm tạo ra có ý nghĩa gì?**

Charter là căn cứ để kiểm tra các công việc về sau có đúng mục tiêu và phạm vi đã thống nhất hay không. Nhóm dùng nó khi lập WBS, xếp lịch, trao đổi với khách hàng và xử lý yêu cầu thay đổi.

**4. Làm thế nào để hoàn thiện sản phẩm?**

**Bước 1 — Mở file.** Lệnh sau mở kết quả có sẵn; nếu chưa có, tool tạo riêng sản phẩm 01:

```powershell
$tep = '.\result\01-Khoi-tao-du-an\01-Project-Charter.xlsx'
if (-not (Test-Path -LiteralPath $tep)) {
    & '.\.venv\Scripts\python.exe' .\src\tool.py create --step 01
}
Invoke-Item -LiteralPath $tep
```

**Bước 2 — Chọn tab `Project_Charter`, đọc nội dung mẫu và điền phần còn thiếu.**

| Vị trí | Bạn cần viết hoặc kiểm tra gì? |
| --- | --- |
| `B4`, `E4`, `G4` | Kiểm tra tên dự án; điền họ tên quản lý dự án và nhà tài trợ. |
| `B6`, `D6`, `E6` | Điền email, điện thoại liên hệ và đơn vị thực hiện. |
| `B8`, `B10`, `C35` | Ghi họ tên người làm, vai trò PO/SM/Developers, đơn vị và liên hệ của từng người. Có thể xuống dòng bằng `Alt+Enter`. |
| `C13:C17` | Rà lại bối cảnh, mục đích, lợi ích, mục tiêu và danh sách bàn giao. Với mục tiêu “100%”, ghi rõ tập dữ liệu/phạm vi và tiêu chí dùng để kiểm tra. |
| `C20:C21` | Xác nhận phần trong/ngoài phạm vi. Bài mẫu không bao gồm nhập thay toàn bộ dữ liệu nghiệp vụ thực tế cho khách hàng. |
| `E8`, `G8`; dòng 25–27 | Kiểm tra ngày bắt đầu/kết thúc và ba mốc UAT, bàn giao theo PDF. |
| `C37` | Đối chiếu công nghệ, bảo mật, hiệu năng, sao lưu/khôi phục với NFR nguồn. Di chuột vào dấu ghi chú của ô để đọc nội dung NFR. |
| Dòng 41–47 | Bổ sung hạng mục, cơ sở dự toán, đơn giá ở E và số lượng ở F. Hai dòng đầu đã có công thức thành tiền; nếu thêm hạng mục ở dòng trống, nhập công thức tương ứng ở G như hướng dẫn dưới bảng. |
| `C51:C54`; dòng 57–63 | Rà bên liên quan, người sử dụng, cách trao đổi và tần suất báo cáo. |
| `C67:C69` | Điều chỉnh rủi ro ban đầu, ràng buộc và các giả định sau khi nhóm đã thảo luận. |
| Dòng 76–78 | Người có thẩm quyền điền họ tên, đơn vị, chữ ký và ngày xác nhận tại các cột C, D, E, F. Khi chưa xác nhận, để trống. |

Ví dụ cách viết phần nhân sự ở `C35`: `[Họ tên] — Developers — phụ trách giao diện và kiểm thử — [email/điện thoại]`. Thay nội dung trong ngoặc bằng thông tin thực tế.

Nếu dùng thêm dòng ngân sách 43, điền hạng mục tại `B43`, cơ sở dự toán tại `C43`, đơn giá tại `E43`, số lượng tại `F43` và gõ `=E43*F43` vào `G43`. Các dòng 44–47 làm tương tự. Giữ công thức tổng `=SUM(G41:G47)` tại `G48`; tổng dự toán không được vượt trần `G10`.

Phần ngân sách hiện tạm chia 90 triệu thực hiện và 10 triệu dự phòng; đây là dự toán giả định. Các tên Nguyễn Văn C, Phạm Thị A, Lê Văn B là nhân vật trong PDF; cần đối chiếu khi áp dụng cho dự án thực tế.

**Bước 3 — Lưu, đóng Excel và kiểm tra.**

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py check --step 01
```

Hoàn thiện khi mục tiêu, phạm vi, bàn giao và các giới hạn đã rõ; thông tin còn chờ xác nhận được ghi rõ để người có trách nhiệm xử lý. Lệnh `check` kiểm tra dữ liệu cơ bản, còn việc đồng ý với Charter do những người tham gia dự án thực hiện.

</details>

<details id="san-pham-02">
<summary><strong>Sản phẩm 02 — WBS: phân chia phạm vi thành các phần việc rõ ràng</strong></summary>

**1. Sản phẩm này là gì?**

WBS là cấu trúc phân chia công việc của dự án thành các nhánh từ lớn đến nhỏ. Quy tắc 100% nghĩa là các phần con phải bao phủ đủ phạm vi phần cha, tránh bỏ sót và tính trùng.

File này có hai sheet để nhìn cùng dự án theo hai cách:

- **`WBS_San_pham`**, theo hình 4-1: phần mềm → ba mô-đun → các chức năng. Ví dụ: Blue Moon → quản lý thu phí → quản lý khoản thu bắt buộc.
- **`WBS_Scrum`**, theo hình 4-3: quản lý dự án; xây dựng phần mềm; chăm sóc/hỗ trợ. Trong từng mô-đun có hoạt động làm rõ yêu cầu, lập kế hoạch Sprint, phát triển và vận hành. Các hoạt động được thực hiện lặp qua các Sprint.

**2. Cần những nguyên liệu gì?**

- Charter 01 đã được rà soát, nhất là phạm vi và sản phẩm bàn giao.
- Bài 4.2, hình 4-1 và 4-3 trong PDF.
- Mẫu `input-docs/Mẫu cấu trúc phân chia công việc.xlsx`.
- 17 Feature của bài trước, cùng các NFR phải đáp ứng trong quá trình phát triển.

**3. Sản phẩm tạo ra có ý nghĩa gì?**

WBS giúp nhóm biết toàn bộ phạm vi cần làm, phát hiện việc còn thiếu và chia việc đủ rõ để giao người thực hiện. Nó cung cấp đầu vào cho việc ước lượng và lập kế hoạch Sprint.

**4. Làm thế nào để hoàn thiện sản phẩm?**

**Bước 1 — Mở file và chọn lần lượt hai tab WBS.**

```powershell
$tep = '.\result\02-Lap-ke-hoach-du-an\02-WBS.xlsx'
if (-not (Test-Path -LiteralPath $tep)) {
    & '.\.venv\Scripts\python.exe' .\src\tool.py create --step 02
}
Invoke-Item -LiteralPath $tep
```

**Bước 2 — Đọc cây công việc từ dòng 6, đối chiếu và bổ sung.**

| Cột | Thuộc tính | Cách hoàn thiện |
| --- | --- | --- |
| A | Cấp | 0 là toàn dự án; cấp tăng lên khi phân chia chi tiết hơn. |
| B | Mã WBS | Kiểm tra mã thể hiện đúng nhánh cha/con, ví dụ `1`, `1.1`, `1.2`. |
| C | Nội dung | Viết rõ sản phẩm hoặc công việc của nhánh. Nếu quá lớn, chia thành các phần nhỏ hơn. |
| D | Phụ trách | Thay vai trò chung bằng người thực tế được giao. |
| E:F | Ngày dự kiến | Điền sau khi đã xác định lịch; có thể để trống khi còn chờ ước lượng. |
| G | Mã Feature/phạm vi | Giữ liên hệ với các mã `FT-xx`; dùng mô tả để làm rõ nhánh bao gồm gì. |
| H | Chi phí dự kiến | Chỉ điền khi có cơ sở ước lượng; tránh cộng cả chi phí cha và con cho cùng phần việc. |

Nếu cần thêm việc con: bấm chuột phải vào số dòng → **Insert**, sao chép định dạng dòng gần đó rồi điền cấp, mã và nội dung mới. Giữ mã `FT-xx` ở dòng đại diện cho Feature; các việc con có thể tham chiếu bằng mã WBS để tránh lặp mã Feature trong cột G.

**Bước 3 — Rà lại phạm vi của cả hai sheet.** Mỗi sheet cần thể hiện đủ 17 Feature của nguồn. Đối chiếu thêm công việc quản lý, tài liệu bàn giao, hỗ trợ và các yêu cầu chất lượng; phân công ai sẽ chịu trách nhiệm cho chúng.

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py check --step 02
```

Lưu và đóng Excel trước khi chạy kiểm tra. Hoàn thiện khi các nhánh đủ phạm vi, công việc đủ rõ để trao đổi việc giao người và ước lượng.

</details>

<details id="san-pham-03">
<summary><strong>Sản phẩm 03 — Kế hoạch Agile: dự kiến công việc cho từng Sprint</strong></summary>

**1. Sản phẩm này là gì?**

Kế hoạch Agile trong bài này là bảng sắp các User Story vào những Sprint dự kiến. **Sprint** là một khoảng thời gian cố định để nhóm hướng tới một mục tiêu và tạo ra phần mềm có thể kiểm tra. Phần mềm được hoàn thiện trong Sprint gọi là **Increment**.

Tại Sprint Planning, PO làm rõ mục tiêu và ưu tiên; Developers lựa chọn công việc phù hợp khả năng, cùng ước lượng và lập kế hoạch. Kế hoạch Sprint tương lai được điều chỉnh dựa trên phản hồi và kết quả thực hiện.

**2. Cần những nguyên liệu gì?**

- Charter 01 và WBS 02 đã được rà soát.
- Mẫu `input-docs/Mẫu lập kế hoạch dự án theo nguyên tắc Agile.xlsx`.
- `2. Ghi nhận yêu cầu/Product_Backlog_BlueMoon.xlsx` để lấy 23 Story, ưu tiên và bốn Sprint dự kiến.
- Sheet `User Story` trong `2. Ghi nhận yêu cầu/User_Story_BlueMoon_.xlsx` để liên hệ Story với Feature và nguồn yêu cầu.
- AC, NFR của bài trước và thông tin về nhân sự, khả năng làm việc, ước lượng của nhóm.

**3. Sản phẩm tạo ra có ý nghĩa gì?**

Bảng này giúp nhóm thống nhất dự kiến làm gì trong từng Sprint, ai làm và căn cứ nào để kiểm tra kết quả. Đây cũng là nguồn dữ liệu chung để tạo Gantt, Timeline và Dashboard.

**4. Làm thế nào để hoàn thiện sản phẩm?**

**Bước 1 — Mở file, chọn tab `Ke_hoach_Agile`.**

```powershell
$tep = '.\result\02-Lap-ke-hoach-du-an\03-Ke-hoach-Agile.xlsx'
if (-not (Test-Path -LiteralPath $tep)) {
    & '.\.venv\Scripts\python.exe' .\src\tool.py create --step 03
}
Invoke-Item -LiteralPath $tep
```

**Bước 2 — Đọc dòng Sprint và các Story nằm bên dưới, rồi điền phần nhóm cần chốt.**

| Cột/ô | Thuộc tính | Bạn cần làm gì? |
| --- | --- | --- |
| B | Có rủi ro? | Chọn Có/Không sau khi rà soát; nếu Có, giải thích ở cột K. |
| C:D | Story, Feature | Giữ mã `US-xx`, mã `FT-xx` và dòng đánh dấu `SPRINT` để tool nhận diện. |
| E | Phụ trách | Ghi tên người thực hiện thay cho “Developers (chưa chỉ định)”. |
| F | Story Points | Điền số điểm sau khi Developers cùng ước lượng; chưa có ước lượng thì để trống. |
| G:H | Bắt đầu/kết thúc | Điều chỉnh lịch Story trong giới hạn Sprint của nó. Dòng Sprint ghi giới hạn thời gian chung. |
| I | Số ngày | Giữ công thức, Excel tính từ ngày bắt đầu/kết thúc. |
| J | Trạng thái | Chọn Chưa bắt đầu, Đang thực hiện, Hoàn thành, Tạm dừng hoặc Quá hạn. |
| K, dòng Sprint | Mục tiêu Sprint | Bổ sung kết quả cụ thể nhóm muốn đạt, ví dụ “Cán bộ BQT đăng nhập được và quản lý được hồ sơ hộ cơ bản”. |
| K, dòng Story | Ghi chú/tiêu chí | Giữ tham chiếu nguồn; bổ sung AC cần kiểm tra, NFR liên quan, vướng mắc và bằng chứng kết quả khi có. |
| `H3` | Tỷ lệ hoàn thành | Giữ công thức đếm số Story hoàn thành trên tổng Story. |

Ví dụ cách điền dòng `US-01` đang ở dòng 7: ghi người thực hiện tại `E7`; nếu nhóm đã thống nhất ước lượng 3 điểm thì nhập `3` tại `F7`; điều chỉnh ngày tại `G7:H7` và chọn trạng thái tại `J7`. Số 3 chỉ là ví dụ cách nhập, bạn dùng ước lượng thực tế của nhóm.

Story Points thể hiện độ lớn tương đối của công việc; không tự quy đổi thành ngày công. Ban đầu các Story dùng toàn bộ cửa sổ Sprint, nên nhóm cần chia lịch và phân công cụ thể khi đã rõ khả năng.

**Bước 3 — Đối chiếu tiêu chí hoàn thành.** Mở AC theo từng mã Story và kiểm tra NFR liên quan. Ví dụ chức năng đăng nhập cần được kiểm tra với yêu cầu mật khẩu, khóa tài khoản và quyền truy cập. PO cần rà phần điều chỉnh thu/audit giao nhau giữa `US-05` và `US-20` trong nguồn bài trước.

Chỉ chọn “Hoàn thành” khi công việc đáp ứng tiêu chí và có bằng chứng kiểm tra. Lưu, đóng Excel rồi chạy:

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py check --step 03
```

Hoàn thiện khi từng Sprint có mục tiêu, công việc được nhóm lựa chọn, người làm và ước lượng được chốt ở mức cần thiết. Mỗi lần sửa kế hoạch này, tạo lại từng sản phẩm 04, 05, 06 để cập nhật các cách xem.

</details>

<details id="san-pham-04">
<summary><strong>Sản phẩm 04 — Gantt: thể hiện lịch công việc bằng thanh thời gian</strong></summary>

**1. Sản phẩm này là gì?**

Gantt là bảng đặt các công việc trên một trục thời gian. Mỗi dòng là một công việc; thanh màu thể hiện khoảng thời gian dự kiến thực hiện. Trong tool này, công việc là các Story thuộc những Sprint của kế hoạch Agile.

**2. Cần những nguyên liệu gì?**

- File kế hoạch Agile 03 đã được bạn bổ sung, lưu và đóng.
- Mẫu `input-docs/Mẫu Gantt Chart quản lý dự án.xlsx`.
- Các dữ liệu từ 03: mã Story, nội dung, phụ trách, ngày và trạng thái.

**3. Sản phẩm tạo ra có ý nghĩa gì?**

Gantt giúp bạn nhìn những việc có lịch trùng nhau, nhận ra người có thể đang được giao quá nhiều việc và trao đổi lại ngày thực hiện. Nó giúp đọc lịch chi tiết của kế hoạch Scrum.

**4. Làm thế nào để hoàn thiện sản phẩm?**

**Bước 1 — Tạo Gantt từ kế hoạch 03 mới nhất rồi mở tab `Gantt`.** Đóng file Gantt nếu đang mở trước khi chạy. Lệnh chỉ tạo lại sản phẩm 04 và sao lưu bản cũ:

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py create --step 04 --replace
Invoke-Item -LiteralPath '.\result\02-Lap-ke-hoach-du-an\04-Gantt.xlsx'
```

**Bước 2 — Đọc và đối chiếu bảng từ dòng 10.**

| Vị trí | Nội dung | Cách hoàn thiện |
| --- | --- | --- |
| B:D | Mã, tên Story, phụ trách | Đối chiếu với 03; nếu thiếu người thực hiện, điền ở cột E của 03. |
| E:F | Ngày bắt đầu/kết thúc | Kiểm tra lịch phù hợp; muốn đổi, sửa G:H của Story tương ứng trong 03. |
| G | Số ngày lịch | Do công thức tính, bao gồm cuối tuần. |
| H | % hoàn thành | Tool lấy từ trạng thái Story: 0% khi chưa hoàn thành, 100% khi đã hoàn thành. |
| I trở đi | Lưới thời gian | Thanh màu đánh dấu ngày làm việc thứ Hai–thứ Sáu nằm trong lịch Story. Cuộn ngang để xem toàn bộ. |

Ví dụ, nếu một người bị giao hai Story lớn cùng lúc, bạn cùng nhóm điều chỉnh phân công hoặc ngày ở 03, lưu/đóng file rồi chạy lại lệnh tạo 04. Gantt được cập nhật theo dữ liệu vừa sửa.

**Bước 3 — Kiểm tra file.** Các thông tin chính được lấy từ 03 nên không cần nhập lại tại đây; di chuột vào ghi chú của tên Story để xem Sprint, Feature và trạng thái.

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py check --step 04
```

Hoàn thiện khi lịch Gantt khớp với kế hoạch Agile đã rà soát. Số ô màu có thể ít hơn số ngày ở cột G vì lưới màu bỏ cuối tuần.

</details>

<details id="san-pham-05">
<summary><strong>Sản phẩm 05 — Timeline: tổng hợp Sprint và mốc dự án</strong></summary>

**1. Sản phẩm này là gì?**

Timeline là lịch tổng quan của dự án, tập trung vào các khoảng thời gian và mốc chính. Trong bài này, nó gồm bốn Sprint và ba mốc UAT/bàn giao.

**2. Cần những nguyên liệu gì?**

- Charter 01 để lấy tên và ngày các mốc.
- Kế hoạch Agile 03 để tổng hợp các Story theo Sprint.
- Mẫu `input-docs/Mẫu timeline dự án.xlsx`.

**3. Sản phẩm tạo ra có ý nghĩa gì?**

Timeline giúp khách hàng và nhóm nắm lịch dự án mà không phải đọc từng Story. Bạn dùng nó để chuẩn bị người tham gia UAT, lịch Review và công việc bàn giao.

**4. Làm thế nào để hoàn thiện sản phẩm?**

**Bước 1 — Lưu/đóng 01 và 03, đóng Timeline nếu đang mở, rồi tạo lại 05.**

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py create --step 05 --replace
Invoke-Item -LiteralPath '.\result\02-Lap-ke-hoach-du-an\05-Timeline.xlsx'
```

**Bước 2 — Chọn tab `Timeline`, đọc các dòng 3–9 và bổ sung.**

| Cột | Nội dung | Bạn cần làm gì? |
| --- | --- | --- |
| B | Có rủi ro? | Ghi nhận nếu Sprint/mốc đang có nguy cơ bị ảnh hưởng và giải thích ở J. |
| C | Tên Sprint/mốc | Đối chiếu với 03 và Charter. |
| D | Mục tiêu dự kiến | Các dòng Sprint ban đầu chứa danh sách Story. Bổ sung câu mô tả kết quả cần đạt để người đọc dễ hiểu. |
| E | Trạng thái | Kiểm tra trạng thái tổng hợp của Sprint; với UAT/bàn giao, cập nhật khi có hoạt động và kết quả thực tế. |
| F | Phụ trách | Bổ sung người điều phối Sprint hoặc người chịu trách nhiệm tổ chức mốc. |
| G:H | Ngày bắt đầu/kết thúc | Ngày Sprint lấy từ các Story trong 03; ngày mốc lấy từ 01. Nếu cần đổi lịch gốc, sửa file nguồn rồi tạo lại 05. |
| I | Số ngày | Giữ giá trị/công thức đã tạo; mốc một ngày có thời lượng 1. |
| J | Ghi chú | Ghi người cần tham dự, đầu vào cần chuẩn bị, rủi ro hoặc biên bản liên quan. |

Ví dụ, ở dòng UAT lần 1, ghi người tổ chức ở cột F và bổ sung vào J: “Chuẩn bị dữ liệu thử, danh sách AC và phiếu ghi nhận lỗi”. Khi buổi UAT đã diễn ra, ghi kết quả/đường dẫn biên bản và cập nhật trạng thái phù hợp.

Bộ mẫu có Sprint từ 02/10 đến 24/12/2023; mốc kết thúc dự án là 30/12/2023. Ngày trên dòng Sprint được tổng hợp từ lịch Story, vì vậy cần đối chiếu thêm với giới hạn Sprint ở 03.

**Bước 3 — Lưu, đóng và kiểm tra.** Phần ghi chú, phụ trách hoặc kết quả bạn bổ sung trực tiếp sẽ cần được đối chiếu lại nếu sau này tạo mới 05 bằng `--replace`.

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py check --step 05
```

Hoàn thiện khi lịch các mốc khớp Charter và mỗi mốc có người chuẩn bị, công việc cần làm rõ ràng.

</details>

<details id="san-pham-06">
<summary><strong>Sản phẩm 06 — Dashboard: đọc nhanh tình hình công việc</strong></summary>

**1. Sản phẩm này là gì?**

Dashboard là bảng báo cáo tổng hợp dữ liệu thành các chỉ số và biểu đồ dễ đọc. File này thể hiện trạng thái Story, phân bố Story theo Sprint và tỷ lệ số Story đã hoàn thành.

**2. Cần những nguyên liệu gì?**

- Kế hoạch Agile 03 có trạng thái đã được bạn kiểm tra.
- Mẫu `input-docs/Mẫu Dashboard báo cáo dự án.xlsx`.
- Ưu tiên từ backlog nguồn; ngày chốt dữ liệu và thông tin báo cáo do bạn bổ sung.

**3. Sản phẩm tạo ra có ý nghĩa gì?**

Dashboard hỗ trợ buổi báo cáo tiến độ: công việc nào đang làm, còn bao nhiêu việc chưa bắt đầu, đã hoàn thành bao nhiêu Story. Người đọc cần biết ngày chốt để hiểu các con số phản ánh thời điểm nào.

**4. Làm thế nào để hoàn thiện sản phẩm?**

**Bước 1 — Cập nhật trạng thái ở 03, lưu/đóng file rồi tạo lại 06.** Đóng Dashboard nếu đang mở:

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py create --step 06 --replace
Invoke-Item -LiteralPath '.\result\02-Lap-ke-hoach-du-an\06-Dashboard.xlsx'
```

**Bước 2 — Chọn tab `Dashboard`, kiểm tra số liệu và điền thông tin báo cáo.**

| Vị trí | Nội dung | Bạn cần làm gì? |
| --- | --- | --- |
| `F3` | Ngày chốt | Điền ngày chốt dữ liệu của báo cáo. Nếu chưa có ngày chốt, giữ “Chưa chốt”. |
| `G3` | Trạng thái dự án | Bổ sung mô tả phù hợp thực tế, ví dụ “Đang lập kế hoạch”; hiện là “Dự thảo kế hoạch”. |
| `H3` | % Story hoàn thành | Giữ công thức số Story hoàn thành / tổng Story. |
| B:I, từ dòng 11 | Danh sách công việc | Đối chiếu người làm, ngày, trạng thái, ưu tiên và Sprint với nguồn. |
| K:L và hai biểu đồ phía trên | Bảng đếm và biểu đồ | Được tính từ dữ liệu của Dashboard; không cần tự nhập lại số lượng. |

Ví dụ, sau khi một Story đã đáp ứng tiêu chí, bạn đổi trạng thái của Story đó thành “Hoàn thành” ở 03, lưu/đóng file rồi tạo lại 06. Dashboard mới sẽ đếm thêm một Story hoàn thành sau khi Excel tính lại công thức.

File phản ánh dữ liệu **tại lúc tạo**. Muốn cập nhật sau khi sửa 03, cần tạo lại 06. Ưu tiên được lấy từ backlog nguồn; nếu thay đổi ưu tiên, sửa nguồn, cập nhật lại 03 theo thông báo phụ thuộc rồi tạo lại Dashboard.

**Bước 3 — Lưu, đóng và kiểm tra.**

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py check --step 06
```

Hoàn thiện khi số liệu khớp dữ liệu đã kiểm tra và có ngày chốt phù hợp. Tỷ lệ này tính theo **số Story**, không phản ánh trực tiếp khối lượng Story Points hay phần ngân sách đã dùng.

</details>

<details id="san-pham-07">
<summary><strong>Sản phẩm 07 — Đánh giá và theo dõi rủi ro: chuẩn bị hành động ứng phó</strong></summary>

**1. Sản phẩm này là gì?**

Danh sách rủi ro ghi lại những sự kiện có thể xảy ra và gây ảnh hưởng đến dự án. Với mỗi rủi ro, nhóm cần đánh giá xác suất, mức ảnh hưởng, chuẩn bị cách xử lý và giao người theo dõi.

File có hai sheet: `Danh_gia_rui_ro` để nhận diện/chấm điểm và `Theo_doi_rui_ro` để theo dõi việc phòng ngừa, ứng phó. Chín tình huống mẫu lấy từ Bảng 4-1 trong PDF: nhân sự, thay đổi yêu cầu, thiếu tài liệu, ít trao đổi, chậm phụ thuộc, thủ tục, nghiệm thu, ngân sách, ước lượng.

**2. Cần những nguyên liệu gì?**

- Bài 4.3, nhất là Bảng 4-1 và phần thang đánh giá trong PDF.
- Charter 01; thông tin nhóm, phạm vi và các yêu cầu của Blue Moon.
- Mẫu `input-docs/Mẫu theo dõi rủi ro dự án.xlsx`.
- Nhận định của nhóm về khả năng xảy ra, ảnh hưởng, người chịu trách nhiệm và hạn rà soát.

**3. Sản phẩm tạo ra có ý nghĩa gì?**

Bảng giúp nhóm chuẩn bị trước khi có sự cố, biết ai đang làm việc gì để giảm rủi ro và kiểm tra hành động đó đã thực hiện tới đâu. Nó cung cấp dữ liệu cho ma trận ưu tiên ở sản phẩm 08.

**4. Làm thế nào để hoàn thiện sản phẩm?**

**Bước 1 — Mở file và chọn tab `Danh_gia_rui_ro`.**

```powershell
$tep = '.\result\03-Quan-ly-rui-ro\07-Theo-doi-rui-ro.xlsx'
if (-not (Test-Path -LiteralPath $tep)) {
    & '.\.venv\Scripts\python.exe' .\src\tool.py create --step 07
}
Invoke-Item -LiteralPath $tep
```

**Bước 2 — Rà từng rủi ro ở các dòng 5–13.**

| Cột | Thuộc tính | Cách hoàn thiện |
| --- | --- | --- |
| A:B | Mã và mô tả | Giữ mã `RR-xx`; sửa mô tả để nhóm hiểu tình huống có thể xảy ra. |
| C | Xác suất P | Chọn 1 — thấp, 2 — trung bình hoặc 3 — cao theo nhận định của nhóm. |
| D | Ảnh hưởng I | Chọn 1, 2 hoặc 3; ghi rõ đang xét ảnh hưởng tới thời gian, chi phí hay chỉ tiêu nào. |
| E | Điểm P×I | Giữ công thức nhân C với D, thang điểm từ 1–9. |
| F | Mức ma trận | Giữ công thức C+D−1, mức 1–5 theo hình trang 9. |
| G | Phòng ngừa/ứng phó | Viết hành động cụ thể, kết quả cần đạt và điều kiện cần xử lý. |
| H | Phụ trách | Thay vai trò bằng tên người thực tế chịu trách nhiệm. |

Đối với chỉ tiêu ảnh hưởng đang xét, PDF minh họa mức thấp dưới 5%, trung bình 5–10%, cao trên 10%. Nhóm cần thống nhất chỉ tiêu trước khi chấm; đây là thang **ảnh hưởng**, không phải phần trăm xác suất.

Ví dụ có sẵn: `RR-04` ở dòng 8 nói về việc nhóm và khách hàng ít trao đổi. P=2, I=2 nên điểm `E8` bằng 4 và mức `F8` bằng 3. Bạn bổ sung tên người theo dõi ở `H8`, rồi làm rõ tại `G8` ai mời BQT dự Review và phản hồi được ghi ở đâu.

**Bước 3 — Chọn tab `Theo_doi_rui_ro`, bổ sung việc thực hiện từ dòng 13.**

| Cột | Nội dung | Bạn cần làm gì? |
| --- | --- | --- |
| B:D | Mã, rủi ro, phụ trách | Tự lấy từ sheet đánh giá; muốn sửa, sửa tại sheet đó. |
| E | Hạn rà soát | Điền ngày người phụ trách phải báo kết quả hoặc xem xét lại rủi ro. Hạn ban đầu tạm là cuối Sprint 1. |
| F | Trạng thái hành động | Chọn trong danh sách theo tình hình làm việc thực tế. |
| G | Ưu tiên | Tự lấy từ mức ma trận: mức 1–2 là Thấp, 3 là Trung bình, 4–5 là Cao. |
| H | Ứng phó/kết quả | Ban đầu liên kết với hành động của sheet đánh giá. Khi có kết quả, có thể thay ô này bằng ghi chép gồm ngày, việc đã làm và bằng chứng. |

Ví dụ cách ghi kết quả ở cột H: `[Ngày rà soát] — đã thực hiện [hành động] — bằng chứng: [đường dẫn biên bản] — việc tiếp theo: [...]`. Chỉ điền những hoạt động đã diễn ra. Bảng phía trên đếm trạng thái **hành động ứng phó**.

**Bước 4 — Lưu, đóng và kiểm tra.**

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py check --step 07
```

Hoàn thiện khi mỗi rủi ro có đánh giá, hành động, người theo dõi và hạn rà soát. Tiếp tục cập nhật trong các buổi rà soát/Sprint Review; mỗi lần đổi P/I, tạo lại sản phẩm 08.

</details>

<details id="san-pham-08">
<summary><strong>Sản phẩm 08 — Ma trận rủi ro: nhìn mức ưu tiên cần xử lý</strong></summary>

**1. Sản phẩm này là gì?**

Ma trận rủi ro là bảng đặt từng rủi ro vào giao điểm của **xác suất P** và **ảnh hưởng I**. Ma trận trong bài có ba mức trên mỗi trục, tạo thành chín ô; mỗi ô mang một trong năm mức ưu tiên.

Theo hình trang 9 của PDF, mức ma trận được tính bằng **P+I−1**, từ 1–5. Điểm **P×I** trong Bảng 4-1 là thang 1–9 và được giữ thành cột riêng. Mẫu Excel gốc 5×5 đã được đổi thành 3×3 để theo lý thuyết này.

**2. Cần những nguyên liệu gì?**

- Sheet `Danh_gia_rui_ro` trong sản phẩm 07 đã được nhóm rà soát, lưu và đóng.
- Hình ma trận trang 9 của PDF.
- Mẫu `input-docs/Mẫu ma trận quản lý rủi ro dự án.xlsx`.

**3. Sản phẩm tạo ra có ý nghĩa gì?**

Ma trận giúp nhìn nhanh những rủi ro có xác suất/ảnh hưởng lớn để thảo luận ưu tiên nguồn lực ứng phó. Kết hợp nó với người phụ trách và hành động trong 07 để quyết định việc cần làm tiếp.

**4. Làm thế nào để hoàn thiện sản phẩm?**

**Bước 1 — Chốt P/I ở 07, đóng ma trận nếu đang mở, rồi tạo lại 08.**

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py create --step 08 --replace
Invoke-Item -LiteralPath '.\result\03-Quan-ly-rui-ro\08-Ma-tran-rui-ro.xlsx'
```

**Bước 2 — Chọn tab `Ma_tran_3x3` và đối chiếu.**

| Vị trí | Cách đọc và kiểm tra |
| --- | --- |
| Ma trận màu phía trên | Chọn mức P theo hàng và I theo cột; ô giao nhau chứa mức ưu tiên và mã rủi ro tương ứng. |
| Bảng từ dòng 30 | Đối chiếu từng mã, mô tả, P, I, điểm tích, mức ưu tiên và người phụ trách với 07. |
| Mức 1 → 5 | Rất thấp → Thấp → Trung bình → Cao → Rất cao. |

Ví dụ `RR-04` có P=2, I=2 thì nằm ở giao điểm hàng P=2 và cột I=2, mức 3 — Trung bình; điểm tích của nó vẫn là 4. Hai con số phản ánh hai thang đánh giá đã nêu ở trên.

**Bước 3 — Hoàn thiện thông tin ở nguồn khi cần.** Nếu còn thiếu người phụ trách hoặc muốn đổi P/I, mở 07 để sửa rồi tạo lại 08. Mã, điểm và người phụ trách của ma trận được lấy từ nguồn nên bạn không cần nhập lại tại 08.

```powershell
& '.\.venv\Scripts\python.exe' .\src\tool.py check --step 08
```

Hoàn thiện khi tất cả rủi ro xuất hiện ở đúng ô và thông tin khớp 07. Ma trận là bản tổng hợp tại lúc tạo file; cần tạo lại sau khi thay đổi đánh giá nguồn.

Nếu công thức hoặc biểu đồ ở bất kỳ sản phẩm nào chưa cập nhật khi mở Excel, chọn **Formulas → Calculation Options → Automatic**, sau đó **Calculate Now** và lưu file.

</details>
