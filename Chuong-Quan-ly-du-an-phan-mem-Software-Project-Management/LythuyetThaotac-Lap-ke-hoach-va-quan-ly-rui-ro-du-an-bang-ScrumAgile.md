🔍**LythuyetThaotac: Lập kế hoạch dự án phần mềm — Project Charter, WBS, Gantt Chart và quản lý rủi ro** — Huong dan xay dung Ke hoach du an(7).pdf

**Giới thiệu bài toán mẫu để học cách thao tác**

Bạn nhận nhiệm vụ xây dựng **phần mềm quản lý và thu phí chung cư Blue Moon**, gồm ba nhóm chức năng:

- **Quản lý thu phí:** tạo khoản thu, ghi nhận thanh toán, thống kê.
- **Quản lý người dùng:** quản lý tài khoản và quyền sử dụng.
- **Quản lý hộ gia đình:** quản lý hộ, nhân khẩu và biến động nhân khẩu.

Muốn triển khai được, bạn cần trả lời lần lượt: dự án cần đạt điều gì → cần tạo ra những gì → phải làm những việc nào → ai làm, làm lúc nào → điều gì có thể khiến kế hoạch thất bại.

Dưới đây là **năm sản phẩm cần tạo**. Mỗi bước đều có **ý nghĩa**, **cách thao tác** và **ví dụ điền dữ liệu**.

Ngân sách **100 triệu đồng** được lấy từ tài liệu. Nhóm bốn người, lịch 12 tuần và các ước lượng công việc bên dưới là **giả định bổ sung để thực hành**, chưa phải cam kết thực tế.

<details>
<summary>-sản phẩm 'Tuyên ngôn dự án — Project Charter'</summary>

**Sản phẩm này dùng để làm gì?**

Đây là tài liệu xác lập dự án: lý do thực hiện, mục tiêu, phạm vi, nguồn lực, người chịu trách nhiệm và người phê duyệt.

Bạn cần tạo được một tài liệu mà người đọc có thể hiểu: **“Chúng ta đồng ý làm dự án gì, trong giới hạn nào và ai chịu trách nhiệm?”**

**Bước 1: Tạo tài liệu và xác định thông tin chung**

**Ý nghĩa:** Giúp mọi người nhận diện cùng một dự án, tránh mỗi người hiểu một tên hoặc một đối tượng phục vụ khác nhau.

**Cách thao tác:**

Mở Word hoặc công cụ soạn thảo bạn đang dùng. Tạo tài liệu có tên gợi ý `01_Tuyen_ngon_du_an_BlueMoon`, sau đó điền:

| Nội dung | Ví dụ điền |
|---|---|
| Tên dự án | Xây dựng phần mềm quản lý và thu phí chung cư Blue Moon |
| Nhà tài trợ dự án | Người đại diện có thẩm quyền phê duyệt nguồn lực dự án |
| Cơ quan tài trợ | Công ty ABC, theo ví dụ trong tài liệu |
| Mức độ ảnh hưởng | Thay đổi cách quản lý thông tin hộ dân và hoạt động thu phí của ban quản trị |
| Phiên bản tài liệu | 1.0 |
| Ngày lập | Ngày thực tế bạn lập tài liệu |

Tên nhà tài trợ phải được xác nhận theo dự án thực tế; không tự coi người dùng phần mềm là người có quyền duyệt ngân sách.

**Bước 2: Xác định đội thực hiện và các bên liên quan**

**Ý nghĩa:** Đội thực hiện trực tiếp làm sản phẩm. Các bên liên quan cung cấp yêu cầu, sử dụng, hỗ trợ hoặc phê duyệt sản phẩm.

**Cách thao tác:**

Tạo hai bảng riêng.

Bảng đội thực hiện mẫu:

| Thành viên | Vai trò chính | Trách nhiệm |
|---|---|---|
| A | Quản lý dự án, phân tích nghiệp vụ | Làm rõ yêu cầu, lập kế hoạch, theo dõi tiến độ |
| B | Lập trình phần xử lý và dữ liệu | Thiết kế dữ liệu, xử lý nghiệp vụ |
| C | Lập trình giao diện | Thiết kế và xây dựng màn hình |
| D | Kiểm thử | Chuẩn bị tình huống kiểm tra, kiểm tra kết quả và báo lỗi |

Bảng các bên liên quan:

| Bên liên quan | Cần tham gia việc gì? |
|---|---|
| Đại diện ban quản trị | Xác nhận phạm vi và tiêu chí nghiệm thu |
| Kế toán chung cư | Giải thích nghiệp vụ thu phí, dùng thử |
| Nhà tài trợ | Duyệt nguồn lực và các quyết định thuộc thẩm quyền |
| Đơn vị triển khai | Cung cấp thông tin môi trường cài đặt, hỗ trợ bàn giao |

Bổ sung họ tên, nơi công tác và thông tin liên hệ vào bản thực tế theo mẫu của tài liệu.

**Bước 3: Viết bối cảnh, mục đích và mục tiêu**

**Ý nghĩa:** Ba nội dung này trả lời ba câu hỏi khác nhau:

| Nội dung | Câu hỏi cần trả lời |
|---|---|
| Bối cảnh | Hiện tại đang có vấn đề gì? |
| Mục đích | Làm dự án để cải thiện điều gì? |
| Mục tiêu | Dựa vào đâu để biết dự án đạt kết quả? |

**Cách thao tác và ví dụ điền:**

**Bối cảnh:**

> Ban quản trị đang theo dõi hộ dân và các khoản thu bằng sổ sách, Excel. Thông tin nằm ở nhiều nơi, gây khó khăn khi tra cứu lịch sử thanh toán và tổng hợp các hộ chưa đóng phí.

