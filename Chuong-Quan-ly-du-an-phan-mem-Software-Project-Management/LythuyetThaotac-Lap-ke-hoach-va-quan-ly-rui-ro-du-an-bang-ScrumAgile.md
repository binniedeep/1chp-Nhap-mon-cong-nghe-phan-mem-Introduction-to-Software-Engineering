-🔍LythuyetThaotac: **Xây dựng kế hoạch dự án phần mềm: Project Charter, WBS, Gantt Chart và quản lý rủi ro** — Tài liệu: **Huong dan xay dung Ke hoach du an(5).pdf**. Huong dan xay dung Ke hoach du an(5).pdf

**Giới thiệu bài toán mẫu để học cách thao tác**

Xuyên suốt các sản phẩm bên dưới, chúng ta sử dụng dự án **xây dựng phần mềm quản lý và thu phí chung cư Blue Moon**.

Ban quản trị đang dùng Excel để quản lý hộ gia đình và các khoản thu nên dễ bỏ sót khoản chưa đóng, khó tổng hợp số tiền đã thu. Dự án cần tạo phần mềm gồm ba module: **quản lý thu phí, quản lý người dùng và quản lý hộ gia đình**.

Quy ước cho ví dụ:

```text
Mã dự án: BM-2027
Tên dự án: Phần mềm quản lý và thu phí chung cư Blue Moon

Quy mô giả định:
- 300 hộ gia đình.
- Khoảng 1.000 nhân khẩu.
- 5 loại phí ban đầu.
- 3 vai trò sử dụng: quản trị viên, kế toán, cán bộ quản lý cư dân.

Ngân sách tối đa: 100.000.000 đồng.
Thời gian: 04/01/2027 đến 26/03/2027.

Nhóm thực hiện:
- Nam: quản lý dự án, phân tích yêu cầu.
- Huy: lập trình.
- Lan: lập trình.
- Mai: kiểm thử và hướng dẫn sử dụng.
```

**Tên người, số liệu và lịch trên là dữ liệu minh họa.** Lịch thực hành tính từ thứ Hai đến thứ Sáu, chưa trừ ngày lễ, Tết; khi lập kế hoạch thật phải cập nhật lịch nghỉ.

Tài liệu gốc hướng dẫn ba nội dung chính: tuyên ngôn dự án, WBS/lịch Gantt và quản lý rủi ro. Tôi tách thành **năm sản phẩm để dễ thao tác**; các trường bổ sung nhằm giúp bạn biến nội dung hướng dẫn thành một kế hoạch có thể sử dụng.

<details>
<summary>-sản phẩm 'Tuyên ngôn dự án — Project Charter'</summary>

Tuyên ngôn dự án là tài liệu chính thức xác nhận dự án được triển khai, xác định các cam kết ban đầu và trao quyền cho người quản lý dự án. Theo tài liệu, nhà tài trợ là bên ban hành tài liệu này; nhóm dự án có thể hỗ trợ soạn thảo.

**Đầu vào cần chuẩn bị:** vấn đề của khách hàng, nhu cầu sử dụng, nguồn kinh phí, nhân sự dự kiến, thời hạn và những điều kiện phải tuân thủ.

**Cách tạo:** mở Word hoặc công cụ soạn thảo, tạo các mục dưới đây, trao đổi với các bên để điền thông tin rồi trình phê duyệt.

- **'Tên dự án':** tên nhận diện công việc mà tổ chức quyết định thực hiện — Chọn tên thể hiện hành động, sản phẩm và nơi áp dụng; dùng thống nhất tên này trong WBS, lịch trình và bảng rủi ro.

  ```text
  Xây dựng phần mềm quản lý và thu phí chung cư Blue Moon.
  ```

- **'Nhà tài trợ dự án':** cá nhân bảo trợ dự án, có thẩm quyền hỗ trợ nguồn lực và quyết định những vấn đề vượt quyền quản lý dự án — Lấy từ quyết định giao nhiệm vụ hoặc thỏa thuận với đơn vị đầu tư.

  ```text
  Nhà tài trợ: ông Minh, đại diện được Ban quản trị giao quyền bảo trợ dự án.

  Trách nhiệm:
  - Phê duyệt tuyên ngôn dự án.
  - Quyết định các thay đổi vượt thẩm quyền quản lý dự án.
  - Hỗ trợ giải quyết trở ngại về nguồn lực.
  ```

- **'Cơ quan tài trợ':** tổ chức cấp hoặc chịu trách nhiệm về kinh phí — Điền tên tổ chức từ thỏa thuận đầu tư; phân biệt tổ chức này với cá nhân nhà tài trợ.

  ```text
  Cơ quan tài trợ: Ban quản trị chung cư Blue Moon.
  Ngân sách được phê duyệt: tối đa 100.000.000 đồng.
  ```

- **'Mức độ ảnh hưởng của dự án':** phạm vi hoạt động và nhóm người chịu tác động khi sản phẩm được đưa vào sử dụng — Xác định bộ phận nào đổi cách làm việc, dữ liệu nào được chuyển sang quản lý bằng phần mềm.

  ```text
  Phần mềm sử dụng nội bộ tại chung cư Blue Moon.

  Ảnh hưởng:
  - Kế toán chuyển từ theo dõi thu phí bằng Excel sang phần mềm.
  - Cán bộ cư dân cập nhật thông tin hộ gia đình trên phần mềm.
  - Ban quản trị xem báo cáo thu phí tập trung.
  ```

- **'Người quản lý dự án':** người chịu trách nhiệm điều phối thực hiện và theo dõi mục tiêu dự án — Điền họ tên, đơn vị, thông tin liên hệ và quyền hạn được giao.

  ```text
  Họ tên: Nam.
  Nơi công tác: Nhóm phát triển BM-2027.
  Email minh họa: nam@example.com.
  Điện thoại: bổ sung số liên hệ công việc.

  Quyền hạn:
  - Phân công công việc cho nhóm.
  - Điều chỉnh phân công trong ngân sách và thời hạn đã duyệt.
  - Trình nhà tài trợ khi cần thay đổi phạm vi hoặc tăng ngân sách.
  ```

- **'Thành viên dự án':** những người trực tiếp thực hiện công việc — Chọn theo năng lực cần có, sau đó ghi thông tin liên hệ, vai trò và khả năng tham gia.

  ```text
  Huy:
  - Vai trò: lập trình module thu phí, tích hợp.
  - Email minh họa: huy@example.com.

  Lan:
  - Vai trò: lập trình module người dùng và hộ gia đình.
  - Email minh họa: lan@example.com.

  Mai:
  - Vai trò: kiểm thử, tài liệu hướng dẫn sử dụng.
  - Email minh họa: mai@example.com.

  Điện thoại và mức độ tham gia:
  - Bổ sung theo xác nhận thực tế của từng thành viên.
  ```

- **'Các bên liên quan và trách nhiệm':** cá nhân hoặc đơn vị có thể ảnh hưởng đến dự án hoặc chịu ảnh hưởng từ dự án — Xác định ai cung cấp yêu cầu, ai sử dụng, ai nghiệm thu và ai hỗ trợ triển khai.

  ```text
  Đại diện khách hàng: ông Cường, trưởng Ban quản trị.
  - Xác nhận phạm vi nghiệp vụ.
  - Đại diện khách hàng nghiệm thu theo thẩm quyền được giao.

  Đại diện người dùng: bà An, kế toán.
  - Cung cấp quy tắc thu phí.
  - Thử nghiệm chức năng và phản hồi kết quả.

  Bộ phận kỹ thuật tòa nhà:
  - Cung cấp máy tính và quyền cài đặt.
  - Phối hợp triển khai.
  ```

