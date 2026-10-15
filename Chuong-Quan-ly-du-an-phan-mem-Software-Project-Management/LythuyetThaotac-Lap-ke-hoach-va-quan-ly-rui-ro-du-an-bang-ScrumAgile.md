### 🔍LythuyetThaotac: Lập kế hoạch dự án phần mềm — Huong dan xay dung Ke hoach du an(7).pdf

**Giới thiệu bài toán mẫu để học cách thao tác**

Bạn cần xây dựng phần mềm quản lý và thu phí chung cư **Blue Moon**, gồm ba module:

- **Quản lý thu phí:** tạo khoản thu, ghi nhận thanh toán, thống kê.
- **Quản lý người dùng:** quản lý tài khoản và phân quyền.
- **Quản lý hộ gia đình:** quản lý hộ, nhân khẩu và biến động nhân khẩu.

Bạn sẽ lần lượt tạo các sản phẩm để trả lời: **Dự án làm gì → cần tạo những gì → phải làm những việc nào → ai làm, khi nào → chuẩn bị gì trước rủi ro.**

Ngân sách **100 triệu đồng** lấy từ tài liệu. Nhóm bốn người, lịch 12 tuần và các ước lượng dưới đây là giả định bổ sung để thực hành. Nguồn: Huong dan xay dung Ke hoach du an(7).pdf

<details>
<summary><strong>-sản phẩm 'Tuyên ngôn dự án — Project Charter' — Xác lập mục tiêu, phạm vi, nguồn lực và trách nhiệm của dự án.</strong></summary>

#### -bước 'Xác định thông tin chung' — Ghi rõ dự án nào đang được thực hiện và ai bảo trợ.

Tạo tài liệu `01_Tuyen_ngon_du_an_BlueMoon`, sau đó điền:

| Nội dung | Ví dụ điền |
|---|---|
| Tên dự án | Xây dựng phần mềm quản lý và thu phí chung cư Blue Moon |
| Nhà tài trợ | Người có thẩm quyền phê duyệt nguồn lực dự án |
| Cơ quan tài trợ | Công ty ABC, theo ví dụ trong tài liệu |
| Mức độ ảnh hưởng | Thay đổi cách quản lý thông tin hộ dân và thu phí |
| Phiên bản | 1.0 |
| Ngày lập | Ngày thực tế lập tài liệu |

Nhà tài trợ, khách hàng và người sử dụng có thể là những người khác nhau. Cần xác nhận đúng vai trò trước khi điền tên.

#### -bước 'Xác định người tham gia' — Phân biệt người trực tiếp làm sản phẩm và người cung cấp yêu cầu, sử dụng hoặc phê duyệt.

Lập bảng đội thực hiện:

| Thành viên mẫu | Vai trò | Trách nhiệm chính |
|---|---|---|
| A | Quản lý dự án, phân tích nghiệp vụ | Làm rõ yêu cầu, lập kế hoạch, theo dõi tiến độ |
| B | Lập trình xử lý và dữ liệu | Thiết kế dữ liệu, xây dựng xử lý nghiệp vụ |
| C | Lập trình giao diện | Thiết kế và xây dựng màn hình |
| D | Kiểm thử | Chuẩn bị tình huống kiểm tra, kiểm thử và báo lỗi |

Lập tiếp bảng các bên liên quan:

| Bên liên quan | Trách nhiệm |
|---|---|
| Đại diện ban quản trị | Xác nhận phạm vi và tiêu chí nghiệm thu |
| Kế toán chung cư | Cung cấp quy tắc thu phí, dùng thử và phản hồi |
| Nhà tài trợ | Duyệt nguồn lực và quyết định thuộc thẩm quyền |
| Đơn vị triển khai | Cung cấp thông tin môi trường cài đặt, hỗ trợ bàn giao |

Trong bản thực tế, bổ sung họ tên, nơi công tác và thông tin liên hệ theo mẫu tài liệu.

#### -bước 'Viết bối cảnh, mục đích và mục tiêu' — Làm rõ vấn đề hiện tại, điều muốn cải thiện và kết quả cần đạt.

Điền ba nội dung riêng:

| Nội dung | Ví dụ |
|---|---|
| **Bối cảnh:** Hiện đang có vấn đề gì? | Ban quản trị theo dõi hộ dân và khoản thu bằng sổ sách, Excel; khó tra cứu lịch sử thanh toán và tổng hợp hộ chưa đóng phí. |
| **Mục đích:** Làm dự án để cải thiện điều gì? | Tập trung thông tin hộ dân, khoản thu và thanh toán để hỗ trợ quản lý, tra cứu và thống kê. |
| **Mục tiêu:** Dựa vào đâu để biết đã đạt kết quả? | Quản lý được các loại phí và thông tin hộ dân thuộc danh sách đã thống nhất; ghi nhận, tra cứu được thanh toán; các tình huống nghiệm thu bắt buộc đều đạt. |

