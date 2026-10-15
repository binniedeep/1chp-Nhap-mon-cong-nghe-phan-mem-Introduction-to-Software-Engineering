🔍**LythuyetThaotac: Lập kế hoạch dự án phần mềm — xây dựng tuyên ngôn dự án, phân rã công việc WBS, lập biểu đồ Gantt và quản lý rủi ro.**

**Bài toán mẫu:** Xây dựng phần mềm quản lý và thu phí tại chung cư Blue Moon, gồm ba module: quản lý thu phí, quản lý người dùng và quản lý hộ gia đình. Từ nhu cầu ban đầu, cần xác định dự án sẽ bàn giao những gì, thực hiện những công việc nào, ai phụ trách, hoàn thành khi nào và xử lý rủi ro ra sao.

**Tư liệu hướng dẫn:** Huong dan xay dung Ke hoach du an(3).pdf

**Tên file/đường dẫn đã gửi:** `/workspace/scratch/a5f4fb08ff28/upload/Huong dan xay dung Ke hoach du an(3).pdf`

**Công cụ thực hành gợi ý:** Word để soạn tuyên ngôn; Excel để lập danh mục công việc, phân công và theo dõi rủi ro; phần mềm lập tiến độ có hỗ trợ quan hệ phụ thuộc để xây dựng Gantt. Tài liệu không bắt buộc một phần mềm cụ thể.

Trong nội dung dưới đây, **dataset là toàn bộ dữ liệu đầu vào cần chuẩn bị**, bao gồm yêu cầu, danh sách chức năng, nhân sự, thời gian, chi phí và các điều kiện thực hiện. Những ví dụ được bổ sung để hướng dẫn thao tác sẽ được ghi rõ là minh họa.

<details>
<summary>-sản phẩm 'Tuyên ngôn dự án — xác lập mục tiêu, phạm vi, nguồn lực và thẩm quyền thực hiện'</summary>

**1. Cơ sở lý thuyết của sản phẩm**

**Tuyên ngôn dự án — Project Charter** là tài liệu chính thức cho phép dự án được triển khai và trao quyền cho người quản lý dự án sử dụng các nguồn lực đã được chấp thuận.

Sản phẩm này trả lời các câu hỏi nền tảng: Vì sao cần làm dự án? Dự án tạo ra kết quả gì? Ai tham gia? Giới hạn thực hiện đến đâu? Ai có quyền phê duyệt?

Cần phân biệt các nội dung sau:

| Nội dung | Ý nghĩa | Ví dụ trong bài toán Blue Moon |
|---|---|---|
| Bối cảnh | Tình trạng dẫn đến nhu cầu thực hiện dự án | Đang quản lý thu phí thủ công, có sử dụng Excel nhưng hiệu quả chưa cao |
| Mục đích | Nhu cầu nghiệp vụ cần giải quyết | Hỗ trợ quản lý thu phí và thông tin hộ dân |
| Mục tiêu | Kết quả có thể kiểm tra, đo lường | Quản lý đầy đủ các loại phí và thông tin hộ gia đình thuộc phạm vi đã thống nhất |
| Phạm vi dự án | Những công việc dự án phải thực hiện | Đặc tả yêu cầu, phân tích, thiết kế, lập trình, kiểm thử và triển khai |
| Phạm vi sản phẩm | Chức năng và đặc điểm phần mềm phải có | Ba module quản lý thu phí, người dùng và hộ gia đình |
| Sản phẩm bàn giao | Những đầu mục phải chuyển giao | Bộ cài, mã nguồn, hướng dẫn, tài liệu kỹ thuật và tài liệu dự án |
| Ràng buộc | Giới hạn bắt buộc phải tuân thủ | Ngân sách, thời hạn, nguồn lực |
| Giả định | Điều được tạm coi là đúng để lập kế hoạch | Khách hàng tham gia dùng thử và phản hồi |
| Phụ thuộc bên ngoài | Điều kiện do bên ngoài nhóm dự án cung cấp | Khách hàng cung cấp quy tắc thu phí và xác nhận yêu cầu |

**Mục tiêu phải có căn cứ đánh giá.** Cụm “quản lý 100% các loại phí” trong tài liệu chỉ kiểm chứng được khi đã có danh sách các loại phí được xác nhận. Nếu danh sách chưa chốt, nhóm chưa thể kết luận đã đáp ứng 100%.

**Phạm vi cần ghi rõ phần loại trừ.** Trong bài mẫu, dự án không bao gồm nhập dữ liệu ban đầu về nhân khẩu, hộ khẩu và các loại phí. Điều này cần được phân biệt với việc lập trình chức năng nhập dữ liệu: phần mềm vẫn có thể cần chức năng đó, còn công việc nhập toàn bộ dữ liệu thật do bên khác thực hiện.

**2. Dataset — dữ liệu cần chuẩn bị**

