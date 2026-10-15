- 🔍LythuyetThaotac: **Lập kế hoạch dự án phần mềm: khởi tạo dự án, phân rã công việc, lập lịch và quản lý rủi ro** — **Huong dan xay dung Ke hoach du an(6).pdf**

Tư liệu gốc: Huong dan xay dung Ke hoach du an(6).pdf

**Giới thiệu bài toán mẫu để học cách thao tác**

Bạn nhận nhiệm vụ xây dựng **phần mềm quản lý chung cư Blue Moon**, gồm ba nhóm chức năng:

- Quản lý người dùng: tài khoản, đăng nhập, phân quyền.
- Quản lý hộ gia đình: căn hộ, hộ gia đình, cư dân.
- Quản lý thu phí: khoản thu, ghi nhận thanh toán, thống kê.

Để luyện tập, giả sử nhóm có **4 người**, thực hiện trong **8 tuần**, ngân sách tối đa **100 triệu đồng**. Đây là số liệu minh họa được đặt lại cho dễ thực hành; tài liệu gốc dùng lịch quý IV năm 2023.

Bốn người trong ví dụ gồm: **An** quản lý dự án; **Bình** thu thập yêu cầu và kiểm thử; **Chi**, **Dũng** lập trình.

Bạn sẽ tạo **7 sản phẩm quản lý dự án** dưới đây. “Sản phẩm” ở đây có thể là một tài liệu, một bảng hoặc một biểu đồ. Bài này hướng dẫn lập kế hoạch xây dựng phần mềm, nên chưa cần viết mã chương trình.

<details>
<summary>-sản phẩm 'Bản tuyên ngôn dự án: thống nhất vì sao làm, làm gì và trong giới hạn nào'</summary>

**1. Hiểu sản phẩm này**

Tuyên ngôn dự án — *Project Charter* — là văn bản chính thức cho phép dự án bắt đầu và xác định quyền hạn của người quản lý dự án.

Hiểu đơn giản: trước khi chia việc, các bên phải thống nhất **mình đang cùng làm dự án nào, để giải quyết vấn đề gì, ai chịu trách nhiệm và được sử dụng bao nhiêu nguồn lực**.

Tài liệu này mô tả dự án ở mức tổng quan. Danh sách công việc chi tiết sẽ được tạo ở các sản phẩm phía sau.

**2. Thao tác tạo**

Mở Word hoặc Google Docs, tạo tài liệu tên **Tuyên ngôn dự án Blue Moon**. Tạo các mục dưới đây và điền dữ liệu mẫu.

| Nội dung cần tạo | Ý nghĩa | Cách điền cho bài toán mẫu |
|---|---|---|
| Tên dự án | Nhận diện dự án | Xây dựng phần mềm quản lý và thu phí chung cư Blue Moon |
| Nhà tài trợ | Người bảo trợ, chấp thuận nguồn lực và các quyết định quan trọng | Đại diện có thẩm quyền của Công ty ABC; ghi tên thật khi thực hiện |
| Đơn vị tài trợ | Tổ chức cung cấp nguồn lực | Công ty ABC |
| Mức độ ảnh hưởng | Dự án thay đổi hoạt động của ai | Thay đổi cách ban quản trị quản lý cư dân và thu phí |
| Người quản lý dự án | Người tổ chức thực hiện và theo dõi dự án | An |
| Thành viên | Những người trực tiếp thực hiện | Bình, Chi, Dũng; bổ sung vai trò và thông tin liên hệ |
| Các bên liên quan | Những người cung cấp yêu cầu, sử dụng hoặc phê duyệt kết quả | Đại diện ban quản trị, kế toán chung cư, đại diện công ty thực hiện |
| Bối cảnh | Vấn đề hiện tại khiến dự án cần được thực hiện | Dữ liệu đang lưu trên Excel; khó tổng hợp tình trạng đóng phí và biến động cư dân |
| Mục đích | Nhu cầu nghiệp vụ muốn giải quyết | Tập trung dữ liệu cư dân và thu phí, hỗ trợ tra cứu và tổng hợp |
| Mục tiêu | Kết quả có thể kiểm tra được | Hoàn thành các chức năng đã thống nhất và vượt qua các tình huống nghiệm thu |
| Sản phẩm bàn giao | Những thứ khách hàng và chủ đầu tư sẽ nhận | Phần mềm, mã nguồn, tài liệu kỹ thuật, hướng dẫn và hồ sơ bàn giao |
| Phạm vi | Công việc, chức năng được làm và những phần bị loại trừ | Ba module đã nêu; không thực hiện nhập toàn bộ dữ liệu cư dân ban đầu |
| Ngân sách | Giới hạn tiền được sử dụng | Tối đa 100 triệu đồng, bao gồm dự phòng |
| Lịch trình chính | Thời điểm bắt đầu, kết thúc và các mốc lớn | Bắt đầu tuần 1; nghiệm thu tuần 7; bàn giao tuần 8 |
| Rủi ro và giả định | Điều có thể gây trở ngại và những điều tạm coi là đúng | Có thể đổi yêu cầu; giả định khách hàng cung cấp quy tắc tính phí đúng hạn |
| Ràng buộc | Giới hạn nhóm phải tuân thủ | Hoàn thành trong 8 tuần; không vượt ngân sách |
| Phụ thuộc bên ngoài | Đầu vào hoặc sự phối hợp do bên ngoài nhóm cung cấp | Ban quản trị cung cấp mẫu khoản thu, dữ liệu mẫu và cử người nghiệm thu |
| Truyền thông | Cách trao đổi, họp và báo cáo | Họp nhanh hằng ngày; báo cáo hằng tuần; họp khách hàng tại các mốc |
| Phê duyệt | Bằng chứng các bên đồng ý cho triển khai | Họ tên, chữ ký, ngày duyệt của các bên có thẩm quyền |