- **'Bối cảnh và động cơ':** tình trạng hiện tại và nguyên nhân khiến dự án cần được thực hiện — Lấy thông tin từ phỏng vấn, quan sát quy trình và kiểm tra các biểu mẫu đang sử dụng.

  ```text
  Ban quản trị đang quản lý 300 hộ gia đình bằng nhiều tệp Excel.

  Vấn đề:
  - Thông tin hộ gia đình bị nhập lặp.
  - Khó xác định hộ chưa hoàn thành nghĩa vụ đóng phí.
  - Kế toán phải tổng hợp báo cáo thủ công.

  Động cơ:
  - Tập trung dữ liệu và giảm thao tác tổng hợp.
  ```

- **'Mục đích dự án':** nhu cầu nghiệp vụ lớn mà dự án hướng đến giải quyết — Viết dựa trên vấn đề ở phần bối cảnh; mô tả lợi ích cần đạt trước khi liệt kê chức năng.

  ```text
  Hỗ trợ Ban quản trị quản lý tập trung hộ gia đình, nhân khẩu
  và các khoản thu; giúp kế toán theo dõi tình trạng đóng phí
  và lập báo cáo theo kỳ.
  ```

- **'Mục tiêu đo lường được':** kết quả cụ thể dùng để đánh giá dự án có đạt yêu cầu hay không — Chọn chỉ tiêu có số lượng, điều kiện kiểm tra và thời hạn; xác nhận với khách hàng trước khi đưa vào cam kết.

  ```text
  MT01: Trước 19/03/2027, phần mềm hỗ trợ đầy đủ 5 loại phí
        trong danh mục đã được khách hàng xác nhận.

  MT02: Phần mềm lưu và tra cứu được bộ dữ liệu kiểm thử gồm
        300 hộ gia đình và 1.000 nhân khẩu.

  MT03: Báo cáo tổng tiền đã thu và chưa thu khớp với kết quả
        đối chiếu của bộ dữ liệu nghiệm thu.

  MT04: Hoàn thành toàn bộ 30 tình huống nghiệm thu đã thống nhất,
        không còn lỗi được các bên phân loại là nghiêm trọng.

  MT05: Hoàn thành bàn giao trước hoặc trong ngày 26/03/2027,
        tổng chi phí không vượt 100.000.000 đồng.
  ```

  Khi dùng những từ như “100%”, phải chỉ rõ **100% của danh mục hoặc tập yêu cầu nào**.

- **'Sản phẩm bàn giao':** các đầu ra khách hàng hoặc chủ đầu tư sẽ nhận — Lấy từ hợp đồng, phạm vi và yêu cầu nghiệm thu; ghi tên cụ thể để sau này đưa vào WBS.

  ```text
  Bàn giao cho khách hàng:
  - Bộ cài phần mềm.
  - Hướng dẫn cài đặt.
  - Hướng dẫn sử dụng.
  - Hồ sơ quyền sử dụng phần mềm theo thỏa thuận.
  - Biên bản nghiệm thu và bàn giao.

  Bàn giao cho đơn vị sở hữu mã nguồn theo thỏa thuận:
  - Mã nguồn.
  - Tài liệu đặc tả yêu cầu.
  - Tài liệu phân tích và thiết kế.
  - Tài liệu kiểm thử.
  - Tài liệu cấu trúc mã nguồn.
  - Tài liệu API nếu có API.
  - Hồ sơ quản lý dự án.
  ```

- **'Phạm vi công việc của dự án':** những hoạt động nhóm cam kết thực hiện và những hoạt động nằm ngoài cam kết — Lấy từ danh sách bàn giao, điều kiện triển khai và thỏa thuận trách nhiệm.

  ```text
  Bao gồm:
  - Khảo sát và đặc tả yêu cầu.
  - Phân tích, thiết kế.
  - Lập trình, tích hợp, kiểm thử.
  - Cài đặt và hướng dẫn sử dụng.
  - Soạn tài liệu và bàn giao.

  Không bao gồm:
  - Nhập toàn bộ dữ liệu cư dân thật thay khách hàng.
  - Mua máy tính mới.
  - Vận hành và bảo trì dài hạn sau khi kết thúc hợp đồng.

  Dữ liệu kiểm thử do nhóm tạo để kiểm tra phần mềm
  không đồng nghĩa với việc nhận nhập dữ liệu thật.
  ```

- **'Phạm vi sản phẩm':** chức năng mà phần mềm sẽ cung cấp — Chọn từ các nhu cầu đã được xác nhận; nhóm thành module để tiếp tục phân rã WBS.

  ```text
  Module 1: Quản lý thu phí.
  - Tạo và cập nhật khoản thu.
  - Ghi nhận đóng phí.
  - Thống kê đã thu, chưa thu.

  Module 2: Quản lý người dùng.
  - Tạo và khóa tài khoản.
  - Đăng nhập, đăng xuất.
  - Phân quyền.

  Module 3: Quản lý hộ gia đình.
  - Thêm, sửa, tra cứu hộ gia đình.
  - Quản lý nhân khẩu thuộc hộ.
  - Ghi nhận thay đổi thông tin.

  Ngoài phạm vi phiên bản này:
  - Ứng dụng di động.
  - Thanh toán ngân hàng trực tuyến.
  ```

- **'Ngân sách':** giới hạn tiền dùng cho dự án và cách dự kiến phân bổ — Ước tính từ khối lượng công việc, nguồn lực, chi phí triển khai và dự phòng; kiểm tra tổng không vượt mức được cấp.

  ```text
  Phát triển phần mềm:               60.000.000 đồng
  Kiểm thử và nghiệm thu:            15.000.000 đồng
  Quản lý dự án:                     10.000.000 đồng
  Tài liệu, triển khai, hướng dẫn:    10.000.000 đồng
  Dự phòng:                          5.000.000 đồng

  Tổng:                            100.000.000 đồng

  Nguyên tắc:
  - Dự phòng đã nằm trong tổng ngân sách.
  - Khi sử dụng dự phòng phải cập nhật số tiền còn lại.
  ```

- **'Lịch trình và các mốc chính':** các thời điểm cam kết ở mức tổng quát — Chọn theo thời hạn khách hàng yêu cầu và khả năng thực hiện; lịch Gantt phía sau phải đáp ứng những mốc này.

  ```text
  Bắt đầu:                         04/01/2027
  Hoàn thành yêu cầu:               08/01/2027
  Hoàn thành thiết kế:              15/01/2027
  Hoàn thành tích hợp:              12/02/2027
  Hoàn thành nghiệm thu thử:        05/03/2027
  Hoàn thành nghiệm thu chính thức: 19/03/2027
  Hoàn thành bàn giao:              26/03/2027
  ```