| Nhóm dữ liệu | Nội dung cần có |
|---|---|
| Nhận diện dự án | Tên dự án, đơn vị tài trợ, người tài trợ, người quản lý |
| Hiện trạng nghiệp vụ | Cách quản lý hiện tại, khó khăn, biểu mẫu và báo cáo đang sử dụng |
| Các bên liên quan | Đại diện khách hàng, người dùng cuối, nhóm phát triển và người phê duyệt |
| Nhu cầu | Các vấn đề cần giải quyết và kết quả mong muốn |
| Danh mục chức năng | Các chức năng thuộc từng module |
| Danh mục bàn giao | Phần mềm, mã nguồn, tài liệu, hướng dẫn và các đầu mục khác |
| Nguồn lực | Thành viên, năng lực, thời gian tham gia, thiết bị |
| Giới hạn | Ngân sách, thời hạn, môi trường triển khai |
| Điều kiện nghiệm thu | Ai nghiệm thu, kiểm tra bằng cách nào, tiêu chí đạt |
| Thông tin phối hợp | Tần suất họp, báo cáo, kênh liên lạc và thời gian phản hồi |

Các dữ liệu có sẵn trong tài liệu gồm ngân sách **100.000.000 đồng**, thời gian thực hiện trong **quý IV/2023**, bàn giao thử nghiệm **30/11/2023**, bàn giao chính thức **15/12/2023** và hoàn thành **30/12/2023**.

Đây là các mốc của bài mẫu. Khi áp dụng cho dự án khác, phải thay bằng dữ liệu thực tế.

**3. Các bước thực hiện phương pháp hoàn thiện sản phẩm và nhận xét kết quả**

**Bước 1 — Tạo tài liệu theo cấu trúc mẫu.**

Trong Word, tạo các phần: thông tin chung; đội ngũ thực hiện; các bên liên quan; tuyên bố phạm vi; chiến lược truyền thông; phê duyệt; ghi chú.

Trong phần tuyên bố phạm vi, bố trí đủ bối cảnh, mục đích, mục tiêu, bàn giao, phạm vi, ngân sách, lịch trình, rủi ro, giả định, ràng buộc và phụ thuộc bên ngoài.

**Bước 2 — Viết hiện trạng và nhu cầu.**

Mô tả vấn đề đang xảy ra bằng thông tin quan sát hoặc được khách hàng xác nhận. Ví dụ: việc tổng hợp các khoản chưa đóng mất nhiều thời gian vì thông tin đang nằm trên nhiều bảng tính.

Không đưa một con số như “mất ba ngày tổng hợp” vào tài liệu nếu chưa có dữ liệu xác minh.

**Bước 3 — Chuyển nhu cầu thành mục tiêu kiểm tra được.**

Ví dụ minh họa:

> Phần mềm cho phép kế toán tra cứu các khoản phải thu, đã thu và còn thiếu của từng hộ theo kỳ thu; số liệu phải đối chiếu đúng với bộ tình huống nghiệm thu đã được khách hàng xác nhận.

Cách viết này cho biết cả hành vi mong muốn lẫn căn cứ kiểm tra.

**Bước 4 — Chốt phạm vi và sản phẩm bàn giao.**

Lập bảng gồm: đầu mục, mô tả, bên nhận và điều kiện chấp nhận.

Ví dụ, “bộ cài phần mềm” cần làm rõ môi trường Windows được hỗ trợ và cách kiểm tra cài đặt thành công. “Tài liệu hướng dẫn” cần xác định hướng dẫn cho nhóm người dùng nào.

**Bước 5 — Bổ sung nguồn lực, ngân sách và mốc thời gian.**

Điền nhân sự thực tế; xác định người quản lý và người phê duyệt. Ngân sách phải bao gồm cả khoản dự phòng theo yêu cầu của bài mẫu.

**Bước 6 — Thiết lập cách phối hợp.**

Theo tài liệu: báo cáo tiến độ hằng tuần; họp nhanh đầu ngày; đánh giá tại các mốc với khách hàng, nhà tài trợ và nhóm thực hiện.

Để áp dụng được, bổ sung người gửi báo cáo, người nhận, nội dung cần báo cáo và cách lưu quyết định.

**Bước 7 — Rà soát và phê duyệt.**

Kiểm tra sự thống nhất giữa mục tiêu, phạm vi, nguồn lực và lịch trình. Những thông tin chưa xác nhận phải được đánh dấu, kèm người chịu trách nhiệm làm rõ.

**Nhận xét kết quả:** Tuyên ngôn hoàn thiện khi các bên hiểu thống nhất về mục tiêu, phạm vi, bàn giao và quyền hạn. Một văn bản đủ biểu mẫu nhưng còn để trống người phê duyệt hoặc tiêu chí nghiệm thu chưa phải căn cứ triển khai đầy đủ.