Nếu viết “quản lý 100% loại phí”, phải chỉ rõ **100% của danh mục nào**, chẳng hạn “danh mục yêu cầu phiên bản 1.0”. Nhờ vậy, mục tiêu mới kiểm tra được.

#### -bước 'Chốt phạm vi' — Xác định những công việc và chức năng được nhận thực hiện.

Tạo bảng:

| Nhóm | Ví dụ điền |
|---|---|
| Công việc thực hiện | Đặc tả yêu cầu, phân tích, thiết kế, lập trình, kiểm thử, triển khai |
| Chức năng thực hiện | Quản lý thu phí, người dùng, hộ gia đình |
| Công việc không bao gồm | Nhập toàn bộ dữ liệu thật ban đầu về hộ dân, nhân khẩu và các loại phí |

Việc không nhận nhập toàn bộ dữ liệu vận hành **không loại bỏ việc tạo dữ liệu mẫu để kiểm thử**.

Nếu muốn bổ sung giới hạn như “chưa tích hợp ngân hàng”, ghi đó là nội dung cần thống nhất với khách hàng trước khi chốt.

#### -bước 'Liệt kê sản phẩm bàn giao' — Xác định người nhận sẽ nhận được gì và kiểm tra bằng cách nào.

Tạo bảng từ danh sách bàn giao trong tài liệu:

| Sản phẩm | Người nhận | Cách kiểm tra mẫu |
|---|---|---|
| Bộ cài phần mềm | Khách hàng | Cài và chạy được trên môi trường đã thống nhất |
| Hướng dẫn cài đặt | Người triển khai | Làm theo tài liệu để cài thành công |
| Hướng dẫn sử dụng | Người dùng | Thực hiện được nghiệp vụ chính theo hướng dẫn |
| Hồ sơ bản quyền/quyền sử dụng | Khách hàng | Có hồ sơ theo thỏa thuận |
| Mã nguồn | Chủ đầu tư | Có đủ mã nguồn và hướng dẫn xây dựng |
| Tài liệu yêu cầu, thiết kế, kiểm thử | Chủ đầu tư | Đủ nội dung và phiên bản đã thống nhất |
| Tài liệu cấu trúc mã nguồn, API | Chủ đầu tư | Phù hợp với phần mềm bàn giao |
| Tài liệu dự án | Chủ đầu tư | Có kế hoạch và hồ sơ theo dõi cần thiết |

Cột “cách kiểm tra” giúp biến lời hứa bàn giao thành nội dung có thể nghiệm thu.

#### -bước 'Điền ngân sách và lịch trình' — Xác định giới hạn kinh phí và thời điểm cần có từng kết quả.

Ghi ngân sách **100.000.000 đồng**, bao gồm xây dựng phần mềm, quản lý dự án và dự phòng như tài liệu.

Ví dụ phân bổ để thực hành:

| Khoản mục | Kinh phí giả định |
|---|---:|
| Xây dựng phần mềm | 75.000.000 |
| Quản lý dự án | 10.000.000 |
| Dự phòng | 15.000.000 |
| **Tổng** | **100.000.000** |

Lập các mốc kết quả:

| Mốc | Thời điểm mẫu | Kết quả cần có |
|---|---|---|
| Chốt yêu cầu | Cuối tuần 2 | Yêu cầu được xác nhận |
| Hoàn thành thiết kế | Cuối tuần 4 | Thiết kế giao diện, dữ liệu và xử lý |
| Hoàn thành chức năng chính | Cuối tuần 8 | Phiên bản có thể kiểm thử |
| Bàn giao dùng thử | Cuối tuần 10 | Người dùng thử các nghiệp vụ mẫu |
| Hoàn tất điều chỉnh | Cuối tuần 11 | Xử lý các vấn đề đã thống nhất |
| Bàn giao chính thức | Cuối tuần 12 | Phần mềm và hồ sơ bàn giao |

Các ngày năm 2023 trong tài liệu thuộc ví dụ gốc. Khi làm dự án của mình, thay bằng ngày thực tế.

#### -bước 'Ghi rủi ro, giả định, ràng buộc và phụ thuộc' — Làm rõ các điều kiện ảnh hưởng đến tính khả thi của kế hoạch.

Điền theo bảng:

| Nhóm | Cách hiểu | Ví dụ |
|---|---|---|
| Rủi ro | Điều có thể xảy ra và gây ảnh hưởng | Thành viên rời nhóm giữa dự án |
| Giả định | Điều tạm coi là đúng để lập kế hoạch | Kế toán tham gia dùng thử và phản hồi |
| Ràng buộc | Giới hạn phải tuân thủ | Ngân sách không vượt 100 triệu đồng |
| Phụ thuộc bên ngoài | Việc cần một bên ngoài nhóm cung cấp hoặc hoàn thành | Ban quản trị cung cấp quy tắc tính phí |