**3. Viết rõ ba nội dung dễ nhầm**

**Mục đích** trả lời: *Dự án giải quyết nhu cầu gì?*

> Giúp ban quản trị quản lý tập trung cư dân và tình trạng thu phí.

**Mục tiêu** trả lời: *Dựa vào đâu biết đã đạt kết quả?*

> Đến tuần 7, phần mềm thực hiện được toàn bộ tình huống nghiệm thu đã thống nhất cho ba module; không còn lỗi làm sai số tiền hoặc khiến chức năng chính không sử dụng được.

**Phạm vi** trả lời: *Dự án bao gồm những gì?*

> Thực hiện khảo sát, đặc tả yêu cầu, thiết kế, lập trình, kiểm thử, triển khai và hướng dẫn sử dụng cho ba module. Không bao gồm nhập toàn bộ dữ liệu cư dân ban đầu hoặc tích hợp thanh toán ngân hàng.

Trong tài liệu gốc, mục tiêu có cụm “quản lý được 100%”. Khi dùng cách viết này, bạn phải chỉ ra **100% của danh sách nào**. Chẳng hạn: “100% loại phí trong danh mục được ban quản trị xác nhận”, thay vì hiểu là mọi loại phí có thể phát sinh trong tương lai.

**4. Phân biệt giả định, ràng buộc và phụ thuộc**

| Loại | Ví dụ | Cách xử lý |
|---|---|---|
| Giả định | Khách hàng phản hồi yêu cầu trong 2 ngày làm việc | Cần xác minh; nếu không đúng thì đánh giá ảnh hưởng |
| Ràng buộc | Ngân sách tối đa 100 triệu đồng | Kế hoạch phải nằm trong giới hạn này |
| Phụ thuộc bên ngoài | Phải có mẫu tính phí do kế toán cung cấp | Ghi rõ ai cung cấp và cần nhận trước thời điểm nào |

**5. Khi nào sản phẩm hoàn thành?**

Khi các bên có thể đọc tài liệu và thống nhất được: **lý do làm, kết quả mong muốn, phạm vi, trách nhiệm, nguồn lực và người phê duyệt**.

Các thay đổi quan trọng sau đó cần được đánh giá ảnh hưởng và phê duyệt; không tự động thêm vào công việc đang làm.

</details>

<details>
<summary>-sản phẩm 'Danh mục sản phẩm bàn giao và tiêu chí nghiệm thu: biết phải giao gì, thế nào là đạt'</summary>

**1. Hiểu sản phẩm này**

**Sản phẩm bàn giao** là kết quả cụ thể nhóm phải cung cấp. **Tiêu chí nghiệm thu** là điều kiện dùng để xác nhận kết quả đó đạt yêu cầu.

Ví dụ:

- “Lập trình đăng nhập” là công việc.
- “Chức năng đăng nhập hoạt động” là kết quả.
- “Tài khoản hợp lệ đăng nhập được, tài khoản bị khóa bị từ chối” là tiêu chí kiểm tra.

Tài liệu gốc liệt kê sản phẩm bàn giao trong tuyên ngôn dự án. Ở đây, ta tách thành một bảng riêng và bổ sung tiêu chí nghiệm thu để dễ chia việc và kiểm tra.

**2. Thao tác tạo**

Tạo bảng có các cột:

**Mã sản phẩm → Tên sản phẩm → Nội dung phải có → Người nhận → Tiêu chí nghiệm thu.**

Điền mẫu:

| Mã | Sản phẩm | Nội dung phải có | Người nhận | Tiêu chí nghiệm thu mẫu |
|---|---|---|---|---|
| SP01 | Bộ phần mềm hoàn chỉnh | Ba module và cơ sở dữ liệu cần thiết | Ban quản trị | Cài đặt được trên các môi trường đã thống nhất; các tình huống nghiệm thu đều đạt |
| SP02 | Mã nguồn | Mã chương trình, cấu hình mẫu, hướng dẫn xây dựng | Chủ đầu tư | Người nhận dựng và chạy được chương trình theo hướng dẫn |
| SP03 | Đặc tả yêu cầu | Chức năng, quy tắc nghiệp vụ, vai trò người dùng | Chủ đầu tư, đại diện khách hàng | Được đại diện khách hàng xác nhận |
| SP04 | Tài liệu thiết kế | Dữ liệu, giao diện, xử lý và phân quyền | Chủ đầu tư | Thống nhất với yêu cầu đã duyệt và phần mềm thực tế |
| SP05 | Hồ sơ kiểm thử | Tình huống kiểm thử, kết quả, danh sách lỗi | Chủ đầu tư | Có kết quả cho từng tình huống; lỗi còn tồn tại được ghi rõ |
| SP06 | Hướng dẫn cài đặt và sử dụng | Cách cài, đăng nhập, thao tác nghiệp vụ | Người cài đặt, người dùng cuối | Người được hướng dẫn thực hiện được các thao tác chính |
| SP07 | Tài liệu mã nguồn và API | Cấu trúc chương trình, cách gọi API nếu có | Đội tiếp nhận kỹ thuật | Người tiếp nhận tìm được thành phần và cách sử dụng cần thiết |
| SP08 | Hồ sơ dự án và bàn giao | Kế hoạch, phê duyệt, biên bản nghiệm thu, hồ sơ bản quyền theo thỏa thuận | Khách hàng, chủ đầu tư | Đủ đầu mục, phiên bản và xác nhận theo thỏa thuận |