</details>

<details>
<summary>-sản phẩm 'WBS theo sản phẩm bàn giao — phân rã phần mềm thành module, tính năng và gói công việc'</summary>

**1. Cơ sở lý thuyết của sản phẩm**

**WBS — Work Breakdown Structure** là cấu trúc phân cấp dùng để phân rã phạm vi công việc thành những phần nhỏ hơn, có thể ước lượng, giao trách nhiệm và kiểm tra hoàn thành.

Theo hướng sản phẩm bàn giao, câu hỏi chính là: **Cần tạo ra những thành phần và kết quả nào để hoàn thành sản phẩm?**

Tài liệu minh họa cấu trúc:

- Mức 0: phần mềm Blue Moon.
- Mức 1: các module.
- Mức tiếp theo: các tính năng.
- Các tính năng trở thành gói công việc; nếu quá lớn thì tiếp tục phân rã.

**Gói công việc — Work Package** là đơn vị thấp nhất trong WBS mà nhóm lựa chọn để quản lý. Một gói cần có kết quả rõ ràng, người chịu trách nhiệm và căn cứ xác nhận đã hoàn thành.

Ví dụ, gói “Tạo khoản thu” có thể cần các hoạt động làm rõ quy tắc nghiệp vụ, thiết kế, lập trình và kiểm thử. Nếu giao trọn gói chưa khả thi, cần tiếp tục phân chia.

**Quy tắc 100%:** Tổng phạm vi các phần con phải bao phủ đầy đủ phạm vi của phần cha. Đồng thời, tránh tính trùng cùng một công việc ở nhiều nhánh.

Cần xác định rõ đang lập **WBS của phần mềm** hay **WBS của toàn bộ dự án**. Cây chỉ có các tính năng phần mềm chưa bao phủ những đầu mục khác như tài liệu, triển khai và quản lý dự án.

**2. Dataset — dữ liệu cần chuẩn bị**

| Dữ liệu | Vai trò |
|---|---|
| Tuyên ngôn đã thống nhất | Xác định giới hạn phạm vi |
| Danh sách module | Tạo các nhánh cấp cao |
| Danh sách chức năng | Phân rã từng module |
| Danh sách bàn giao | Tránh bỏ sót tài liệu, bộ cài và các đầu mục khác |
| Mô tả nghiệp vụ | Xác định một tính năng cần tạo ra kết quả gì |
| Tiêu chí chấp nhận | Xác định lúc nào gói công việc hoàn thành |
| Năng lực nhóm | Quyết định mức phân rã phù hợp |

Ví dụ, để phân rã gói “Thu phí”, cần biết thu theo hộ hay theo căn hộ, có cho phép đóng từng phần không, xử lý điều chỉnh thế nào và cần lưu chứng từ gì. Đây là những câu hỏi cần khảo sát, không phải các yêu cầu đã được tài liệu xác nhận.

**3. Các bước thực hiện phương pháp hoàn thiện sản phẩm và nhận xét kết quả**

**Bước 1 — Đặt tên nút gốc và giới hạn cây.**

Nếu thực hiện đúng ví dụ phân rã phần mềm trong tài liệu, dùng nút gốc “Phần mềm quản lý và thu phí chung cư Blue Moon”.

**Bước 2 — Tạo ba nhánh module.**

| Mã WBS | Thành phần |
|---|---|
| 1 | Quản lý thu phí |
| 2 | Quản lý người dùng |
| 3 | Quản lý hộ gia đình |

**Bước 3 — Phân rã theo chức năng.**

Các tính năng được nêu trực tiếp trong hình minh họa của tài liệu gồm:

| Mã WBS | Tính năng |
|---|---|
| 1.1 | Tạo khoản thu |
| 1.2 | Thu phí |
| 1.3 | Thống kê các khoản đóng góp |
| 2.1 | Đăng ký tài khoản |

Các phần còn lại trong hình được để dấu “…”. Vì vậy, phải bổ sung từ danh sách yêu cầu đã khảo sát; không coi hình minh họa là danh mục chức năng đầy đủ.

Ví dụ bổ sung để thực hành: quản lý vai trò người dùng, cập nhật thông tin hộ và ghi nhận biến động nhân khẩu. Các chức năng này cần được xác nhận trước khi đưa vào phạm vi chính thức.

**Bước 4 — Viết mô tả cho từng gói công việc.**

Tạo bảng “Từ điển WBS” trong Excel hoặc Word:

| Thuộc tính | Ví dụ minh họa |
|---|---|
| Mã | 1.1 |
| Tên gói | Tạo khoản thu |
| Kết quả | Chức năng tạo và lưu khoản thu theo quy tắc đã xác nhận |
| Đầu vào | Mô tả nghiệp vụ, dữ liệu mẫu, thiết kế liên quan |
| Người chịu trách nhiệm | Thành viên được phân công |
| Điều kiện hoàn thành | Đáp ứng yêu cầu và vượt qua các trường hợp kiểm thử liên quan |
| Ngoài phạm vi | Không bao gồm nhập toàn bộ khoản thu thật ban đầu |