Với phụ thuộc, thêm **người cung cấp và hạn cần nhận**. Ví dụ: “Kế toán cung cấp danh mục phí trước cuối tuần 1”.

Các ràng buộc trong tài liệu còn có thời gian dự án không quá bốn tháng và chỉ bổ sung nhân lực khi không vượt ngân sách.

#### -bước 'Quy định cách trao đổi thông tin' — Xác định ai cần nhận thông tin nào và vào lúc nào.

Lập bảng:

| Hoạt động | Thành phần | Tần suất | Nội dung cần lưu |
|---|---|---|---|
| Họp nhanh | Nhóm thực hiện | Hằng ngày | Việc đang làm, vướng mắc |
| Báo cáo tiến độ | Quản lý, nhà tài trợ, nhóm | Hằng tuần | Tiến độ, rủi ro, quyết định cần xử lý |
| Đánh giá mốc | Khách hàng, nhà tài trợ, nhóm | Theo mốc | Kết quả được chấp nhận, việc cần sửa |

Các quyết định làm thay đổi phạm vi, chi phí hoặc lịch phải được ghi nhận để các bên cùng theo dõi.

#### -bước 'Rà soát và phê duyệt' — Kiểm tra nội dung thống nhất trước khi dùng làm căn cứ triển khai.

Đọc lại để kiểm tra:

- Mục tiêu có nằm trong phạm vi không?
- Sản phẩm bàn giao có đủ không?
- Tổng ngân sách có đúng không?
- Lịch có phù hợp nguồn lực không?
- Vai trò và người có quyền xác nhận đã rõ chưa?

Tạo bảng **họ tên — chữ ký — ngày phê duyệt** cho các vai trò theo mẫu. Nếu là bài tập mô phỏng, ghi rõ “dự thảo phục vụ học tập”.

</details>

<details>
<summary><strong>-sản phẩm 'WBS theo sản phẩm bàn giao' — Chia phạm vi dự án thành những thành phần có kết quả kiểm tra được.</strong></summary>

#### -bước 'Lấy đầu vào từ tuyên ngôn' — Dùng phạm vi và danh sách bàn giao đã thống nhất để phân rã công việc.

Mở tuyên ngôn, lấy ba module cùng các hồ sơ, tài liệu và công việc bàn giao.

Tạo bảng:

| Mã WBS | Cấp | Tên thành phần | Kết quả cần có |
|---|---:|---|---|

Ở bước này tập trung vào **cần có những gì**, chưa cần điền lịch hoặc người làm.

#### -bước 'Xác định nút gốc' — Chốt phạm vi mà toàn bộ cấu trúc phải bao quát.

Nếu chỉ phân rã phần mềm như hình trong tài liệu, dùng:

> 0 — Phần mềm quản lý và thu phí Blue Moon.

Nếu phân rã toàn dự án, dùng:

> 0 — Dự án xây dựng phần mềm quản lý và thu phí Blue Moon.

Trong ví dụ này chọn **toàn dự án**, nên cấu trúc còn phải bao quát quản lý, tài liệu, triển khai và bàn giao.

#### -bước 'Chia thành các nhóm kết quả lớn' — Tạo những nhánh chính cần hoàn thành để dự án hoàn thành.

Điền:

| Mã | Thành phần |
|---|---|
| 1 | Bộ hồ sơ quản lý dự án |
| 2 | Module quản lý thu phí |
| 3 | Module quản lý người dùng |
| 4 | Module quản lý hộ gia đình |
| 5 | Bộ tài liệu kỹ thuật và hướng dẫn |
| 6 | Gói triển khai và bàn giao |

Ba module lấy theo tài liệu; các nhánh còn lại giúp bao quát phạm vi toàn dự án đã chọn.

#### -bước 'Phân rã module thành gói công việc' — Chia mỗi module thành các phần có thể mô tả và kiểm tra riêng.

Ví dụ:

| Mã | Gói công việc | Kết quả cần có |
|---|---|---|
| 2.1 | Chức năng tạo khoản thu | Tạo và lưu khoản thu theo quy tắc đã chốt |
| 2.2 | Chức năng ghi nhận thanh toán | Lưu đúng hộ, khoản thu và thông tin thanh toán |
| 2.3 | Chức năng thống kê | Hiển thị số liệu theo bộ lọc đã chốt |
| 3.1 | Chức năng quản lý tài khoản | Quản lý tài khoản theo yêu cầu |
| 3.2 | Chức năng phân quyền | Giới hạn thao tác theo vai trò |
| 4.1 | Chức năng quản lý hộ | Lưu và tra cứu thông tin hộ |
| 4.2 | Chức năng quản lý nhân khẩu | Lưu nhân khẩu gắn với hộ |
| 4.3 | Chức năng ghi nhận biến động | Theo dõi thay đổi nhân khẩu |