**Mục đích:**

> Xây dựng phần mềm tập trung thông tin hộ dân, khoản thu và thanh toán để hỗ trợ ban quản trị quản lý và thống kê.

**Mục tiêu mẫu:**

- Quản lý được toàn bộ loại phí thuộc danh mục hai bên đã thống nhất.
- Quản lý được thông tin hộ và nhân khẩu theo các trường dữ liệu đã chốt.
- Ghi nhận được khoản thanh toán và tra cứu được lịch sử đóng phí.
- Các tình huống nghiệm thu bắt buộc đều đạt; không còn lỗi nghiêm trọng ngăn cản nghiệp vụ chính.

Khi viết “100%”, phải xác định **100% của danh sách nào**. Ví dụ: “100% loại phí trong danh mục yêu cầu phiên bản 1.0”, để có căn cứ kiểm tra.

**Bước 4: Chốt phạm vi làm và phạm vi không làm**

**Ý nghĩa:** Phạm vi xác định ranh giới dự án. Đây là căn cứ để nhận biết yêu cầu mới có làm tăng công việc hay không.

**Cách thao tác:**

Tách thành phạm vi công việc và phạm vi chức năng.

| Nhóm | Ví dụ điền |
|---|---|
| Công việc thực hiện | Đặc tả yêu cầu, phân tích, thiết kế, lập trình, kiểm thử, triển khai |
| Chức năng thực hiện | Quản lý thu phí, người dùng, hộ gia đình |
| Công việc không bao gồm | Nhập toàn bộ dữ liệu thật ban đầu về hộ dân, nhân khẩu và các loại phí |

Nội dung không bao gồm ở trên được nêu trong tài liệu. Nếu bạn muốn thêm giới hạn như “chưa tích hợp ngân hàng”, phải ghi đó là **đề xuất phạm vi cần thống nhất**.

Ví dụ quan trọng: nhóm vẫn phải tạo **dữ liệu mẫu để kiểm thử**, dù không nhận trách nhiệm nhập toàn bộ dữ liệu vận hành cho khách hàng.

**Bước 5: Liệt kê sản phẩm bàn giao và cách kiểm tra**

**Ý nghĩa:** “Lập trình xong” chưa đủ để bàn giao. Cần biết khách hàng nhận những gì và kiểm tra bằng cách nào.

**Cách thao tác:**

Tạo bảng:

| Sản phẩm bàn giao | Người nhận | Cách kiểm tra mẫu |
|---|---|---|
| Bộ cài phần mềm | Khách hàng | Cài được trên các phiên bản Windows đã thống nhất |
| Hướng dẫn cài đặt | Người triển khai | Làm theo tài liệu để cài thành công |
| Hướng dẫn sử dụng | Người dùng | Thực hiện được các nghiệp vụ chính theo hướng dẫn |
| Hồ sơ bản quyền/quyền sử dụng | Khách hàng | Có hồ sơ theo thỏa thuận |
| Mã nguồn | Chủ đầu tư | Nhận đủ mã nguồn và hướng dẫn xây dựng |
| Tài liệu yêu cầu, thiết kế, kiểm thử | Chủ đầu tư | Có đủ nội dung và phiên bản đã thống nhất |
| Tài liệu cấu trúc mã nguồn, API | Chủ đầu tư | Mô tả phù hợp với phần mềm bàn giao |
| Tài liệu dự án | Chủ đầu tư | Có kế hoạch và hồ sơ theo dõi cần thiết |

Các cách kiểm tra trong bảng là gợi ý bổ sung để bạn biến danh sách bàn giao thành nội dung có thể nghiệm thu.

**Bước 6: Điền ngân sách và các mốc lịch trình**

**Ý nghĩa:** Ngân sách giới hạn nguồn lực. Mốc lịch trình xác định thời điểm cần có kết quả cụ thể.

**Cách thao tác:**

Ghi tổng ngân sách **100.000.000 đồng**, bao gồm xây dựng phần mềm, quản lý dự án và dự phòng như tài liệu.

Để tập phân bổ, có thể dùng ví dụ:

| Khoản mục | Kinh phí giả định |
|---|---:|
| Xây dựng phần mềm | 75.000.000 |
| Quản lý dự án | 10.000.000 |
| Dự phòng | 15.000.000 |
| **Tổng** | **100.000.000** |

Sau đó lập các mốc:

| Mốc | Thời điểm mẫu | Kết quả cần có |
|---|---|---|
| Chốt yêu cầu | Cuối tuần 2 | Danh sách yêu cầu được xác nhận |
| Hoàn thành thiết kế | Cuối tuần 4 | Thiết kế giao diện, dữ liệu và xử lý |
| Hoàn thành chức năng chính | Cuối tuần 8 | Phiên bản có thể kiểm thử |
| Bàn giao dùng thử | Cuối tuần 10 | Người dùng thực hiện các nghiệp vụ mẫu |
| Hoàn tất điều chỉnh | Cuối tuần 11 | Xử lý các vấn đề đã thống nhất |
| Bàn giao chính thức | Cuối tuần 12 | Phần mềm và hồ sơ bàn giao |

Các ngày năm 2023 trong tài liệu là lịch của ví dụ gốc. Khi lập dự án của bạn, thay bằng ngày phù hợp với kế hoạch thực tế.

**Bước 7: Phân biệt rủi ro, giả định, ràng buộc và phụ thuộc**

**Ý nghĩa:** Bốn nhóm này ảnh hưởng khác nhau đến cách lập kế hoạch.

**Cách thao tác:**

Điền từng nhóm theo câu hỏi sau:

| Nhóm | Cách hiểu | Ví dụ |
|---|---|---|
| Rủi ro | Điều chưa chắc xảy ra nhưng có thể gây ảnh hưởng | Một thành viên rời nhóm giữa dự án |
| Giả định | Điều tạm coi là đúng để lập kế hoạch | Kế toán sẽ tham gia dùng thử và phản hồi |
| Ràng buộc | Giới hạn phải tuân thủ | Ngân sách không vượt 100 triệu đồng |
| Phụ thuộc bên ngoài | Việc cần một bên ngoài nhóm cung cấp hoặc hoàn thành | Ban quản trị cung cấp quy tắc tính phí trước khi chốt yêu cầu |

Với mỗi phụ thuộc, bổ sung **người cung cấp** và **hạn cần nhận**. Ví dụ: “Kế toán cung cấp danh mục phí trước cuối tuần 1”.

**Bước 8: Viết cách trao đổi thông tin**

**Ý nghĩa:** Nhóm cần biết thông tin nào được trao đổi, trao đổi với ai và vào lúc nào.

**Cách thao tác:**

| Hoạt động | Thành phần | Tần suất | Kết quả cần lưu |
|---|---|---|---|
| Họp nhanh | Nhóm thực hiện | Hằng ngày | Việc đang làm, vướng mắc |
| Báo cáo tiến độ | Quản lý, nhà tài trợ, nhóm | Hằng tuần | Tiến độ, rủi ro, quyết định cần xử lý |
| Đánh giá mốc | Khách hàng, nhà tài trợ, nhóm | Theo mốc | Kết quả được chấp nhận và việc cần sửa |

**Bước 9: Rà soát và phê duyệt**

**Ý nghĩa:** Các bên xác nhận cùng hiểu và chấp nhận nội dung dự án.

**Cách thao tác:**

Đọc lại để kiểm tra mục tiêu có nằm trong phạm vi, sản phẩm bàn giao có đủ và ngân sách có cộng đúng không. Sau đó tạo bảng họ tên, chữ ký và ngày phê duyệt cho các vai trò theo mẫu tài liệu.

Nếu là bài tập mô phỏng, ghi rõ **“dự thảo phục vụ học tập”**, không điền chữ ký giả.

**Dấu hiệu hoàn thành:** Người đọc có thể xác định được dự án làm gì, bàn giao gì, giới hạn nguồn lực và ai có quyền xác nhận.

</details>

<details>
<summary>-sản phẩm 'Cấu trúc phân cấp công việc theo sản phẩm bàn giao — WBS'</summary>

**Sản phẩm này dùng để làm gì?**

WBS chia phạm vi lớn thành các phần nhỏ để quản lý. Theo cách tổ chức này, bạn bắt đầu bằng câu hỏi: **“Muốn có sản phẩm hoàn chỉnh thì cần những thành phần nào?”**

**Bước 1: Lấy phạm vi và danh sách bàn giao làm đầu vào**

**Ý nghĩa:** WBS phải xuất phát từ những gì dự án đã thống nhất.

**Cách thao tác:**

Mở tuyên ngôn dự án, lấy ba module và danh sách tài liệu phải bàn giao.

Bạn có thể lập bảng trong Word hoặc Excel với các cột:

| Mã WBS | Cấp | Tên thành phần | Kết quả cần có |
|---|---:|---|---|

Chưa cần điền ngày hoặc người thực hiện ở bước này.

**Bước 2: Xác định nút gốc**

**Ý nghĩa:** Nút gốc quyết định toàn bộ phạm vi mà cấu trúc bên dưới phải bao quát.

**Cách thao tác:**

Nếu chỉ phân rã phần mềm như hình trong tài liệu, đặt:

> 0 — Phần mềm quản lý và thu phí Blue Moon.

Nếu muốn bao quát **toàn bộ dự án**, đặt:

> 0 — Dự án xây dựng phần mềm quản lý và thu phí Blue Moon.

Hai phạm vi này khác nhau: WBS của toàn dự án còn cần bao quát quản lý, tài liệu, triển khai và bàn giao.

Trong bài thực hành này, dùng phạm vi **toàn dự án**.

**Bước 3: Chia thành các nhóm kết quả lớn**

**Ý nghĩa:** Mỗi nhánh là một phần kết quả cần có để hoàn thành dự án.

**Cách thao tác và ví dụ điền:**

| Mã WBS | Thành phần |
|---|---|
| 1 | Bộ hồ sơ quản lý dự án |
| 2 | Module quản lý thu phí |
| 3 | Module quản lý người dùng |
| 4 | Module quản lý hộ gia đình |
| 5 | Bộ tài liệu kỹ thuật và hướng dẫn |
| 6 | Gói triển khai và bàn giao |

Ba nhánh module được lấy theo tài liệu; các nhánh còn lại giúp bao quát phạm vi toàn dự án đã chọn.

**Bước 4: Phân rã module thành các gói công việc**

**Ý nghĩa:** Gói công việc cần đủ cụ thể để biết phải tạo ra kết quả gì và có thể kiểm tra khi hoàn thành.

**Cách thao tác:**

Dưới mỗi module, thêm các chức năng. Ví dụ:

| Mã WBS | Gói công việc | Kết quả cần có |
|---|---|---|
| 2.1 | Chức năng tạo khoản thu | Tạo và lưu khoản thu theo quy tắc đã thống nhất |
| 2.2 | Chức năng ghi nhận thanh toán | Lưu thanh toán đúng hộ và khoản thu |
| 2.3 | Chức năng thống kê | Hiển thị số liệu theo bộ lọc đã chốt |
| 3.1 | Chức năng quản lý tài khoản | Quản lý tài khoản theo phạm vi yêu cầu |
| 3.2 | Chức năng phân quyền | Giới hạn thao tác theo vai trò |
| 4.1 | Chức năng quản lý hộ gia đình | Lưu và tra cứu thông tin hộ |
| 4.2 | Chức năng quản lý nhân khẩu | Lưu thông tin nhân khẩu gắn với hộ |
| 4.3 | Chức năng ghi nhận biến động | Theo dõi thay đổi nhân khẩu theo yêu cầu |

Danh sách chức năng chi tiết là ví dụ thực hành; cần đối chiếu yêu cầu của dự án bạn trước khi chốt.

**Bước 5: Viết mô tả cho một gói công việc**

**Ý nghĩa:** Tên “tạo khoản thu” còn ngắn; người được giao cần biết dữ liệu, giới hạn và tiêu chí hoàn thành.

**Cách thao tác:**

Chọn gói `2.1`, lập mô tả:

| Nội dung | Ví dụ điền |
|---|---|
| Mã | 2.1 |
| Tên | Chức năng tạo khoản thu |
| Đầu vào | Quy tắc nghiệp vụ đã chốt, danh mục loại phí |
| Kết quả | Người có quyền tạo được khoản thu hợp lệ |
| Dữ liệu mẫu | Mã khoản thu, tên khoản thu, loại phí, kỳ thu, số tiền hoặc quy tắc tính |
| Phạm vi xử lý | Kiểm tra dữ liệu, lưu và hiển thị khoản thu |
| Điều kiện hoàn thành | Lưu đúng dữ liệu hợp lệ; báo lỗi khi thiếu dữ liệu bắt buộc; chỉ người có quyền được thao tác |

Các trường dữ liệu phải do yêu cầu nghiệp vụ quyết định. Ví dụ phí tính theo diện tích sẽ cần dữ liệu khác khoản đóng góp tự nguyện.

**Bước 6: Tách tiếp nếu gói còn quá lớn**

**Ý nghĩa:** Một chức năng có thể cần nhiều người và nhiều loại công việc để hoàn thành.

**Cách thao tác:**

Với gói `2.1`, liệt kê các hoạt động:

- Làm rõ yêu cầu tạo khoản thu.
- Thiết kế dữ liệu và giao diện.
- Lập trình xử lý và giao diện.
- Tích hợp.
- Kiểm thử, sửa lỗi.
- Xác nhận kết quả.

Giữ liên kết các hoạt động này với mã `2.1`. Chúng sẽ được chuyển sang bảng nhiệm vụ ở sản phẩm tiếp theo.

**Bước 7: Kiểm tra quy tắc 100%**

**Ý nghĩa:** Toàn bộ phần con phải bao quát đúng phạm vi của phần cha.

**Cách thao tác:**

Với từng nhánh, tự hỏi:

> Nếu hoàn thành tất cả phần con thì phần cha đã thực sự hoàn thành chưa?

Ví dụ, module thu phí có cả tạo khoản thu, ghi nhận thanh toán và thống kê thì không thể chỉ liệt kê “tạo khoản thu”.

Đồng thời kiểm tra:

- Không bỏ sót kiểm thử, tài liệu và bàn giao.
- Không đưa việc ngoài phạm vi vào kế hoạch.
- Không tính cùng một công việc ở hai nhánh. Ví dụ: tài liệu kiểm thử có thể thuộc bộ hồ sơ kỹ thuật; việc thực hiện kiểm thử thuộc các hoạt động xây dựng chức năng.

**Dấu hiệu hoàn thành:** Mỗi phần việc cần làm đều tìm được vị trí trong WBS và mỗi gói có kết quả kiểm tra được.

</details>

<details>
<summary>-sản phẩm 'Cấu trúc phân cấp công việc theo quy trình — Waterfall hoặc Scrum'</summary>

**Sản phẩm này dùng để làm gì?**

Đây là cách tổ chức khác của WBS, bắt đầu từ câu hỏi: **“Nhóm đi qua những giai đoạn hoặc hoạt động nào để tạo sản phẩm?”**

Tài liệu minh họa cả Waterfall và Scrum. Bạn học cả hai cách, nhưng khi lập kế hoạch thực tế nên chọn một cấu trúc chính để theo dõi, tránh cộng trùng khối lượng.

**Bước 1: Chọn cách tổ chức phù hợp**

**Ý nghĩa:** Cách tổ chức công việc cần phù hợp với cách nhóm dự định phát triển phần mềm.

**Cách thao tác:**

| Cách tổ chức | Cách dùng trong bài thực hành |
|---|---|
| Theo Waterfall | Nhóm công việc thành yêu cầu, thiết kế, lập trình, kiểm thử, triển khai |
| Theo Scrum | Tổ chức công việc theo các đợt phát triển ngắn, tạo kết quả có thể kiểm tra và nhận phản hồi |

Scrum không chỉ là đổi tên các giai đoạn. Một cây WBS cũng chưa thể hiện đầy đủ cách vận hành Scrum.

**Bước 2: Tạo khung WBS theo Waterfall**

**Ý nghĩa:** Mỗi nhánh lớn tập hợp công việc thuộc một giai đoạn hoặc nhóm hoạt động.

**Cách thao tác:**

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

Chỉ bổ sung vận hành lâu dài nếu công việc đó thuộc phạm vi đã thống nhất.

**Bước 3: Phân rã từng giai đoạn theo đầu ra**

**Ý nghĩa:** Tên giai đoạn chưa đủ để giao việc. Cần biết giai đoạn đó tạo ra những gì.

**Cách thao tác:**