Với yêu cầu “chạy trên các phiên bản Windows khác nhau” trong tài liệu gốc, cần ghi rõ **những phiên bản nào được hỗ trợ** để có thể kiểm thử và nghiệm thu.

**3. Viết tiêu chí nghiệm thu cho một chức năng cụ thể**

Lấy chức năng **ghi nhận thu phí**:

| Nội dung kiểm tra | Kết quả mong đợi |
|---|---|
| Chọn một căn hộ và kỳ thu | Hiển thị đúng khoản phải thu của căn hộ trong kỳ đó |
| Nhập số tiền đã nộp hợp lệ | Lưu được bản ghi thanh toán |
| Tra cứu lại | Hiển thị đúng số tiền, ngày nộp và người ghi nhận |
| Xem thống kê | Tổng tiền khớp với các giao dịch đã ghi nhận |
| Tài khoản không có quyền thu phí | Không thực hiện được thao tác ghi nhận |

Những quy tắc như cho phép nộp một phần, sửa giao dịch hoặc hủy giao dịch phải được hỏi và xác nhận trong bước thu thập yêu cầu.

**4. Liên hệ với sản phẩm tiếp theo**

Danh mục này là đầu vào để lập WBS. Nếu phải bàn giao hướng dẫn sử dụng thì WBS phải có công việc tạo hướng dẫn; không thể chỉ có công việc lập trình.

**Sản phẩm hoàn thành khi:** mọi đầu mục cần giao đều có nội dung và cách xác nhận đạt yêu cầu.

</details>

<details>
<summary>-sản phẩm 'Cấu trúc phân rã công việc WBS: chia toàn bộ dự án thành các phần có thể quản lý'</summary>

**1. Hiểu sản phẩm này**

WBS — *Work Breakdown Structure* — là cấu trúc chia một dự án lớn thành các phần nhỏ hơn.

Nó trả lời câu hỏi: **Để hoàn thành toàn bộ dự án, cần hoàn thành những phần việc nào?**

WBS chưa trả lời chi tiết “ngày nào làm”. Ngày thực hiện sẽ được xác định khi lập lịch.

**2. Hai cách phân rã trong tài liệu**

| Cách phân rã | Câu hỏi dùng để chia | Ví dụ |
|---|---|---|
| Theo sản phẩm bàn giao | Phần mềm gồm những thành phần nào? | Thu phí → Tạo khoản thu, Ghi nhận thanh toán, Thống kê |
| Theo quy trình | Dự án đi qua những nhóm hoạt động nào? | Phân tích → Thiết kế → Lập trình → Kiểm thử → Triển khai |

Bạn có thể dùng một cách làm cấu trúc chính, rồi bổ sung chiều còn lại khi chia nhỏ. Các hình trong tài liệu là ví dụ; không bắt buộc mọi dự án phải có đúng các nhánh đó.

**3. Thao tác tạo WBS theo sản phẩm**

Tạo bảng gồm **Mã WBS – Tên thành phần – Kết quả cần tạo**.

Trước hết, phân rã riêng phần mềm:

| Mã | Thành phần | Kết quả cần tạo |
|---|---|---|
| 1 | Phần mềm Blue Moon | Phần mềm hoàn chỉnh |
| 1.1 | Quản lý người dùng | Nhóm chức năng tài khoản và quyền truy cập |
| 1.1.1 | Đăng nhập | Kiểm tra thông tin tài khoản và cho phép truy cập |
| 1.1.2 | Quản lý tài khoản | Tạo, sửa, khóa tài khoản theo yêu cầu |
| 1.1.3 | Phân quyền | Giới hạn chức năng theo vai trò |
| 1.2 | Quản lý hộ gia đình | Nhóm chức năng quản lý hộ và cư dân |
| 1.2.1 | Quản lý hộ gia đình | Thêm, sửa và tra cứu thông tin hộ |
| 1.2.2 | Quản lý cư dân | Ghi nhận cư dân thuộc từng hộ |
| 1.2.3 | Biến động cư dân | Ghi nhận thay đổi theo nghiệp vụ đã thống nhất |
| 1.3 | Quản lý thu phí | Nhóm chức năng quản lý khoản thu và thanh toán |
| 1.3.1 | Tạo khoản thu | Khai báo khoản thu, kỳ thu và quy tắc áp dụng |
| 1.3.2 | Ghi nhận thanh toán | Lưu thông tin tiền đã nộp |
| 1.3.3 | Thống kê thu phí | Tổng hợp đã thu, chưa thu theo yêu cầu |