Danh sách chi tiết này là ví dụ thực hành; khi làm thật cần đối chiếu yêu cầu đã được xác nhận.

#### -bước 'Mô tả rõ từng gói' — Ghi đầu vào, đầu ra và tiêu chí hoàn thành để người nhận hiểu đúng việc.

Chọn gói `2.1`, điền:

| Nội dung | Ví dụ |
|---|---|
| Tên gói | Chức năng tạo khoản thu |
| Đầu vào | Quy tắc nghiệp vụ và danh mục loại phí đã chốt |
| Kết quả | Người có quyền tạo được khoản thu hợp lệ |
| Dữ liệu mẫu | Mã, tên khoản thu, loại phí, kỳ thu, số tiền hoặc quy tắc tính |
| Phạm vi xử lý | Kiểm tra dữ liệu, lưu và hiển thị khoản thu |
| Điều kiện hoàn thành | Lưu đúng dữ liệu hợp lệ; báo lỗi khi thiếu dữ liệu bắt buộc; kiểm soát quyền thao tác |

Trường dữ liệu phải xuất phát từ nghiệp vụ. Chẳng hạn phí theo diện tích cần dữ liệu và quy tắc khác khoản đóng góp tự nguyện.

#### -bước 'Tách gói lớn thành hoạt động' — Chia nhỏ khi một gói cần nhiều người hoặc nhiều loại công việc.

Với gói `2.1`, liệt kê:

- Làm rõ yêu cầu.
- Thiết kế dữ liệu và giao diện.
- Lập trình xử lý và giao diện.
- Tích hợp.
- Kiểm thử và sửa lỗi.
- Xác nhận kết quả.

Giữ mã liên kết với gói `2.1` để sau này biết từng nhiệm vụ phục vụ chức năng nào.

#### -bước 'Kiểm tra quy tắc 100%' — Bảo đảm phần con bao quát đúng phạm vi của phần cha.

Với mỗi nhánh, hỏi:

> Nếu hoàn thành tất cả phần con thì phần cha đã thực sự hoàn thành chưa?

Ví dụ, module thu phí không thể chỉ có “tạo khoản thu” nếu phạm vi còn bao gồm thanh toán và thống kê.

Kiểm tra thêm việc bỏ sót hoặc tính trùng. Chẳng hạn **thực hiện kiểm thử** và **bàn giao tài liệu kiểm thử** có liên hệ nhưng là hai kết quả cần mô tả rõ.

</details>

<details>
<summary><strong>-sản phẩm 'WBS theo quy trình — Waterfall hoặc Scrum' — Tổ chức công việc theo cách nhóm phát triển và hoàn thiện phần mềm.</strong></summary>

#### -bước 'Chọn cách tổ chức' — Xác định kế hoạch chính được trình bày theo giai đoạn hay theo các đợt phát triển.

| Cách tổ chức | Cách dùng trong bài thực hành |
|---|---|
| Waterfall | Nhóm việc theo yêu cầu, thiết kế, lập trình, kiểm thử, triển khai |
| Scrum | Tổ chức phát triển theo các Sprint, tạo kết quả có thể kiểm tra và nhận phản hồi |

Tài liệu minh họa cả hai. Bạn có thể học cả hai cách nhưng nên dùng một cấu trúc chính để quản lý, tránh cộng trùng công việc.

#### -bước 'Lập khung theo Waterfall' — Chia dự án thành các nhóm hoạt động lớn.

Tạo bảng:

| Mã | Nhánh công việc |
|---|---|
| 1 | Quản lý dự án |
| 2 | Xây dựng phần mềm |
| 2.1 | Phân tích yêu cầu |
| 2.2 | Thiết kế |
| 2.3 | Lập trình |
| 2.4 | Kiểm thử |
| 3 | Hỗ trợ người dùng |
| 4 | Triển khai và bàn giao |

Chỉ đưa vận hành lâu dài vào nếu đó là phạm vi đã thống nhất.

#### -bước 'Phân rã từng giai đoạn' — Chuyển tên giai đoạn thành công việc có đầu ra cụ thể.

Ví dụ nhánh thiết kế:

| Mã | Công việc | Đầu ra |
|---|---|---|
| 2.2.1 | Thiết kế chức năng | Luồng xử lý nghiệp vụ |
| 2.2.2 | Thiết kế giao diện | Bản thiết kế màn hình |
| 2.2.3 | Thiết kế dữ liệu | Mô hình dữ liệu và mô tả trường |
| 2.2.4 | Rà soát thiết kế | Danh sách vấn đề và thiết kế đã sửa |
| 2.2.5 | Thiết kế phân quyền | Bảng quyền theo vai trò |