Ví dụ phân rã nhánh thiết kế:

| Mã | Công việc | Đầu ra |
|---|---|---|
| 2.2.1 | Thiết kế chức năng | Luồng xử lý nghiệp vụ |
| 2.2.2 | Thiết kế giao diện | Bản thiết kế màn hình |
| 2.2.3 | Thiết kế dữ liệu | Mô hình dữ liệu và mô tả trường |
| 2.2.4 | Rà soát thiết kế | Danh sách vấn đề và thiết kế đã sửa |
| 2.2.5 | Thiết kế phân quyền | Bảng quyền theo vai trò |

Tiếp tục chia `2.2.3` theo ba module, rồi đến từng chức năng nếu cần.

Ví dụ với “tạo khoản thu”, đầu ra thiết kế dữ liệu cần thể hiện được khoản thu lưu những trường nào và liên hệ với loại phí ra sao.

**Bước 4: Tạo phương án tổ chức theo Scrum**

**Ý nghĩa:** Chia việc phát triển thành những đợt ngắn, mỗi đợt có mục tiêu và kết quả sử dụng được theo tiêu chí đã thống nhất.

**Cách thao tác:**

Dùng cùng phạm vi Blue Moon, thử lập kế hoạch sơ bộ:

| Đợt phát triển mẫu | Mục tiêu | Kết quả dự kiến |
|---|---|---|
| Sprint 1 | Tạo nền tảng tài khoản và dữ liệu hộ | Người có quyền đăng nhập, quản lý thông tin hộ cơ bản |
| Sprint 2 | Quản lý khoản thu | Tạo và xem khoản thu |
| Sprint 3 | Ghi nhận thanh toán | Lưu thanh toán, tra cứu lịch sử |
| Sprint 4 | Thống kê và hoàn thiện | Xem thống kê, hoàn thiện kết quả theo phản hồi |

Đây là ví dụ chia đợt, cần điều chỉnh theo năng lực nhóm và phụ thuộc thực tế.

Trong mỗi Sprint, chọn các mục cần làm, phân rã thành nhiệm vụ, thực hiện, kiểm tra kết quả và nhận phản hồi. Không coi Sprint chỉ là thời gian viết mã rồi để toàn bộ kiểm thử đến cuối dự án.

**Bước 5: Nối quy trình với sản phẩm bàn giao**

**Ý nghĩa:** Bạn cần chứng minh công việc trong quy trình thực sự tạo ra các kết quả đã cam kết.

**Cách thao tác:**

Lập bảng liên kết:

| Sản phẩm cần có | Công việc tạo ra |
|---|---|
| Tài liệu yêu cầu | Phỏng vấn, mô tả nghiệp vụ, xác nhận yêu cầu |
| Thiết kế dữ liệu | Phân tích dữ liệu, thiết kế, rà soát |
| Chức năng tạo khoản thu | Thiết kế, lập trình, tích hợp, kiểm thử |
| Bộ cài | Đóng gói, kiểm tra cài đặt |
| Hướng dẫn sử dụng | Viết hướng dẫn, kiểm tra bằng thao tác thực tế |

Nếu có sản phẩm mà chưa có công việc tạo ra, kế hoạch đang thiếu. Nếu có công việc không phục vụ phạm vi nào, cần xem lại lý do đưa vào.

**Dấu hiệu hoàn thành:** Bạn nhìn được công việc theo quy trình, đồng thời truy ngược được mỗi công việc phục vụ sản phẩm nào.

</details>

<details>
<summary>-sản phẩm 'Bảng nhiệm vụ, phân công và biểu đồ Gantt'</summary>

**Sản phẩm này dùng để làm gì?**

WBS cho biết có những phần việc gì. Bảng nhiệm vụ và Gantt bổ sung: **ai làm, mất bao lâu, phụ thuộc việc nào và thực hiện khi nào**.

Tài liệu nêu Gantt trong Bài 4.2 nhưng chưa hướng dẫn chi tiết thao tác. Phần dưới bổ sung cách làm bằng bảng để bạn thực hành ngay.

**Bước 1: Chọn gói công việc để lập lịch**

**Ý nghĩa:** Bắt đầu từ một gói nhỏ giúp bạn hiểu đầy đủ cách chuyển từ WBS sang lịch.

**Cách thao tác:**

Chọn gói `2.1 — Chức năng tạo khoản thu`.

Đọc lại mô tả đầu vào, đầu ra và điều kiện hoàn thành của gói. Bảng dưới chỉ lập lịch cho chức năng này, **chưa phải lịch của toàn bộ dự án**.

**Bước 2: Chuyển thành các nhiệm vụ có đầu ra**

**Ý nghĩa:** Một nhiệm vụ cần đủ rõ để người nhận biết phải làm gì và giao lại kết quả gì.

**Cách thao tác:**

Tạo bảng với dữ liệu mẫu:

| Mã | Nhiệm vụ | Đầu ra | Người phụ trách |
|---|---|---|---|
| T01 | Chốt yêu cầu tạo khoản thu | Quy tắc và trường dữ liệu đã xác nhận | A |
| T02 | Thiết kế dữ liệu | Thiết kế bảng, trường, ràng buộc | B |
| T03 | Thiết kế giao diện | Bản thiết kế màn hình | C |
| T04 | Lập trình xử lý và lưu dữ liệu | Phần xử lý hoạt động được | B |
| T05 | Lập trình giao diện | Màn hình nhập và hiển thị | C |
| T06 | Tích hợp | Giao diện lưu được dữ liệu qua phần xử lý | B |
| T07 | Kiểm thử | Kết quả kiểm tra, danh sách lỗi | D |
| T08 | Sửa lỗi | Phiên bản đã sửa | B |
| T09 | Kiểm tra lại | Kết quả xác nhận sau sửa | D |