Đây là **WBS cho phạm vi phần mềm**. Nếu cần WBS bao quát **toàn bộ dự án**, phải bổ sung các kết quả như tài liệu yêu cầu, tài liệu thiết kế, kiểm thử, triển khai, hướng dẫn và quản lý dự án.

**4. WBS tổng thể theo quy trình để dùng cho bài mẫu**

| Mã | Nhóm công việc | Các phần việc bên trong |
|---|---|---|
| 1 | Khởi tạo và quản lý | Tuyên ngôn, kế hoạch, họp, báo cáo, theo dõi thay đổi, kết thúc dự án |
| 2 | Phân tích yêu cầu | Khảo sát, xác định chức năng, quy tắc nghiệp vụ, tiêu chí nghiệm thu |
| 3 | Thiết kế | Thiết kế dữ liệu, giao diện, xử lý, phân quyền và rà soát thiết kế |
| 4 | Xây dựng phần mềm | Quản lý người dùng, hộ gia đình, thu phí và tích hợp |
| 5 | Kiểm thử và nghiệm thu | Kiểm thử hệ thống, sửa lỗi, kiểm thử lại, người dùng nghiệm thu |
| 6 | Tài liệu và bàn giao | Hướng dẫn, đóng gói, triển khai, đào tạo và hồ sơ bàn giao |

Trong bài mẫu tiếp theo, ta dùng cấu trúc tổng thể này để không bỏ sót công việc ngoài lập trình.

**5. Cách biết đã chia đủ nhỏ**

Ví dụ “Xây dựng module thu phí” còn lớn. Có thể chia tiếp thành:

- Xác nhận quy tắc tính phí.
- Thiết kế dữ liệu khoản thu và thanh toán.
- Xây dựng thao tác tạo khoản thu.
- Xây dựng thao tác ghi nhận thanh toán.
- Xây dựng thống kê.
- Kiểm thử các trường hợp liên quan.

Một phần việc đã đủ rõ để quản lý khi bạn xác định được **kết quả, người chịu trách nhiệm, cách ước lượng và điều kiện hoàn thành**.

**6. Áp dụng quy tắc 100%**

Tài liệu yêu cầu: hoàn thành mọi phần con thì phần cha cũng phải hoàn thành.

Vì vậy cần kiểm tra:

- Có thiếu phần việc nào cần để hoàn thành phần cha không?
- Có phần việc nào nằm ngoài phạm vi đã thống nhất không?
- Có hai nhánh cùng tính một phần việc, dẫn đến đếm trùng không?

Ví dụ, nếu phần cha là “Module thu phí hoàn chỉnh” nhưng các phần con chỉ có “viết giao diện” và “viết xử lý”, vẫn thiếu kiểm thử và các kết quả liên quan cần thiết để xác nhận hoàn thành.

</details>

<details>
<summary>-sản phẩm 'Bảng nhiệm vụ, phân công và ước lượng: biến WBS thành việc giao được cho từng người'</summary>

**1. Hiểu sản phẩm này**

Sau khi biết các nhóm công việc, bạn cần xác định **ai làm, làm bao lâu, cần đầu vào gì và tạo ra kết quả nào**.

Một nhiệm vụ nên mô tả đủ rõ để người nhận bắt đầu làm và người kiểm tra xác nhận được lúc hoàn thành.

**2. Những thuộc tính cần tạo**

| Thuộc tính | Ý nghĩa | Ví dụ |
|---|---|---|
| Mã nhiệm vụ | Định danh để tham chiếu | T07 |
| Mã WBS | Cho biết nhiệm vụ thuộc phần nào của dự án | Nhánh 4 – Xây dựng phần mềm |
| Tên nhiệm vụ | Hành động và đối tượng cụ thể | Xây dựng module thu phí |
| Đầu vào | Thông tin cần có để làm | Quy tắc tính phí, thiết kế dữ liệu |
| Đầu ra | Kết quả phải tạo | Module thu phí chạy được |
| Người phụ trách | Người chịu trách nhiệm chính | Dũng |
| Nỗ lực | Tổng lượng lao động | 8 ngày công |
| Thời lượng | Khoảng thời gian thực hiện theo lịch | 8 ngày làm việc nếu một người làm toàn thời gian |
| Công việc trước | Điều kiện cần hoàn thành trước | T05 |
| Điều kiện hoàn thành | Bằng chứng nhiệm vụ đã xong | Chức năng đạt kiểm thử và được rà soát |

**Nỗ lực và thời lượng khác nhau.** Hai người cùng làm một nhiệm vụ trong 3 ngày có thể tạo ra 6 ngày công. Tuy nhiên, thêm người không bảo đảm mọi nhiệm vụ đều hoàn thành nhanh tương ứng.

**3. Bảng nhiệm vụ mẫu**

Để bảng dễ theo dõi, các nhiệm vụ dưới đây được trình bày ở mức tổng hợp. Khi giao việc thực tế, tiếp tục chia nhỏ những module còn lớn.