Tiếp tục chia thiết kế dữ liệu theo ba module, rồi theo từng chức năng nếu cần.

Ví dụ, thiết kế dữ liệu cho “tạo khoản thu” phải chỉ rõ khoản thu có trường nào, trường nào bắt buộc và liên hệ với loại phí ra sao.

#### -bước 'Lập phương án theo Scrum' — Chia mục tiêu phát triển thành các đợt ngắn có kết quả kiểm tra được.

Dùng cùng phạm vi Blue Moon, thử chia:

| Sprint mẫu | Mục tiêu | Kết quả dự kiến |
|---|---|---|
| Sprint 1 | Tạo nền tảng tài khoản và dữ liệu hộ | Đăng nhập, quản lý thông tin hộ cơ bản |
| Sprint 2 | Quản lý khoản thu | Tạo và xem khoản thu |
| Sprint 3 | Ghi nhận thanh toán | Lưu thanh toán, tra cứu lịch sử |
| Sprint 4 | Thống kê và hoàn thiện | Xem thống kê, điều chỉnh theo phản hồi |

Trong mỗi Sprint, nhóm chọn công việc, phân rã nhiệm vụ, thực hiện, kiểm tra và nhận phản hồi. Không để toàn bộ kiểm thử đến cuối dự án.

Đây là ví dụ tổ chức công việc; cây WBS hoặc bảng Sprint riêng lẻ chưa thể hiện đầy đủ cách vận hành Scrum.

#### -bước 'Liên kết công việc với sản phẩm' — Kiểm tra mỗi hoạt động tạo ra kết quả gì trong phạm vi đã cam kết.

Lập bảng:

| Sản phẩm cần có | Công việc tạo ra |
|---|---|
| Tài liệu yêu cầu | Phỏng vấn, mô tả nghiệp vụ, xác nhận yêu cầu |
| Thiết kế dữ liệu | Phân tích dữ liệu, thiết kế, rà soát |
| Chức năng tạo khoản thu | Thiết kế, lập trình, tích hợp, kiểm thử |
| Bộ cài | Đóng gói, kiểm tra cài đặt |
| Hướng dẫn sử dụng | Viết hướng dẫn, kiểm tra bằng thao tác thực tế |

Sản phẩm chưa có công việc tạo ra nghĩa là kế hoạch đang thiếu. Công việc chưa gắn với phạm vi nào cần được xem lại lý do đưa vào.

</details>

<details>
<summary><strong>-sản phẩm 'Bảng nhiệm vụ, phân công và Gantt' — Xác định ai làm, làm bao lâu, phụ thuộc việc nào và thực hiện khi nào.</strong></summary>

#### -bước 'Chọn gói cần lập lịch' — Lấy một phần việc đủ nhỏ để chuyển từ WBS sang kế hoạch thực hiện.

Chọn `2.1 — Chức năng tạo khoản thu`.

Đọc lại đầu vào, đầu ra và điều kiện hoàn thành. Ví dụ dưới đây chỉ lập lịch cho chức năng này, chưa phải toàn dự án.

Tài liệu nêu Gantt trong Bài 4.2 nhưng chưa hướng dẫn chi tiết; cách lập bảng và tô lịch dưới đây là phần bổ sung để thực hành.

#### -bước 'Lập danh sách nhiệm vụ và phân công' — Mỗi nhiệm vụ có người phụ trách và kết quả phải giao.

Tạo bảng:

| Mã | Nhiệm vụ | Đầu ra | Người |
|---|---|---|---|
| T01 | Chốt yêu cầu | Quy tắc và trường dữ liệu đã xác nhận | A |
| T02 | Thiết kế dữ liệu | Thiết kế bảng, trường, ràng buộc | B |
| T03 | Thiết kế giao diện | Bản thiết kế màn hình | C |
| T04 | Lập trình xử lý, lưu dữ liệu | Phần xử lý hoạt động được | B |
| T05 | Lập trình giao diện | Màn hình nhập và hiển thị | C |
| T06 | Tích hợp | Giao diện lưu được dữ liệu qua phần xử lý | B |
| T07 | Kiểm thử | Kết quả kiểm tra, danh sách lỗi | D |
| T08 | Sửa lỗi | Phiên bản đã sửa | B |
| T09 | Kiểm tra lại | Kết quả xác nhận sau sửa | D |

T08 đang giả định chủ yếu là lỗi phần xử lý. Nếu phát sinh lỗi giao diện, cần bố trí C và cập nhật kế hoạch.