T08 đang dự kiến chủ yếu là lỗi phần xử lý. Nếu phát sinh lỗi giao diện, cần bố trí C và cập nhật lịch.

**Bước 3: Điền quan hệ phụ thuộc**

**Ý nghĩa:** Công việc có thứ tự do cần sử dụng kết quả của nhau.

**Cách thao tác:**

Điền mã công việc trước vào cột “Phụ thuộc”:

| Mã | Phụ thuộc | Lý do |
|---|---|---|
| T01 | Không | Bắt đầu làm rõ yêu cầu |
| T02 | T01 | Thiết kế dữ liệu theo yêu cầu |
| T03 | T01 | Thiết kế màn hình theo yêu cầu |
| T04 | T02 | Lập trình theo thiết kế dữ liệu |
| T05 | T03 | Lập trình theo thiết kế giao diện |
| T06 | T04, T05 | Có cả hai phần mới tích hợp được |
| T07 | T06 | Kiểm tra luồng đã tích hợp |
| T08 | T07 | Sửa theo lỗi được phát hiện |
| T09 | T08 | Kiểm tra phiên bản sau sửa |

Trong ví dụ này, hai phần lập trình song song cần thống nhất trước cách trao đổi dữ liệu và cách báo lỗi.

**Bước 4: Ước lượng thời lượng và công sức**

**Ý nghĩa:** Hai đại lượng này liên quan nhưng khác nhau:

- **Thời lượng:** Công việc kéo dài bao nhiêu ngày làm việc.
- **Công sức:** Tổng lượng lao động cần bỏ ra, chẳng hạn ngày công.

**Cách thao tác:**

Hỏi người thực hiện về khối lượng, độ khó và kinh nghiệm với việc tương tự. Sau đó điền:

| Mã | Thời lượng mẫu | Công sức mẫu |
|---|---:|---:|
| T01 | 1 ngày | 1 ngày công |
| T02 | 1 ngày | 1 ngày công |
| T03 | 1 ngày | 1 ngày công |
| T04 | 2 ngày | 2 ngày công |
| T05 | 2 ngày | 2 ngày công |
| T06 | 1 ngày | 1 ngày công |
| T07 | 2 ngày | 2 ngày công |
| T08 | 1 ngày | 1 ngày công |
| T09 | 1 ngày | 1 ngày công |

Ví dụ giả định mỗi người làm toàn thời gian trong khoảng được phân công, nên thời lượng và công sức của từng nhiệm vụ có cùng con số.

**Bước 5: Xếp lịch theo phụ thuộc và người thực hiện**

**Ý nghĩa:** Một lịch hợp lý phải đáp ứng cả thứ tự công việc và khả năng làm việc của từng người.

**Cách thao tác:**

Quy ước D1 là ngày làm việc đầu tiên, rồi lập:

| Mã | Người | Bắt đầu | Kết thúc |
|---|---|---|---|
| T01 | A | D1 | D1 |
| T02 | B | D2 | D2 |
| T03 | C | D2 | D2 |
| T04 | B | D3 | D4 |
| T05 | C | D3 | D4 |
| T06 | B | D5 | D5 |
| T07 | D | D6 | D7 |
| T08 | B | D8 | D8 |
| T09 | D | D9 | D9 |

T02 và T03 có thể song song vì cùng có đầu vào từ T01 và do hai người khác nhau thực hiện.

Lịch mẫu kéo dài **9 ngày làm việc**, trong khi tổng công sức là **12 ngày công**, do một số nhiệm vụ được thực hiện đồng thời.

**Bước 6: Vẽ Gantt bằng cách tô các ô thời gian**

**Ý nghĩa:** Gantt biểu diễn khoảng thời gian của từng nhiệm vụ để dễ nhìn việc song song và việc nối tiếp.

**Cách thao tác trong bảng tính:**

1. Giữ các cột mã, nhiệm vụ, người, phụ thuộc, thời lượng.
2. Thêm các cột D1 đến D9 ở bên phải.
3. Với mỗi nhiệm vụ, tô màu các ô từ ngày bắt đầu đến ngày kết thúc.
4. Thêm mốc “Xác nhận chức năng tạo khoản thu” sau khi T09 đạt yêu cầu.

Hình dung kết quả:

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

Mốc là một điểm xác nhận, thường có thời lượng bằng 0. Công việc kiểm tra để đạt mốc vẫn phải có thời lượng trong kế hoạch.

**Bước 7: Kiểm tra và mở rộng ra toàn dự án**

**Ý nghĩa:** Lịch của một chức năng chưa cho biết tổng thời gian hoàn thành phần mềm.

**Cách thao tác:**

Lặp lại quy trình cho các gói khác, sau đó ghép vào cùng lịch và kiểm tra:

- Một người có bị giao hai nhiệm vụ toàn thời gian cùng lúc không?
- Công việc có bắt đầu trước khi nhận đủ đầu vào không?
- Có thời gian tích hợp giữa các module không?
- Có kiểm thử toàn hệ thống, dùng thử, tài liệu và bàn giao không?
- Có tính ngày nghỉ và thời gian chờ phản hồi không?

Ví dụ, không thể tiếp tục giao B lập trình chức năng khác trong D3–D4 nếu B đã được dành toàn thời gian cho T04.

**Bước 8: Theo dõi thực tế và điều chỉnh lịch**

**Ý nghĩa:** Kế hoạch cần phản ánh kết quả thực tế để giúp ra quyết định.

**Cách thao tác:**

