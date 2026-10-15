- 🔍LythuyetThaotac: **Tool lập kế hoạch dự án phần mềm — thực hành xây dựng kế hoạch quản lý và thu phí chung cư Blue Moon — Huong dan xay dung Ke hoach du an(2).pdf**. Huong dan xay dung Ke hoach du …

**Quy ước của hướng dẫn:** gọi tool là `MYTOOL-KeHoachDuAn`. Tài liệu PDF cung cấp nghiệp vụ nhưng không có mã nguồn; vì vậy **tên file và các lệnh chạy `src` bên dưới là thiết kế đề xuất để triển khai tool, chưa thể chạy ngay khi chưa có chương trình tương ứng**. Các nội dung bổ sung ngoài PDF được ghi rõ là đề xuất.

<details>
<summary>-nhóm thao tác 'chuẩn bị dữ liệu và hiểu thứ tự tạo các sản phẩm'</summary>

**Bài toán mẫu:** ban quản trị Blue Moon đang quản lý thu phí bằng phương thức thủ công và Excel, cần xây dựng phần mềm quản lý thu phí, người dùng và hộ gia đình.

**Trình tự thực hiện:** xác định dự án → phê duyệt phạm vi → phân rã công việc → lập lịch thực hiện. Việc nhận diện rủi ro bắt đầu từ lúc khởi tạo và được cập nhật xuyên suốt các bước.

| Bước | Sản phẩm | Câu hỏi sản phẩm phải trả lời |
|---|---|---|
| 01 | Tuyên ngôn dự án | Vì sao làm, làm gì, ai tham gia, giới hạn nào? |
| 02 | WBS và mô tả gói công việc | Phải hoàn thành những phần việc nào? |
| 03 | Lịch trình và biểu đồ Gantt | Ai làm, làm khi nào, phụ thuộc công việc nào? |
| 04 | Kế hoạch quản lý rủi ro | Điều gì có thể gây trở ngại, xử lý ra sao? |

**Tổ chức dữ liệu đề xuất:** trong `i-o`, tạo các thư mục `01-khoi-tao`, `02-phan-ra-cong-viec`, `03-lap-lich`, `04-quan-ly-rui-ro`. Mỗi thư mục chứa đầu vào, bản nháp chương trình sinh ra và bản đã được người dùng rà soát.

**Phân biệt trách nhiệm:**

- **Người dùng:** cung cấp yêu cầu, nhân sự, ước lượng, cam kết ngân sách, ngày bàn giao và quyết định phê duyệt.
- **Chương trình:** kiểm tra dữ liệu, dựng bảng/sơ đồ, tính ngày hoặc mức rủi ro theo quy tắc đã chọn.
- **Người dùng hoàn thiện:** xem xét kết quả, sửa giả định chưa phù hợp và xác nhận khả năng thực hiện.

**Nguyên tắc:** chương trình tạo được tài liệu không có nghĩa nội dung đã được khách hàng hoặc nhà tài trợ chấp thuận.

</details>

<details>
<summary>-nhóm thao tác 'tạo và hoàn thiện tuyên ngôn dự án — Bài 4.1'</summary>

**-sản phẩm 'tuyên ngôn dự án Blue Moon — xác định mục tiêu, phạm vi, nguồn lực và phê duyệt'**

**1. Lý thuyết: sản phẩm này là gì?**

**Tuyên ngôn dự án (Project Charter)** là văn bản chính thức cho phép dự án tồn tại và trao quyền cho người quản lý dự án sử dụng nguồn lực để thực hiện dự án. Theo tài liệu, nhà tài trợ là bên ban hành văn bản này.

Cần phân biệt:

| Thuộc tính | Ý nghĩa | Ví dụ trong bài toán |
|---|---|---|
| Bối cảnh | Hiện trạng dẫn đến nhu cầu làm dự án | Quản lý thủ công, Excel chưa đáp ứng tốt |
| Mục đích | Vấn đề nghiệp vụ muốn giải quyết | Hỗ trợ quản lý dân cư và thu phí |
| Mục tiêu | Kết quả có thể kiểm tra, đo lường | Quản lý đầy đủ các loại phí thuộc phạm vi đã thống nhất |
| Phạm vi sản phẩm | Những chức năng phần mềm phải có | Quản lý thu phí, người dùng, hộ gia đình |
| Phạm vi dự án | Những công việc nhóm phải thực hiện | Đặc tả, thiết kế, lập trình, kiểm thử, triển khai |
| Sản phẩm bàn giao | Những thứ phải giao để nghiệm thu | Phần mềm, mã nguồn, tài liệu kỹ thuật, hướng dẫn sử dụng |
| Ràng buộc | Giới hạn bắt buộc phải tuân thủ | Ngân sách, thời hạn |
| Giả định | Điều tạm coi là đúng để lập kế hoạch | Người dùng tham gia dùng thử và góp ý |

**2. Nguyên liệu đầu vào**

Tạo file đề xuất: `i-o/01-khoi-tao/01-thong-tin-du-an.json`.

Người dùng cần điền:

- Tên dự án, nhà tài trợ, đơn vị tài trợ.
- Người quản lý, thành viên, vai trò và thông tin liên hệ.
- Đại diện khách hàng, người sử dụng, các bên liên quan.
- Bối cảnh, mục đích, mục tiêu và tiêu chí kiểm tra.
- Phạm vi được làm, phạm vi loại trừ.
- Sản phẩm bàn giao.
- Ngân sách, mốc thời gian, giả định, ràng buộc.
- Cách trao đổi, báo cáo và người có thẩm quyền phê duyệt.

**Dữ liệu có sẵn trong PDF:** ngân sách 100.000.000 đồng; các mốc bàn giao 30/11/2023, 15/12/2023 và hoàn thành 30/12/2023. Đây là **mốc của bài mẫu**, cần thay nếu thực hành cho dự án khác.

**3. Lệnh chạy `src` — giao diện đề xuất**

Mở thư mục gốc `MYTOOL-KeHoachDuAn` bằng VSCode → chọn **Terminal → New Terminal** → dùng terminal PowerShell. Chương trình dự kiến nhận file JSON và tạo bản Markdown:

```powershell
python ".\src\tao_tuyen_ngon.py" `
    --input ".\i-o\01-khoi-tao\01-thong-tin-du-an.json" `
    --output ".\i-o\01-khoi-tao\02-tuyen-ngon-du-an.md"
```

**4. Bổ sung, sửa và xem xét thuộc tính**

- Trong VSCode, mở file đầu vào → sửa thông tin còn thiếu → lưu bằng **Ctrl+S** → chạy lại chương trình.
- Nếu mục tiêu ghi “quản lý 100%”, phải xác định **100% của danh sách nào và kiểm tra bằng cách nào**. Ví dụ: mọi loại phí trong danh mục yêu cầu đều có chức năng tạo khoản thu, ghi nhận thanh toán và tra cứu.
- Phân biệt **“không thực hiện nhập dữ liệu ban đầu”** với **“phần mềm không có chức năng nhập dữ liệu”**: hai điều này khác nhau. PDF loại trừ công việc nhập liệu ban đầu khỏi phạm vi dự án.
- Tách rõ bản thử nghiệm, bản chính thức và ngày kết thúc dự án.
- Đối chiếu ngân sách với chi phí phát triển, quản lý và dự phòng; không tính dự phòng hai lần.
- Chỉ điền tên, chữ ký, ngày phê duyệt khi có xác nhận thực tế.

**5. Ý nghĩa của sản phẩm**

Tuyên ngôn tạo căn cứ thống nhất để nhóm lập WBS, lịch trình và kế hoạch rủi ro. Nếu phạm vi chưa rõ, những sản phẩm lập kế hoạch phía sau sẽ thiếu cơ sở.

</details>

<details>
<summary>-nhóm thao tác 'phân rã phạm vi thành WBS và gói công việc — Bài 4.2'</summary>

**-sản phẩm 'WBS và mô tả gói công việc — chuyển phạm vi thành các phần việc có thể giao và kiểm tra'**