**Bước 5 — Kiểm tra mức phân rã.**

Nếu chưa thể ước lượng hoặc giao trách nhiệm rõ ràng, tiếp tục chia nhỏ. Nếu các mục quá vụn và không tạo thêm giá trị quản lý, có thể gộp lại.

Không có một số tầng cố định phù hợp với mọi dự án.

**Bước 6 — Đối chiếu quy tắc 100%.**

Kiểm tra từng nhánh: hoàn thành toàn bộ các phần con đã đủ để phần cha hoàn thành chưa?

Nếu đang lập WBS toàn dự án, bổ sung các nhánh bàn giao tài liệu, triển khai, nghiệm thu và quản lý dự án theo phạm vi đã chốt.

**Nhận xét kết quả:** WBS đạt yêu cầu khi mỗi yêu cầu và đầu mục bàn giao đều có chỗ tương ứng; các gói không chồng chéo; từng gói có thể được ước lượng và nghiệm thu. WBS thể hiện cấu trúc phạm vi, chưa thể hiện đầy đủ thứ tự thực hiện hay lịch bắt đầu, kết thúc.

</details>

<details>
<summary>-sản phẩm 'WBS theo quy trình — tổ chức công việc theo các pha Waterfall hoặc các phân đoạn Scrum'</summary>

**1. Cơ sở lý thuyết của sản phẩm**

WBS theo quy trình phân rã công việc theo **cách tổ chức thực hiện dự án**.

Tài liệu đưa ra hai cách minh họa:

| Cách tổ chức | Hướng phân rã trong tài liệu | Điều cần kiểm tra |
|---|---|---|
| Theo quy trình Waterfall | Các nhóm công việc lớn → phân tích, thiết kế, cài đặt, kiểm thử → công việc chi tiết | Mỗi pha có đầu vào, đầu ra và điều kiện hoàn thành |
| Theo quy trình Scrum | Các nhóm công việc → module → thiết lập yêu cầu, lập kế hoạch phân đoạn, phát triển, vận hành | Mỗi phân đoạn tạo ra kết quả có thể kiểm tra và lấy phản hồi |

**Waterfall** tổ chức các hoạt động theo những pha được xác định. Khi lập kế hoạch, cần làm rõ điều kiện chuyển pha và cách xử lý khi đầu vào thay đổi.

**Scrum** tổ chức phát triển theo các vòng lặp có thời lượng cố định gọi là Sprint. Phạm vi công việc của mỗi Sprint được lựa chọn và làm rõ để tạo ra phần sản phẩm đáp ứng tiêu chí hoàn thành.

Hình trong tài liệu là minh họa cách phân rã phục vụ lập kế hoạch. Một cây WBS theo hình này chưa đủ để mô tả toàn bộ cách vận hành Scrum.

Dù chọn cách nào, mỗi nhánh cần gắn với kết quả cụ thể. “Thiết kế” nên có đầu ra là tài liệu hoặc mô hình thiết kế được rà soát; “kiểm thử” nên có ca kiểm thử, kết quả chạy và thông tin lỗi.

**2. Dataset — dữ liệu cần chuẩn bị**

| Dữ liệu | Nội dung |
|---|---|
| Phạm vi dự án | Những hoạt động phải thực hiện |
| WBS sản phẩm hoặc danh sách chức năng | Những thành phần cần được phát triển |
| Quy trình được chọn | Waterfall hoặc cách tổ chức theo vòng lặp |
| Tiêu chuẩn đầu ra | Nội dung cần có của tài liệu, mã nguồn, kiểm thử |
| Nhân sự | Vai trò và năng lực thực hiện từng nhóm việc |
| Cơ chế phản hồi | Ai rà soát, ai xác nhận, khi nào có phản hồi |
| Phạm vi hỗ trợ, vận hành | Có thuộc dự án không, thực hiện đến thời điểm nào |

Tài liệu có minh họa các nhánh chăm sóc, hỗ trợ và vận hành. Khi áp dụng, cần đối chiếu hợp đồng hoặc tuyên ngôn để xác định phần nào thực sự thuộc phạm vi.

**3. Các bước thực hiện phương pháp hoàn thiện sản phẩm và nhận xét kết quả**

**Bước 1 — Chọn cách tổ chức thực hiện.**

Với bài thực hành, có thể chọn Waterfall để dễ quan sát sự chuyển tiếp giữa yêu cầu, thiết kế, lập trình và kiểm thử.

Nếu chọn cách phát triển theo Sprint, cần xác định danh sách công việc ưu tiên và những phần sản phẩm dự kiến hoàn thành qua từng vòng lặp.