| Mã | Nhiệm vụ | Người phụ trách | Ngày công | Công việc trước |
|---|---|---|---:|---|
| T01 | Lập tuyên ngôn và kế hoạch ban đầu | An | 2 | — |
| T02 | Khảo sát và chốt yêu cầu | Bình | 3 | T01 |
| T03 | Thiết kế dữ liệu | Chi | 3 | T02 |
| T04 | Thiết kế giao diện | Dũng | 3 | T02 |
| T05 | Xây dựng module người dùng | Dũng | 5 | T03, T04 |
| T06 | Xây dựng module hộ gia đình | Chi | 7 | T03, T04 |
| T07 | Xây dựng module thu phí | Dũng | 8 | T05 |
| T08 | Tích hợp các module | Chi | 3 | T06, T07 |
| T09 | Kiểm thử hệ thống | Bình | 5 | T08 |
| T10 | Sửa lỗi và hỗ trợ kiểm thử lại | Chi | 3 | T09 |
| T11 | Viết hướng dẫn và hoàn thiện tài liệu | Dũng | 4 | T08 |
| T12 | Tổ chức người dùng nghiệm thu | Bình | 2 | T10, T11 |
| T13 | Đóng gói và triển khai | Chi | 2 | T12 |
| T14 | Đào tạo và bàn giao | An | 2 | T13 |
| T15 | Theo dõi, báo cáo và quản lý thay đổi | An | 8 | Phân bổ trong suốt dự án |
| **Tổng** | | | **60** | |

Ở đây, T07 được xếp sau T05 vì cùng do Dũng thực hiện và bài mẫu ưu tiên hoàn thành phần người dùng trước. T03 cũng phải hoàn thành trước T07 thông qua chuỗi phụ thuộc T03 → T05 → T07.

Nỗ lực của Bình ở T09 và T12 bao gồm việc chuẩn bị kiểm thử và kiểm tra lại tương ứng. Nếu khối lượng kiểm tra lại tăng, phải cập nhật ước lượng.

**4. Cách ước lượng có căn cứ**

Không điền “8 ngày” chỉ vì cảm thấy hợp lý. Hãy chia nhỏ T07:

| Phần việc | Ngày công minh họa |
|---|---:|
| Xây dựng tạo khoản thu | 2 |
| Xây dựng ghi nhận thanh toán | 3 |
| Xây dựng thống kê | 2 |
| Tự kiểm tra và hoàn thiện | 1 |
| **Tổng** | **8** |

Sau đó hỏi người thực hiện, đối chiếu công việc tương tự và ghi lại giả định, chẳng hạn “quy tắc tính phí đã được xác nhận”.

**Sản phẩm hoàn thành khi:** mỗi nhiệm vụ đều có người phụ trách, kết quả rõ ràng và ước lượng đủ căn cứ để lập lịch.

</details>

<details>
<summary>-sản phẩm 'Bảng ngân sách: kiểm tra kế hoạch có nằm trong số tiền được phép dùng không'</summary>

**1. Hiểu sản phẩm này**

Tuyên ngôn ghi giới hạn ngân sách; bảng ngân sách giải thích **tiền dự kiến được sử dụng cho những gì**.

Phần này triển khai chi tiết mục ngân sách trong tài liệu gốc. Các đơn giá dưới đây chỉ dùng để học cách tính.

**2. Thao tác tạo**

Lấy số ngày công từ bảng nhiệm vụ. Giả sử chi phí quy đổi là **1 triệu đồng/ngày công** cho mọi thành viên.

| Người | Nhiệm vụ tương ứng | Tổng ngày công | Thành tiền |
|---|---|---:|---:|
| An | T01, T14, T15 | 12 | 12 triệu |
| Bình | T02, T09, T12 | 10 | 10 triệu |
| Chi | T03, T06, T08, T10, T13 | 18 | 18 triệu |
| Dũng | T04, T05, T07, T11 | 20 | 20 triệu |
| **Tổng nhân công** | | **60** | **60 triệu** |

Công thức:

**Chi phí nhân công = Tổng ngày công × Đơn giá ngày công.**

Tiếp theo, bổ sung các chi phí khác:

| Khoản mục | Ngân sách mẫu |
|---|---:|
| Nhân công | 60 triệu |
| Hạ tầng phát triển và kiểm thử | 8 triệu |
| Công cụ và giấy phép cần mua | 5 triệu |
| Chi phí trực tiếp cho triển khai, đào tạo | 7 triệu |
| Dự phòng | 20 triệu |
| **Tổng** | **100 triệu** |

Khoản triển khai, đào tạo 7 triệu ở đây là chi phí trực tiếp như đi lại hoặc thuê thiết bị; công lao động đã được tính trong bảng nhân công để tránh tính hai lần.

**3. Cách dùng bảng khi có thay đổi**

Giả sử khách hàng yêu cầu thêm chức năng xuất báo cáo, dự kiến cần 4 ngày công:

- Chi phí nhân công tăng thêm: **4 triệu đồng**.
- Kiểm tra chức năng có cần thêm công cụ hoặc hạ tầng không.
- Kiểm tra ảnh hưởng đến lịch thực hiện.
- Trình người có thẩm quyền quyết định trước khi đưa vào kế hoạch.

Có tiền dự phòng không có nghĩa là mọi yêu cầu mới đều tự động được thực hiện. Dự phòng phải được sử dụng theo thỏa thuận quản lý của dự án.

**Sản phẩm hoàn thành khi:** tổng chi phí có căn cứ, không tính trùng và nằm trong giới hạn được duyệt.

</details>