**1. Lý thuyết: sản phẩm này là gì?**

**WBS (Work Breakdown Structure)** là cấu trúc phân cấp phân rã toàn bộ công việc thuộc phạm vi dự án thành các phần nhỏ hơn.

**Gói công việc (Work Package)** là phần ở cấp thấp nhất của WBS đang sử dụng, đủ rõ để ước lượng, giao trách nhiệm và kiểm tra hoàn thành. Nếu vẫn quá lớn, tiếp tục phân rã; khi lập lịch, có thể xác định các hoạt động để hoàn thành gói đó.

**Quy tắc 100%:** các mục con phải bao phủ đầy đủ phạm vi của mục cha; tránh bỏ sót hoặc tính trùng công việc.

PDF giới thiệu hai cách tổ chức:

| Cách phân rã | Cách hiểu | Ví dụ |
|---|---|---|
| Theo sản phẩm bàn giao | Chia theo phần sản phẩm cần tạo | Phần mềm → module thu phí → chức năng thu phí |
| Theo quy trình | Chia theo nhóm hoạt động hoặc pha thực hiện | Dự án → xây dựng phần mềm → thiết kế → thiết kế dữ liệu |

**WBS không phải lịch làm việc:** mã `2.1` thể hiện vị trí trong cấu trúc, không tự mang nghĩa phải làm trước mã `2.2`.

**2. Nguyên liệu đầu vào**

- Tuyên ngôn đã được rà soát.
- Danh sách chức năng/yêu cầu.
- Danh sách sản phẩm bàn giao.
- Những công việc hỗ trợ: quản lý, kiểm thử, tài liệu, triển khai và bàn giao.
- Cách phân rã nhóm lựa chọn.

Tạo file đề xuất: `i-o/02-phan-ra-cong-viec/01-danh-sach-cong-viec.csv`.

| Thuộc tính đề xuất | Người dùng cần điền |
|---|---|
| `ma` | Mã duy nhất của mục WBS |
| `macha` | Mã mục cha; để trống với mục gốc |
| `ten` | Tên phần việc hoặc sản phẩm |
| `dauvao` | Những dữ liệu/tài liệu cần có |
| `dau ra` | Sản phẩm cụ thể tạo ra |
| `tieuchichapnhan` | Điều kiện để xác nhận hoàn thành |
| `nguoiphutrach` | Người chịu trách nhiệm |

**Ví dụ phân rã một phần chức năng:** quản lý thu phí → tạo khoản thu, ghi nhận thu phí, thống kê các khoản đóng góp.

Đây mới là một nhánh sản phẩm; muốn lập WBS toàn dự án cần bổ sung các công việc để thiết kế, xây dựng, kiểm thử và bàn giao những chức năng đó.

**3. Lệnh chạy `src` — giao diện đề xuất**

```powershell
python ".\src\tao_wbs.py" `
    --input ".\i-o\02-phan-ra-cong-viec\01-danh-sach-cong-viec.csv" `
    --output ".\i-o\02-phan-ra-cong-viec\02-wbs.html"
```

**4. Bổ sung, sửa và xem xét thuộc tính**

- Mở file CSV trong VSCode hoặc phần mềm bảng tính; mỗi dòng là một mục WBS.
- Thêm mục con bằng cách tạo mã mới và điền đúng `macha`.
- Kiểm tra mọi `macha` đều tham chiếu đến mục tồn tại; không có mục tự làm cha của chính nó hoặc tạo vòng lặp.
- Thay tên chung chung như “xử lý chức năng” bằng đầu ra rõ: “hoàn thiện chức năng ghi nhận thanh toán”.
- Với gói “kiểm thử ghi nhận thanh toán”, tiêu chí có thể là: các ca kiểm thử đã thống nhất được thực hiện, lỗi được ghi nhận và các lỗi chặn nghiệm thu được xử lý.
- Đối chiếu lại danh sách bàn giao: có phần mềm nhưng thiếu tài liệu cài đặt thì WBS vẫn chưa đầy đủ.
- Không cộng đồng thời chi phí của mục cha và toàn bộ mục con nếu mục cha đã là tổng của các mục con.