#### -bước 'Xác định phụ thuộc' — Chỉ rõ nhiệm vụ cần kết quả của nhiệm vụ nào trước khi bắt đầu.

Điền:

| Mã | Phụ thuộc | Lý do |
|---|---|---|
| T01 | Không | Bắt đầu làm rõ yêu cầu |
| T02 | T01 | Thiết kế dữ liệu theo yêu cầu |
| T03 | T01 | Thiết kế màn hình theo yêu cầu |
| T04 | T02 | Lập trình theo thiết kế dữ liệu |
| T05 | T03 | Lập trình theo thiết kế giao diện |
| T06 | T04, T05 | Cần cả hai phần để tích hợp |
| T07 | T06 | Kiểm tra luồng đã tích hợp |
| T08 | T07 | Sửa theo lỗi phát hiện |
| T09 | T08 | Kiểm tra phiên bản sau sửa |

T04 và T05 làm song song được khi nhóm đã thống nhất cách trao đổi dữ liệu và cách báo lỗi giữa hai phần.

#### -bước 'Ước lượng và xếp lịch' — Kết hợp thời lượng, quan hệ phụ thuộc và thời gian của người thực hiện.

Phân biệt:

- **Thời lượng:** Công việc kéo dài bao nhiêu ngày làm việc.
- **Công sức:** Tổng lượng lao động cần bỏ ra, ví dụ ngày công.

Giả định mỗi người làm toàn thời gian trong khoảng được phân công. Quy ước D1 là ngày làm việc đầu tiên:

| Mã | Người | Thời lượng | Công sức | Bắt đầu | Kết thúc |
|---|---|---:|---:|---|---|
| T01 | A | 1 ngày | 1 ngày công | D1 | D1 |
| T02 | B | 1 ngày | 1 ngày công | D2 | D2 |
| T03 | C | 1 ngày | 1 ngày công | D2 | D2 |
| T04 | B | 2 ngày | 2 ngày công | D3 | D4 |
| T05 | C | 2 ngày | 2 ngày công | D3 | D4 |
| T06 | B | 1 ngày | 1 ngày công | D5 | D5 |
| T07 | D | 2 ngày | 2 ngày công | D6 | D7 |
| T08 | B | 1 ngày | 1 ngày công | D8 | D8 |
| T09 | D | 1 ngày | 1 ngày công | D9 | D9 |

T02 và T03 cùng thực hiện ở D2 vì dùng chung đầu vào từ T01 và do hai người khác nhau làm.

Toàn bộ lịch kéo dài **9 ngày làm việc**, với tổng công sức **12 ngày công**. Hai con số khác nhau do có việc thực hiện song song.

#### -bước 'Vẽ Gantt' — Biểu diễn khoảng thời gian làm từng nhiệm vụ để nhìn rõ việc song song và nối tiếp.

Trong bảng tính:

1. Giữ các cột mã, nhiệm vụ, người, phụ thuộc và thời lượng.
2. Thêm các cột D1 đến D9.
3. Tô màu ô tương ứng với thời gian thực hiện.
4. Thêm mốc xác nhận chức năng sau khi T09 đạt yêu cầu.

Kết quả có dạng:

| Nhiệm vụ | D1 | D2 | D3 | D4 | D5 | D6 | D7 | D8 | D9 |
|---|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| T01 | ● | | | | | | | | |
| T02 | | ● | | | | | | | |
| T03 | | ● | | | | | | | |
| T04 | | | ● | ● | | | | | |
| T05 | | | ● | ● | | | | | |
| T06 | | | | | ● | | | | |
| T07 | | | | | | ● | ● | | |
| T08 | | | | | | | | ● | |
| T09 | | | | | | | | | ● |

**Mốc** là một điểm xác nhận, thường có thời lượng bằng 0. Công việc kiểm tra để đạt mốc vẫn cần được dành thời gian.

#### -bước 'Ghép lịch toàn dự án và kiểm tra' — Bảo đảm các chức năng dùng chung nguồn lực vẫn thực hiện được.

Lặp lại cách làm cho các gói khác, ghép vào cùng lịch rồi kiểm tra:

- Một người có bị giao hai việc toàn thời gian cùng lúc không?
- Công việc có bắt đầu trước khi nhận đủ đầu vào không?
- Có thời gian tích hợp giữa các module không?
- Có kiểm thử hệ thống, dùng thử, tài liệu và bàn giao không?
- Đã tính ngày nghỉ và thời gian chờ phản hồi chưa?

Ví dụ, không tiếp tục giao B một nhiệm vụ toàn thời gian khác trong D3–D4 khi B đã làm T04.

#### -bước 'Cập nhật theo thực tế' — Dùng tiến độ thực hiện để điều chỉnh phần kế hoạch còn lại.