**Bước 2 — Tạo các nhóm công việc cấp cao.**

Theo ví dụ Waterfall trong tài liệu: quản lý dự án, xây dựng phần mềm, chăm sóc hỗ trợ và vận hành phần mềm.

**Bước 3 — Phân rã nhóm xây dựng phần mềm.**

| Nhóm công việc | Công việc chi tiết minh họa | Đầu ra cần có |
|---|---|---|
| Phân tích | Khảo sát thu phí, làm rõ thông tin hộ, xác định người dùng | Yêu cầu được xác nhận |
| Thiết kế | Thiết kế chức năng, giao diện, dữ liệu, phân quyền và rà soát | Hồ sơ thiết kế |
| Cài đặt/lập trình | Phát triển từng module, kết nối các thành phần | Mã nguồn và bản chạy |
| Kiểm thử | Chuẩn bị tình huống, thực hiện kiểm thử, sửa và kiểm tra lại lỗi | Kết quả kiểm thử |
| Triển khai, bàn giao | Chuẩn bị bộ cài, hướng dẫn, hỗ trợ nghiệm thu | Bộ bàn giao được kiểm tra |

Các hoạt động trong bảng là cách triển khai thực hành, cần điều chỉnh theo dự án.

**Bước 4 — Gắn công việc với module.**

Ví dụ, dưới “Thiết kế dữ liệu” có thể chia thành thiết kế dữ liệu quản lý thu phí, người dùng và hộ gia đình, giống hướng minh họa của tài liệu.

Cần có bước rà soát chung để các module dùng thống nhất mã hộ, mã người dùng và các quan hệ dữ liệu.

**Bước 5 — Nếu chọn Scrum, phân rã theo kết quả của từng Sprint.**

Ví dụ thực hành cho nhóm chức năng thu phí:

- Làm rõ yêu cầu tạo khoản thu.
- Lựa chọn phần việc có thể hoàn thành trong Sprint.
- Thiết kế, lập trình và kiểm thử phần việc đã chọn.
- Trình diễn kết quả, lấy phản hồi và cập nhật công việc tiếp theo.

Không nên coi “lập trình xong” là hoàn thành nếu phần việc chưa đáp ứng tiêu chí kiểm thử và chất lượng đã thống nhất.

**Bước 6 — Đối chiếu với WBS sản phẩm.**

Mỗi thành phần bàn giao phải có các công việc cần thiết để tạo ra và kiểm tra nó. Mỗi công việc trong quy trình cũng phải có lý do tồn tại và đầu ra rõ ràng.

**Nhận xét kết quả:** WBS theo quy trình giúp nhìn thấy công sức cần thiết ngoài lập trình. Hai cách phân rã theo sản phẩm và quy trình là những góc nhìn bổ sung; không cộng tổng hai cây như hai khối lượng độc lập, vì nhiều nội dung đang mô tả cùng một phạm vi.

</details>

<details>
<summary>-sản phẩm 'Bảng công việc và biểu đồ Gantt — ước lượng, phân công, thiết lập phụ thuộc và theo dõi tiến độ'</summary>

**1. Cơ sở lý thuyết của sản phẩm**

**Biểu đồ Gantt** biểu diễn công việc trên trục thời gian. Mỗi thanh cho biết khoảng thực hiện của một công việc; các mốc thể hiện những sự kiện quan trọng như nghiệm thu hoặc bàn giao.

Để lập Gantt có ý nghĩa, cần chuyển các gói WBS thành hoạt động có thời lượng, quan hệ phụ thuộc và người thực hiện.

Các khái niệm cần phân biệt:

| Khái niệm | Ý nghĩa |
|---|---|
| Khối lượng lao động — Effort | Tổng công sức cần bỏ ra, thường tính bằng giờ công hoặc ngày công |
| Thời lượng — Duration | Khoảng thời gian cần để hoàn thành công việc theo lịch làm việc |
| Quan hệ phụ thuộc | Điều kiện ràng buộc thứ tự giữa các công việc |
| Nguồn lực | Người hoặc phương tiện được phân công |
| Mốc — Milestone | Sự kiện đánh dấu kết quả quan trọng, thường có thời lượng bằng 0 |
| Đường găng — Critical Path | Chuỗi hoạt động quyết định thời điểm hoàn thành theo mô hình tiến độ hiện tại |
| Lịch cơ sở — Baseline | Phiên bản lịch đã được chấp thuận để so sánh với thực tế |

Một công việc cần năm ngày công chưa chắc hoàn thành trong năm ngày lịch. Người phụ trách có thể chỉ tham gia một phần thời gian hoặc phải chờ kết quả từ bên khác.