**5. Ý nghĩa của sản phẩm**

WBS giúp tránh bỏ sót phạm vi và tạo nền tảng cho ước lượng, phân công, lập lịch. **Mô tả gói công việc** giúp người nhận hiểu thế nào là làm xong, thay vì chỉ biết tên việc.

</details>

<details>
<summary>-nhóm thao tác 'lập lịch thực hiện và biểu đồ Gantt — Bài 4.2'</summary>

**-sản phẩm 'lịch trình và biểu đồ Gantt — xác định thời gian, phụ thuộc và người thực hiện'**

**1. Lý thuyết: sản phẩm này là gì?**

**Biểu đồ Gantt** biểu diễn các công việc trên trục thời gian: mỗi thanh thể hiện khoảng thực hiện một công việc.

Cần phân biệt:

| Thuật ngữ | Ý nghĩa |
|---|---|
| Thời lượng (Duration) | Khoảng thời gian làm việc cần để hoàn thành hoạt động |
| Công sức (Effort) | Tổng thời gian lao động, ví dụ 24 giờ công |
| Quan hệ phụ thuộc (Dependency) | Ràng buộc giữa các công việc |
| Mốc (Milestone) | Sự kiện đánh dấu kết quả quan trọng, thường có thời lượng bằng 0 |
| Lịch làm việc (Calendar) | Quy định ngày làm, giờ làm, ngày nghỉ |

**Ví dụ:** 24 giờ công không nhất thiết bằng 3 ngày lịch. Nếu một người chỉ dành 4 giờ/ngày cho dự án thì cần 6 ngày làm việc; thêm người cũng không tự bảo đảm thời lượng giảm theo tỷ lệ.

Quan hệ cơ bản để bắt đầu học là **kết thúc–bắt đầu (Finish-to-Start)**: công việc sau chỉ bắt đầu khi công việc trước kết thúc.

**2. Nguyên liệu đầu vào**

Tạo file đề xuất: `i-o/03-lap-lich/01-lich-cong-viec.csv`, dựa trên các hoạt động đã xác định từ WBS.

Cần có:

- Mã và tên công việc.
- Gói WBS tương ứng.
- Thời lượng, đơn vị thời gian.
- Công việc tiền nhiệm.
- Người thực hiện và khả năng tham gia.
- Ngày bắt đầu dự án, lịch làm việc, ngày nghỉ.
- Các mốc bàn giao bắt buộc.

**Ví dụ bổ sung để luyện tập**, không phải thời lượng do PDF quy định:

| Mã | Hoạt động | Thời lượng | Tiền nhiệm |
|---|---|---:|---|
| A | Xác nhận yêu cầu thu phí | 2 ngày làm việc | Không |
| B | Thiết kế dữ liệu thu phí | 2 ngày làm việc | A |
| C | Lập trình chức năng thu phí | 4 ngày làm việc | B |
| D | Kiểm thử chức năng thu phí | 2 ngày làm việc | C |

Nếu không chồng lấn và không có thời gian chờ: tổng thời lượng chuỗi = 2 + 2 + 4 + 2 = **10 ngày làm việc**.

**3. Lệnh chạy `src` — giao diện đề xuất**

```powershell
python ".\src\tao_gantt.py" `
    --input ".\i-o\03-lap-lich\01-lich-cong-viec.csv" `
    --calendar ".\i-o\03-lap-lich\02-lich-lam-viec.json" `
    --output ".\i-o\03-lap-lich\03-gantt.html"
