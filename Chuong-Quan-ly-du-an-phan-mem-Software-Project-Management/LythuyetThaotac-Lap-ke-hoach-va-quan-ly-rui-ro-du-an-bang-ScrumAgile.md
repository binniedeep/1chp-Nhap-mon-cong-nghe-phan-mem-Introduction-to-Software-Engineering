### 🔍LythuyetThaotac: Khởi tạo, lập kế hoạch và quản lý rủi ro dự án phần mềm — Huong dan xay dung Ke hoach du an(8).pdf - https://lms.hust.edu.vn/mod/page/view.php?id=63968
https://husteduvn.sharepoint.com/sites/Elearning2/Shared%20Documents/Elearning/2023/02.%20Tr%C6%B0%E1%BB%9Dng%20CNTT%26TT/02_IT3180_Nh%E1%BA%ADp%20m%C3%B4n%20C%C3%B4ng%20ngh%E1%BB%87%20ph%E1%BA%A7n%20m%E1%BB%81m/PDF/IT3180_Pr03_Prj-C4_intro_final.pdf

Tài liệu hướng dẫn gốc: Huong dan xay dung Ke hoach du an(8).pdf

Mình chuẩn hóa nội dung thành **8 sản phẩm quản lý dự án**. Trong mỗi sản phẩm, các bước đều có **ý nghĩa, cách thao tác và dữ liệu minh họa** để bạn có thể mở mẫu lên rồi thực hiện.

### Giới thiệu bài toán mẫu để học cách thao tác

Ta cần xây dựng **phần mềm quản lý và thu phí chung cư Blue Moon**, gồm ba module:

- **Quản lý hộ gia đình:** lưu thông tin căn hộ, chủ hộ và thành viên.
- **Quản lý người dùng:** tài khoản đăng nhập và phân quyền.
- **Quản lý thu phí:** tạo khoản thu, ghi nhận đóng tiền và thống kê.

Các dữ liệu sau là **giả định để thực hành**, được dùng thống nhất trong phần hướng dẫn:

| Nội dung | Dữ liệu thực hành |
|---|---|
| Thời gian dự án | 05/10/2026–25/12/2026, tương ứng 12 tuần |
| Ngân sách tối đa | 100.000.000 đồng |
| Khách hàng | Ban quản trị chung cư Blue Moon |
| Nhà tài trợ | Đại diện Công ty ABC |
| An | Quản lý dự án, phân tích yêu cầu |
| Bình | Lập trình xử lý nghiệp vụ và dữ liệu |
| Chi | Lập trình giao diện |
| Dũng | Kiểm thử và hỗ trợ triển khai |
| Quy mô dữ liệu để kiểm thử | 200 hộ gia đình |
| Ngày báo cáo minh họa | 27/11/2026 |

**Cách chuẩn bị:** mở từng file rồi chọn **File → Save As** để tạo bản thực hành. Ưu tiên sheet có chữ `BLANK`; riêng WBS chỉ có một sheet.

Các file hiện là những workbook riêng. Bạn cần giữ thống nhất tên dự án, mã công việc, ngày tháng và ngân sách giữa chúng; chúng chưa tự liên kết với nhau.

Các công thức bên dưới dùng dấu phẩy phân cách đối số. Nếu Excel của bạn yêu cầu dấu chấm phẩy, thay dấu phẩy phân cách bằng `;`.

---

<details>
<summary>-sản phẩm 'Điều lệ dự án — Project Charter' - 'Thống nhất lý do làm dự án, phạm vi, nguồn lực và căn cứ phê duyệt'</summary>

Mẫu sử dụng: Mẫu Project Charter.xlsx

**Sản phẩm cần tạo:** một điều lệ đủ rõ để khách hàng, nhà tài trợ và đội thực hiện cùng hiểu: dự án làm gì, bàn giao gì, mất bao lâu, được chi bao nhiêu và ai chịu trách nhiệm.

#### Bước 1: Điền thông tin nhận diện — Xác định dự án và người chịu trách nhiệm

**Ý nghĩa:** thông tin này giúp phân biệt người tài trợ, người quản lý và đơn vị sử dụng kết quả.

**Cách thao tác:**

Mở sheet `BLANK - Project Charter`, điền:

| Vị trí | Nội dung | Ví dụ |
|---|---|---|
| B4 | PROJECT NAME | Phần mềm quản lý và thu phí chung cư Blue Moon |
| E4 | PROJECT MANAGER | An |
| G4 | PROJECT SPONSOR | Đại diện Công ty ABC |
| B6 | EMAIL | Email thực tế của quản lý dự án |
| D6 | PHONE | Số điện thoại thực tế |
| E6 | ORGANIZATIONAL UNIT(S) | Công ty ABC và Ban quản trị Blue Moon |
| E8 | EXPECTED START DATE | 05/10/2026 |
| G8 | EXPECTED COMPLETION DATE | 25/12/2026 |

Các mục `GREEN BELTS ASSIGNED`, `BLACK BELTS ASSIGNED` thuộc bối cảnh cải tiến quy trình của mẫu. Với bài toán này, có thể ghi **Không áp dụng**.

Nhập ngày dưới dạng ngày của Excel, sau đó chọn **Ctrl+1 → Custom → dd/mm/yyyy**.

#### Bước 2: Viết vấn đề, mục đích và mục tiêu — Làm rõ dự án cần giải quyết điều gì

**Ý nghĩa:** cần phân biệt ba câu hỏi:

- **Vấn đề:** hiện tại đang gặp khó khăn gì?
- **Mục đích:** muốn cải thiện điều gì?
- **Mục tiêu:** dựa vào kết quả nào để biết đã đạt?

**Cách thao tác và điền dữ liệu:**

| Vị trí | Nội dung cần viết | Ví dụ |
|---|---|---|
| C13 | PROBLEM OR ISSUE | Dữ liệu hộ dân và thu phí được quản lý bằng nhiều file Excel, khó đối chiếu khoản đã đóng và chưa đóng. |
| C14 | PURPOSE OF PROJECT | Tập trung thông tin hộ gia đình và hỗ trợ quản lý thu phí trên một phần mềm. |
| C15 | BUSINESS CASE | Giảm thao tác tổng hợp thủ công, tăng khả năng tra cứu và đối chiếu số tiền thu. |
| C16 | GOALS / METRICS | Quản lý được bộ dữ liệu kiểm thử 200 hộ; xử lý đầy đủ danh mục phí đã thống nhất; 20 tình huống nghiệm thu bắt buộc đều đạt; bàn giao trước hoặc đúng 25/12/2026 trong ngân sách 100 triệu đồng. |

**Cách kiểm tra:** mục tiêu “phần mềm dễ dùng” còn khó đánh giá. Hãy bổ sung tình huống cụ thể, chẳng hạn: “Kế toán tìm được danh sách hộ chưa đóng một khoản phí theo tháng”.

#### Bước 3: Xác định sản phẩm bàn giao và phạm vi — Chốt những gì phải tạo ra

**Ý nghĩa:** sản phẩm bàn giao là thứ khách hàng hoặc chủ đầu tư nhận được. Phạm vi bao gồm cả công việc cần thực hiện để tạo ra chúng.

**Cách thao tác:**

Tại **C17 — EXPECTED DELIVERABLES**, liệt kê:

- Bộ cài phần mềm và cấu hình triển khai.
- Ba module đã thống nhất.
- Mã nguồn.
- Tài liệu đặc tả yêu cầu và phân tích thiết kế.
- Bộ tình huống kiểm thử, kết quả kiểm thử và biên bản nghiệm thu.
- Hướng dẫn cài đặt, hướng dẫn sử dụng.
- Tài liệu cấu trúc mã nguồn, tài liệu API nếu sản phẩm có API.
- Hồ sơ quản lý dự án.
- Chứng nhận bản quyền phần mềm nếu thực hiện đầy đủ đầu mục bàn giao nêu trong đề bài PDF.

Tại **C20 — WITHIN SCOPE**, ghi:

> Khảo sát, đặc tả yêu cầu, thiết kế, lập trình, kiểm thử, triển khai và hướng dẫn sử dụng ba module quản lý hộ gia đình, quản lý người dùng và quản lý thu phí.

Tại **C21 — OUTSIDE OF SCOPE**, ghi:

> Không bao gồm việc nhập toàn bộ dữ liệu dân cư thực tế thay cho khách hàng; chưa triển khai ứng dụng điện thoại hoặc thanh toán trực tuyến trong phiên bản này.

**Mối liên hệ:** từng đầu mục trong phạm vi phải xuất hiện trong WBS ở sản phẩm tiếp theo.

#### Bước 4: Điền các mốc chính — Xác định những lần cần xem xét và xác nhận kết quả

**Ý nghĩa:** một mốc là thời điểm có kết quả cần xác nhận, ví dụ yêu cầu đã được duyệt hoặc khách hàng đã nghiệm thu.

**Cách thao tác:**

Trong phần `TENTATIVE SCHEDULE`, từ hàng 25 trở xuống:

- Cột B: tên mốc.
- Cột E: ngày bắt đầu.
- Cột G: ngày hoàn thành.

Có thể điền:

| Mốc | Ngày hoàn thành |
|---|---|
| Yêu cầu được phê duyệt | 16/10/2026 |
| Thiết kế được thông qua | 30/10/2026 |
| Hoàn thành các chức năng chính | 27/11/2026 |
| Hoàn thành kiểm thử hệ thống | 11/12/2026 |
| Hoàn thành nghiệm thu người dùng | 18/12/2026 |
| Bàn giao chính thức | 25/12/2026 |

Với một mốc được biểu diễn bằng một ngày, điền cùng ngày vào phần bắt đầu và hoàn thành.

#### Bước 5: Lập nguồn lực và ngân sách — Kiểm tra khả năng thực hiện trong giới hạn cho phép

**Ý nghĩa:** nguồn lực cho biết ai làm và cần phương tiện gì. Ngân sách cho biết mức chi được phép sử dụng.

**Cách thao tác:**

Tại **C35 — PROJECT TEAM**, ghi bốn thành viên và vai trò trong bài toán mẫu.

Tại **C36 — SUPPORT RESOURCES**, ghi:

> Đại diện Ban quản trị cung cấp nghiệp vụ; kế toán tham gia dùng thử và đối chiếu kết quả.

Tại **C37 — SPECIAL NEEDS**, ghi:

> Máy tính kiểm thử, môi trường triển khai và bộ dữ liệu mẫu được khách hàng xác nhận.

Trong phần `COSTS`, nhập đơn giá vào cột E, số lượng vào cột F. Cột G đã có công thức thành tiền.

| Hàng | Khoản chi | Đơn giá | Số lượng | Thành tiền |
|---|---|---:|---:|---:|
| 41 | Công của An | 400.000 đồng/công | 30 công | 12.000.000 |
| 42 | Công của Bình | 800.000 đồng/công | 40 công | 32.000.000 |
| 43 | Công của Chi | 700.000 đồng/công | 40 công | 28.000.000 |
| 44 | Công của Dũng | 600.000 đồng/công | 20 công | 12.000.000 |
| 45 | Chưa sử dụng | 0 | 0 | 0 |
| 46 | Công cụ, môi trường kiểm thử | 6.000.000 | 1 gói | 6.000.000 |
| 47 | Dự phòng | 10.000.000 | 1 khoản | 10.000.000 |

Trong ví dụ này, một công là một ngày làm việc của một người.

**Kết quả cần thấy:** ô **G48 = 100.000.000**; ô **G10** lấy tổng chi phí từ G48. Giữ các công thức này.

Phần `EXPECTED BENEFITS` có thể mô tả lợi ích định tính. Nếu chưa có căn cứ quy đổi lợi ích ra tiền, ghi **Chưa định lượng** ở phần diễn giải.

#### Bước 6: Ghi rủi ro, ràng buộc và giả định — Làm rõ điều kiện mà kế hoạch đang dựa vào

**Ý nghĩa:**

- **Rủi ro:** sự kiện chưa chắc xảy ra nhưng có thể ảnh hưởng dự án.
- **Ràng buộc:** giới hạn phải tuân thủ.
- **Giả định:** điều đang tạm coi là đúng để lập kế hoạch.

**Cách thao tác:**

| Vị trí | Ví dụ |
|---|---|
| C67 — RISKS | Khách hàng bổ sung yêu cầu; thành viên nghỉ; dữ liệu mẫu cung cấp chậm; khách hàng từ chối nghiệm thu. |
| C68 — CONSTRAINTS | Tổng ngân sách không quá 100 triệu đồng; bàn giao chậm nhất 25/12/2026. |
| C69 — ASSUMPTIONS | Kế toán phản hồi nghiệp vụ trong thời gian đã thống nhất; bốn thành viên tham gia theo mức phân bổ công việc; khách hàng cung cấp dữ liệu mẫu. |

Bổ sung nội dung phụ thuộc bên ngoài:

> Việc xác nhận yêu cầu và nghiệm thu phụ thuộc vào lịch làm việc của đại diện Ban quản trị và kế toán.

**Cách kiểm tra:** mỗi giả định quan trọng cần có người theo dõi. Nếu khách hàng không cung cấp dữ liệu đúng hẹn, phải đánh giá lại tiến độ.

#### Bước 7: Bổ sung truyền thông và phê duyệt — Biến điều lệ thành cam kết được xác nhận

**Ý nghĩa:** tài liệu PDF yêu cầu chiến lược truyền thông và phê duyệt. Mẫu Excel chưa bố trí đầy đủ hai phần này.

**Cách thao tác:**

Bổ sung ở vùng trống phía dưới hoặc trong một sheet phụ:

| Hoạt động | Người tham gia | Tần suất | Kết quả cần lưu |
|---|---|---|---|
| Họp nhanh | Đội dự án | Hằng ngày | Việc hôm nay và vướng mắc |
| Báo cáo tiến độ | An, nhà tài trợ | Hằng tuần | Báo cáo tiến độ, chi phí, rủi ro |
| Xem xét sản phẩm | Đội dự án, khách hàng | Theo mốc bàn giao | Ý kiến và nội dung được xác nhận |

Điền thông tin người lập ở hàng 72. Bổ sung bảng phê duyệt gồm **vai trò, họ tên, ngày xác nhận và chữ ký hoặc bằng chứng xác nhận**.

**Điều kiện hoàn thành sản phẩm:** phạm vi, đầu ra, mốc, nguồn lực và ngân sách thống nhất; các bên có thẩm quyền đã xác nhận điều lệ.

</details>

<details>
<summary>-sản phẩm 'Cấu trúc phân chia công việc — WBS' - 'Chia toàn bộ phạm vi thành những phần có thể giao, ước lượng và kiểm tra'</summary>

Mẫu sử dụng: Mẫu cấu trúc phân chia công việc.xlsx

**Sản phẩm cần tạo:** một cây phân cấp công việc bao phủ toàn bộ phạm vi đã chốt trong điều lệ.

#### Bước 1: Chọn cách phân rã — Quyết định chia dự án theo sản phẩm hay quy trình

**Ý nghĩa:** PDF giới thiệu hai cách chính:

| Cách chia | Ví dụ |
|---|---|
| Theo sản phẩm bàn giao | Phần mềm → module thu phí → chức năng ghi nhận đóng tiền |
| Theo quy trình | Phát triển phần mềm → thiết kế → thiết kế dữ liệu |

Trong bài thực hành, ta chọn **chia theo sản phẩm bàn giao**, đồng thời có các nhánh dành cho quản lý, kiểm thử và bàn giao.

**Cách thao tác:**

- Đổi ô **A1** thành tên dự án.
- Điền **C3 = 05/10/2026**.
- Xem tên dự án ở đầu bảng là gốc chung; các hàng cấp 1 phía dưới là những nhánh lớn.

#### Bước 2: Nhập cấp và tên công việc — Tạo quan hệ cha–con

**Ý nghĩa:** cột `Level` quyết định cấp phân rã. Cột `WBS` sinh mã từ các cấp đó.

**Cách thao tác:**

Từ hàng 6, nhập cột A và C như bảng sau. **Giữ công thức ở cột B**.