Thêm các cột:

> Trạng thái — Bắt đầu thực tế — Kết thúc thực tế — Vướng mắc.

Nếu T04 trễ một ngày và các việc sau không có thời gian dự trữ, cập nhật T06 cùng các việc phụ thuộc. Ghi nguyên nhân, phương án xử lý và ảnh hưởng đến mốc xác nhận.

Không chỉ sửa ngày của nhiệm vụ bị trễ mà bỏ qua những việc đang chờ kết quả của nó.

</details>

<details>
<summary><strong>-sản phẩm 'Sổ đăng ký rủi ro và kế hoạch ứng phó' — Nhận diện điều có thể cản trở mục tiêu và chuẩn bị cách xử lý.</strong></summary>

#### -bước 'Thống nhất cách chấm rủi ro' — Chọn một thang đánh giá nhất quán trước khi điền bảng.

Tài liệu có điểm chưa thống nhất:

- Bảng ví dụ trang 7 có các con số tương ứng với cách nhân xác suất và tác động.
- Ma trận trang 9 dùng năm mức với kết quả khác.
- Hai dòng cuối phần mô tả mức độ ở trang 8 bị lặp nhãn “Mức 4”, “Mức 5”.

Bài thực hành này **dùng ma trận trang 9** và tính lại các ví dụ theo ma trận đó.

#### -bước 'Tạo bảng và mô tả rủi ro' — Ghi rõ sự kiện, nguyên nhân và hậu quả để biết cần theo dõi điều gì.

Tạo các cột:

> Mã — Mô tả — Nguyên nhân — Hậu quả — Xác suất — Tác động — Mức ưu tiên — Phòng ngừa — Dấu hiệu kích hoạt — Cách xử lý — Người theo dõi — Trạng thái.

Viết theo mẫu:

> Do [nguyên nhân], có thể xảy ra [sự kiện], dẫn đến [hậu quả].

Ví dụ:

> Do B đồng thời tham gia dự án khác, B có thể không hoàn thành T04 đúng lịch, làm chậm tích hợp và kiểm thử chức năng tạo khoản thu.

Đối chiếu các nhóm rủi ro trong tài liệu:

| Nhóm | Ví dụ |
|---|---|
| Nhân sự | Thành viên bận nhiều dự án hoặc rời nhóm |
| Yêu cầu | Bổ sung, thay đổi yêu cầu |
| Tài liệu | Hồ sơ kỹ thuật chưa hoàn thiện |
| Trao đổi | Hiểu sai nghiệp vụ do thiếu tương tác |
| Tiến độ | Việc trước chậm làm việc sau bị chậm |
| Hợp đồng, thủ tục | Điều kiện phê duyệt làm đình trệ dự án |
| Nghiệm thu | Khách hàng không chấp nhận sản phẩm |
| Ngân sách | Kinh phí bị cắt giảm |
| Ước lượng | Thời gian và chi phí được dự tính quá lạc quan |

Chỉ đưa vào những rủi ro có ý nghĩa với dự án, kèm lý do đánh giá.

#### -bước 'Chấm xác suất' — Đánh giá khả năng sự kiện xảy ra dựa trên thông tin hiện có.

| Điểm | Mức | Cách hiểu |
|---|---|---|
| 1 | Thấp | Hiếm xảy ra, ít dấu hiệu cho thấy sẽ xảy ra |
| 2 | Vừa | Có cơ sở hợp lý hoặc từng xảy ra thỉnh thoảng |
| 3 | Cao | Có dấu hiệu rõ hoặc thường xuyên xảy ra |

Ví dụ, nếu B đã thông báo lịch làm dự án khác, phải đối chiếu lịch đó với T04 để đánh giá khả năng thiếu thời gian.

Không tự đổi ba mức thành tỷ lệ phần trăm nếu nhóm chưa có quy ước.

#### -bước 'Chấm tác động' — Đánh giá hậu quả nếu rủi ro thực sự xảy ra.

Tài liệu gợi ý xem xét phạm vi, chất lượng và chi phí:

| Điểm | Mức | Căn cứ thực hành |
|---|---|---|
| 1 | Thấp | Ảnh hưởng nhỏ, dưới 5% theo chỉ tiêu đã chọn |
| 2 | Vừa | Ảnh hưởng từ 5% đến 10%, cần điều chỉnh có kiểm soát |
| 3 | Cao | Ảnh hưởng trên 10% hoặc làm một mục tiêu quan trọng không đạt |

Cột chi phí mức vừa trong tài liệu bị lặp nội dung từ chất lượng; bảng trên đã diễn đạt lại để sử dụng.