```

**4. Bổ sung, sửa và xem xét thuộc tính**

- Điền lịch làm việc trước khi tính ngày kết thúc; không trộn ngày lịch với ngày làm việc.
- Điền quan hệ phụ thuộc dựa trên điều kiện thực hiện, thay vì nối mọi công việc thành một chuỗi.
- Kiểm tra không có phụ thuộc vòng: A chờ B nhưng B lại chờ A.
- Kiểm tra một người có bị giao nhiều việc đồng thời vượt khả năng tham gia hay không.
- Khi trễ hạn, xem xét phạm vi, nguồn lực, phụ thuộc và ước lượng; không chỉ sửa ngày để biểu đồ “đẹp”.
- Giữ riêng ngày kế hoạch và ngày thực tế nếu theo dõi tiến độ.
- Các mốc nghiệm thu trong lịch phải thống nhất với tuyên ngôn.

**Lưu ý về tài liệu nguồn:** PDF nêu Gantt trong tên Bài 4.2 nhưng phần minh họa chủ yếu là WBS; các trường lập lịch và ví dụ trên là phần bổ sung để thực hành.

**5. Ý nghĩa của sản phẩm**

Lịch trình cho biết kế hoạch có khả thi với thời hạn và nguồn lực hay không. Gantt giúp nhìn rõ các hoạt động chồng lấn, các khoảng chờ và ảnh hưởng khi một công việc bị chậm.

</details>

<details>
<summary>-nhóm thao tác 'lập và hoàn thiện kế hoạch quản lý rủi ro — Bài 4.3'</summary>

**-sản phẩm 'danh mục rủi ro, mức ưu tiên và phương án ứng phó'**

**1. Lý thuyết: sản phẩm này là gì?**

**Rủi ro** là sự kiện hoặc điều kiện chưa chắc xảy ra nhưng nếu xảy ra sẽ ảnh hưởng đến mục tiêu dự án. Bài thực hành tập trung vào những ảnh hưởng bất lợi.

**Phân biệt:** “thành viên có thể rời dự án” là rủi ro; “thành viên đã rời dự án” là vấn đề đang xảy ra, cần xử lý thực tế.

Một mô tả dễ hiểu có cấu trúc: **nguyên nhân → sự kiện có thể xảy ra → ảnh hưởng**.

Ví dụ: một thành viên đang tham gia nhiều dự án → có thể không đủ thời gian thực hiện module thu phí → chậm lịch tích hợp và nghiệm thu.

**2. Nguyên liệu đầu vào**

Tạo file đề xuất: `i-o/04-quan-ly-rui-ro/01-danh-muc-rui-ro.csv`.

Dữ liệu lấy từ phạm vi, WBS, lịch trình, nhân sự, ngân sách và trao đổi với các bên liên quan.

| Thuộc tính | Nội dung cần điền |
|---|---|
| Mã rủi ro | Mã duy nhất |
| Mô tả | Nguyên nhân, sự kiện, ảnh hưởng |
| Xác suất | Thấp = 1; vừa = 2; cao = 3 |
| Tác động | Thấp = 1; vừa = 2; cao = 3 |
| Biện pháp phòng ngừa | Làm gì trước khi rủi ro xảy ra? |
| Phương án xử lý | Làm gì khi rủi ro xảy ra? |
| Người phụ trách | Ai theo dõi và thực hiện? |
| Dấu hiệu kích hoạt | Khi nào cần hành động? |
| Trạng thái | Đang theo dõi, đã xảy ra, đã đóng… |

Các trường người phụ trách, dấu hiệu kích hoạt và trạng thái là **đề xuất bổ sung** để kế hoạch có thể sử dụng trong thực tế.

**3. Chọn thống nhất quy tắc đánh giá**

**Tài liệu có điểm không thống nhất:**

- Bảng 4-1 ghi trường hợp xác suất 2, tác động 2 có giá trị **4**.
- Ma trận cuối tài liệu xếp cùng trường hợp vào **Mức 3**.
- Phần diễn giải trang 8 lặp nhãn Mức 4 và Mức 5 ở hai dòng cuối.

Vì vậy, không được nhập các giá trị đó vào một cột rồi coi là cùng một đại lượng.

Để bám **ma trận cuối tài liệu**, có thể dùng:

| Xác suất ↓ / Tác động → | Thấp: 1 | Vừa: 2 | Cao: 3 |
|---|---:|---:|---:|
| Thấp: 1 | Mức 1 | Mức 2 | Mức 3 |
| Vừa: 2 | Mức 2 | Mức 3 | Mức 4 |
| Cao: 3 | Mức 3 | Mức 4 | Mức 5 |

Với đúng ma trận này: **mức ưu tiên = xác suất + tác động − 1**. Đây là cách biểu diễn lại bảng, không phải công thức áp dụng cho mọi phương pháp đánh giá rủi ro.

Nếu nhóm còn dùng **điểm = xác suất × tác động**, hãy lưu ở cột riêng. Ví dụ: xác suất 2, tác động 2 → **điểm tích = 4**, nhưng **mức theo ma trận = 3**.

**4. Lệnh chạy `src` — giao diện đề xuất**

```powershell
python ".\src\tao_ke_hoach_rui_ro.py" `
    --input ".\i-o\04-quan-ly-rui-ro\01-danh-muc-rui-ro.csv" `
    --method "ma-tran-tai-lieu" `
    --output ".\i-o\04-quan-ly-rui-ro\02-ke-hoach-rui-ro.html"
```