Quan hệ phổ biến là **kết thúc–bắt đầu — Finish to Start**: công việc sau bắt đầu khi công việc trước hoàn thành. Tuy nhiên, không nên nối tất cả công việc thành một chuỗi nếu chúng có thể thực hiện song song.

**2. Dataset — dữ liệu cần chuẩn bị**

| Trường dữ liệu | Nội dung |
|---|---|
| Mã công việc | Mã duy nhất để tham chiếu |
| Mã WBS | Gói công việc mà hoạt động thuộc về |
| Tên công việc | Hành động cụ thể và rõ kết quả |
| Thời lượng | Ước lượng dựa trên độ phức tạp và năng lực |
| Công việc tiền nhiệm | Công việc phải hoàn thành hoặc đạt điều kiện trước đó |
| Người thực hiện | Thành viên và mức độ tham gia |
| Lịch làm việc | Ngày làm việc, ngày nghỉ, thời gian vắng mặt |
| Mốc bắt buộc | Dùng thử, bàn giao chính thức, hoàn thành dự án |
| Điều kiện hoàn thành | Sản phẩm hoặc bằng chứng xác nhận xong |
| Chi phí liên quan | Đơn giá công, thiết bị, dịch vụ và khoản khác nếu cần kiểm soát ngân sách |

**3. Các bước thực hiện phương pháp hoàn thiện sản phẩm và nhận xét kết quả**

**Bước 1 — Lập danh sách hoạt động từ WBS.**

Không dùng một dòng “Làm phần mềm” cho toàn bộ dự án. Phân chia đủ để có thể ước lượng, giao người và theo dõi.

Bảng dưới đây là **ví dụ một phần kế hoạch**, thời lượng do người hướng dẫn giả định:

| Mã | Công việc | Thời lượng | Tiền nhiệm | Vai trò phụ trách |
|---|---|---:|---|---|
| A | Khảo sát và xác nhận yêu cầu | 5 ngày làm việc | — | Phân tích nghiệp vụ |
| B | Thiết kế dữ liệu chung | 3 ngày làm việc | A | Thiết kế |
| C | Thiết kế giao diện | 3 ngày làm việc | A | Thiết kế giao diện |
| D | Phát triển quản lý người dùng | 5 ngày làm việc | B, C | Lập trình |
| E | Phát triển quản lý hộ gia đình | 7 ngày làm việc | B, C | Lập trình |
| F | Phát triển quản lý thu phí | 8 ngày làm việc | B, C | Lập trình |
| G | Tích hợp và kiểm thử hệ thống | 5 ngày làm việc | D, E, F | Nhóm phát triển và kiểm thử |
| H | Khách hàng kiểm thử chấp nhận | 3 ngày làm việc | G | Khách hàng và nhóm dự án |

Bảng này chưa bao gồm toàn bộ công việc quản lý, tài liệu, sửa lỗi và bàn giao. Các quan hệ phụ thuộc thực tế còn phải được kiểm tra theo kiến trúc phần mềm.

**Bước 2 — Thiết lập lịch làm việc.**

Trong công cụ lập tiến độ, khai báo ngày bắt đầu, số ngày làm việc mỗi tuần, ngày nghỉ và mức độ tham gia của từng thành viên.

Chỉ sau đó mới tính ngày bắt đầu, kết thúc từ thời lượng.

**Bước 3 — Nhập công việc và liên kết tiền nhiệm.**

Tạo các cột tương ứng với bảng dữ liệu. Liên kết công việc bằng mã tiền nhiệm thay vì chỉ nhập thủ công ngày bắt đầu cho mọi dòng.

Cách này giúp lịch cập nhật khi một công việc thay đổi thời lượng.

**Bước 4 — Gán người và kiểm tra quá tải.**

Trong bảng minh họa, D, E và F có thể bắt đầu sau B, C về mặt logic. Nhưng nếu chỉ có một người lập trình toàn thời gian, không thể giả định cả ba cùng được thực hiện toàn thời gian.

Điều chỉnh thứ tự, mức tham gia hoặc nhân sự để có lịch khả thi.

**Bước 5 — Thêm các mốc bàn giao.**

Theo bài mẫu:

| Mốc | Ngày |
|---|---|
| Bàn giao phiên bản thử nghiệm | 30/11/2023 |
| Bàn giao phiên bản chính thức | 15/12/2023 |
| Hoàn thành dự án | 30/12/2023 |

Bố trí thời gian lấy phản hồi, sửa lỗi, kiểm tra lại và hoàn thiện tài liệu giữa các mốc. Không mặc định ngày bàn giao thử nghiệm cũng là ngày phần mềm đã được nghiệm thu.

**Bước 6 — Rà soát thời hạn và ngân sách.**

Nếu lịch tính ra vượt mốc, xác định nguyên nhân: thiếu người, ước lượng chưa phù hợp, chờ khách hàng hay phạm vi quá lớn.