- **'Rủi ro sơ bộ':** các sự kiện chưa chắc xảy ra nhưng có thể ảnh hưởng mục tiêu — Chọn những rủi ro lớn có thể nhận biết ngay lúc khởi tạo; sau đó phát triển thành bảng quản lý rủi ro.

  ```text
  R01: Khách hàng bổ sung quy tắc thu phí sau khi chốt yêu cầu.
  R02: Một lập trình viên không thể tiếp tục tham gia.
  R03: Khách hàng chậm phản hồi khi nghiệm thu.
  R04: Phần mềm cài đặt không thành công trên máy đích.
  ```

- **'Giả định':** điều nhóm tạm xem là đúng để lập kế hoạch nhưng vẫn cần kiểm chứng — Chọn những điều kiện ảnh hưởng đến ước tính; mỗi giả định quan trọng cần có người xác nhận.

  ```text
  GD01: Khách hàng cung cấp biểu mẫu thu phí trước 06/01/2027.
  GD02: Huy và Lan tham gia theo mức nguồn lực đã thống nhất.
  GD03: Người dùng tham gia thử nghiệm trong tuần 01–05/03/2027.
  GD04: Phạm vi ban đầu được xác nhận trước khi lập trình.

  Nếu có yêu cầu thay đổi:
  - Đánh giá lại thời gian, chi phí và phạm vi trước khi duyệt.
  ```

- **'Ràng buộc':** giới hạn bắt buộc phải tuân thủ — Lấy từ ngân sách, hợp đồng, chính sách tổ chức và điều kiện kỹ thuật đã xác nhận.

  ```text
  RB01: Tổng chi phí không vượt 100.000.000 đồng.
  RB02: Hoàn thành bàn giao chậm nhất ngày 26/03/2027.
  RB03: Nhóm thực hiện ban đầu gồm 4 người.
  RB04: Phần mềm phải chạy trên cấu hình máy đích
        được hai bên xác nhận trong giai đoạn yêu cầu.
  ```

- **'Yếu tố phụ thuộc bên ngoài':** điều kiện do bên ngoài nhóm kiểm soát nhưng cần có để nhóm thực hiện công việc — Xác định bên cung cấp, nội dung cần cung cấp và thời điểm cần nhận.

  ```text
  PT01:
  - Cần: danh mục phí và cách tính.
  - Bên cung cấp: kế toán chung cư.
  - Hạn cần nhận: 06/01/2027.

  PT02:
  - Cần: máy tính đích và quyền cài đặt.
  - Bên cung cấp: bộ phận kỹ thuật tòa nhà.
  - Hạn cần nhận: trước đợt kiểm tra triển khai.

  PT03:
  - Cần: đại diện khách hàng tham gia nghiệm thu.
  - Bên cung cấp: Ban quản trị.
  - Thời điểm: theo lịch nghiệm thu đã thống nhất.
  ```

- **'Chiến lược truyền thông':** quy định ai trao đổi với ai, bằng kênh nào, khi nào và về nội dung gì — Chọn theo nhu cầu phối hợp và ra quyết định của từng bên.

  ```text
  Họp nhóm:
  - Đầu giờ mỗi ngày làm việc.
  - Nội dung: việc đã làm, việc sắp làm, trở ngại.

  Báo cáo tiến độ:
  - Nam gửi nhà tài trợ vào chiều thứ Sáu.
  - Kênh: email.
  - Nội dung: tiến độ, chi phí, rủi ro, quyết định cần xử lý.

  Đánh giá theo mốc:
  - Có khách hàng và nhóm dự án.
  - Lập biên bản xác nhận kết quả, việc còn lại và người xử lý.
  ```

- **'Phê duyệt':** thông tin xác nhận các bên có thẩm quyền đã chấp thuận tuyên ngôn — Điền đúng người ký và ngày ký thực tế; để trống chữ ký khi tài liệu mới là bản nháp.

  ```text
  Nhà tài trợ:
  - Họ tên: Minh.
  - Chữ ký: chưa ký.
  - Ngày: chưa xác nhận.

  Đại diện cơ quan tài trợ:
  - Họ tên: bổ sung người có thẩm quyền.
  - Chữ ký: chưa ký.
  - Ngày: chưa xác nhận.

  Người quản lý dự án:
  - Họ tên: Nam.
  - Chữ ký: chưa ký.
  - Ngày: chưa xác nhận.
  ```

- **'Ghi chú':** thông tin làm rõ cách hiểu hoặc nội dung chưa được chốt — Chỉ ghi điều có ích cho người đọc; nội dung ảnh hưởng cam kết phải được cập nhật vào mục chính tương ứng.

  ```text
  - Các thông tin trong bản học tập là dữ liệu giả định.
  - Cấu hình máy đích cần xác nhận khi khảo sát.
  - Thời gian bảo trì sau bàn giao cần thỏa thuận riêng.
  ```

**Mối liên hệ trong sản phẩm:** bối cảnh giải thích vì sao cần dự án; mục đích xác định nhu cầu; mục tiêu đưa ra cách đánh giá; phạm vi và sản phẩm bàn giao xác định việc cần làm; ngân sách, lịch trình và ràng buộc giới hạn cách thực hiện.

</details>

<details>
<summary>-sản phẩm 'Cấu trúc phân cấp công việc theo sản phẩm bàn giao — Deliverable-based WBS'</summary>

WBS theo sản phẩm bàn giao phân rã kết quả lớn thành các kết quả nhỏ hơn để có thể giao việc và kiểm soát hoàn thành.

Tài liệu minh họa phần mềm ở mức 0, các module ở mức 1 và các tính năng ở các mức tiếp theo. Khi lập WBS cho **toàn bộ dự án**, bạn còn cần bao quát tài liệu, triển khai và quản lý dự án trong phạm vi đã cam kết.

**Đầu vào cần chuẩn bị:** phạm vi sản phẩm, phạm vi công việc, danh sách bàn giao và tiêu chí nghiệm thu trong tuyên ngôn.

- **'Tên nút gốc':** tên đối tượng bao trùm toàn bộ WBS — Chọn rõ đang phân rã riêng phần mềm hay toàn bộ dự án để áp dụng quy tắc 100% đúng phạm vi.

  ```text
  Mã: 0
  Tên: Dự án phần mềm quản lý và thu phí chung cư Blue Moon.

  Phạm vi WBS này:
  - Toàn bộ công việc của dự án đã được phê duyệt.
  ```

- **'Mã WBS':** mã định danh thể hiện vị trí một phần tử trong cấu trúc — Đặt mã theo cấp cha–con; dùng mã này để nối công việc với lịch trình và rủi ro.

  ```text
  1       Module quản lý thu phí
  1.1     Chức năng tạo và cập nhật khoản thu
  1.2     Chức năng ghi nhận đóng phí
  1.3     Báo cáo đã thu và chưa thu
  ```

- **'Tên sản phẩm hoặc thành phần':** tên đầu ra mà phần tử WBS cần tạo — Lấy từ danh sách bàn giao và các chức năng đã xác nhận; ưu tiên tên thể hiện kết quả cụ thể.

  ```text
  Mã: 1.2
  Tên: Chức năng ghi nhận đóng phí.

  Đầu ra:
  - Giao diện ghi nhận đóng phí.
  - Dữ liệu giao dịch được lưu.
  - Kết quả cập nhật vào báo cáo thu phí.
  ```