| Hàng | Level — cột A | Mã WBS dự kiến — cột B | Task Description — cột C |
|---:|---:|---|---|
| 6 | 1 | 1 | Hồ sơ quản lý dự án |
| 7 | 2 | 1.1 | Điều lệ và kế hoạch được phê duyệt |
| 8 | 2 | 1.2 | Báo cáo tiến độ và hồ sơ kiểm soát |
| 9 | 1 | 2 | Phần mềm hoàn chỉnh |
| 10 | 2 | 2.1 | Module quản lý hộ gia đình |
| 11 | 2 | 2.2 | Module quản lý người dùng |
| 12 | 2 | 2.3 | Module quản lý thu phí |
| 13 | 3 | 2.3.1 | Chức năng tạo khoản thu |
| 14 | 3 | 2.3.2 | Chức năng ghi nhận đóng tiền |
| 15 | 3 | 2.3.3 | Chức năng thống kê và xuất báo cáo |
| 16 | 1 | 3 | Bộ kiểm thử hệ thống và biên bản nghiệm thu |
| 17 | 1 | 4 | Bộ cài, mã nguồn và hồ sơ bàn giao |

Xóa các cấp và mô tả mẫu còn dư phía dưới để tránh nhầm thành công việc thật.

**Cách kiểm tra:** ba chức năng `2.3.1–2.3.3` phải nằm dưới `2.3`; các nhánh `2.1`, `2.2`, `2.3` cùng cấp.

#### Bước 3: Mô tả gói công việc — Làm rõ thế nào được coi là hoàn thành

**Ý nghĩa:** gói công việc là phần thấp nhất mà bạn đang quản lý trong WBS. Nó cần đủ rõ để giao người làm, ước lượng và nghiệm thu.

**Cách thao tác:**

Điền cột **G — Notes** cho từng gói. Nếu mô tả dài, tạo thêm sheet `Mo ta goi cong viec` và dùng mã WBS để đối chiếu.

Ví dụ gói `2.3.2`:

| Thuộc tính | Nội dung minh họa |
|---|---|
| Tên | Chức năng ghi nhận đóng tiền |
| Đầu vào | Danh sách hộ, khoản thu, số tiền phải đóng |
| Kết quả | Giao dịch đóng tiền được lưu và hiển thị đúng |
| Công việc cần làm | Làm rõ quy tắc, lập trình xử lý, lập trình giao diện, kiểm thử đơn vị |
| Người chịu trách nhiệm | Bình |
| Người phối hợp | Chi, Dũng |
| Tiêu chí hoàn thành | Chọn đúng hộ và khoản thu; lưu đúng số tiền; báo cáo phản ánh đúng giao dịch; các trường hợp kiểm thử đã thống nhất đều đạt |

Nếu vẫn không thể ước lượng hoặc giao trách nhiệm rõ ràng, tiếp tục chia nhỏ.

#### Bước 4: Điền người phụ trách, ngày và chi phí — Gắn nguồn lực với từng phần công việc

**Ý nghĩa:** WBS xác định cần làm những gì. Các cột bổ sung giúp chuẩn bị dữ liệu cho lịch và ngân sách.

**Cách thao tác:**

| Cột | Cách điền |
|---|---|
| D — Assigned To | Một người chịu trách nhiệm chính |
| E — Start | Ngày bắt đầu dự kiến |
| F — End | Ngày hoàn thành dự kiến |
| G — Notes | Đầu vào, tiêu chí hoàn thành, phụ thuộc |
| H — Chi phí | Chi phí dự kiến của gói |

Ví dụ phần mềm:

| Gói | Chi phí |
|---|---:|
| 2.1 — Quản lý hộ gia đình | 18.000.000 |
| 2.2 — Quản lý người dùng | 12.000.000 |
| 2.3.1 — Tạo khoản thu | 8.000.000 |
| 2.3.2 — Ghi nhận đóng tiền | 12.000.000 |
| 2.3.3 — Thống kê, báo cáo | 10.000.000 |

Tại **H12**, tính chi phí module thu phí:

```excel
=SUM(H13:H15)
```

Tại **H9**, tính chi phí phần mềm:

```excel
=SUM(H10:H12)
```

Kết quả lần lượt là **30 triệu** và **60 triệu đồng**.

Có thể phân bổ các nhánh lớn còn lại: quản lý 12 triệu, kiểm thử 8 triệu, triển khai và bàn giao 10 triệu. Tổng công việc là **90 triệu**, cộng **10 triệu dự phòng** trong điều lệ thành **100 triệu**.

**Cách kiểm tra:** khi tính tổng, chỉ cộng các nhánh cùng cấp hoặc các gói thấp nhất. Cộng cả hàng cha và hàng con sẽ làm trùng chi phí.

#### Bước 5: Kiểm tra quy tắc 100% — Đảm bảo cây đủ phạm vi và không chồng chéo

**Ý nghĩa:** theo PDF, hoàn thành tất cả công việc con phải đồng nghĩa với hoàn thành công việc cha.

**Cách thao tác:**

Đối chiếu WBS với danh sách bàn giao trong điều lệ:

| Nội dung trong điều lệ | Vị trí phải tìm thấy trong WBS |
|---|---|
| Ba module phần mềm | Nhánh 2 |
| Quản lý và kiểm soát dự án | Nhánh 1 |
| Kiểm thử hệ thống, nghiệm thu | Nhánh 3 |
| Bộ cài, mã nguồn, hướng dẫn và hồ sơ bàn giao | Nhánh 4 |

Kiểm tra thêm:

- Tài liệu yêu cầu và thiết kế đã được phân công ở đâu?
- Kiểm thử đơn vị của module và kiểm thử toàn hệ thống có phạm vi phân biệt rõ không?
- Công việc nào còn chưa có người chịu trách nhiệm?
- Có đầu mục nào được tính ở hai nhánh không?

**Điều kiện hoàn thành sản phẩm:** mọi đầu ra trong điều lệ đều truy được đến gói công việc; mỗi gói có người phụ trách và tiêu chí hoàn thành.

</details>

<details>
<summary>-sản phẩm 'Lịch thực hiện và biểu đồ Gantt' - 'Biến công việc thành lịch có thời lượng, thứ tự và người thực hiện'</summary>

Mẫu sử dụng: Mẫu Gantt Chart quản lý dự án.xlsx

**Sản phẩm cần tạo:** bảng tiến độ để trả lời công việc nào làm trước, khi nào bắt đầu, bao lâu thì xong và giao cho ai.

#### Bước 1: Chuyển gói công việc thành hoạt động — Xác định những việc cần xếp lịch

**Ý nghĩa:** một sản phẩm trong WBS có thể cần nhiều hoạt động để tạo ra. Ví dụ, chức năng thu tiền cần xử lý nghiệp vụ, giao diện, tích hợp và kiểm thử.

**Cách thao tác:**

Mở sheet `Simple Gantt Chart - BLANK`.

Để học thao tác trước, dùng tám dòng từ **10–17** cho các giai đoạn chính:

| ID | Công việc | Chủ trì | Bắt đầu | Kết thúc | Ngày làm việc |
|---|---|---|---|---|---:|
| T01 | Khởi tạo, chốt phạm vi | An | 05/10/2026 | 09/10/2026 | 5 |
| T02 | Phân tích yêu cầu | An | 12/10/2026 | 16/10/2026 | 5 |
| T03 | Thiết kế giao diện và dữ liệu | Bình | 19/10/2026 | 30/10/2026 | 10 |
| T04 | Xây dựng module hộ gia đình, người dùng | Chi | 02/11/2026 | 13/11/2026 | 10 |
| T05 | Xây dựng module thu phí | Bình | 16/11/2026 | 27/11/2026 | 10 |
| T06 | Tích hợp, kiểm thử hệ thống | Dũng | 30/11/2026 | 11/12/2026 | 10 |
| T07 | Nghiệm thu người dùng | Dũng | 14/12/2026 | 18/12/2026 | 5 |
| T08 | Triển khai và bàn giao | An | 21/12/2026 | 25/12/2026 | 5 |

Điền vào các cột:

- B: ID.
- C: tên công việc.
- D: người chủ trì.
- E: bắt đầu.
- F: kết thúc.
- G: thời lượng.
- H: phần trăm hoàn thành.

Định dạng cột B là **Text** khi dùng mã phân cấp như `2.3.1`.

Bảng trên là lịch tổng quát. Để quản lý thực tế, cần mở rộng thành các hoạt động chi tiết và thêm công việc quản lý diễn ra xuyên suốt dự án.