Chỉ điều chỉnh thời lượng khi có căn cứ. Mọi phương án tăng người hoặc mua thêm dịch vụ cũng phải được kiểm tra với ngân sách 100 triệu đồng của bài mẫu.

**Bước 7 — Lưu lịch cơ sở và cập nhật thực tế.**

Sau khi kế hoạch được chấp thuận, lưu phiên bản gốc. Khi theo dõi, cập nhật ngày thực tế, phần việc còn lại, lỗi đang chặn và dự báo hoàn thành.

Phần trăm hoàn thành nên gắn với kết quả kiểm chứng được. Ví dụ “bốn trong năm chức năng đã vượt kiểm thử” rõ nghĩa hơn “cảm thấy hoàn thành 80%”.

**Nhận xét kết quả:** Gantt đạt yêu cầu khi có đủ công việc trong phạm vi, quan hệ hợp lý, người thực hiện không quá tải và các mốc có khả năng đạt được. Một biểu đồ có thanh thời gian đẹp nhưng thiếu phụ thuộc hoặc lịch nguồn lực chưa chứng minh được tính khả thi.

</details>

<details>
<summary>-sản phẩm 'Kế hoạch quản lý rủi ro — nhận diện, đánh giá, ưu tiên và theo dõi biện pháp ứng phó'</summary>

**1. Cơ sở lý thuyết của sản phẩm**

**Rủi ro dự án** là sự kiện hoặc điều kiện chưa chắc chắn có thể ảnh hưởng đến mục tiêu dự án. Phần hướng dẫn trong tài liệu tập trung vào các rủi ro bất lợi.

Cần phân biệt:

| Khái niệm | Ví dụ |
|---|---|
| Rủi ro | Thành viên có thể rời dự án trong giai đoạn phát triển |
| Vấn đề đã xảy ra | Thành viên đã thông báo nghỉ và chưa có người thay |
| Giả định | Khách hàng sẽ tham gia kiểm thử đúng lịch |
| Ràng buộc | Không được vượt ngân sách đã phê duyệt |

Một mô tả rủi ro rõ nên thể hiện **nguyên nhân → sự kiện có thể xảy ra → hậu quả**.

Ví dụ:

> Do một thành viên đồng thời tham gia nhiều dự án, người đó có thể không hoàn thành chức năng thu phí đúng hạn, làm chậm tích hợp và bàn giao thử nghiệm.

Tài liệu đánh giá xác suất và tác động theo ba mức: thấp, vừa, cao, tương ứng 1, 2, 3. Xác suất thể hiện khả năng xảy ra; tác động thể hiện mức thiệt hại nếu xảy ra. Không nên suy tác động từ xác suất.

**Điểm cần làm rõ trong tài liệu:** Bảng ví dụ trang 7 có điểm phù hợp với phép nhân xác suất × tác động, nhưng ma trận trang 9 dùng hệ thống mức 1–5 khác. Chẳng hạn, xác suất vừa và tác động vừa được ghi điểm 4 ở bảng ví dụ, còn ma trận xếp mức 3. Trang 8 cũng lặp nhãn “Mức 4”, “Mức 5” ở hai mô tả cuối.

Để minh họa nhất quán, phần này **dùng ma trận trang 9**:

| Xác suất \ Tác động | Thấp — 1 | Vừa — 2 | Cao — 3 |
|---|---:|---:|---:|
| Thấp — 1 | Mức 1 | Mức 2 | Mức 3 |
| Vừa — 2 | Mức 2 | Mức 3 | Mức 4 |
| Cao — 3 | Mức 3 | Mức 4 | Mức 5 |

Nếu chọn phương pháp nhân điểm, phải công bố thang điểm và ngưỡng phân loại riêng; không dùng lẫn với ma trận này.

**2. Dataset — dữ liệu cần chuẩn bị**

| Nhóm dữ liệu | Nội dung cần có |
|---|---|
| Phạm vi và yêu cầu | Chức năng khó, phần chưa rõ, khả năng thay đổi |
| Nhân sự | Kỹ năng, thời gian tham gia, người thay thế |
| Tiến độ | Công việc dài, đường găng, mốc bắt buộc |
| Ngân sách | Khoản dự phòng và các chi phí có thể tăng |
| Kỹ thuật | Công nghệ mới, tích hợp, môi trường cài đặt |
| Khách hàng | Khả năng cung cấp dữ liệu, phản hồi và nghiệm thu |
| Kinh nghiệm | Sự cố từng gặp ở dự án tương tự |
| Thang đánh giá | Quy ước xác suất, tác động và mức ưu tiên |

Khi có thể, dùng bằng chứng để đánh giá. Ví dụ: lịch phân công cho thấy thành viên chỉ có thể tham gia hai ngày mỗi tuần là căn cứ cụ thể hơn nhận định “có thể thiếu người”.