Nếu xét nhiều mặt, nhóm có thể quy ước **lấy điểm tác động cao nhất**. Ví dụ tăng chi phí 3% nhưng ảnh hưởng 15% phạm vi thì lấy tác động bằng 3. Đây là quy ước bổ sung, cần ghi rõ trong kế hoạch.

#### -bước 'Tra mức ưu tiên' — Kết hợp xác suất và tác động bằng đúng ma trận đã chọn.

| Xác suất \ Tác động | Thấp — 1 | Vừa — 2 | Cao — 3 |
|---|---:|---:|---:|
| Thấp — 1 | Mức 1 | Mức 2 | Mức 3 |
| Vừa — 2 | Mức 2 | Mức 3 | Mức 4 |
| Cao — 3 | Mức 3 | Mức 4 | Mức 5 |

Ví dụ:

- Xác suất 2, tác động 2 → **mức 3**.
- Xác suất 2, tác động 3 → **mức 4**.
- Xác suất 3, tác động 3 → **mức 5**.

Không nhân hai điểm rồi dùng kết quả làm mức của ma trận này.

Diễn giải năm mức theo thứ tự tăng dần:

| Mức | Ý nghĩa |
|---|---|
| 1 | Hầu như không ảnh hưởng |
| 2 | Không ảnh hưởng đáng kể |
| 3 | Có ảnh hưởng nhưng dự án vẫn thực hiện được |
| 4 | Ảnh hưởng đáng kể, một số công việc không thực hiện được |
| 5 | Không thể tiếp tục trong điều kiện hiện tại |

#### -bước 'Viết biện pháp ứng phó' — Chuẩn bị cả việc làm trước và việc làm khi có dấu hiệu xảy ra.

Ví dụ rủi ro thiếu nhân sự:

| Nội dung | Ví dụ điền |
|---|---|
| Phòng ngừa | Xác nhận lịch tham gia; chia sẻ kiến thức; cập nhật mã nguồn và hướng dẫn |
| Dấu hiệu kích hoạt | B báo không thể dành đủ thời gian đã cam kết cho T04 |
| Cách xử lý | Đánh giá việc còn lại, phân công lại, cập nhật lịch và báo ảnh hưởng |
| Người theo dõi | A |
| Trạng thái | Đang theo dõi |

Người được phân công thay thế phải có thời gian và năng lực phù hợp.

Điền tiếp các rủi ro mẫu; các điểm dưới đây là giả định để thực hành:

| Mã | Rủi ro | Xác suất | Tác động | Mức | Hành động chính | Theo dõi |
|---|---|---:|---:|---:|---|---|
| R01 | Thành viên không đủ thời gian | 2 | 3 | 4 | Chốt lịch, chia sẻ kiến thức, chuẩn bị phân công lại | A |
| R02 | Bổ sung yêu cầu | 2 | 2 | 3 | Đánh giá ảnh hưởng trước khi nhận làm | A |
| R03 | Tài liệu kỹ thuật chưa đủ | 1 | 3 | 3 | Kiểm tra tài liệu tại từng mốc | B |
| R04 | Hiểu sai nghiệp vụ | 2 | 2 | 3 | Xác nhận quy tắc bằng dữ liệu mẫu | A |
| R05 | Ước lượng quá lạc quan | 2 | 3 | 4 | Rà soát ước lượng cùng người thực hiện | A |
| R06 | Khách hàng từ chối nghiệm thu | 1 | 3 | 3 | Chốt tiêu chí sớm, tổ chức dùng thử | A |

Xếp mức cao trước. Với cùng mức, ưu tiên rủi ro sắp tác động hoặc ảnh hưởng trực tiếp đến mốc quan trọng.

#### -bước 'Đưa hành động vào lịch' — Biến biện pháp phòng ngừa thành nhiệm vụ có người làm và thời hạn.

Ví dụ để giảm R04:

| Nội dung | Điền vào kế hoạch |
|---|---|
| Nhiệm vụ | Xác nhận quy tắc tính phí bằng dữ liệu mẫu |
| Người phụ trách | A |
| Thời điểm | Trước thiết kế dữ liệu |
| Đầu ra | Các trường hợp tính phí được kế toán xác nhận |

Tương tự, thêm nhiệm vụ rà soát hồ sơ trước bàn giao để giảm rủi ro thiếu tài liệu.

#### -bước 'Theo dõi và cập nhật' — Điều chỉnh đánh giá theo tình hình và xử lý ngay khi sự kiện xảy ra.

Trong buổi theo dõi tiến độ, kiểm tra dấu hiệu, cập nhật điểm, người xử lý và hạn hành động.

Nếu B thực sự không thể tiếp tục T04, ghi nhận đó là **vấn đề hiện tại**, thực hiện phương án phân công lại và cập nhật Gantt. Khi đó, chỉ ghi “tiếp tục theo dõi rủi ro” sẽ không đủ.

</details>