#### Bước 2: Ước lượng thời lượng — Phân biệt số ngày diễn ra với lượng công sức

**Ý nghĩa:** hai người cùng làm ba ngày tạo ra sáu công, nhưng hoạt động vẫn diễn ra trong ba ngày.

**Cách thao tác:**

Với từng hoạt động, hỏi:

1. Có những thao tác nào cần thực hiện?
2. Ai có thể làm?
3. Người đó dành được bao nhiêu thời gian?
4. Có phải chờ đầu vào hoặc phản hồi không?

Ví dụ, có thể chia T05 thành:

| Hoạt động | Người thực hiện | Lịch minh họa |
|---|---|---|
| Rà soát quy tắc thu phí | An, Bình | 16/11 |
| Lập trình xử lý | Bình | 17–20/11 |
| Lập trình giao diện | Chi | 17–20/11 |
| Tích hợp | Bình, Chi | 23–24/11 |
| Kiểm tra chức năng, sửa lỗi | Dũng và lập trình viên | 25–27/11 |

Trong mẫu gốc, thời lượng là phép trừ ngày và có thể để trống khi bắt đầu, kết thúc cùng ngày. Với quy ước làm từ thứ Hai đến thứ Sáu, thay công thức **G10** bằng:

```excel
=IF(OR(E10="",F10=""),"",NETWORKDAYS(E10,F10))
```

Sao chép xuống G17.

Công thức này tính cả ngày bắt đầu và kết thúc, bỏ thứ Bảy và Chủ nhật. Nếu dự án có lịch nghỉ riêng, cần bổ sung lịch đó.

#### Bước 3: Xác định tiền nhiệm — Nối công việc với đầu vào cần có

**Ý nghĩa:** tiền nhiệm là công việc cần hoàn thành trước khi hoạt động sau có thể bắt đầu.

**Cách thao tác:**

Bổ sung cột `Tiền nhiệm` ở bên phải bảng, chẳng hạn tại **BQ9**.

Ví dụ:

| Công việc | Tiền nhiệm |
|---|---|
| T02 | T01 |
| T03 | T02 |
| T04 | T03 |
| T05 | T04 |
| T06 | T04, T05 |
| T07 | T06 |
| T08 | T07 |

Đây là quan hệ của lịch minh họa. Khi phân rã chi tiết, một số hoạt động có thể chạy song song.

Nếu T02 bắt đầu vào ngày làm việc tiếp theo sau T01, có thể nhập **E11**:

```excel
=WORKDAY(F10,1)
```

Mẫu hiện chưa có cơ chế tự xử lý toàn bộ quan hệ phụ thuộc. Khi một việc thay đổi, phải cập nhật các việc liên quan hoặc thiết lập công thức tương ứng.

#### Bước 4: Tạo thanh Gantt tự đổi theo ngày — Thiết lập trục thời gian và tô màu

**Ý nghĩa:** phần bên phải mẫu là lưới 12 tuần, mỗi tuần năm cột. Mẫu hiện không có quy tắc tự tô thanh theo ngày bắt đầu và kết thúc.

**Cách thao tác:**

1. Tại **I9**, nhập:

```excel
=DATE(2026,10,5)
```

2. Tại **J9**, nhập:

```excel
=WORKDAY(I9,1)
```

3. Kéo công thức J9 sang đến **BP9**.
4. Định dạng I9:BP9 thành `dd/mm`.
5. Xóa màu tô thủ công cũ trong vùng hoạt động cần dùng.
6. Chọn **I10:BP17**.
7. Vào **Home → Conditional Formatting → New Rule → Use a formula to determine which cells to format**.
8. Nhập:

```excel
=AND(I$9>=$E10,I$9<=$F10,$E10<>"",$F10<>"")
```

9. Chọn màu thanh rồi nhấn **OK**.

**Giải thích:** mỗi ô được tô khi ngày ở đầu cột nằm trong khoảng bắt đầu–kết thúc của công việc trên cùng hàng.

Sửa nhãn pha ở hàng 7 nếu chúng không khớp với kế hoạch mới.

**Cách kiểm tra:** thay thử ngày kết thúc của một việc. Thanh tương ứng phải thay đổi theo.

#### Bước 5: Kiểm tra nguồn lực — Xem lịch có thực hiện được hay không

**Ý nghĩa:** nhiều việc có thể chạy song song khi người và nguồn lực đáp ứng được.

**Cách thao tác:**

Lọc theo từng người ở cột D, xem các khoảng thời gian bị trùng.

Ví dụ, nếu Bình vừa phải lập trình xử lý thu phí toàn thời gian, vừa phải thiết kế một module khác trong cùng tuần, cần:

- Điều chỉnh thời điểm thực hiện.
- Phân công người khác.
- Hoặc chia rõ phần thời gian Bình dành cho từng việc.

Với công việc có nhiều người, lưu danh sách phối hợp và mức tham gia trong phần ghi chú hoặc bảng nguồn lực bổ sung.

#### Bước 6: Cập nhật hoàn thành — Phản ánh kết quả công việc đã tạo ra

**Ý nghĩa:** phần trăm hoàn thành phải dựa trên kết quả và tiêu chí đã thống nhất.

**Cách thao tác:**

- Định dạng H10:H17 là Percentage.
- Điền 0% khi chưa làm.
- Điền mức trung gian theo phần kết quả đã hoàn thành.
- Chỉ điền 100% khi đạt tiêu chí hoàn thành.

Ví dụ T05 có năm đầu ra đã thống nhất và mới hoàn thành ba đầu ra có trọng số tương đương, có thể ghi 60%.

**Điều kiện hoàn thành sản phẩm:** lịch bao phủ công việc trong WBS, có người thực hiện, thời lượng hợp lý, phụ thuộc rõ và không có xung đột nguồn lực chưa xử lý.

</details>

<details>
<summary>-sản phẩm 'Timeline dự án' - 'Trình bày tiến độ ở mức dễ theo dõi và trao đổi với các bên liên quan'</summary>

Mẫu sử dụng: Mẫu timeline dự án.xlsx

**Sản phẩm cần tạo:** một bản nhìn nhanh về các giai đoạn, người phụ trách, thời gian và trạng thái.

#### Bước 1: Chọn mức thông tin — Giữ các đầu mục phù hợp với người xem

**Ý nghĩa:** người quản lý cần nhìn các giai đoạn và mốc bàn giao; người thực hiện cần lịch hoạt động chi tiết.

**Cách thao tác:**

Mở sheet `BLANK - Project Timeline`. Dùng tám giai đoạn T01–T08 đã lập trong Gantt làm tám dòng từ **3–10**.

Giữ mã T01–T08 trong tên hoặc ghi chú để đối chiếu giữa hai file.

#### Bước 2: Điền các trường — Chuyển lịch đã thống nhất vào timeline

**Ý nghĩa:** dữ liệu được lấy từ lịch thực hiện, giúp hai sản phẩm dùng cùng một kế hoạch.

**Cách thao tác:**

| Cột | Nội dung | Ví dụ cho T05 |
|---|---|---|
| B — AT RISK | Có nguy cơ không đạt kế hoạch hay không | Có, nếu quy tắc thu chưa được chốt |
| C — TASK NAME | Tên đầu mục chính | T05 — Xây dựng module thu phí |
| D — SUB TASK NAME | Phần việc liên quan | WBS 2.3.1–2.3.3 |
| E — STATUS | Trạng thái | In Progress |
| F — ASSIGNED TO | Người chủ trì | Bình |
| G — START DATE | Bắt đầu | 16/11/2026 |
| H — END DATE | Kết thúc | 27/11/2026 |
| I — DURATION | Thời lượng | Giữ công thức |
| J — COMMENTS | Vướng mắc hoặc giải thích | Chờ xác nhận mẫu thống kê |

Trạng thái trong danh sách của mẫu gồm `Not Started`, `In Progress`, `Complete`, `On Hold`.

#### Bước 3: Hiểu cách tính thời lượng — Đọc đúng đơn vị của timeline

**Ý nghĩa:** mẫu timeline dùng **ngày lịch**, còn Gantt ở trên đã được thiết lập dùng **ngày làm việc**.

Công thức gốc ở I3 là:

```excel
=IF(G3=0,"",H3-G3+1)
```

Có thể dùng phiên bản kiểm tra đủ hai ngày:

```excel
=IF(OR(G3="",H3=""),"",H3-G3+1)
```

**Cách thao tác:** nhập công thức tại I3 rồi kéo xuống I10.

Ví dụ T05 từ 16–27/11 có:

- **12 ngày lịch** trên timeline.
- **10 ngày làm việc** trong Gantt.

Hai con số dùng đơn vị khác nhau nên cần ghi rõ đơn vị ở tiêu đề.

#### Bước 4: Kiểm tra biểu đồ — Đảm bảo thanh thời gian lấy đúng dữ liệu

**Ý nghĩa:** biểu đồ chỉ đúng khi nhãn, ngày bắt đầu và thời lượng khớp từng dòng.

**Cách thao tác:**

Nhấp phải biểu đồ → **Select Data**, kiểm tra:

- Nhãn công việc: C3:C10.
- Chuỗi ngày bắt đầu: G3:G10.
- Chuỗi thời lượng: I3:I10.

Nếu biểu đồ hiển thị sai khoảng thời gian:

1. Nhấp phải trục thời gian → **Format Axis**.
2. Điều chỉnh `Bounds — Minimum/Maximum` theo thời gian dự án.
3. Nếu cần nhập số ngày Excel, dùng một ô chứa `DATE(...)`, đổi định dạng sang General để lấy số tương ứng.

Với lịch mẫu, ngày 05/10/2026 có số ngày Excel là **46300**; có thể dùng giới hạn cuối **46382** để bao phủ hết 25/12/2026.

#### Bước 5: Cập nhật trạng thái và cảnh báo — Làm rõ việc nào cần can thiệp

**Ý nghĩa:** trạng thái cho biết đang làm tới đâu; `AT RISK` cho biết khả năng không đạt kế hoạch.

**Cách thao tác:**

Khi họp tiến độ, kiểm tra từng dòng:

- Công việc đã bắt đầu chưa?
- Có đầu vào đang bị chờ không?
- Ngày hoàn thành dự kiến có còn khả thi không?
- Có cần đổi trạng thái sang `On Hold` không?
- Ai xử lý vướng mắc và xử lý trước ngày nào?

**Điều kiện hoàn thành sản phẩm:** timeline khớp với Gantt và chỉ rõ các giai đoạn, trạng thái, đầu mối cùng những vướng mắc cần giải quyết.

</details>

<details>
<summary>-sản phẩm 'Kế hoạch phát triển theo Agile/Sprint' - 'Chia giai đoạn phát triển thành các vòng ngắn có kết quả dùng thử và phản hồi'</summary>

Mẫu sử dụng: Mẫu lập kế hoạch dự án theo nguyên tắc Agile.xlsx

**Sản phẩm cần tạo:** kế hoạch cho từng Sprint, trong đó mỗi Sprint có mục tiêu, công việc được chọn và tiêu chí hoàn thành.

Trong ví dụ, ta dùng ba Sprint cho giai đoạn phát triển từ **02/11–11/12/2026**. Các bước khảo sát ban đầu và nghiệm thu, bàn giao cuối dự án vẫn nằm trong kế hoạch tổng thể.

#### Bước 1: Tạo danh sách yêu cầu cần làm — Chuẩn bị đầu vào để chọn cho từng Sprint

**Ý nghĩa:** danh sách yêu cầu cần làm thường được gọi là **Product Backlog**. Mỗi mục cần đủ rõ về giá trị và kết quả mong muốn.

**Cách thao tác:**

Mở sheet `Agile Project Plan - BLANK`. Có thể bổ sung sheet `Backlog` để lưu:

| Trường | Ví dụ |
|---|---|
| Mã | YC-PHI-02 |
| Yêu cầu | Ghi nhận hộ gia đình đóng tiền |
| Người sử dụng | Kế toán |
| Giá trị | Theo dõi đúng tình trạng đóng phí |
| Ưu tiên | Cao |
| Tiêu chí chấp nhận | Chọn hộ, chọn khoản thu, nhập tiền, lưu giao dịch và đối chiếu được trên báo cáo |
| Liên hệ WBS | 2.3.2 |

Có thể diễn đạt yêu cầu:

> Là kế toán, tôi muốn ghi nhận hộ A101 đóng phí dịch vụ để theo dõi tình trạng thanh toán của hộ đó.

#### Bước 2: Lập mục tiêu và chọn công việc cho từng Sprint — Xác định kết quả sau mỗi vòng

**Ý nghĩa:** Sprint cần có kết quả sử dụng hoặc kiểm tra được.

**Cách thao tác:**

Điền thông tin dự án ở C3:F3. Tại phần công việc:

| Sprint | Vị trí | Thời gian | Mục tiêu |
|---|---|---|---|
| Sprint 1 | Hàng 6; việc con ở 7–9 | 02–13/11 | Dùng được quản lý hộ gia đình và người dùng |
| Sprint 2 | Hàng 10; việc con ở 11–13 | 16–27/11 | Tạo khoản thu, ghi nhận đóng tiền, xem thống kê |
| Sprint 3 | Hàng 14; việc con ở 15–17 | 30/11–11/12 | Tích hợp hệ thống, sửa lỗi, chuẩn bị bản nghiệm thu |

Chọn công việc theo ưu tiên, phụ thuộc và thời gian thực tế của thành viên.

#### Bước 3: Điền từng công việc — Làm rõ loại việc, người làm và ước lượng

**Ý nghĩa:** các cột giúp đội dự án thống nhất nội dung và trách nhiệm.

**Cách thao tác:**

| Cột | Cách dùng |
|---|---|
| B — AT RISK | Đánh dấu nếu có nguy cơ không hoàn thành |
| C — TASK NAME | Tên yêu cầu hoặc hoạt động |
| D — FEATURE TYPE | Loại việc, ví dụ Feature, Bug, Technical, Testing |
| E — RESPONSIBLE | Người chịu trách nhiệm chính |
| F — STORY POINTS | Ước lượng tương đối |
| G — START | Bắt đầu |
| H — FINISH | Hoàn thành dự kiến |
| I — DURATION | Thời lượng |
| J — STATUS | Trạng thái |
| K — COMMENTS | Tiêu chí, vướng mắc hoặc thông tin cần phối hợp |

Ví dụ Sprint 2:

| Hàng | Công việc | Chủ trì | Điểm minh họa |
|---|---|---|---:|
| 11 | YC-PHI-01 — Tạo khoản thu | Bình | 5 |
| 12 | YC-PHI-02 — Ghi nhận đóng tiền | Chi | 8 |
| 13 | YC-PHI-03 — Thống kê khoản thu | Bình | 5 |

**Story Point** phản ánh tương đối về khối lượng, độ phức tạp và sự không chắc chắn. Đội có thể dùng dãy 1, 2, 3, 5, 8 để so sánh.

Các điểm trên là ví dụ ước lượng. Cần xem xét khả năng thực hiện của đội trước khi cam kết nhận vào Sprint.

#### Bước 4: Bổ sung công thức và trạng thái — Hoàn thiện phần mẫu trống chưa thiết lập

**Ý nghĩa:** sheet Agile trống hiện chưa có công thức thời lượng.

**Cách thao tác:**

Tại I6 nhập:

```excel
=IF(OR(G6="",H6=""),"",H6-G6+1)
```

Kéo xuống I17. Ghi rõ cột I tính **ngày lịch**.

Tính tổng điểm của các việc con:

```excel
F6: =SUM(F7:F9)
F10: =SUM(F11:F13)
F14: =SUM(F15:F17)
```

Với cột J, có thể tạo danh sách trạng thái:

1. Chọn J6:J17.
2. Vào **Data → Data Validation → List**.
3. Nhập các trạng thái: `Not Started`, `In Progress`, `Complete`, `On Hold`, `Overdue`.

Khi dùng vùng dữ liệu cho danh sách, đặt các trạng thái trong một vùng trống rồi chọn vùng đó làm `Source`.

#### Bước 5: Định nghĩa hoàn thành — Thống nhất điều kiện trước khi chuyển sang Complete

**Ý nghĩa:** một mục đã lập trình xong vẫn có thể còn thiếu kiểm thử hoặc chưa đáp ứng nghiệp vụ.

**Cách thao tác:**

Ghi tiêu chí ở cột K hoặc sheet Backlog:

> Chức năng đáp ứng tiêu chí chấp nhận, đã được kiểm thử theo phạm vi thống nhất, đã sửa các lỗi cản trở sử dụng và có thể trình diễn trên môi trường dùng thử.

Cuối Sprint:

- Trình diễn kết quả cho khách hàng.
- Ghi nhận phản hồi.
- Xác nhận mục nào thực sự hoàn thành.
- Đưa phần chưa hoàn thành về danh sách để xem xét lại.
- Cập nhật các yêu cầu thay đổi được chấp thuận.

#### Bước 6: Tính tiến độ theo điểm đã hoàn thành — Theo dõi kết quả của các Sprint

**Ý nghĩa:** chỉ tính điểm của những mục đã đạt điều kiện hoàn thành.

**Cách thao tác:**

Bổ sung cột **L — Điểm đã hoàn thành**.

Tại L6:

```excel
=SUMIFS(F7:F9,J7:J9,"Complete")
```

Tại L10 và L14, dùng công thức tương tự cho các vùng 11–13 và 15–17.

Tại H3:

```excel
=IF(SUM(F6,F10,F14)=0,"",SUM(L6,L10,L14)/SUM(F6,F10,F14))
```

Đổi nhãn H2 thành **% điểm đã hoàn thành**.

Ví dụ ba Sprint có tổng 50 điểm và hoàn thành 34 điểm thì kết quả là **68%**.

Chỉ số này đo phần công việc được đưa vào ba Sprint. Khi báo cáo toàn dự án, cần tính cả các phần việc ngoài giai đoạn phát triển.

**Điều kiện hoàn thành sản phẩm:** mỗi Sprint có mục tiêu, phạm vi, người chịu trách nhiệm, ước lượng và tiêu chí hoàn thành; phản hồi sau Sprint được lưu và xử lý.

</details>

<details>
<summary>-sản phẩm 'Kế hoạch và ma trận đánh giá rủi ro' - 'Nhận diện điều có thể làm dự án không đạt mục tiêu và xác định thứ tự xử lý'</summary>

Mẫu sử dụng: Mẫu ma trận quản lý rủi ro dự án.xlsx

**Sản phẩm cần tạo:** danh sách rủi ro đã được đánh giá, có người theo dõi, hành động ngăn ngừa và phương án ứng phó.

#### Bước 1: Chọn thang đánh giá — Thống nhất cách đọc mức rủi ro

**Ý nghĩa:** tài liệu và các mẫu đang dùng những thang khác nhau:

| Nguồn | Cấu trúc |
|---|---|
| PDF, ma trận trang 9 | Xác suất 1–3, tác động 1–3, kết quả mức 1–5 |
| Sheet `Risk Matrix` | Ma trận 5×5, kết quả Low, Medium, High, Very High |
| Mẫu theo dõi rủi ro | Ba nhóm High, Medium, Low |

Ngoài ra, bảng mô tả rủi ro trong PDF có các số theo kiểu tích xác suất × tác động, còn ma trận cuối tài liệu dùng năm mức. Phần diễn giải cuối trang 8 cũng bị lặp số mức.

**Cách thực hiện trong bài học:** lấy **ma trận 3×3 ở trang 9** làm căn cứ chính. Phần chuyển sang ba nhóm để dùng với mẫu theo dõi sẽ được quy định riêng ở bước 4.

#### Bước 2: Viết rủi ro thành sự kiện rõ ràng — Làm rõ nguyên nhân và hậu quả

**Ý nghĩa:** mô tả đủ rõ sẽ giúp chọn biện pháp xử lý đúng.

Dùng cấu trúc:

> Do nguyên nhân…, có thể xảy ra sự kiện…, dẫn đến hậu quả…

**Cách thao tác:**

Trong workbook, tạo sheet `Danh gia`, với các cột:

| Cột | Nội dung |
|---|---|
| A | Mã rủi ro |
| B | Mô tả rủi ro |
| C | Xác suất |
| D | Tác động |
| E | Mức theo ma trận |
| F | Nhóm theo dõi |
| G | Người theo dõi |
| H | Ngăn ngừa |
| I | Ứng phó |
| J | Dấu hiệu kích hoạt |
| K | Hạn hành động |

Ví dụ mô tả:

> Do Bình tham gia nhiều dự án, có thể không hoàn thành phần xử lý thu phí đúng hạn, dẫn đến trễ kiểm thử hệ thống.

Các nhóm rủi ro cần rà soát theo PDF gồm nhân sự, thay đổi yêu cầu, thiếu tài liệu, giao tiếp, chậm tiến độ, hợp đồng hoặc phê duyệt, nghiệm thu, ngân sách và ước lượng.

#### Bước 3: Đánh giá xác suất và tác động — Gán điểm dựa trên căn cứ

**Ý nghĩa:**

- **Xác suất:** khả năng sự kiện xảy ra.
- **Tác động:** mức thiệt hại nếu sự kiện xảy ra.

**Cách thao tác:**

Dùng thang:

| Điểm | Xác suất | Tác động |
|---:|---|---|
| 1 | Thấp | Thấp |
| 2 | Vừa | Vừa |
| 3 | Cao | Cao |

Khi xét chi phí, tài liệu chia mức tác động theo các ngưỡng **dưới 5%, 5–10%, trên 10%**. Với ngân sách 100 triệu, mức tăng trên 10 triệu thuộc nhóm tác động cao về chi phí.

Đây là điểm phân loại; điểm xác suất 2 không có nghĩa là xác suất 2%.

Có thể điền bảng đánh giá minh họa:

| Mã | Rủi ro | Xác suất | Tác động | Mức theo ma trận |
|---|---|---:|---:|---:|
| RR01 | Nhân sự bận dự án khác hoặc rời nhóm | 2 | 3 | 4 |
| RR02 | Thay đổi, bổ sung yêu cầu | 2 | 2 | 3 |
| RR03 | Thiếu tài liệu kỹ thuật khi bàn giao | 2 | 2 | 3 |
| RR04 | Thiếu trao đổi dẫn đến hiểu sai nghiệp vụ | 2 | 2 | 3 |
| RR05 | Công việc trước chậm làm trễ việc sau | 2 | 3 | 4 |
| RR06 | Hợp đồng hoặc phê duyệt bị chậm | 1 | 2 | 2 |
| RR07 | Khách hàng từ chối nghiệm thu | 2 | 3 | 4 |
| RR08 | Ngân sách bị cắt giảm | 1 | 3 | 3 |
| RR09 | Ước lượng thời gian, chi phí quá lạc quan | 2 | 3 | 4 |

Các điểm trên là đánh giá giả định của bài toán mẫu; khi làm dự án thật phải có lý do cho từng điểm.

#### Bước 4: Tạo ma trận 3×3 và công thức tra mức — Xếp ưu tiên thống nhất

**Ý nghĩa:** ma trận cho biết một cặp xác suất–tác động tương ứng với mức nào.

**Cách thao tác:**

Tạo sheet `Ma tran 3x3`, điền:

| Xác suất \ Tác động | 1 — Thấp | 2 — Vừa | 3 — Cao |
|---|---:|---:|---:|
| 1 — Thấp | 1 | 2 | 3 |
| 2 — Vừa | 2 | 3 | 4 |
| 3 — Cao | 3 | 4 | 5 |

Bố trí phần số trong **B2:D4**.

Tại E2 của sheet `Danh gia`, nhập:

```excel
=IF(OR(C2="",D2=""),"",INDEX('Ma tran 3x3'!$B$2:$D$4,C2,D2))
```

Dùng **Data Validation → Whole number → between 1 and 3** cho cột C và D.

Để tương thích mẫu theo dõi ba nhóm, bài thực hành quy định:

| Mức 3×3 | Nhóm theo dõi |
|---|---|
| 1–2 | Low |
| 3 | Medium |
| 4–5 | High |

Đây là **quy ước bổ sung cho bài thực hành**.

Tại F2:

```excel
=IF(E2="","",IF(E2<=2,"Low",IF(E2=3,"Medium","High")))
```

Kéo hai công thức xuống các dòng rủi ro.

Nếu dùng nguyên mẫu 5×5, đọc định nghĩa ở `Risk Matrix Key`, đánh giá theo năm mức rồi tra đúng giao điểm. Ví dụ `Possible` × `Major` cho kết quả `High`. Việc chuyển từ 3×3 sang 5×5 cần đánh giá lại theo định nghĩa của thang mới.