- **'Cấp phân rã và phần tử cha':** vị trí của thành phần trong hệ thống lớn hơn — Xác định thành phần đó thuộc sản phẩm nào; tránh đặt một chức năng vào nhiều nhánh rồi tính công việc hai lần.

  ```text
  Phần tử: 1.2 — Chức năng ghi nhận đóng phí.
  Cấp: 2.
  Phần tử cha: 1 — Module quản lý thu phí.

  Khi 1.1, 1.2 và 1.3 đều hoàn thành,
  module 1 mới đáp ứng đầy đủ phạm vi đã phân rã.
  ```

- **'Gói công việc':** phần tử ở mức thấp nhất được quản lý trong WBS — Tiếp tục chia nhỏ đến khi có thể ước tính, giao người chịu trách nhiệm và kiểm tra kết quả. Gói công việc vẫn có thể chứa nhiều hoạt động thực hiện.

  ```text
  Mã gói: 1.2
  Tên gói: Chức năng ghi nhận đóng phí.
  Người chịu trách nhiệm: Huy.

  Phạm vi:
  - Chọn hộ gia đình.
  - Chọn khoản thu.
  - Nhập số tiền và ngày đóng.
  - Lưu giao dịch.
  - Cập nhật kết quả thống kê.

  Không thuộc gói:
  - Tích hợp thanh toán ngân hàng.
  ```

- **'Tiêu chí hoàn thành':** điều kiện dùng để kết luận đầu ra của gói công việc đã đạt — Lấy từ yêu cầu được duyệt và tình huống kiểm thử; viết sao cho có thể quan sát hoặc đối chiếu.

  ```text
  Gói 1.2 hoàn thành khi:
  - Lưu được giao dịch có dữ liệu hợp lệ.
  - Từ chối số tiền bằng 0 hoặc âm theo quy tắc đã duyệt.
  - Giao dịch liên kết đúng hộ và khoản thu.
  - Người không có quyền không thực hiện được thao tác.
  - Báo cáo phản ánh đúng số tiền vừa ghi nhận.
  - Các tình huống kiểm thử của gói được thực hiện đạt.
  ```

- **'Cấu trúc WBS đầy đủ và quy tắc 100%':** danh sách phân cấp bao quát toàn bộ phạm vi đã chọn — Đối chiếu từng sản phẩm bàn giao với WBS; tổng các phần tử con phải bao quát phần tử cha và tránh chồng lặp.

  ```text
  0. Dự án phần mềm Blue Moon

      1. Module quản lý thu phí
          1.1. Chức năng tạo và cập nhật khoản thu
          1.2. Chức năng ghi nhận đóng phí
          1.3. Báo cáo đã thu và chưa thu

      2. Module quản lý người dùng
          2.1. Chức năng tạo và khóa tài khoản
          2.2. Chức năng đăng nhập, đăng xuất
          2.3. Chức năng phân quyền

      3. Module quản lý hộ gia đình
          3.1. Chức năng quản lý thông tin hộ
          3.2. Chức năng quản lý nhân khẩu
          3.3. Chức năng ghi nhận thay đổi thông tin

      4. Bộ tài liệu
          4.1. Đặc tả yêu cầu
          4.2. Phân tích và thiết kế
          4.3. Tài liệu và kết quả kiểm thử
          4.4. Hướng dẫn cài đặt, sử dụng
          4.5. Tài liệu cấu trúc mã nguồn và API nếu có

      5. Bộ sản phẩm phát hành và bàn giao
          5.1. Bộ cài đã tích hợp và kiểm tra
          5.2. Mã nguồn phiên bản bàn giao
          5.3. Hồ sơ quyền sử dụng theo thỏa thuận
          5.4. Kết quả hướng dẫn người dùng
          5.5. Biên bản nghiệm thu, bàn giao

      6. Hồ sơ quản lý dự án
          6.1. Kế hoạch dự án được duyệt
          6.2. Báo cáo theo dõi và kiểm soát
          6.3. Hồ sơ thay đổi và quyết định
          6.4. Báo cáo kết thúc dự án
  ```

  Trong cấu trúc này, việc lập trình và kiểm tra chức năng nằm trong các gói module; nhánh 5.1 bao gồm phần tích hợp, đóng gói và kiểm tra ở mức toàn hệ thống. Khi chi tiết hóa, cần ghi rõ ranh giới để tránh tính trùng.

**Mối liên hệ với sản phẩm trước:** tuyên ngôn xác định cần bàn giao những gì; WBS biến danh sách đó thành các phần có thể giao việc. Nếu thêm “ứng dụng di động” vào WBS, bạn phải xử lý thay đổi phạm vi vì tuyên ngôn hiện tại chưa bao gồm sản phẩm này.

</details>

<details>
<summary>-sản phẩm 'Cấu trúc phân cấp công việc theo quy trình — Process-based WBS'</summary>

WBS theo quy trình tổ chức công việc theo các pha hoặc cách vận hành dự án. Tài liệu đưa ra minh họa theo **Waterfall** và **Scrum**.

Đây là **cách nhìn khác của cùng một phạm vi**. Khi lập kế hoạch chính thức, chọn cấu trúc phù hợp; nếu giữ nhiều cách nhìn thì phải có ánh xạ để tránh cộng trùng khối lượng.

**Đầu vào cần chuẩn bị:** tuyên ngôn, danh sách bàn giao, yêu cầu nghiệp vụ và quy trình phát triển được lựa chọn.

- **'Quy trình phát triển được chọn':** cách tổ chức quá trình tạo phần mềm — Chọn dựa trên độ rõ của yêu cầu, khả năng khách hàng phản hồi và cách nhóm làm việc; ghi lý do để người đọc hiểu cấu trúc WBS.

  ```text
  Quy trình dùng trong kế hoạch mẫu: Waterfall.

  Lý do giả định:
  - Ba module chính đã được xác định.
  - Khách hàng có thể xác nhận quy tắc thu phí từ đầu.
  - Bài học cần thể hiện rõ yêu cầu → thiết kế → lập trình → kiểm thử.

  Thay đổi phát sinh vẫn phải được đánh giá và phê duyệt.
  ```

- **'Các pha hoặc nhóm công việc cấp cao':** các nhóm hoạt động lớn bao quát quá trình triển khai — Lấy từ quy trình đã chọn và phạm vi công việc; bổ sung quản lý, tài liệu, triển khai nếu chúng nằm trong cam kết.

  ```text
  0. Dự án Blue Moon
      1. Quản lý dự án
      2. Khảo sát và đặc tả yêu cầu
      3. Phân tích và thiết kế
      4. Phát triển phần mềm
      5. Tích hợp, kiểm thử và nghiệm thu
      6. Triển khai, hướng dẫn và bàn giao
  ```

- **'Công việc con':** những phần việc cần thực hiện để hoàn thành một pha — Phân rã từ đầu ra của pha; chỉ dừng khi công việc đủ rõ để ước tính và kiểm tra.

  ```text
  3. Phân tích và thiết kế
      3.1. Thiết kế chức năng
      3.2. Thiết kế giao diện
      3.3. Thiết kế dữ liệu
          3.3.1. Dữ liệu thu phí
          3.3.2. Dữ liệu người dùng
          3.3.3. Dữ liệu hộ gia đình
      3.4. Thiết kế phân quyền
      3.5. Rà soát và hoàn thiện thiết kế
  ```