<details>
<summary>-sản phẩm 'Lịch thực hiện và biểu đồ Gantt: biết công việc diễn ra khi nào'</summary>

**1. Hiểu sản phẩm này**

Biểu đồ Gantt thể hiện công việc theo thời gian:

- Mỗi hàng là một nhiệm vụ.
- Trục ngang là thời gian.
- Thanh ngang thể hiện khoảng thực hiện nhiệm vụ.

**WBS cho biết phải làm những phần nào; Gantt cho biết các phần đó diễn ra khi nào.**

Tài liệu gốc nêu Gantt ở tên Bài 4.2 nhưng chưa hướng dẫn thao tác cụ thể. Phần dưới bổ sung cách tạo.

**2. Quy ước lịch cho bài mẫu**

Giả sử mỗi tuần có 5 ngày làm việc, không tính ngày nghỉ lễ:

| Tuần | Các ngày làm việc |
|---|---|
| Tuần 1 | Ngày 1–5 |
| Tuần 2 | Ngày 6–10 |
| Tuần 3 | Ngày 11–15 |
| Tuần 4 | Ngày 16–20 |
| Tuần 5 | Ngày 21–25 |
| Tuần 6 | Ngày 26–30 |
| Tuần 7 | Ngày 31–35 |
| Tuần 8 | Ngày 36–40 |

**3. Xếp lịch theo bảng nhiệm vụ**

Các nhiệm vụ T01–T14 được giả sử làm toàn thời gian trong khoảng được giao.

| Mã | Nhiệm vụ | Bắt đầu | Kết thúc |
|---|---|---:|---:|
| T01 | Khởi tạo và lập kế hoạch | 1 | 2 |
| T02 | Khảo sát yêu cầu | 3 | 5 |
| T03 | Thiết kế dữ liệu | 6 | 8 |
| T04 | Thiết kế giao diện | 6 | 8 |
| T05 | Module người dùng | 9 | 13 |
| T06 | Module hộ gia đình | 9 | 15 |
| T07 | Module thu phí | 14 | 21 |
| T08 | Tích hợp | 22 | 24 |
| T09 | Kiểm thử hệ thống | 25 | 29 |
| T10 | Sửa lỗi | 30 | 32 |
| T11 | Hoàn thiện tài liệu | 26 | 29 |
| T12 | Người dùng nghiệm thu | 33 | 34 |
| T13 | Triển khai | 35 | 36 |
| T14 | Đào tạo và bàn giao | 37 | 38 |

T15 là công việc quản lý thực hiện ngắt quãng trong 8 tuần, tổng cộng 8 ngày công. Cần dành thời gian cụ thể cho An và tránh trùng với thời gian An làm toàn thời gian ở T01, T14.

**4. Vì sao có việc làm song song?**

- T03 và T04 cùng bắt đầu ngày 6 vì đã có yêu cầu và do hai người khác nhau thực hiện.
- T05 và T06 cùng bắt đầu ngày 9 vì đã có thiết kế và không tranh chấp người thực hiện.
- T08 chờ cả T06 và T07 hoàn thành nên bắt đầu ngày 22.
- T11 có thể làm song song với kiểm thử vì Dũng phụ trách tài liệu, Bình phụ trách kiểm thử.

Công thức cho quan hệ “xong việc trước mới bắt đầu việc sau”:

**Ngày bắt đầu sớm nhất = Ngày kết thúc muộn nhất của các việc trước + 1.**

Sau đó phải kiểm tra thêm người phụ trách có rảnh không. Đủ đầu vào chưa chắc đã đủ nhân lực.

**5. Thao tác tạo Gantt trong Excel hoặc Google Sheets**

Tạo bảng:

| Cột | Nội dung |
|---|---|
| A | Mã nhiệm vụ |
| B | Tên nhiệm vụ |
| C | Người phụ trách |
| D | Ngày bắt đầu |
| E | Ngày kết thúc |
| F | Thời lượng |
| G trở đi | Các ngày 1 đến 40 |

Thực hiện lần lượt:

1. Nhập các nhiệm vụ T01–T14 từ hàng 2.
2. Nhập ngày bắt đầu và kết thúc theo bảng trên.
3. Tại F2, nhập `=E2-D2+1`, rồi kéo xuống.
4. Tại G1 nhập `1`, H1 nhập `2`, kéo dãy đến ngày `40`.
5. Chọn vùng lịch `G2:AT15`.
6. Mở **Định dạng có điều kiện / Conditional Formatting**.
7. Chọn dùng công thức và nhập:

```excel
=AND(G$1>=$D2,G$1<=$E2)
```

8. Chọn màu tô.

Nếu ứng dụng dùng dấu chấm phẩy để ngăn cách đối số, đổi dấu phẩy thành dấu chấm phẩy.

Kết quả: mỗi nhiệm vụ được tô màu từ ngày bắt đầu đến ngày kết thúc. T15 nên có hàng riêng, đánh dấu những ngày hoặc phần ngày quản lý đã được phân bổ; không tô 40 ngày rồi hiểu là 40 ngày công.

**6. Thêm các mốc kiểm soát**