Thêm các cột “Trạng thái”, “Bắt đầu thực tế”, “Kết thúc thực tế”, “Vướng mắc”.

Nếu T04 trễ một ngày và các công việc sau không có thời gian dự trữ, hãy cập nhật T06 và các công việc phụ thuộc. Ghi lại nguyên nhân, phương án xử lý và ảnh hưởng tới mốc xác nhận.

**Dấu hiệu hoàn thành:** Mỗi nhiệm vụ có người phụ trách, đầu ra, thời lượng, phụ thuộc và vị trí trên lịch.

</details>

<details>
<summary>-sản phẩm 'Sổ đăng ký rủi ro và kế hoạch ứng phó'</summary>

**Sản phẩm này dùng để làm gì?**

Sản phẩm này giúp nhóm phát hiện trước những việc có thể cản trở mục tiêu, xác định mức ưu tiên và chuẩn bị cách xử lý.

**Lưu ý khi đọc tài liệu:** Bảng ví dụ trang 7 có các con số tương ứng với cách nhân xác suất và tác động, trong khi ma trận trang 9 dùng năm mức khác. Trang 8 còn lặp nhãn “Mức 4”, “Mức 5” ở hai dòng cuối.

Để thực hành nhất quán, phần dưới **chọn ma trận trang 9**. Các mức rủi ro trong ví dụ được tính lại theo ma trận đó.

**Bước 1: Tạo bảng ghi nhận rủi ro**

**Ý nghĩa:** Rủi ro cần được ghi thành thông tin có thể giao người theo dõi.

**Cách thao tác:**

Tạo các cột:

> Mã — Mô tả — Nguyên nhân — Hậu quả — Xác suất — Tác động — Mức ưu tiên — Phòng ngừa — Dấu hiệu kích hoạt — Cách xử lý — Người theo dõi — Trạng thái.

Tài liệu có các cột mô tả, xác suất, tác động, mức độ và phòng ngừa. Các cột còn lại được bổ sung để dễ thực hiện.

**Bước 2: Viết rủi ro thành tình huống cụ thể**

**Ý nghĩa:** Mô tả cụ thể giúp biết cần theo dõi điều gì và bảo vệ phần nào của kế hoạch.

**Cách thao tác:**

Dùng cấu trúc:

> Do [nguyên nhân], có thể xảy ra [sự kiện], dẫn đến [hậu quả].

Ví dụ:

> Do B đồng thời tham gia dự án khác, B có thể không hoàn thành T04 đúng lịch, làm chậm tích hợp và kiểm thử chức năng tạo khoản thu.

Đối chiếu thêm các nhóm rủi ro được tài liệu gợi ý:

| Nhóm | Ví dụ cần xem xét |
|---|---|
| Nhân sự | Thành viên bận nhiều dự án hoặc rời nhóm |
| Yêu cầu | Bổ sung, thay đổi yêu cầu |
| Tài liệu | Hồ sơ kỹ thuật chưa hoàn thiện |
| Trao đổi | Hiểu sai yêu cầu do thiếu tương tác |
| Tiến độ | Công việc trước chậm làm việc sau bị chậm |
| Hợp đồng, thủ tục | Điều kiện phê duyệt hoặc hợp đồng làm đình trệ dự án |
| Nghiệm thu | Khách hàng không chấp nhận sản phẩm |
| Ngân sách | Nguồn kinh phí bị cắt giảm |
| Ước lượng | Thời gian và chi phí được dự tính quá lạc quan |

Chỉ đưa vào sổ những rủi ro có ý nghĩa với dự án của bạn, kèm lý do đánh giá.

**Bước 3: Chấm xác suất**

**Ý nghĩa:** Xác suất thể hiện khả năng sự kiện xảy ra.

**Cách thao tác:**

| Điểm | Mức | Cách hiểu |
|---|---|---|
| 1 | Thấp | Hiếm xảy ra, ít dấu hiệu cho thấy sẽ xảy ra |
| 2 | Vừa | Có cơ sở hợp lý hoặc đã từng xảy ra thỉnh thoảng |
| 3 | Cao | Có dấu hiệu rõ hoặc thường xuyên xảy ra |

Ví dụ, B đã thông báo phải dành nhiều ngày cho dự án khác thì đánh giá khả năng thiếu thời gian phải dựa vào lịch cam kết đó.

Không tự quy đổi ba mức thành tỷ lệ phần trăm cụ thể nếu nhóm chưa có quy ước.

**Bước 4: Chấm tác động**

**Ý nghĩa:** Tác động trả lời: nếu xảy ra, dự án bị ảnh hưởng đến mức nào?

**Cách thao tác:**

Tài liệu gợi ý đánh giá theo phạm vi, chất lượng và chi phí, với các khoảng dưới 5%, từ 5% đến 10%, trên 10%.

Có thể viết lại thang thực hành:

| Điểm | Mức | Ví dụ căn cứ |
|---|---|---|
| 1 | Thấp | Ảnh hưởng nhỏ, dưới 5% theo chỉ tiêu đã chọn |
| 2 | Vừa | Ảnh hưởng từ 5% đến 10%, cần điều chỉnh có kiểm soát |
| 3 | Cao | Ảnh hưởng trên 10% hoặc làm một mục tiêu quan trọng không đạt |

Cột chi phí ở mức vừa trong bản gốc có nội dung bị lặp từ cột chất lượng; cách diễn đạt trên đã được làm rõ để sử dụng.

Nếu đánh giá nhiều mặt, nhóm có thể thống nhất **lấy điểm cao nhất** làm tác động chung. Đây là quy ước bổ sung của bài thực hành, cần ghi rõ.