- **'Đầu ra của công việc':** kết quả phải có sau khi thực hiện hoạt động — Chọn đầu ra chứng minh được công việc đã hoàn thành; ánh xạ với sản phẩm bàn giao hoặc gói WBS tương ứng.

  ```text
  Công việc: 3.3.1 — Thiết kế dữ liệu thu phí.

  Đầu vào:
  - Quy tắc thu phí đã xác nhận.
  - Các biểu mẫu khách hàng cung cấp.

  Đầu ra:
  - Mô hình dữ liệu thu phí.
  - Mô tả trường dữ liệu và quan hệ.
  - Quy tắc kiểm tra dữ liệu.

  Liên kết:
  - Là một phần của tài liệu phân tích và thiết kế.
  - Hỗ trợ phát triển module quản lý thu phí.
  ```

- **'Người phụ trách và tiêu chí hoàn thành':** người điều phối kết quả và điều kiện để chuyển sang bước tiếp theo — Chọn theo chuyên môn, đồng thời xác định người rà soát để tránh tự kết luận hoàn thành.

  ```text
  Công việc: 3.3.1 — Thiết kế dữ liệu thu phí.
  Người thực hiện: Huy.
  Người rà soát: Lan và Nam.

  Hoàn thành khi:
  - Dữ liệu hỗ trợ đủ 5 loại phí đã xác nhận.
  - Có quan hệ giữa hộ gia đình, khoản thu và giao dịch.
  - Các nhận xét rà soát đã được xử lý.
  - Thiết kế được xác nhận để lập trình.
  ```

- **'Hoạt động chi tiết để thực hiện gói công việc':** các bước nhỏ dùng để tạo đầu ra — Lấy một gói WBS rồi liệt kê việc thực hiện, người làm và thời lượng; đây là dữ liệu chuyển sang lịch Gantt.

  ```text
  Gói bàn giao liên quan:
  1.2 — Chức năng ghi nhận đóng phí.

  Các hoạt động chi tiết:
  T03.01: Làm rõ xử lý chi tiết của chức năng — Huy — 1 ngày.
  T03.02: Hoàn thiện giao diện nhập giao dịch — Huy — 1 ngày.
  T03.03: Lập trình xử lý và lưu giao dịch — Huy — 3 ngày.
  T03.04: Kiểm tra chức năng và xử lý lỗi — Huy — 1 ngày.

  Tổng thời lượng tuần tự dự kiến: 6 ngày làm việc.

  Trong kế hoạch tổng:
  - Nhóm hoạt động này thuộc T03 — Phát triển module thu phí.
  - T03 còn bao gồm chức năng khoản thu và báo cáo.
  ```

- **'Cách tổ chức nếu chọn Scrum':** cấu trúc công việc theo các đợt phát triển và kết quả tăng thêm — Nếu chọn Scrum, lấy danh sách yêu cầu ưu tiên làm đầu vào, xác định mục tiêu từng Sprint và điều kiện hoàn thành.

  ```text
  Ví dụ cùng dự án Blue Moon nếu tổ chức theo Scrum:

  0. Dự án Blue Moon
      1. Quản lý dự án và phối hợp khách hàng
      2. Phát triển phần mềm qua các Sprint
          2.1. Quản lý yêu cầu và ưu tiên Product Backlog
          2.2. Sprint 1
              Mục tiêu: có tài khoản và dữ liệu hộ gia đình cơ bản
          2.3. Sprint 2
              Mục tiêu: tạo khoản thu và ghi nhận đóng phí
          2.4. Sprint 3
              Mục tiêu: báo cáo, hoàn thiện và tích hợp
      3. Hướng dẫn, triển khai và bàn giao

  Mỗi Sprint bao gồm:
  - Lập kế hoạch Sprint.
  - Phân tích, thiết kế, lập trình, kiểm thử phần được chọn.
  - Review kết quả và Retrospective.

  Đây là phương án tổ chức thay thế.
  Lịch minh họa ở sản phẩm tiếp theo sử dụng phương án Waterfall.
  ```

**Mối liên hệ giữa hai WBS:** WBS theo sản phẩm trả lời “cần tạo đầu ra nào”; WBS theo quy trình trả lời “tổ chức những công việc nào để tạo các đầu ra đó”. Một chức năng có thể được thực hiện qua nhiều pha, nên mã công việc và mã sản phẩm cần được phân biệt.

</details>

<details>
<summary>-sản phẩm 'Danh sách công việc và lịch trình dự án — Gantt Chart'</summary>

Lịch Gantt biểu diễn công việc theo thời gian, giúp theo dõi thời điểm bắt đầu, kết thúc, thời lượng và quan hệ phụ thuộc.

WBS là đầu vào của lịch trình. **Vị trí trên cây WBS không tự quyết định thứ tự thực hiện**: hai công việc ở hai nhánh khác nhau vẫn có thể làm song song.

**Đầu vào cần chuẩn bị:** các gói WBS, danh sách hoạt động, nguồn lực, ước tính thời lượng, quan hệ phụ thuộc và mốc cam kết.

Các trường dưới đây là hướng dẫn triển khai thêm; PDF nêu nội dung WBS/Gantt nhưng không cung cấp đầy đủ mẫu trường chi tiết.

- **'Mã công việc và liên kết WBS':** mã duy nhất của hoạt động và mã phạm vi mà hoạt động phục vụ — Tạo mã công việc riêng rồi liên kết đến WBS để truy ngược lý do phải thực hiện.

  ```text
  Mã công việc: T03.
  Tên: Phát triển module quản lý thu phí.

  WBS liên quan:
  - 1.1. Chức năng tạo và cập nhật khoản thu.
  - 1.2. Chức năng ghi nhận đóng phí.
  - 1.3. Báo cáo đã thu và chưa thu.

  T03 là dòng tổng hợp;
  có thể mở rộng thành T03.01, T03.02... để theo dõi chi tiết.
  ```

- **'Tên công việc':** mô tả hành động cần thực hiện — Lấy từ hoạt động đã phân rã, dùng động từ và đối tượng rõ ràng để người được giao hiểu cần làm gì.

  ```text
  T01: Khảo sát và xác nhận yêu cầu.
  T02: Phân tích và thiết kế.
  T03: Phát triển module quản lý thu phí.

  Tránh đặt tên quá chung:
  - Làm phần mềm.
  - Xử lý công việc.
  ```

- **'Người thực hiện và mức phân bổ':** nguồn lực được giao cho công việc và phần năng lực sử dụng — Chọn theo chuyên môn, lịch rảnh và khối lượng đang có; kiểm tra tổng phân bổ của một người trên các công việc song song.

  ```text
  Công việc: T03.
  Người thực hiện chính: Huy.
  Phân bổ trực tiếp: trung bình 80% thời gian làm việc.

  Phần thời gian còn lại:
  - Trao đổi nhóm.
  - Đóng góp tài liệu.
  - Hỗ trợ rà soát.

  Khi nhiều công việc chạy đồng thời:
  - Tổng phân bổ của Huy không được vượt khả năng đã cam kết.
  ```

- **'Lịch làm việc':** quy tắc xác định ngày nào được tính là ngày thực hiện — Điền ngày làm trong tuần, số giờ mỗi ngày và các ngày nghỉ trước khi tính lịch kết thúc.

  ```text
  Lịch thực hành:
  - Thứ Hai đến thứ Sáu.
  - 8 giờ/ngày.
  - Thứ Bảy, Chủ nhật nghỉ.
  - Chưa đưa ngày lễ, Tết vào phép tính.

  Lịch dùng cho dự án thật:
  - Cập nhật ngày nghỉ và lịch vắng của thành viên.
  - Tính lại các ngày kết thúc bị ảnh hưởng.
  ```