#### Bước 5: Lập ngăn ngừa và ứng phó — Chuẩn bị hành động trước và sau khi rủi ro xảy ra

**Ý nghĩa:**

- **Ngăn ngừa:** giảm khả năng xảy ra hoặc giảm hậu quả.
- **Ứng phó:** hành động khi có dấu hiệu hoặc khi sự kiện đã xảy ra.
- **Dấu hiệu kích hoạt:** điều kiện để bắt đầu phương án ứng phó.

**Cách thao tác:**

Điền các cột G–K. Ví dụ:

| Rủi ro | Ngăn ngừa | Dấu hiệu kích hoạt | Ứng phó |
|---|---|---|---|
| RR01 — Thiếu nhân sự | Lưu mã nguồn chung, rà soát chéo, có người nắm phần việc dự phòng | Thành viên không thể tham gia quá thời gian đã thống nhất | Phân công lại và đánh giá lại lịch, chi phí |
| RR02 — Thay đổi yêu cầu | Chốt phạm vi, dùng biểu mẫu yêu cầu thay đổi | Khách hàng đề nghị thêm hoặc sửa chức năng | Phân tích ảnh hưởng và xin quyết định điều chỉnh |
| RR07 — Từ chối nghiệm thu | Thống nhất tiêu chí, demo sớm, chuẩn bị dữ liệu kiểm thử | Một tình huống nghiệm thu bắt buộc không đạt | Sửa lỗi, kiểm thử lại và tổ chức nghiệm thu lại |

Với mỗi hành động, điền người chịu trách nhiệm và hạn hoàn thành cụ thể.

#### Bước 6: Rà soát định kỳ — Cập nhật đánh giá theo tình hình mới

**Ý nghĩa:** khả năng xảy ra và tác động có thể thay đổi khi dự án tiến triển.

**Cách thao tác:**

Trong họp tuần:

1. Kiểm tra hành động ngăn ngừa đã thực hiện chưa.
2. Xem dấu hiệu kích hoạt có xuất hiện không.
3. Đánh giá lại xác suất và tác động.
4. Ghi ngày rà soát và căn cứ thay đổi.
5. Chuyển các hành động cần thực hiện sang bảng theo dõi ở sản phẩm tiếp theo.

**Điều kiện hoàn thành sản phẩm:** rủi ro quan trọng đều có mô tả, căn cứ đánh giá, người theo dõi, biện pháp và dấu hiệu kích hoạt.

</details>

<details>
<summary>-sản phẩm 'Bảng theo dõi hành động xử lý rủi ro' - 'Theo dõi ai phải làm gì, hạn nào và đang xử lý đến đâu'</summary>

Mẫu sử dụng: Mẫu theo dõi rủi ro dự án.xlsx

**Sản phẩm cần tạo:** một bảng vận hành để đôn đốc các hành động ngăn ngừa và ứng phó.

#### Bước 1: Chuyển biện pháp thành công việc — Viết hành động có thể kiểm tra

**Ý nghĩa:** “quản lý nhân sự tốt” còn khó theo dõi. “Hoàn tất bàn giao chéo phần xử lý thu phí trước 13/11” có người làm, hạn và kết quả cụ thể.

**Cách thao tác:**

Mở sheet `BLANK - Project Risk`, nhập từ hàng **13**.

Một rủi ro có thể có nhiều hành động. Dùng mã như:

- `RR01-H01`: hành động 1 của rủi ro RR01.
- `RR01-H02`: hành động 2 của cùng rủi ro.

#### Bước 2: Điền thông tin hành động — Gắn trách nhiệm và thời hạn

**Cách thao tác:**

| Cột | Ý nghĩa | Cách điền |
|---|---|---|
| B — TASK ID | Mã hành động | RR01-H01 |
| C — TASK | Việc cần thực hiện | Hoàn tất bàn giao chéo phần xử lý thu phí |
| D — ASSIGNED TO | Người chịu trách nhiệm | Bình |
| E — DEADLINE | Hạn hoàn thành | 13/11/2026 |
| F — STATUS | Trạng thái hành động | Complete |
| G — RISK LEVEL | Nhóm rủi ro liên quan | High |
| H — COMMENTS | Kết quả, bằng chứng, vướng mắc | Đã rà soát mã nguồn và bàn giao tài liệu |

Ví dụ tại ngày báo cáo 27/11/2026:

| Mã hành động | Công việc | Người làm | Hạn | Trạng thái | Nhóm |
|---|---|---|---|---|---|
| RR01-H01 | Hoàn tất bàn giao chéo | Bình | 13/11/2026 | Complete | High |
| RR02-H01 | Lập quy trình duyệt thay đổi | An | 16/10/2026 | Complete | Medium |
| RR07-H01 | Chốt bộ tình huống nghiệm thu | Dũng | 11/12/2026 | In Progress | High |

#### Bước 3: Dùng đúng trạng thái và nhóm — Giúp các công thức đếm được dữ liệu

**Ý nghĩa:** bảng tổng hợp phía trên đang đếm theo đúng chuỗi chữ trong danh sách.

**Cách thao tác:**

Chọn ở danh sách thả xuống:

| Giá trị | Cách hiểu |
|---|---|
| Not Started | Chưa bắt đầu hành động |
| In Progress | Đang thực hiện |
| Complete | Hành động đã hoàn thành |
| On Hold | Đang tạm dừng |
| Overdue | Đã quá hạn và chưa hoàn thành |

Cột G dùng `High`, `Medium`, `Low`, lấy theo quy ước ở bảng đánh giá.

Nếu đổi tên trạng thái sang tiếng Việt, phải cập nhật đồng thời danh sách, công thức và quy tắc màu.

#### Bước 4: Kiểm tra bảng tổng hợp — Đối chiếu con số với các hành động đã nhập

**Ý nghĩa:** phần trên mẫu giúp đếm số hành động theo trạng thái và nhóm rủi ro.

Ví dụ công thức D5:

```excel
=COUNTIFS(F13:F37,"Not Started",G13:G37,"High")
```

**Cách thao tác:**

Với ba dòng ví dụ, kiểm tra bảng tổng hợp phải phản ánh:

- Tổng ba hành động.
- Hai hành động `Complete`.
- Một hành động `In Progress`.
- Hai hành động gắn nhóm `High`.
- Một hành động gắn nhóm `Medium`.

Các công thức hiện xét vùng hàng **13–37**. Nếu nhập thêm ngoài vùng này, phải mở rộng công thức và danh sách chọn tương ứng.

**Lưu ý về cách đọc:** khi một rủi ro có nhiều hành động, số dòng và tổng đếm trong mẫu phản ánh **số hành động**, không còn bằng số rủi ro riêng biệt.

#### Bước 5: Đóng hành động và đánh giá lại rủi ro — Kiểm tra hiệu quả của việc đã làm

**Ý nghĩa:** hoàn thành một hành động ngăn ngừa chưa có nghĩa là rủi ro đã biến mất.

**Cách thao tác:**

Khi chuyển sang `Complete`:

1. Ghi kết quả hoặc vị trí bằng chứng vào H.
2. Quay lại sheet `Danh gia`.
3. Xem rủi ro còn tồn tại không.
4. Cập nhật đánh giá còn lại.
5. Tạo hành động mới nếu cần.

Ví dụ đã bàn giao chéo mã nguồn nhưng Bình vẫn có thể nghỉ. Khi đó, rủi ro còn tồn tại, nhưng hậu quả có thể giảm.

**Điều kiện hoàn thành sản phẩm:** mọi hành động đang mở có người phụ trách, hạn và trạng thái; hành động hoàn thành có bằng chứng và được dùng để đánh giá lại rủi ro.

</details>

<details>
<summary>-sản phẩm 'Dashboard báo cáo dự án' - 'Tổng hợp tiến độ, ngân sách và những việc cần quyết định tại một ngày báo cáo'</summary>

Mẫu sử dụng: Mẫu Dashboard báo cáo dự án.xlsx

**Sản phẩm cần tạo:** một báo cáo ngắn giúp người xem biết dự án đang ở đâu và cần xử lý việc gì.