**3. Các bước thực hiện phương pháp hoàn thiện sản phẩm và nhận xét kết quả**

**Bước 1 — Nhận diện rủi ro theo từng nhóm.**

Dựa trên tài liệu, rà soát ít nhất các nhóm: nhân sự, thay đổi yêu cầu, tài liệu chưa hoàn thiện, phối hợp kém, chậm tiến độ, hợp đồng, nghiệm thu, ngân sách và ước lượng quá lạc quan.

Đối chiếu từng nhóm với dự án thực tế để tránh sao chép những rủi ro không liên quan.

**Bước 2 — Viết mô tả rõ nguyên nhân và hậu quả.**

Thay “rủi ro kỹ thuật” bằng mô tả như:

> Nhóm chưa kiểm tra bộ cài trên môi trường Windows đã cam kết, nên có thể phát hiện lỗi tương thích gần ngày bàn giao và phải sửa gấp.

Đây là ví dụ bổ sung để thực hành.

**Bước 3 — Chấm xác suất và tác động theo cùng một quy ước.**

Tài liệu gợi ý đánh giá tác động qua phạm vi, chất lượng và chi phí. Chẳng hạn, mức tăng chi phí dưới 5%, từ 5–10% và trên 10% được dùng để phân biệt các mức.

Nhóm cần thống nhất cách chọn tác động tổng thể khi một rủi ro ảnh hưởng nhiều mặt. Không tự động lấy trung bình nếu điều đó che khuất một hậu quả nghiêm trọng.

**Bước 4 — Lập sổ đăng ký rủi ro.**

Bảng dưới đây là **minh họa đánh giá**, không phải điểm số đã được xác nhận của dự án:

| Mã | Rủi ro | Xác suất | Tác động | Mức theo ma trận | Biện pháp phòng ngừa |
|---|---|---:|---:|---:|---|
| R1 | Thành viên chủ chốt không còn đủ thời gian tham gia | 2 | 3 | 4 | Chia sẻ kiến thức, chuẩn bị người thay thế |
| R2 | Yêu cầu thay đổi sau khi đã thiết kế | 2 | 2 | 3 | Xác nhận yêu cầu, áp dụng quy trình xét thay đổi |
| R3 | Tài liệu kỹ thuật không theo kịp mã nguồn | 2 | 2 | 3 | Cập nhật và rà soát cùng từng phần bàn giao |
| R4 | Khách hàng phản hồi chậm, ảnh hưởng nghiệm thu | 2 | 3 | 4 | Chốt lịch dùng thử và người phản hồi |
| R5 | Ước lượng thiếu công sức tích hợp và sửa lỗi | 2 | 3 | 4 | Rà soát ước lượng, dành thời gian cho tích hợp và kiểm tra lại |

**Bước 5 — Bổ sung trách nhiệm và phương án khi xảy ra.**

Mỗi rủi ro nên có người theo dõi, dấu hiệu kích hoạt, hạn thực hiện biện pháp và phương án ứng phó.

Ví dụ với R1:

| Nội dung | Cách ghi minh họa |
|---|---|
| Người theo dõi | Quản lý dự án |
| Phòng ngừa | Rà soát mức tham gia hằng tuần; yêu cầu chia sẻ mã nguồn và tài liệu |
| Dấu hiệu kích hoạt | Thành viên thông báo giảm thời gian dưới mức đã cam kết |
| Khi xảy ra | Đánh giá lại phần việc còn lại, chuyển giao và cập nhật lịch |
| Kiểm tra bổ sung | Tác động của phương án chuyển giao đến chi phí và các mốc |

**Bước 6 — Xếp ưu tiên và đưa biện pháp vào kế hoạch.**

Theo ma trận đã chọn, xử lý các rủi ro mức cao trước. Với rủi ro cùng mức, xem xét thêm thời điểm có thể xảy ra và mức độ ảnh hưởng đến mốc quan trọng.

Nếu biện pháp là “đào tạo người dự phòng” hoặc “kiểm tra tương thích bộ cài”, phải đưa hoạt động này vào bảng công việc, có người làm và thời gian thực hiện.

**Bước 7 — Cập nhật định kỳ.**

Trong các buổi đánh giá tiến độ, kiểm tra rủi ro mới, thay đổi xác suất, tác động và hiệu quả của biện pháp đã thực hiện.

Khi rủi ro xảy ra, chuyển sang theo dõi như một vấn đề thực tế. Sau khi ứng phó, đánh giá phần rủi ro còn lại.

**Nhận xét kết quả:** Kế hoạch rủi ro hoàn thiện khi mỗi rủi ro quan trọng có căn cứ đánh giá, người chịu trách nhiệm, biện pháp cụ thể và cách nhận biết lúc cần hành động. Những câu như “cố gắng tránh chậm tiến độ” chưa đủ để tổ chức thực hiện.

</details>