- **'Thời lượng — Duration':** khoảng thời gian làm việc cần để hoàn thành hoạt động — Ước tính từ khối lượng, năng lực và mức phân bổ; ghi rõ đơn vị ngày làm việc.

  ```text
  Công việc: T03.
  Thời lượng: 10 ngày làm việc.

  Bắt đầu: 18/01/2027.
  Kết thúc: 29/01/2027.

  Khoảng này gồm hai tuần lịch,
  tương ứng 10 ngày làm việc theo lịch thực hành.
  ```

- **'Khối lượng lao động — Effort':** tổng lượng lao động cần bỏ ra, thường đo bằng giờ công hoặc ngày công — Ước tính riêng với thời lượng; một công việc kéo dài 10 ngày không có nghĩa mọi người tham gia đều làm đủ 10 ngày công.

  ```text
  Công việc: T03.
  Thời lượng: 10 ngày làm việc.
  Khối lượng trực tiếp dự kiến của Huy: 8 ngày công.

  Nếu phân bổ đều:
  - 8 ngày công / 10 ngày = 80% thời gian của Huy.

  Cần cộng riêng công sức của người khác nếu có.
  ```

- **'Công việc tiền nhiệm và loại phụ thuộc':** công việc hoặc điều kiện cần hoàn thành trước khi công việc khác được thực hiện — Chọn theo logic kỹ thuật và nghiệp vụ; quan hệ phổ biến là Finish-to-Start, tức việc trước xong thì việc sau mới bắt đầu.

  ```text
  T02:
  - Tiền nhiệm: T01.
  - Quan hệ: Finish-to-Start.

  T06:
  - Tiền nhiệm: T03, T04, T05.
  - Quan hệ: Finish-to-Start.

  Ý nghĩa:
  - T06 chỉ bắt đầu khi các module cần tích hợp đã hoàn thành.
  ```

- **'Ngày bắt đầu và ngày kết thúc':** khoảng thời gian dự kiến thực hiện — Tính từ thời lượng, lịch làm việc, tiền nhiệm và khả năng nguồn lực; không chỉ nhập ngày theo mong muốn.

  ```text
  T04 — Phát triển module người dùng:
  - Người thực hiện: Lan.
  - Bắt đầu: 18/01/2027.
  - Kết thúc: 22/01/2027.

  T05 — Phát triển module hộ gia đình:
  - Người thực hiện: Lan.
  - Bắt đầu: 25/01/2027.
  - Kết thúc: 05/02/2027.

  Hai công việc được bố trí tuần tự để phù hợp nguồn lực của Lan.
  ```

- **'Mốc — Milestone':** sự kiện đánh dấu một kết quả quan trọng, thường có thời lượng bằng 0 — Chọn các điểm phê duyệt, hoàn thành pha hoặc bàn giao; phân biệt thời gian thực hiện hoạt động với thời điểm xác nhận kết quả.

  ```text
  Hoạt động:
  T08 — Thực hiện nghiệm thu thử.
  Thời gian: 01/03/2027 đến 05/03/2027.

  Mốc:
  M03 — Hoàn thành nghiệm thu thử.
  Ngày: 05/03/2027.
  Thời lượng: 0 ngày.
  ```

- **'Kết quả đầu ra và điều kiện hoàn thành':** bằng chứng để công nhận công việc đã xong — Lấy từ tiêu chí gói WBS và yêu cầu chất lượng; tránh cập nhật hoàn thành chỉ vì đã hết thời gian dự kiến.

  ```text
  T07 — Kiểm thử hệ thống.

  Đầu ra:
  - Kết quả chạy bộ kiểm thử.
  - Danh sách lỗi.
  - Báo cáo kiểm thử.

  Điều kiện hoàn thành:
  - Các tình huống trong phạm vi T07 đã được thực hiện.
  - Lỗi được ghi nhận và phân loại.
  - Không còn lỗi nghiêm trọng ngăn cản bắt đầu nghiệm thu thử.
  ```

- **'Tiến độ thực tế':** thông tin phản ánh công việc đã thực hiện đến thời điểm cập nhật — Ghi ngày thực tế, phần đã hoàn thành và phần còn lại; xác định cách tính phần trăm trước khi sử dụng.

  ```text
  Công việc: T03.
  Ngày cập nhật: 22/01/2027.

  Trạng thái: đang thực hiện.
  Bắt đầu thực tế: 18/01/2027.

  Ước tính theo khối lượng các phần việc:
  - Đã hoàn thành: 40%.
  - Còn lại: 60%.

  Dự báo kết thúc: 29/01/2027.
  Căn cứ: kết quả các hoạt động chi tiết và phần việc còn lại.
  ```

- **'Lịch trình tổng hợp':** tập hợp các công việc, nguồn lực và quan hệ phụ thuộc — Điền từ các trường trên; rà soát xem lịch có bao phủ toàn bộ phạm vi và đáp ứng các mốc trong tuyên ngôn.

  ```text
  Ngày bắt đầu dự án: 04/01/2027.
  Ngày kết thúc dự kiến: 26/03/2027.

  Các dòng dưới đây là kế hoạch tổng hợp.
  Khi theo dõi chi tiết, mở rộng các dòng phát triển
  thành hoạt động tương ứng với từng gói WBS.
  ```

| Mã | Công việc | Người phụ trách | Bắt đầu | Kết thúc | Ngày làm việc | Tiền nhiệm |
|---|---|---|---|---|---:|---|
| T01 | Khảo sát, xác nhận yêu cầu | Nam | 04/01 | 08/01 | 5 | — |
| T02 | Phân tích, thiết kế | Nam | 11/01 | 15/01 | 5 | T01 |
| T03 | Phát triển module thu phí | Huy | 18/01 | 29/01 | 10 | T02 |
| T04 | Phát triển module người dùng | Lan | 18/01 | 22/01 | 5 | T02 |
| T05 | Phát triển module hộ gia đình | Lan | 25/01 | 05/02 | 10 | T04 |
| T06 | Tích hợp các module | Huy | 08/02 | 12/02 | 5 | T03, T05 |
| T07 | Kiểm thử hệ thống | Mai | 15/02 | 26/02 | 10 | T06 |
| T08 | Nghiệm thu thử với khách hàng | Mai | 01/03 | 05/03 | 5 | T07 |
| T09 | Sửa lỗi, hoàn thiện phiên bản | Huy | 08/03 | 12/03 | 5 | T08 |
| T10 | Nghiệm thu chính thức | Nam | 15/03 | 19/03 | 5 | T09 |
| T11 | Triển khai, hướng dẫn, bàn giao | Nam | 22/03 | 26/03 | 5 | T10 |
| T12 | Soạn và cập nhật tài liệu | Mai | 11/01 | 26/03 | 55 | T01 |
| T13 | Quản lý và kiểm soát dự án | Nam | 04/01 | 26/03 | 60 | — |

Tất cả ngày trong bảng thuộc năm **2027**. “Người phụ trách” có thể phối hợp với thành viên khác; ví dụ Huy và Lan cùng xử lý lỗi module mình phụ trách trong T09.