| Mốc | Thời điểm | Bằng chứng hoàn thành |
|---|---|---|
| Chốt yêu cầu | Cuối ngày 5 | Danh sách yêu cầu được xác nhận |
| Hoàn thành tích hợp | Cuối ngày 24 | Các module chạy chung được |
| Hoàn thành nghiệm thu | Cuối ngày 34 | Kết quả và biên bản nghiệm thu |
| Hoàn thành bàn giao | Cuối ngày 38 | Hồ sơ bàn giao được xác nhận |

Ngày 39–40 là khoảng đệm của lịch mẫu. Khoảng đệm thời gian khác với khoản dự phòng tiền trong ngân sách.

**Sản phẩm hoàn thành khi:** mọi nhiệm vụ có vị trí trên lịch, quan hệ trước sau hợp lý và không có người bị giao vượt khả năng làm việc.

</details>

<details>
<summary>-sản phẩm 'Kế hoạch quản lý rủi ro: nhận diện trở ngại, ưu tiên và chuẩn bị cách xử lý'</summary>

**1. Hiểu sản phẩm này**

Rủi ro là điều **chưa chắc xảy ra**, nhưng nếu xảy ra sẽ ảnh hưởng đến dự án.

Ví dụ:

> Nếu kế toán cung cấp quy tắc tính phí muộn, thiết kế và lập trình module thu phí có thể bị chậm.

Câu này có đủ ba phần: **nguyên nhân → sự kiện có thể xảy ra → hậu quả**.

Nếu quy tắc đã bị cung cấp muộn, đó là vấn đề hiện tại cần xử lý, không còn chỉ là rủi ro.

**2. Chỉnh lại điểm chưa thống nhất trong tài liệu trước khi dùng**

Tài liệu có hai chỗ cần lưu ý:

- Bảng 4-1 có các giá trị khớp với cách nhân xác suất và tác động, chẳng hạn **2 × 2 = 4**.
- Ma trận trang 9 lại quy định **xác suất 2, tác động 2 → mức 3**.
- Cuối trang 8, hai mô tả cuối bị ghi lặp nhãn “Mức 4”, “Mức 5”; theo thứ tự giảm dần và ma trận trang 9, chúng cần được hiểu tương ứng là **mức 2**, **mức 1**.

Để làm bài mẫu nhất quán, ta **dùng ma trận trang 9**. Không lấy kết quả phép nhân rồi coi ngay đó là mức rủi ro của ma trận.

**3. Tạo bảng quy ước đánh giá**

**Xác suất** cho biết khả năng xảy ra:

| Điểm | Mức | Cách hiểu |
|---|---|---|
| 1 | Thấp | Hiếm xảy ra, ít dấu hiệu cho thấy sẽ xảy ra |
| 2 | Vừa | Có khả năng xảy ra, đã từng gặp hoặc có căn cứ hợp lý |
| 3 | Cao | Có nhiều dấu hiệu hoặc đã thường xuyên xảy ra |

**Tác động** cho biết hậu quả nếu xảy ra.

Tài liệu xem xét phạm vi, chất lượng và chi phí. Để dễ thực hành, có thể cụ thể hóa riêng tiêu chí chi phí như sau:

| Điểm | Mức | Tiêu chí chi phí minh họa |
|---|---|---|
| 1 | Thấp | Làm tăng chi phí dưới 5% |
| 2 | Vừa | Làm tăng chi phí từ 5% đến 10% |
| 3 | Cao | Làm tăng chi phí trên 10% |

Với ngân sách cơ sở 100 triệu đồng, tăng 7 triệu tương ứng 7%, nên thuộc tác động chi phí mức 2.

Một rủi ro có thể ảnh hưởng nhiều mặt. Trong bài mẫu, quy ước lấy **mức tác động cao nhất trong các mặt đã đánh giá**, đồng thời ghi rõ lý do. Đây là quy ước bổ sung để dùng bảng nhất quán.

**4. Tạo ma trận xác định mức rủi ro**

| Xác suất \ Tác động | Thấp — 1 | Vừa — 2 | Cao — 3 |
|---|---:|---:|---:|
| Thấp — 1 | Mức 1 | Mức 2 | Mức 3 |
| Vừa — 2 | Mức 2 | Mức 3 | Mức 4 |
| Cao — 3 | Mức 3 | Mức 4 | Mức 5 |

Với đúng ma trận này, có thể tính nhanh:

**Mức rủi ro = Điểm xác suất + Điểm tác động − 1.**

Đây là công thức tương đương **ma trận đang dùng**, không phải công thức bắt buộc cho mọi dự án.

Diễn giải các mức theo thứ tự nhất quán:

| Mức | Cách hiểu |
|---|---|
| 1 | Hầu như không ảnh hưởng hoặc ảnh hưởng không rõ ràng |
| 2 | Không ảnh hưởng đáng kể |
| 3 | Có ảnh hưởng nhưng dự án vẫn thực hiện được |
| 4 | Ảnh hưởng đáng kể; có thể khiến một số công việc không thực hiện được |
| 5 | Nghiêm trọng đến mức không thể tiếp tục theo điều kiện hiện tại |

**5. Tạo danh sách rủi ro**

Tạo bảng với các cột:

**Mã – Mô tả – Xác suất – Tác động – Mức rủi ro – Phòng ngừa – Người theo dõi.**

Các điểm dưới đây là đánh giá minh họa cho dự án mẫu, không phải kết quả phải sao chép từ tài liệu.