**5. Bổ sung, sửa và xem xét thuộc tính**

- Người dùng đánh giá xác suất và tác động dựa trên thông tin dự án; chương trình chỉ kiểm tra và tính theo quy tắc được chọn.
- Với mỗi đánh giá, ghi lý do. Ví dụ: xác suất vừa vì thành viên đã thông báo lịch học trùng; tác động cao vì đang là người duy nhất hiểu module.
- Tránh biện pháp chung chung như “cố gắng hoàn thành”: thay bằng “tài liệu hóa module, bố trí người dự phòng và rà soát tiến độ hằng tuần”.
- Tách **phòng ngừa** với **xử lý khi xảy ra**: chia sẻ kiến thức trước là phòng ngừa; phân công lại sau khi người phụ trách nghỉ là xử lý.
- Sắp xếp mức ưu tiên giảm dần; các rủi ro cùng mức cần xem thêm hạn hành động và mức ảnh hưởng cụ thể.
- Rà soát lại khi đổi yêu cầu, nhân sự, ngân sách hoặc lịch bàn giao.
- Trước khi nộp, thống nhất với giảng viên/nhóm về cách xử lý các điểm không nhất quán trong tài liệu.

**6. Ý nghĩa của sản phẩm**

Kế hoạch rủi ro giúp nhóm chuẩn bị hành động và nguồn lực trước khi gặp trở ngại. Giá trị của sản phẩm nằm ở **người chịu trách nhiệm, dấu hiệu cần hành động và phương án cụ thể**, bên cạnh bảng chấm điểm.

</details>

<details>
<summary>-nhóm thao tác 'kiểm tra sự thống nhất và hoàn thiện bộ sản phẩm'</summary>

**-sản phẩm 'bộ kế hoạch dự án đã rà soát để trình phê duyệt'**

**Đầu vào:** tuyên ngôn, WBS, lịch trình/Gantt và kế hoạch rủi ro đã được người dùng hoàn thiện.

| Kiểm tra | Điều kiện đạt |
|---|---|
| Phạm vi → WBS | Mỗi phần phạm vi và sản phẩm bàn giao đều có công việc tương ứng |
| WBS → lịch trình | Các hoạt động cần thiết đã được lập lịch và giao người thực hiện |
| Lịch trình → tuyên ngôn | Các mốc bàn giao và giới hạn thời gian nhất quán |
| Công việc → ngân sách | Chi phí được dự tính đầy đủ, tránh cộng trùng |
| Rủi ro → kế hoạch | Biện pháp ứng phó cần thời gian hoặc chi phí đã được tính đến |
| Nội dung → phê duyệt | Những điểm cần quyết định có người xác nhận |

**Cách hoàn thiện:** sửa ở dữ liệu đầu vào → chạy lại chương trình tương ứng → đối chiếu kết quả với các sản phẩm liên quan. Tránh chỉ sửa bản xuất vì lần sinh tiếp theo có thể làm mất thay đổi.

**Ý nghĩa:** bộ sản phẩm phải kể được một câu chuyện thống nhất: **dự án cam kết làm gì → phải làm những việc nào → thực hiện bằng nguồn lực và lịch nào → chuẩn bị ra sao trước rủi ro**.

</details>