T12 và T13 là hoạt động xuyên suốt, thực hiện theo từng phần thời gian. **55 và 60 ngày là khoảng thời gian hoạt động, không phải 55 và 60 ngày công toàn thời gian.** Tài liệu cần cho từng pha phải có hạn riêng; hồ sơ bàn giao cần hoàn tất trước mốc kết thúc T11.

- **'Cách biểu diễn trên Gantt':** hình thức hiển thị khoảng thời gian và quan hệ công việc — Trong công cụ quản lý dự án, nhập công việc, thời lượng, nguồn lực và tiền nhiệm; mỗi hoạt động được thể hiện bằng thanh thời gian, mỗi mốc bằng ký hiệu mốc.

  ```text
  T03 và T04:
  - Cùng bắt đầu ngày 18/01.
  - Có thể làm song song vì Huy và Lan phụ trách khác nhau.

  T04 và T05:
  - Thực hiện tuần tự.
  - Tránh bố trí Lan làm toàn thời gian cho hai việc cùng lúc.

  T06:
  - Nằm sau thời điểm hoàn thành các module cần tích hợp.

  Mốc bàn giao:
  - Đặt tại ngày 26/03/2027.
  ```

**Mối liên hệ với các sản phẩm trước:** WBS giúp tránh bỏ sót việc; lịch trình xác định khi nào làm và ai làm. Nếu lịch dự kiến vượt ngày 26/03 hoặc nguồn lực bị quá tải, cần điều chỉnh kế hoạch và xử lý các cam kết liên quan.

</details>

<details>
<summary>-sản phẩm 'Kế hoạch quản lý rủi ro và bảng theo dõi rủi ro'</summary>

Kế hoạch quản lý rủi ro xác định các sự kiện có thể ảnh hưởng dự án, cách đánh giá mức độ và cách chuẩn bị ứng phó.

**Đầu vào cần chuẩn bị:** mục tiêu, giả định, ràng buộc, WBS, lịch trình, ngân sách và thông tin từ các bên liên quan.

**Lưu ý khi sử dụng tài liệu:** bảng trang 7 dùng các điểm như 2 và 4 theo cách phù hợp với phép nhân xác suất × tác động; ma trận trang 9 lại quy định **năm mức**, trong đó xác suất 2 và tác động 2 cho **mức 3**. Trang 8 còn lặp nhãn mức 4 và mức 5 ở hai dòng cuối. Ví dụ dưới đây **thống nhất dùng ma trận trang 9**, với mức 1 thấp nhất và mức 5 cao nhất.

- **'Mã hoặc STT rủi ro':** định danh dùng để theo dõi một rủi ro xuyên suốt dự án — Đặt mã duy nhất và giữ nguyên khi cập nhật thông tin.

  ```text
  Mã: R01.
  STT: 1.
  Tên ngắn: Thay đổi yêu cầu thu phí.
  ```

- **'Mô tả rủi ro':** diễn đạt sự kiện chưa chắc xảy ra và hậu quả nếu xảy ra — Lấy từ giả định chưa được kiểm chứng, điểm yếu của kế hoạch hoặc phụ thuộc bên ngoài; viết rõ nguyên nhân, sự kiện và ảnh hưởng.

  ```text
  Do các quy tắc thu phí chưa được rà soát đầy đủ,
  khách hàng có thể bổ sung cách tính mới sau khi lập trình bắt đầu,
  khiến nhóm phải sửa dữ liệu và xử lý thu phí,
  làm tăng chi phí và chậm kiểm thử.
  ```

- **'Phạm vi hoặc công việc bị ảnh hưởng':** mục tiêu, sản phẩm hoặc hoạt động chịu tác động — Đối chiếu rủi ro với mã WBS và mã công việc trong lịch trình.

  ```text
  Rủi ro: R01.

  WBS bị ảnh hưởng:
  - 1.1. Chức năng tạo và cập nhật khoản thu.
  - 1.2. Chức năng ghi nhận đóng phí.
  - 1.3. Báo cáo đã thu và chưa thu.

  Công việc bị ảnh hưởng:
  - T03. Phát triển module thu phí.
  - T07. Kiểm thử hệ thống.
  ```

- **'Xác suất':** đánh giá khả năng xảy ra của rủi ro — Chọn theo dữ liệu quá khứ, tình hình hiện tại và dấu hiệu cụ thể; tài liệu sử dụng ba mức định tính, không quy định tỷ lệ phần trăm.

  ```text
  Thấp (1):
  - Rất hiếm xảy ra hoặc ít có cơ sở cho rằng sẽ xảy ra.

  Vừa (2):
  - Có khả năng xảy ra và có căn cứ hợp lý.

  Cao (3):
  - Có dấu hiệu rõ hoặc từng xảy ra thường xuyên.

  R01:
  - Xác suất: Vừa (2).
  - Căn cứ: khách hàng còn một số quy tắc thu phí chưa thống nhất.
  ```

- **'Tác động':** mức ảnh hưởng đến mục tiêu nếu rủi ro xảy ra — Ước lượng ảnh hưởng đến phạm vi, chất lượng và chi phí; ghi căn cứ thay vì chỉ chọn nhãn.

  ```text
  Thang tham khảo từ tài liệu:

  Thấp (1):
  - Dưới 5% phạm vi hoặc chi phí bị ảnh hưởng.

  Vừa (2):
  - Khoảng 5% đến 10% phạm vi hoặc chi phí bị ảnh hưởng.

  Cao (3):
  - Trên 10% phạm vi hoặc chi phí bị ảnh hưởng.
  - Hoặc chất lượng giảm đến mức không thể chấp nhận.

  R01:
  - Chi phí phát sinh ước tính: 8.000.000 đồng.
  - So với ngân sách 100.000.000 đồng: 8%.
  - Tác động theo chi phí: Vừa (2).
  ```

  Nếu các khía cạnh có mức khác nhau, cần thống nhất quy tắc tổng hợp. Trong ví dụ này, nhóm chọn mức cao nhất trong các khía cạnh đã đánh giá để ưu tiên xử lý.

- **'Mức độ rủi ro':** kết quả kết hợp xác suất và tác động — Tra đúng ma trận đã chọn; không thay bằng phép nhân khi đang dùng hệ năm mức của trang 9.

  ```text
  R01:
  - Xác suất P = 2.
  - Tác động I = 2.
  - Tra ma trận: mức 3.

  Công thức tương đương riêng với ma trận này:
  Mức = P + I - 1
       = 2 + 2 - 1
       = 3.
  ```

| Xác suất \ Tác động | Thấp — 1 | Vừa — 2 | Cao — 3 |
|---|---:|---:|---:|
| Thấp — 1 | Mức 1 | Mức 2 | Mức 3 |
| Vừa — 2 | Mức 2 | Mức 3 | Mức 4 |
| Cao — 3 | Mức 3 | Mức 4 | Mức 5 |