Ví dụ, một rủi ro tăng chi phí 3% nhưng ảnh hưởng 15% phạm vi thì theo quy ước này lấy tác động bằng 3.

**Bước 5: Tra ma trận để xác định mức ưu tiên**

**Ý nghĩa:** Kết hợp khả năng xảy ra và hậu quả để biết rủi ro nào cần quan tâm trước.

**Cách thao tác:**

Dùng đúng ma trận trang cuối:

| Xác suất \ Tác động | Thấp — 1 | Vừa — 2 | Cao — 3 |
|---|---:|---:|---:|
| Thấp — 1 | Mức 1 | Mức 2 | Mức 3 |
| Vừa — 2 | Mức 2 | Mức 3 | Mức 4 |
| Cao — 3 | Mức 3 | Mức 4 | Mức 5 |

Ví dụ:

- Xác suất 2, tác động 2 → **mức 3**.
- Xác suất 2, tác động 3 → **mức 4**.
- Xác suất 3, tác động 3 → **mức 5**.

**Không nhân hai điểm rồi dùng kết quả làm mức của ma trận này.** Chẳng hạn 2 × 2 = 4, nhưng ô tương ứng trong ma trận là mức 3.

Theo thứ tự từ nhẹ đến nặng, năm mức được hiểu là: hầu như không ảnh hưởng → không đáng kể → có ảnh hưởng nhưng dự án vẫn tiếp tục → ảnh hưởng đáng kể → không thể tiếp tục trong điều kiện hiện tại.

**Bước 6: Viết phòng ngừa và cách xử lý khi xảy ra**

**Ý nghĩa:** Phòng ngừa làm giảm khả năng hoặc hậu quả; cách xử lý cho biết nhóm phải làm gì khi dấu hiệu xuất hiện hoặc sự kiện xảy ra.

**Cách thao tác:**

Ví dụ cho rủi ro thiếu nhân sự:

| Nội dung | Ví dụ điền |
|---|---|
| Phòng ngừa | Xác nhận lịch tham gia; chia sẻ kiến thức; cập nhật mã nguồn và hướng dẫn thường xuyên |
| Dấu hiệu kích hoạt | B báo không thể dành đủ thời gian đã cam kết cho T04 |
| Cách xử lý | Đánh giá phần việc còn lại, phân công lại phù hợp, cập nhật lịch và báo ảnh hưởng |
| Người theo dõi | A |
| Trạng thái | Đang theo dõi |

Người nhận việc thay thế phải có thời gian và năng lực phù hợp; không chỉ ghi tên dự phòng.

**Bước 7: Điền bảng mẫu và sắp xếp ưu tiên**

**Ý nghĩa:** Có danh sách cụ thể để dùng trong họp tiến độ.

**Cách thao tác:**

Các điểm dưới đây là đánh giá giả định để minh họa:

| Mã | Rủi ro | Xác suất | Tác động | Mức | Hành động chính | Theo dõi |
|---|---|---:|---:|---:|---|---|
| R01 | Thành viên không đủ thời gian | 2 | 3 | 4 | Chốt lịch, chia sẻ kiến thức, chuẩn bị phân công lại | A |
| R02 | Khách hàng bổ sung yêu cầu | 2 | 2 | 3 | Ghi nhận thay đổi, đánh giá ảnh hưởng trước khi nhận làm | A |
| R03 | Tài liệu kỹ thuật chưa đủ | 1 | 3 | 3 | Kiểm tra tài liệu tại từng mốc | B |
| R04 | Nhóm hiểu sai nghiệp vụ | 2 | 2 | 3 | Dùng ví dụ dữ liệu và xác nhận quy tắc với kế toán | A |
| R05 | Ước lượng quá lạc quan | 2 | 3 | 4 | Nhờ người thực hiện rà soát ước lượng và cập nhật theo kết quả thực tế | A |
| R06 | Khách hàng từ chối nghiệm thu | 1 | 3 | 3 | Chốt tiêu chí sớm, tổ chức dùng thử trước bàn giao | A |

Sắp xếp mức cao trước. Với rủi ro cùng mức, ưu tiên xem xét rủi ro sắp tác động hoặc ảnh hưởng trực tiếp đến mốc quan trọng.

**Bước 8: Đưa hành động ứng phó vào kế hoạch công việc**

**Ý nghĩa:** Một hành động chỉ nằm trong bảng rủi ro có thể bị quên. Hành động cần thời gian phải xuất hiện trong lịch.

**Cách thao tác:**

Ví dụ, để giảm rủi ro hiểu sai cách tính phí:

- Thêm nhiệm vụ “Xác nhận quy tắc tính phí bằng dữ liệu mẫu”.
- Giao A phụ trách.
- Đặt trước thiết kế dữ liệu.
- Đầu ra là các trường hợp tính phí đã được kế toán xác nhận.

Với rủi ro thiếu tài liệu, thêm nhiệm vụ rà soát hồ sơ trước mốc bàn giao.

**Bước 9: Cập nhật khi có thông tin mới**

**Ý nghĩa:** Xác suất và tác động thay đổi theo tình hình dự án.

**Cách thao tác:**

Trong buổi theo dõi tiến độ, kiểm tra dấu hiệu, cập nhật điểm, người xử lý và hạn hành động.

Nếu sự kiện đã xảy ra, ví dụ B thực sự không thể tiếp tục T04, hãy ghi nhận đó là **vấn đề hiện tại**, thực hiện phương án xử lý và cập nhật Gantt.

**Dấu hiệu hoàn thành:** Mỗi rủi ro quan trọng đều có căn cứ đánh giá, người theo dõi và hành động cụ thể gắn với kế hoạch.

</details>