| Mã | Rủi ro | Xác suất | Tác động | Mức | Phòng ngừa | Theo dõi |
|---|---|---:|---:|---:|---|---|
| R01 | Thành viên bận dự án khác hoặc rời nhóm | 2 | 3 | 4 | Chia sẻ kiến thức, lưu tài liệu, chuẩn bị người tiếp nhận | An |
| R02 | Khách hàng thêm yêu cầu sau khi chốt | 2 | 2 | 3 | Xác nhận phạm vi, quy định cách tiếp nhận và duyệt thay đổi | An |
| R03 | Tài liệu kỹ thuật không theo kịp mã nguồn | 1 | 2 | 2 | Cập nhật tài liệu cùng phần việc, rà soát trước bàn giao | Chi |
| R04 | Trao đổi thiếu rõ ràng gây hiểu sai nghiệp vụ | 2 | 2 | 3 | Dùng ví dụ cụ thể, ghi lại quyết định, xác nhận với khách hàng | Bình |
| R05 | Công việc trước chậm làm công việc sau chậm | 2 | 3 | 4 | Theo dõi nhiệm vụ phụ thuộc và xử lý sớm dấu hiệu trễ | An |
| R06 | Vướng mắc hợp đồng làm dự án bị trì hoãn | 1 | 3 | 3 | Làm rõ điều khoản và trách nhiệm trước khi triển khai | An |
| R07 | Khách hàng từ chối nghiệm thu | 2 | 3 | 4 | Thống nhất tiêu chí, demo sớm, kiểm thử theo dữ liệu mẫu | Bình |
| R08 | Nguồn ngân sách bị cắt giảm | 1 | 3 | 3 | Xác nhận nguồn tiền, theo dõi chi phí và thứ tự ưu tiên | An |
| R09 | Ước lượng thời gian và chi phí quá lạc quan | 2 | 3 | 4 | Chia nhỏ nhiệm vụ, hỏi người thực hiện, so sánh việc tương tự | An |

**6. Bổ sung cách ứng phó khi rủi ro xảy ra**

“Phòng ngừa” và “ứng phó” là hai việc khác nhau:

- Phòng ngừa: làm trước để giảm khả năng hoặc hậu quả.
- Ứng phó: hành động khi xuất hiện dấu hiệu hoặc sự kiện đã xảy ra.

Ví dụ cho R02:

| Thuộc tính | Nội dung mẫu |
|---|---|
| Dấu hiệu kích hoạt | Khách hàng yêu cầu thêm chức năng ngoài danh sách đã duyệt |
| Hành động ngay | Ghi nhận yêu cầu, làm rõ nội dung và người đề xuất |
| Phân tích | Ước lượng công, chi phí, ảnh hưởng thiết kế và lịch |
| Quyết định cần có | Người có thẩm quyền chấp thuận thực hiện, đổi ưu tiên hoặc để giai đoạn sau |
| Cập nhật | Sửa phạm vi, nhiệm vụ, ngân sách và lịch sau khi được duyệt |
| Người chịu trách nhiệm | An |

Ví dụ cho R01:

> Nếu Chi nghỉ dài ngày, An xác định các nhiệm vụ bị ảnh hưởng, bố trí người tiếp nhận, sử dụng tài liệu đã chuẩn bị và cập nhật lịch theo năng lực thực tế.

**7. Cách sử dụng bảng trong quá trình làm**

Mỗi tuần, người quản lý cùng nhóm:

1. Kiểm tra rủi ro nào có dấu hiệu xảy ra.
2. Cập nhật xác suất và tác động nếu có thông tin mới.
3. Kiểm tra các biện pháp phòng ngừa đã thực hiện chưa.
4. Giao hành động và thời hạn xử lý cho rủi ro cần ưu tiên.
5. Bổ sung rủi ro mới; ghi trạng thái đã đóng hoặc đã chuyển thành vấn đề cần giải quyết.

**Sản phẩm hoàn thành khi:** nhóm biết các trở ngại chính, thứ tự ưu tiên, người theo dõi và hành động cần thực hiện.

</details>

**Cách nối các sản phẩm khi tự làm bài**

| Thứ tự | Dùng đầu vào nào? | Tạo ra kết quả gì? |
|---|---|---|
| 1 | Bối cảnh và nhu cầu khách hàng | Tuyên ngôn dự án |
| 2 | Phạm vi và mục tiêu | Danh mục bàn giao, tiêu chí nghiệm thu |
| 3 | Danh mục bàn giao | WBS bao quát toàn bộ công việc |
| 4 | Các phần việc trong WBS | Nhiệm vụ, người phụ trách và ước lượng |
| 5 | Nỗ lực và nguồn lực cần dùng | Ngân sách chi tiết |
| 6 | Nhiệm vụ, phụ thuộc và khả năng nhân sự | Lịch thực hiện, Gantt |
| 7 | Toàn bộ kế hoạch và các giả định | Kế hoạch quản lý rủi ro |

Đối chiếu với đề gốc: **Bài 4.1** lấy tuyên ngôn và danh mục bàn giao; **Bài 4.2** lấy WBS, bảng nhiệm vụ và Gantt; **Bài 4.3** lấy quy ước đánh giá cùng danh sách rủi ro. Bảng ngân sách giúp kiểm tra các phần này có khả thi và thống nhất với nhau hay không.