- **'Hành động ngăn ngừa':** việc làm trước nhằm giảm khả năng xảy ra hoặc giảm hậu quả — Chọn hành động xử lý đúng nguyên nhân; chuyển thành công việc có người phụ trách và thời hạn.

  ```text
  R01 — Thay đổi yêu cầu thu phí.

  Ngăn ngừa:
  - Thu đủ biểu mẫu và quy tắc thu phí.
  - Dùng ví dụ cụ thể để khách hàng kiểm tra cách tính.
  - Xác nhận danh mục yêu cầu trước khi lập trình.
  - Thống nhất quy trình đề nghị và phê duyệt thay đổi.

  Người thực hiện: Nam.
  Hạn hoàn thành chính: trước khi T03 bắt đầu.
  ```

- **'Phương án ứng phó khi xảy ra':** việc thực hiện khi sự kiện rủi ro đã trở thành thực tế — Chọn phương án phù hợp giới hạn ngân sách, thời hạn và quyền quyết định.

  ```text
  Nếu khách hàng đề nghị thêm cách tính phí:

  1. Ghi nhận yêu cầu thay đổi.
  2. Xác định chức năng và tài liệu bị ảnh hưởng.
  3. Ước tính lại công việc, chi phí và thời gian.
  4. Trình người có thẩm quyền quyết định.
  5. Nếu được duyệt, cập nhật phạm vi, WBS và lịch trình.

  Không tự đưa yêu cầu mới vào kế hoạch đã cam kết.
  ```

- **'Người phụ trách rủi ro':** người theo dõi diễn biến và bảo đảm biện pháp ứng phó được thực hiện — Chọn người có khả năng quan sát và điều phối; có thể phân công người thực hiện hành động khác.

  ```text
  R01:
  - Người phụ trách rủi ro: Nam.
  - Người đánh giá tác động kỹ thuật: Huy.
  - Người xác nhận nghiệp vụ: đại diện kế toán khách hàng.
  - Người phê duyệt thay đổi vượt thẩm quyền: nhà tài trợ.
  ```

- **'Dấu hiệu kích hoạt':** thông tin cho thấy rủi ro đang đến gần hoặc cần bắt đầu ứng phó — Chọn dấu hiệu quan sát được, gắn với mốc trong lịch trình.

  ```text
  R01:
  - Sau ngày 08/01/2027 vẫn còn quy tắc thu phí chưa xác nhận.
  - Khách hàng gửi thêm công thức tính phí ngoài danh mục đã duyệt.

  Khi xuất hiện:
  - Nam tổ chức đánh giá ảnh hưởng.
  - Cập nhật bảng rủi ro và hồ sơ thay đổi.
  ```

- **'Trạng thái và thời điểm rà soát':** tình hình hiện tại của rủi ro cùng lịch cập nhật — Ghi rõ rủi ro đang theo dõi, đã xảy ra hay đã đóng; đánh giá lại sau khi thực hiện biện pháp.

  ```text
  R01:
  - Trạng thái: đang theo dõi.
  - Rà soát: mỗi thứ Sáu và khi có yêu cầu mới.
  - Ngày cập nhật minh họa: 08/01/2027.

  Sau khi xác nhận yêu cầu:
  - Xác suất được đánh giá lại từ 2 xuống 1.
  - Tác động giữ ở mức 2.
  - Mức rủi ro còn lại: 1 + 2 - 1 = 2.

  Việc giảm điểm cần có căn cứ, không thực hiện tự động.
  ```

- **'Dự phòng liên quan':** phần tiền, thời gian hoặc nguồn lực được chuẩn bị để xử lý bất định — Lấy từ ngân sách và kế hoạch đã duyệt; kiểm tra dự phòng có đủ so với phương án ứng phó hay không.

  ```text
  Dự phòng tiền toàn dự án: 5.000.000 đồng.

  R01 có thể làm phát sinh: 8.000.000 đồng.

  Đánh giá:
  - Dự phòng hiện tại không đủ cho toàn bộ tác động ước tính.
  - Cần giảm ảnh hưởng, điều chỉnh phạm vi hoặc trình phương án khác.
  - Không mặc định được vượt ngân sách 100.000.000 đồng.
  ```

- **'Bảng rủi ro tổng hợp':** danh sách giúp nhóm so sánh và ưu tiên xử lý — Mỗi dòng là một rủi ro; dùng chung thang đo và ghi rõ hành động cụ thể.

  ```text
  Quy tắc sử dụng:
  - Chấm P và I theo thang 1–3.
  - Tra mức rủi ro theo ma trận năm mức.
  - Ưu tiên xem xét rủi ro có mức cao.
  - Với các rủi ro cùng mức, xét thêm thời điểm có thể xảy ra
    và mức độ cấp bách của hành động.
  ```

| Mã | Rủi ro trong dự án Blue Moon | P | I | Mức | Hành động chính | Phụ trách |
|---|---|---:|---:|---:|---|---|
| R01 | Bổ sung quy tắc thu phí sau khi chốt yêu cầu | 2 | 2 | 3 | Xác nhận quy tắc, kiểm soát thay đổi | Nam |
| R02 | Một lập trình viên không thể tiếp tục tham gia | 2 | 3 | 4 | Chia sẻ mã nguồn, rà soát chéo, chuẩn bị phân công lại | Nam |
| R03 | Khách hàng chậm tham gia nghiệm thu | 2 | 2 | 3 | Xác nhận lịch và người đại diện trước T08 | Nam |
| R04 | Bộ cài không hoạt động trên máy đích | 2 | 3 | 4 | Xác nhận cấu hình, kiểm tra cài đặt sớm | Huy |
| R05 | Tài liệu không theo kịp thay đổi mã nguồn | 2 | 2 | 3 | Cập nhật tài liệu cùng từng phần bàn giao | Mai |
| R06 | Ước tính thời gian hoặc chi phí quá lạc quan | 2 | 3 | 4 | Chia nhỏ việc, rà soát ước tính, cập nhật phần còn lại | Nam |
| R07 | Các thành viên hiểu khác nhau về yêu cầu | 2 | 2 | 3 | Dùng tình huống mẫu, ghi quyết định và rà soát chung | Nam |
| R08 | Một công việc tiền nhiệm bị chậm | 2 | 2 | 3 | Theo dõi phụ thuộc, điều chỉnh nguồn lực và lịch | Nam |
| R09 | Khách hàng từ chối nghiệm thu | 1 | 3 | 3 | Thống nhất tiêu chí, cho dùng thử, lưu kết quả đối chiếu | Nam |

Các điểm trong bảng là **ước lượng minh họa cho dự án mẫu**, cần đánh giá lại khi có dữ liệu thực tế.

**Mối liên hệ xuyên suốt qua một tình huống**

```text
Tình huống:
Khách hàng đề nghị thêm thanh toán ngân hàng trực tuyến
sau khi nhóm bắt đầu lập trình.

Tuyên ngôn:
- Chức năng này đang nằm ngoài phạm vi.

WBS:
- Chưa có gói công việc tạo và kiểm tra tích hợp ngân hàng.

Lịch Gantt:
- Chưa bố trí thời gian và nguồn lực cho chức năng mới.

Bảng rủi ro:
- R01 có dấu hiệu xảy ra.
- Nam khởi động quy trình đánh giá thay đổi.

Nếu yêu cầu được phê duyệt:
- Cập nhật phạm vi và danh sách bàn giao.
- Thêm các gói WBS cần thiết.
- Ước tính nguồn lực, chi phí và thời gian.
- Cập nhật lịch, ngân sách và tiêu chí nghiệm thu.
- Đánh giá thêm các rủi ro mới của việc tích hợp.
```

</details>