#### Bước 1: Chốt ngày báo cáo — Xác định thời điểm mà các con số phản ánh

**Ý nghĩa:** mọi trạng thái, chi phí và việc tồn đọng cần được cập nhật đến cùng một thời điểm.

**Cách thao tác:**

Mở sheet `MẪU DASHBOARD BÁO CÁO DỰ ÁN`.

Điền:

| Ô | Nội dung |
|---|---|
| B3 | Phần mềm quản lý và thu phí chung cư Blue Moon |
| F3 | 27/11/2026 |
| G3 | Đánh giá chung tại ngày báo cáo |
| H3 | Sẽ thiết lập công thức ở bước 3 |

Ví dụ G3 có thể ghi **Đúng kế hoạch**, sau khi đối chiếu tiến độ, chi phí và rủi ro tại ngày báo cáo.

#### Bước 2: Cập nhật bảng nhiệm vụ — Đưa dữ liệu nền vào Dashboard

**Ý nghĩa:** biểu đồ trạng thái và ưu tiên lấy dữ liệu từ bảng nhiệm vụ.

**Cách thao tác:**

Nhập tám giai đoạn T01–T08 vào hàng **11–18**:

| Cột | Dữ liệu |
|---|---|
| B | Tên nhiệm vụ, có kèm mã |
| C | Người phụ trách |
| D | Ngày bắt đầu |
| E | Ngày kết thúc |
| F | Thời lượng |
| G | Trạng thái |
| H | Ưu tiên |
| I | Bình luận |

Lấy tên, người và ngày từ Gantt.

Tại ngày 27/11, **giả sử** T01–T05 đã hoàn thành, T06–T08 chưa bắt đầu. Khi đó:

- Năm dòng đầu: `Complete`.
- Ba dòng sau: `Not Started`.

Xóa tên `Task 9`, `Task 10`… và các dữ liệu nhập mẫu không sử dụng, đồng thời giữ các công thức cần thiết.

Nếu thống nhất thời lượng của Dashboard theo ngày lịch, dùng F11:

```excel
=IF(OR(D11="",E11=""),"",E11-D11+1)
```

Kéo xuống F18.

#### Bước 3: Thiết lập phần trăm hoàn thành — Xác định rõ chỉ số đang đo điều gì

**Ý nghĩa:** ô H3 trong mẫu trống đang chứa số nhập sẵn, chưa phải công thức tính tiến độ dự án.

Để học cách tính đơn giản, ta dùng **tỷ lệ nhiệm vụ đã hoàn thành**.

**Cách thao tác:**

- Đổi H2 thành **% nhiệm vụ hoàn thành**.
- Tại H3 nhập:

```excel
=IF(C39=0,"",C36/C39)
```

Trong mẫu:

- C36: số nhiệm vụ `Complete`.
- C39: tổng số nhiệm vụ đã được phân loại trạng thái.

Định dạng H3 là Percentage.

Với năm nhiệm vụ hoàn thành trên tổng tám nhiệm vụ:

```text
5 / 8 = 62,5%
```

**Cách đọc:** 62,5% là tỷ lệ theo số nhiệm vụ. Các nhiệm vụ trong phép tính có trọng số bằng nhau. Nếu muốn đo theo khối lượng hoặc công sức, cần lập trọng số và cách tính riêng.

#### Bước 4: Điền ngân sách và chi phí thực tế — Đối chiếu mức chi với kế hoạch

**Ý nghĩa:** ngân sách là mức được phê duyệt; chi phí thực tế là phần đã phát sinh đến ngày báo cáo.

**Cách thao tác:**

| Ô | Nội dung | Ví dụ |
|---|---|---:|
| G33 | DỰ KIẾN | 100.000.000 |
| G34 | THỰC TẾ | 54.000.000 |

Chi phí thực tế phải lấy từ bảng ghi nhận chi phí hoặc chứng từ, cập nhật đến 27/11.

Nếu cần quản lý khả năng vượt ngân sách, bổ sung chỉ tiêu **Dự báo tổng chi phí khi hoàn thành**.

Ví dụ:

> Đã phát sinh 54 triệu, dự báo cần thêm 44 triệu để hoàn thành, tổng dự báo là 98 triệu.

Phần ngân sách chưa chi hiện tại chưa phải khoản tiết kiệm cuối dự án.

#### Bước 5: Cập nhật việc đang chờ — Làm rõ nội dung cần người quản lý can thiệp

**Ý nghĩa:** báo cáo cần cho biết những quyết định và hành động còn tồn đọng.

**Cách thao tác:**

Trong phần `PENDING ITEMS`:

| Ô | Nội dung | Ví dụ |
|---|---|---|
| G42 | Decisions | Một quyết định đang chờ duyệt bộ dữ liệu nghiệm thu |
| G43 | Actions | Hai hành động đang mở: chuẩn bị dữ liệu và xác nhận lịch dùng thử |
| G44 | Change Requests | Một yêu cầu thay đổi mẫu báo cáo đang chờ đánh giá |

Nhập số lượng vào các ô và lưu danh sách chi tiết gồm mã, người xử lý, hạn và nội dung.

Các con số này trong mẫu là ô nhập liệu; cần cập nhật từ danh sách theo dõi tương ứng.

#### Bước 6: Kiểm tra nguồn biểu đồ — Đảm bảo hình hiển thị đúng dữ liệu và đơn vị

**Ý nghĩa:** các biểu đồ phụ thuộc vùng dữ liệu và cài đặt trục. Mẫu hiện có một số điểm cần chỉnh khi dùng dữ liệu mới.

**Cách thao tác:**

**Với biểu đồ timeline:**

Nhấp phải → **Select Data**, chỉnh cho tám nhiệm vụ:

- Nhãn: B11:B18.
- Ngày bắt đầu: D11:D18.
- Thời lượng: F11:F18.

Trong sheet trống, chuỗi thời lượng của biểu đồ hiện bắt đầu từ F10, lệch so với các dòng nhiệm vụ. Chỉnh lại để các vùng cùng bắt đầu và kết thúc trên một hàng.

Điều chỉnh giới hạn trục thời gian sang khoảng dự án năm 2026.

**Với biểu đồ ngân sách:**

Trục giá trị đang có giới hạn tối đa cố định **90.000**, không phù hợp dữ liệu hàng chục triệu đồng.

Nhấp phải trục giá trị → **Format Axis → Bounds → Maximum → Automatic**, hoặc đặt giới hạn phù hợp ngân sách.

**Với trạng thái và ưu tiên:**

Đối chiếu tổng đếm với các dòng nhiệm vụ thật. Đảm bảo nhiệm vụ có tên đều được điền trạng thái để không bị bỏ khỏi tổng.

#### Bước 7: Đối chiếu các sản phẩm — Kiểm tra báo cáo có truy được về dữ liệu gốc

**Ý nghĩa:** một con số trên Dashboard cần giải thích được bằng công việc, chi phí hoặc hành động cụ thể.

**Cách thao tác:**

Chọn một chức năng và truy theo chuỗi dữ liệu:

| Nội dung | Vị trí đối chiếu |
|---|---|
| Chức năng ghi nhận đóng tiền thuộc phạm vi | Điều lệ dự án |
| Chức năng mang mã 2.3.2 | WBS |
| Chức năng được xây dựng trong T05 | Gantt và Timeline |
| Chức năng được chọn cho Sprint 2 | Kế hoạch Agile |
| Khả năng không đạt yêu cầu nghiệm thu | RR07 trong bảng đánh giá |
| Hành động chốt tình huống nghiệm thu | RR07-H01 trong bảng theo dõi |
| Trạng thái phát triển tại ngày báo cáo | Dòng T05 trên Dashboard |

Với dữ liệu minh họa, các số cần đối chiếu được là:

- **8 nhiệm vụ**, trong đó **5 Complete**.
- **62,5% nhiệm vụ hoàn thành**.
- Ngân sách **100 triệu đồng**.
- Chi phí thực tế minh họa **54 triệu đồng**.
- Các quyết định và hành động đang chờ có danh sách chi tiết đi kèm.

**Điều kiện hoàn thành sản phẩm:** Dashboard phản ánh đúng ngày báo cáo; các con số truy được về dữ liệu gốc; biểu đồ dùng đúng vùng dữ liệu và đơn vị.

</details>
