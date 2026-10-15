-🔍**LythuyetThaotac: Khởi tạo dự án, phân rã công việc WBS, lập biểu đồ Gantt và quản lý rủi ro** — tư liệu: Huong dan xay dung Ke hoach du an(4).pdf

**Giới thiệu bài toán mẫu để học cách thao tác:** Ban quản trị chung cư Blue Moon đang quản lý hộ dân và thu phí bằng Excel. Nhóm dự án cần xây dựng phần mềm gồm ba module: **quản lý thu phí, quản lý người dùng và quản lý hộ gia đình**.

Từ bài toán này, bạn tạo bốn sản phẩm: **tuyên ngôn dự án → cấu trúc phân cấp công việc WBS → lịch trình Gantt → bảng quản lý rủi ro**. Các sản phẩm phải liên kết với nhau: phạm vi trong tuyên ngôn quyết định công việc trong WBS; công việc trong WBS được đưa vào Gantt; rủi ro cho biết những gì có thể làm các công việc đó không hoàn thành như dự kiến.

Ví dụ dưới đây giữ ngân sách **100 triệu đồng** và các mốc **quý IV/2023** của tài liệu. Tên thành viên, phân bổ ngân sách, công việc chi tiết và tiêu chí kiểm tra bổ sung là **dữ liệu minh họa để thực hành**.

<details>
<summary>-sản phẩm 'Tuyên ngôn dự án — Project Charter'</summary>

**Sản phẩm này là gì?** Đây là tài liệu xác lập lý do thực hiện dự án, kết quả cần đạt, phạm vi, nguồn lực và quyền hạn thực hiện. Theo tài liệu, nhà tài trợ ban hành tuyên ngôn để chính thức cho phép dự án tồn tại và trao quyền sử dụng nguồn lực cho người quản lý dự án.

Bạn có thể tạo một tài liệu Word gồm các nhóm thông tin sau.

**Các thuộc tính cần tạo**

- **“Tên dự án”**: Là tên định danh chung của dự án — phải được dùng thống nhất trong WBS, Gantt và bảng rủi ro — điền: **“Xây dựng phần mềm quản lý và thu phí ở chung cư Blue Moon”**.

- **“Nhà tài trợ dự án”**: Là cá nhân bảo trợ, hỗ trợ quyết định và cấp hoặc huy động nguồn lực cho dự án — liên hệ với ngân sách, phê duyệt và xử lý vấn đề vượt quyền quản lý dự án — điền tên, chức danh của người được tổ chức giao vai trò này; ví dụ: **“Ông Minh, Giám đốc Công ty ABC”**.

- **“Cơ quan tài trợ”**: Là tổ chức đứng sau việc tài trợ — liên hệ với nhà tài trợ và nguồn kinh phí — điền: **“Công ty ABC”**. Cần phân biệt tên tổ chức với tên cá nhân đại diện.

- **“Mức độ ảnh hưởng của dự án”**: Mô tả dự án tác động đến ai và thay đổi cách làm việc nào — lấy đầu vào từ hiện trạng và nhóm người sử dụng — điền: **“Phần mềm nội bộ, thay đổi cách quản lý thông tin hộ dân và thu phí của Ban quản trị Blue Moon”**.

- **“Người quản lý dự án”**: Là người điều phối công việc, nguồn lực, tiến độ và báo cáo — phải xuất hiện nhất quán trong phân công WBS, Gantt và chiến lược truyền thông — điền: **“Nguyễn An — quản lý dự án”**, kèm nơi công tác, điện thoại và email thực tế.

- **“Thành viên dự án”**: Là danh sách những người trực tiếp thực hiện — là đầu vào để phân công công việc và kiểm tra khả năng đáp ứng lịch trình — tạo các cột **họ tên, nơi công tác, điện thoại, email**. Ví dụ: **Bình phụ trách yêu cầu; Chi phụ trách lập trình; Dũng phụ trách kiểm thử**.

- **“Các bên liên quan và trách nhiệm”**: Là các cá nhân, đơn vị có ảnh hưởng hoặc chịu ảnh hưởng bởi dự án — liên hệ với việc cung cấp yêu cầu, phản hồi, nghiệm thu và hỗ trợ triển khai — điền rõ từng vai trò. Ví dụ: **trưởng ban quản trị xác nhận phạm vi; kế toán giải thích cách thu phí và dùng thử; đại diện Công ty ABC phối hợp hợp đồng**.

- **“Bối cảnh và động cơ”**: Là hiện trạng và nguyên nhân khiến dự án cần được thực hiện — cung cấp căn cứ cho mục đích và mục tiêu — điền: **“Thông tin đang nằm ở nhiều bảng Excel, khó tổng hợp khoản thu và theo dõi biến động hộ dân”**.

- **“Mục đích dự án”**: Là nhu cầu nghiệp vụ dự án cần giải quyết — được rút ra từ vấn đề trong bối cảnh, sau đó cụ thể hóa thành mục tiêu — điền: **“Hỗ trợ Ban quản trị quản lý tập trung hộ dân, các loại phí và tình hình đóng phí”**.

- **“Mục tiêu đo lường được”**: Là kết quả có thể kiểm tra để xác định dự án đạt yêu cầu hay chưa — phải liên hệ với phạm vi và tiêu chí nghiệm thu; đầu vào là nhu cầu đã thống nhất — điền: **“Phần mềm hỗ trợ quản lý 100% loại phí và các trường thông tin hộ dân thuộc danh mục đã được hai bên xác nhận”**. Muốn đo “100%”, cần có danh mục làm mẫu số; chẳng hạn hỗ trợ đủ **5/5 loại phí đã thống nhất**.

- **“Sản phẩm bàn giao”**: Là các đầu ra phải chuyển giao khi hoàn thành — mỗi đầu ra phải được tạo ra bởi công việc trong WBS và có mốc bàn giao trong Gantt — liệt kê **tên sản phẩm, người nhận và điều kiện nhận**. Theo mẫu PDF, gồm bộ cài, chứng nhận bản quyền, hướng dẫn sử dụng, hướng dẫn cài đặt; mã nguồn, đặc tả yêu cầu, tài liệu thiết kế, kiểm thử, cấu trúc mã nguồn, API và tài liệu dự án.

- **“Phạm vi công việc được thực hiện”**: Là những loại công việc nhóm cam kết làm — quyết định các nhánh công việc cần có trong WBS — điền: **“Đặc tả yêu cầu, phân tích, thiết kế, lập trình, kiểm thử và triển khai phần mềm”**.

- **“Phạm vi sản phẩm”**: Là những chức năng, module phần mềm phải cung cấp — là đầu vào trực tiếp cho WBS theo sản phẩm bàn giao — điền ba module: **quản lý thu phí; quản lý người dùng; quản lý hộ gia đình**.

- **“Ngoài phạm vi”**: Là những công việc dự án không cam kết thực hiện — giúp tránh việc đưa thêm công việc vào WBS mà chưa điều chỉnh kế hoạch — điền theo tài liệu: **“Không bao gồm nhập liệu thông tin đầu vào như nhân khẩu, hộ khẩu và các loại phí”**. Việc thiết kế chức năng nhập liệu vẫn nằm trong phạm vi nếu yêu cầu có chức năng đó; việc nhập toàn bộ dữ liệu thật ban đầu là công việc khác.

- **“Ngân sách”**: Là tổng kinh phí được phép sử dụng — phải đủ cho các công việc đã xác định và phù hợp với giới hạn dự án — điền: **100.000.000 đồng**. Có thể minh họa phân bổ **80 triệu xây dựng phần mềm + 10 triệu quản lý dự án + 10 triệu dự phòng**. Tổng các khoản phải bằng ngân sách chung.

- **“Lịch trình và mốc chính”**: Là thời điểm bắt đầu, bàn giao và hoàn thành dự kiến — ràng buộc lịch chi tiết trong Gantt — điền theo PDF: **thực hiện trong quý IV/2023; dùng thử lần đầu ngày 30/11; bàn giao chính thức ngày 15/12; hoàn thành ngày 30/12**.

- **“Rủi ro sơ bộ”**: Là những sự kiện chưa chắc xảy ra nhưng có thể ảnh hưởng dự án — được phân tích chi tiết trong bảng quản lý rủi ro — điền: **“Khách hàng thay đổi yêu cầu sau khi đã thiết kế, làm tăng công sức và có thể chậm mốc 30/11”**.

- **“Giả định”**: Là điều nhóm tạm coi là đúng để lập kế hoạch, nhưng cần theo dõi xác nhận — nếu giả định không đúng, lịch trình hoặc chi phí có thể phải thay đổi — điền: **“Kế toán chung cư có thể tham gia dùng thử và phản hồi đúng lịch”**.

- **“Ràng buộc”**: Là giới hạn bắt buộc phải tuân thủ — ảnh hưởng cách lựa chọn nhân lực, lịch trình và giải pháp — điền theo PDF: **“Thời gian không quá bốn tháng; tổng chi phí không vượt 100 triệu đồng”**.

- **“Phụ thuộc bên ngoài”**: Là điều kiện do người hoặc tổ chức ngoài nhóm thực hiện cung cấp — liên hệ với các công việc phải chờ trong Gantt và rủi ro chậm tiến độ — điền: **“Ban quản trị cung cấp quy định thu phí, mẫu biểu và người có thẩm quyền xác nhận yêu cầu”**.

- **“Chiến lược truyền thông”**: Là cách các bên trao đổi và nhận thông tin dự án — lấy đầu vào từ danh sách bên liên quan và các mốc cần quyết định — điền **người gửi, người nhận, nội dung, kênh và tần suất**. Ví dụ: **An gửi báo cáo tiến độ hằng tuần qua email; nhóm họp nhanh đầu ngày; khách hàng và nhà tài trợ họp tại các mốc bàn giao**.

- **“Phê duyệt”**: Là phần ghi nhận các bên có thẩm quyền chấp thuận tuyên ngôn — xác nhận phạm vi, ngân sách, lịch trình và trách nhiệm đã thống nhất — tạo các cột **vai trò, họ tên, chữ ký, ngày ký** cho nhà tài trợ, đại diện cơ quan tài trợ và người quản lý dự án. Khi làm bài mẫu, có thể để trống chữ ký.

- **“Ghi chú”**: Là thông tin bổ sung giúp hiểu đúng tài liệu — dùng cho những điều chưa phù hợp đặt vào trường khác, nhưng không thay thế các cam kết chính — ví dụ: **“Danh mục loại phí được xác nhận trong phụ lục yêu cầu”**.

**Ví dụ liên kết đầy đủ giữa các thuộc tính**

Hiện trạng **quản lý bằng Excel khó tổng hợp** tạo ra mục đích **quản lý tập trung việc thu phí**. Mục đích được cụ thể hóa thành mục tiêu **hỗ trợ đủ 5 loại phí đã thống nhất**.

Mục tiêu dẫn đến phạm vi **module quản lý thu phí**, rồi tạo ra sản phẩm bàn giao **phần mềm và tài liệu sử dụng**. Nhóm phải bố trí người xây dựng, kiểm thử và bàn giao trước các mốc đã cam kết trong ngân sách 100 triệu đồng.

Để làm được, nhóm phụ thuộc vào việc kế toán cung cấp quy định tính phí. Nếu việc cung cấp chậm, rủi ro tiến độ xuất hiện. Người quản lý phải phản ánh trong báo cáo và điều chỉnh công việc phù hợp với ràng buộc đã được phê duyệt.

**Cách kiểm tra sản phẩm:** Mỗi mục tiêu phải có phạm vi thực hiện tương ứng; mỗi sản phẩm bàn giao phải có người nhận; lịch trình, ngân sách và nhân lực phải đủ để tạo ra các đầu ra đã cam kết.

</details>

<details>
<summary>-sản phẩm 'Cấu trúc phân cấp công việc — WBS'</summary>

**Sản phẩm này là gì?** WBS chia phạm vi dự án thành những phần nhỏ hơn để biết cần hoàn thành những gì. Bạn có thể trình bày bằng sơ đồ cây hoặc bảng phân cấp.

Tài liệu minh họa ba cách tổ chức: **theo sản phẩm bàn giao, theo quy trình Waterfall và theo quy trình Scrum**. Đây là các cách nhìn khác nhau; không mặc định phải làm ba WBS độc lập cho cùng một dự án.

**Các thuộc tính cần tạo**

- **“Nút gốc”**: Là phần việc tổng thể mà sơ đồ đại diện — phải thống nhất với phạm vi được phân rã — điền: **“Dự án phần mềm quản lý và thu phí Blue Moon”** nếu bao quát toàn dự án, hoặc **“Phần mềm quản lý và thu phí Blue Moon”** nếu chỉ phân rã sản phẩm phần mềm.

- **“Cách phân rã”**: Là nguyên tắc dùng để chia một nút cha thành các nút con — quyết định tên gọi và ý nghĩa các cấp — chọn **theo sản phẩm bàn giao** để nhìn rõ module, tính năng; chọn **theo quy trình** để nhìn rõ các nhóm hoạt động tạo ra sản phẩm.

- **“Mã WBS”**: Là mã thể hiện vị trí trong cây — liên hệ với mã nút cha và được dùng để truy vết sang Gantt, bảng rủi ro — điền theo dạng **1 → 1.1 → 1.1.1**. Ví dụ: **1. Quản lý thu phí; 1.1. Tạo khoản thu**.

- **“Tên nút hoặc tên công việc”**: Là tên phần phạm vi tại vị trí đó — phải cụ thể hơn nút cha và không trùng ý nghĩa với nút anh em — điền **“Tạo khoản thu”**, **“Thu phí”**, **“Thống kê các khoản đóng góp”** thay vì những tên khó kiểm tra như “Xử lý phần mềm”.

- **“Nút cha”**: Là phần phạm vi chứa nút hiện tại — giúp kiểm tra công việc thuộc nhóm nào — ví dụ: **“Tạo khoản thu” có nút cha là “Quản lý thu phí”**. Trong bảng có thể tạo cột **Mã cha = 1** cho dòng có mã **1.1**.

- **“Cấp phân rã”**: Là độ sâu của nút trong cây — được suy ra từ quan hệ cha con — điền **cấp 0: toàn bộ; cấp 1: module; cấp 2: tính năng** đối với ví dụ theo sản phẩm trong PDF. Các cấp không tự biểu thị thời gian thực hiện.

- **“Gói công việc”**: Là phần việc ở mức thấp nhất của WBS đang sử dụng, đủ rõ để quản lý — liên hệ với việc ước lượng và giao trách nhiệm — chọn **“Tạo khoản thu”** làm gói nếu nhóm có thể xác định rõ đầu ra, công sức và người chịu trách nhiệm. Nếu quá lớn, tiếp tục chia hoặc lập các hoạt động thực hiện chi tiết.

- **“Đầu ra của gói công việc”**: Là kết quả phải có khi gói hoàn thành — lấy từ yêu cầu hoặc sản phẩm bàn giao trong tuyên ngôn — điền: **“Chức năng tạo khoản thu có giao diện, lưu dữ liệu và kiểm tra dữ liệu hợp lệ”**. Thuộc tính này có thể ghi trong bảng mô tả WBS để sơ đồ cây không quá dài.

- **“Điều kiện hoàn thành”**: Là căn cứ xác nhận đầu ra đã đạt — liên hệ với mục tiêu và kiểm thử — điền: **“Tạo được khoản thu hợp lệ; dữ liệu lưu đúng; dữ liệu thiếu hoặc sai bị từ chối; các ca kiểm thử đã thống nhất đều đạt”**.

- **“Người chịu trách nhiệm”**: Là người theo dõi và chịu trách nhiệm về đầu ra của gói — lấy từ đội ngũ trong tuyên ngôn, sau đó dùng khi phân công Gantt — điền: **“Chi phụ trách hoàn thành chức năng; Dũng thực hiện kiểm thử”**. Một gói có thể cần nhiều người phối hợp.

- **“Hoạt động thực hiện gói công việc”**: Là các bước cần tiến hành để tạo đầu ra — được dùng làm đầu vào lập lịch Gantt khi cần quản lý chi tiết — với gói **Tạo khoản thu**, điền: **làm rõ yêu cầu → thiết kế → lập trình → kiểm thử**. Không mặc định mỗi bước phải xuất hiện trên sơ đồ WBS nếu chúng đã được quản lý trong bảng hoạt động riêng.

- **“Quy tắc 100%”**: Là yêu cầu các phần con cộng lại bao quát toàn bộ phạm vi của phần cha, đồng thời tránh tính trùng công việc — kiểm tra dựa trên phạm vi và sản phẩm bàn giao — nếu nút gốc là toàn dự án, cần bao quát cả **quản lý dự án, tài liệu, kiểm thử, triển khai và bàn giao**, chứ không chỉ có ba module chức năng.

**Ví dụ cách phân rã theo sản phẩm bàn giao**

Bảng dưới đây minh họa phần phạm vi chức năng của phần mềm:

| Mã WBS | Mã cha | Tên nút | Đầu ra cần có |
|---|---|---|---|
| 0 | — | Phần mềm Blue Moon | Phần mềm gồm ba module |
| 1 | 0 | Quản lý thu phí | Nhóm chức năng thu phí |
| 1.1 | 1 | Tạo khoản thu | Tạo và lưu khoản thu |
| 1.2 | 1 | Thu phí | Ghi nhận việc đóng phí |
| 1.3 | 1 | Thống kê các khoản đóng góp | Tổng hợp số tiền đã đóng |
| 2 | 0 | Quản lý người dùng | Nhóm chức năng tài khoản |
| 2.1 | 2 | Đăng ký tài khoản | Tạo tài khoản theo quy định |
| 3 | 0 | Quản lý hộ gia đình | Nhóm chức năng hộ dân |
| 3.1 | 3 | Quản lý thông tin hộ | Tạo, xem và cập nhật hồ sơ hộ |

Đây là **bảng minh họa chưa phân rã hết**, không phải WBS hoàn chỉnh của toàn dự án.

**Ví dụ cách phân rã theo quy trình Waterfall**

Theo hướng minh họa trong PDF, bạn bắt đầu bằng các nhánh **quản lý dự án, xây dựng phần mềm, chăm sóc hỗ trợ, vận hành phần mềm**.

Trong nhánh xây dựng phần mềm, chia tiếp thành **phân tích, thiết kế, cài đặt và kiểm thử**. Nhánh thiết kế có thể chia thành **thiết kế chức năng, giao diện, dữ liệu, rà soát và phân quyền**.

Ví dụ một đường dẫn trong cây: **Xây dựng phần mềm → Thiết kế → Thiết kế dữ liệu → Module quản lý thu phí → Tạo khoản thu**.

Nhánh này mô tả **phần thiết kế dữ liệu** của tính năng tạo khoản thu. Công việc lập trình và kiểm thử tính năng đó phải được quản lý ở các nhánh tương ứng, tránh hiểu rằng thiết kế xong là hoàn thành toàn bộ tính năng.

**Ví dụ cách phân rã theo quy trình Scrum**

Theo hình minh họa của PDF: **Xây dựng phần mềm → Quản lý thu phí → Thiết lập yêu cầu, Lập kế hoạch phân đoạn, Phát triển, Vận hành**.

Trong nhánh **Phát triển**, chia tiếp thành **Tạo khoản thu, Thu phí, Thống kê các khoản đóng góp**.

Đây là cách tài liệu minh họa WBS khi tổ chức theo Scrum; bản thân WBS chưa thể hiện đầy đủ Sprint, Product Backlog hay lịch thực hiện từng Sprint.

**Ví dụ liên kết đầy đủ giữa các thuộc tính**

Tuyên ngôn xác định phần mềm phải quản lý thu phí. Bạn tạo nút **1. Quản lý thu phí**, rồi chia thành các nút **1.1, 1.2, 1.3**.

Gói **1.1. Tạo khoản thu** có đầu ra là chức năng tạo khoản thu, người chịu trách nhiệm là Chi và điều kiện hoàn thành là các ca kiểm thử đã thống nhất đều đạt.

Để lập lịch, nhóm chuyển gói này thành các hoạt động làm rõ yêu cầu, thiết kế, lập trình và kiểm thử. Các hoạt động cùng tham chiếu mã **WBS 1.1**, giúp biết chúng đang phục vụ sản phẩm nào.

**Cách kiểm tra sản phẩm:** Đọc từ dưới lên: các đầu ra cấp con có đủ để hoàn thành cấp cha không? Có đầu ra trong tuyên ngôn chưa được giao cho nhánh nào không? Có công việc đang bị tính hai lần không?

</details>

<details>
<summary>-sản phẩm 'Lịch trình dự án — Biểu đồ Gantt'</summary>

**Sản phẩm này là gì?** Đây là kế hoạch thể hiện công việc diễn ra khi nào, kéo dài bao lâu, phụ thuộc vào công việc nào và do ai thực hiện.

PDF nêu Gantt trong yêu cầu Bài 4.2 nhưng không hướng dẫn chi tiết các trường. Những thuộc tính dưới đây là phần triển khai bổ sung để bạn có thể tạo lịch từ WBS bằng bảng tính hoặc công cụ quản lý dự án.

**Các thuộc tính cần tạo**

- **“Lịch làm việc”**: Là quy định ngày và giờ được tính để thực hiện công việc — quyết định cách chuyển thời lượng thành ngày bắt đầu, kết thúc — chọn rõ **ngày lịch** hoặc **ngày làm việc**, số giờ/ngày và ngày nghỉ. Ví dụ bên dưới dùng **ngày lịch để minh họa**; điều này không có nghĩa nhân viên làm việc tất cả các ngày.

- **“Mã hoạt động”**: Là mã riêng cho từng dòng lịch — dùng khi khai báo quan hệ phụ thuộc — điền **A01, A02, A03…**. Mã hoạt động có thể khác mã WBS vì một gói WBS có nhiều hoạt động.

- **“Mã WBS tham chiếu”**: Là mã chỉ gói công việc mà hoạt động phục vụ — tạo liên kết giữa lịch và phạm vi — ví dụ hoạt động **“Lập trình tạo khoản thu”** tham chiếu **WBS 1.1** trong WBS theo sản phẩm nêu trên.

- **“Tên hoạt động”**: Là hành động cụ thể cần thực hiện — lấy từ việc triển khai các gói WBS — điền **“Thiết kế dữ liệu khoản thu”**, **“Lập trình tạo khoản thu”**, **“Kiểm thử tạo khoản thu”**.

- **“Công việc tiền nhiệm”**: Là hoạt động cần đáp ứng điều kiện trước khi hoạt động hiện tại diễn ra — lấy từ quy trình và nhu cầu sử dụng đầu ra — điền **“Kiểm thử tạo khoản thu có tiền nhiệm là Lập trình tạo khoản thu”**.

- **“Kiểu phụ thuộc”**: Là cách hai hoạt động liên kết về thời gian — kết hợp với tiền nhiệm để xác định lịch — ví dụ **FS, Finish-to-Start: hoạt động trước kết thúc thì hoạt động sau mới được bắt đầu**. Có thể dùng SS khi hai hoạt động được phép bắt đầu song song, nhưng phải có lý do thực tế.

- **“Thời lượng”**: Là khoảng thời gian hoạt động diễn ra theo lịch đã chọn — đầu vào gồm khối lượng việc, năng suất, nhân lực và kinh nghiệm — điền **“3 ngày làm việc”** hoặc **“3 ngày lịch”**, không ghi “3 ngày” khi chưa xác định cách tính.

- **“Khối lượng công sức”**: Là lượng lao động cần thiết, thường đo bằng giờ công hoặc ngày công — liên hệ với thời lượng và số người có thể tham gia — ví dụ **16 giờ công** có thể được bố trí trong hai ngày nếu một người dành đủ tám giờ/ngày. Nếu người đó chỉ dành bốn giờ/ngày, thời lượng dự kiến tăng lên bốn ngày.

- **“Ngày bắt đầu”**: Là thời điểm dự kiến khởi động hoạt động — phụ thuộc ngày sẵn sàng của tiền nhiệm, lịch làm việc và người thực hiện — ví dụ: **“Bắt đầu kiểm thử sau khi đã có bản dựng phần mềm đủ điều kiện kiểm thử”**.

- **“Ngày kết thúc”**: Là thời điểm dự kiến hoàn thành hoạt động — được tính từ ngày bắt đầu và thời lượng theo lịch — với cách tính ngày lịch bao gồm cả hai đầu, hoạt động bắt đầu **01/10** và kéo dài **14 ngày** sẽ kết thúc **14/10**.

- **“Người thực hiện”**: Là người được bố trí làm hoạt động — lấy từ đội dự án và trách nhiệm của gói WBS — điền **Chi** cho hoạt động lập trình, **Dũng** cho kiểm thử. Cần kiểm tra một người có đang được giao nhiều việc toàn thời gian trùng nhau không.

- **“Mốc thời gian — Milestone”**: Là điểm đánh dấu một sự kiện quan trọng — lấy từ tuyên ngôn và điều kiện nghiệm thu — điền **“Bàn giao bản dùng thử — 30/11/2023”**. Trong lịch, mốc thường có thời lượng bằng **0**; công việc chuẩn bị và thực hiện nghiệm thu phải được lập lịch riêng nếu cần thời gian.

- **“Phần trăm hoàn thành”**: Là mức tiến triển được cập nhật tại thời điểm báo cáo — phải có căn cứ từ công việc hoặc đầu ra đã hoàn thành — điền **0% khi chưa làm, 100% khi đạt điều kiện hoàn thành**. Không tự coi đã trôi qua nửa thời gian là hoàn thành 50%.

- **“Thanh Gantt”**: Là phần hiển thị khoảng bắt đầu đến kết thúc trên trục thời gian — được tạo từ dữ liệu ngày tháng của từng hoạt động — mỗi dòng công việc có một thanh; mốc thường được thể hiện bằng một ký hiệu tại đúng ngày.

**Ví dụ lịch tổng quát cho bài toán Blue Moon**

Bảng này dùng **ngày lịch** và tổng hợp công việc theo giai đoạn. Khi quản lý chi tiết, bạn phân rã tiếp thành hoạt động của từng gói WBS.

| Mã | Hoạt động hoặc mốc | Bắt đầu | Kết thúc | Thời lượng | Tiền nhiệm | Phụ trách |
|---|---|---|---|---:|---|---|
| A01 | Khảo sát và xác nhận yêu cầu | 01/10/2023 | 14/10/2023 | 14 ngày | — | Bình |
| A02 | Phân tích và thiết kế | 15/10/2023 | 28/10/2023 | 14 ngày | A01, FS | Bình, Chi |
| A03 | Lập trình ba module | 29/10/2023 | 18/11/2023 | 21 ngày | A02, FS | Chi |
| A04 | Tích hợp, kiểm thử và chuẩn bị bản dùng thử | 19/11/2023 | 29/11/2023 | 11 ngày | A03, FS | Chi, Dũng |
| M01 | Bàn giao bản dùng thử | 30/11/2023 | 30/11/2023 | 0 | A04, FS | An |
| A05 | Xử lý phản hồi và hoàn thiện bản chính thức | 01/12/2023 | 14/12/2023 | 14 ngày | M01, FS | Bình, Chi, Dũng |
| M02 | Bàn giao phiên bản chính thức | 15/12/2023 | 15/12/2023 | 0 | A05, FS | An |
| A06 | Hoàn tất chuyển giao và đóng dự án | 16/12/2023 | 30/12/2023 | 15 ngày | M02, FS | An và nhóm |
| M03 | Hoàn thành dự án | 30/12/2023 | 30/12/2023 | 0 | A06, FS | An |

Các hoạt động nghiệm thu, đào tạo và hoàn thiện tài liệu cần được phân bổ rõ bên trong những giai đoạn phù hợp; không thể chỉ ghi mốc bàn giao rồi mặc định mọi việc chuẩn bị đã được thực hiện.

**Ví dụ liên kết đầy đủ giữa các thuộc tính**

Gói WBS **1.1. Tạo khoản thu** tạo ra ba hoạt động liên tiếp:

| Mã | Hoạt động | WBS tham chiếu | Công sức minh họa | Người thực hiện | Tiền nhiệm |
|---|---|---|---:|---|---|
| T01 | Thiết kế chức năng tạo khoản thu | 1.1 | 8 giờ | Bình | Yêu cầu đã xác nhận |
| T02 | Lập trình chức năng tạo khoản thu | 1.1 | 16 giờ | Chi | T01, FS |
| T03 | Kiểm thử chức năng tạo khoản thu | 1.1 | 8 giờ | Dũng | T02, FS |

Từ công sức và mức sẵn sàng của từng người, bạn xác định thời lượng, rồi tính ngày bắt đầu và kết thúc.

Nếu T02 chậm, T03 có thể phải lùi. Nếu việc này làm chậm tích hợp hoặc bản dùng thử, mốc 30/11 bị ảnh hưởng. Khi đó phải đối chiếu ràng buộc trong tuyên ngôn và cập nhật rủi ro, thay vì chỉ sửa ngày trên biểu đồ.

**Cách kiểm tra sản phẩm:** Mọi hoạt động phải truy được về phạm vi; các quan hệ phụ thuộc phải có lý do; người thực hiện phải có thời gian; các mốc phải phù hợp với tuyên ngôn dự án.

</details>

<details>
<summary>-sản phẩm 'Bảng kế hoạch quản lý rủi ro dự án'</summary>

**Sản phẩm này là gì?** Đây là bảng ghi nhận điều gì có thể xảy ra, khả năng xảy ra, hậu quả và hành động cần thực hiện để giảm ảnh hưởng.

**Điểm cần xử lý trước khi điền:** PDF có sự không thống nhất trong cách đánh giá:

- Bảng 4-1 ghi một số điểm theo tích xác suất và tác động, chẳng hạn **2 × 2 = 4**.
- Ma trận cuối tài liệu lại quy định **xác suất 2, tác động 2 → mức 3**.
- Đoạn diễn giải năm mức ở trang 8 bị lặp nhãn “Mức 4”, “Mức 5”.

Để ví dụ nhất quán, phần dưới **tra mức rủi ro bằng ma trận cuối PDF**, không lấy tích làm mức rủi ro. Nếu cần giữ điểm tích để tham khảo, phải tạo cột riêng và đặt tên rõ.

**Các thuộc tính cần tạo**

- **“Mã hoặc số thứ tự rủi ro”**: Là định danh riêng của từng rủi ro — dùng để liên kết với công việc và theo dõi cập nhật — điền **R01, R02, R03…**.

- **“Mô tả rủi ro”**: Là phát biểu về một sự kiện chưa chắc xảy ra và hậu quả có thể có — lấy đầu vào từ phạm vi, giả định, nhân lực, tiến độ và phụ thuộc bên ngoài — điền theo mẫu **“Nếu… thì… dẫn đến…”**. Ví dụ: **“Nếu khách hàng bổ sung quy tắc tính phí sau khi lập trình, nhóm phải sửa thiết kế và mã nguồn, có thể chậm bàn giao”**.

- **“Phạm vi hoặc công việc bị ảnh hưởng”**: Là nơi rủi ro tác động — tham chiếu module, mã WBS hoặc mã hoạt động Gantt — điền **“Module thu phí; WBS 1.1; hoạt động lập trình và kiểm thử tạo khoản thu”**. Đây là trường bổ sung giúp bảng rủi ro liên kết với kế hoạch.

- **“Xác suất”**: Là mức đánh giá khả năng sự kiện xảy ra — dựa vào lịch sử, dấu hiệu hiện tại và đánh giá của nhóm — chọn **Thấp (1), Vừa (2), Cao (3)** theo bảng hướng dẫn. Ví dụ: **Vừa (2)** nếu đã có các lần yêu cầu thay đổi và vẫn còn điểm nghiệp vụ chưa rõ. Các số 1, 2, 3 là điểm thứ bậc, không phải phần trăm xác suất.

- **“Tác động”**: Là mức hậu quả nếu rủi ro xảy ra — liên hệ với phạm vi, chất lượng và chi phí — chọn **Thấp (1), Vừa (2), Cao (3)**. Ví dụ: chọn **Cao (3)** nếu ước tính sự kiện làm tăng chi phí trên 10%, phù hợp ngưỡng chi phí mức cao trong PDF.

- **“Căn cứ đánh giá”**: Là bằng chứng hoặc lý do chọn xác suất và tác động — giúp người khác hiểu vì sao một rủi ro được ưu tiên — điền: **“Quy tắc thu phí chưa được xác nhận; thay đổi dự kiến ảnh hưởng nhiều màn hình và cấu trúc dữ liệu”**. Đây là trường bổ sung, tránh chấm điểm theo cảm giác mà không giải thích.

- **“Mức độ rủi ro”**: Là kết quả kết hợp xác suất và tác động để ưu tiên xử lý — phụ thuộc trực tiếp hai thuộc tính trên — tra ma trận. Ví dụ: **xác suất 2 + tác động 3 → mức 4** theo ô tương ứng.

- **“Hành động ngăn ngừa”**: Là việc thực hiện trước khi rủi ro xảy ra để giảm khả năng hoặc hậu quả — phải xử lý đúng nguyên nhân trong mô tả — điền: **“Xác nhận quy tắc tính phí bằng văn bản; dùng ví dụ dữ liệu để rà soát; thống nhất quy trình tiếp nhận thay đổi”**.

- **“Dấu hiệu kích hoạt”**: Là dấu hiệu cho biết cần đưa rủi ro ra xử lý hoặc chuyển sang phương án ứng phó — liên hệ với cơ chế theo dõi — điền: **“Khách hàng gửi quy tắc tính phí mới sau khi tài liệu thiết kế đã được xác nhận”**. Đây là trường bổ sung.

- **“Phương án ứng phó khi xảy ra”**: Là việc làm khi sự kiện đã xuất hiện — phải dựa vào tác động thực tế và ràng buộc dự án — điền: **“Đánh giá phần việc phát sinh; xác định ảnh hưởng chi phí, lịch trình; trình người có thẩm quyền quyết định trước khi cập nhật kế hoạch”**. Đây là trường bổ sung, khác với hành động ngăn ngừa.

- **“Người phụ trách rủi ro”**: Là người theo dõi và điều phối xử lý — lấy từ đội dự án và trách nhiệm liên quan — điền **An** cho rủi ro thay đổi phạm vi, **Chi** cho rủi ro kỹ thuật. Đây là trường bổ sung.

- **“Trạng thái và ngày rà soát”**: Là thông tin cho biết rủi ro còn cần theo dõi hay đã được xử lý — liên hệ với báo cáo tiến độ và cuộc họp — điền **“Đang theo dõi — rà soát hằng tuần”**, hoặc **“Đã xảy ra — đang xử lý”**. Đây là trường bổ sung.

**Thang xác suất để điền**

| Điểm | Mức | Cách hiểu để thực hành |
|---:|---|---|
| 1 | Thấp | Hiếm xảy ra hoặc ít dấu hiệu cho thấy sẽ xảy ra |
| 2 | Vừa | Thỉnh thoảng xảy ra hoặc có căn cứ hợp lý để dự kiến |
| 3 | Cao | Thường xuyên xảy ra hoặc hiện có nhiều dấu hiệu đáng chú ý |

**Ma trận xác định mức rủi ro theo cuối PDF**

| Xác suất \ Tác động | Thấp (1) | Vừa (2) | Cao (3) |
|---|---:|---:|---:|
| Thấp (1) | Mức 1 | Mức 2 | Mức 3 |
| Vừa (2) | Mức 2 | Mức 3 | Mức 4 |
| Cao (3) | Mức 3 | Mức 4 | Mức 5 |

Khi dùng ma trận này, **mức 1 thấp nhất, mức 5 nghiêm trọng nhất**. Có thể viết lại nhãn theo thứ tự nhất quán: **1 — hầu như không ảnh hưởng; 2 — ảnh hưởng không đáng kể; 3 — ảnh hưởng nhưng dự án vẫn thực hiện được; 4 — ảnh hưởng đáng kể; 5 — có thể khiến dự án không thể tiếp tục**.

**Ví dụ bảng rủi ro đã điền**

Các điểm dưới đây là đánh giá minh họa cho bài toán mẫu.

| Mã | Mô tả | Xác suất | Tác động | Mức theo ma trận | Hành động ngăn ngừa | Phụ trách |
|---|---|---:|---:|---:|---|---|
| R01 | Thay đổi quy tắc tính phí sau thiết kế, gây sửa lại chức năng | 2 | 3 | 4 | Xác nhận quy tắc và ví dụ tính phí trước lập trình | An |
| R02 | Lập trình viên nghỉ hoặc bị điều sang dự án khác | 1 | 2 | 2 | Chia sẻ kiến thức, cập nhật mã nguồn và chuẩn bị bàn giao | An |
| R03 | Tài liệu kỹ thuật chưa hoàn thiện khi bàn giao | 1 | 3 | 3 | Giao người viết, rà soát tài liệu tại từng mốc | Bình |
| R04 | Khách hàng không bố trí người dùng thử đúng lịch | 2 | 2 | 3 | Chốt lịch và người thay thế trước mốc 30/11 | An |
| R05 | Ước lượng công sức quá thấp, làm thiếu thời gian hoàn thiện | 2 | 2 | 3 | Rà soát ước lượng theo WBS và khả năng nhân lực | An, Chi |

**Ví dụ liên kết đầy đủ giữa các thuộc tính**

R01 xuất phát từ giả định trong tuyên ngôn rằng yêu cầu đã thống nhất sẽ ổn định. Rủi ro ảnh hưởng đến gói WBS **Tạo khoản thu**, vì quy tắc tính phí quyết định dữ liệu cần lưu và cách xử lý.

Nhóm đánh giá xác suất **2**, tác động **3**, rồi tra ma trận được **mức 4**. Vì vậy, An bố trí hành động ngăn ngừa: cùng khách hàng rà soát các tình huống tính phí trước khi thiết kế được xác nhận.

Nếu khách hàng gửi quy tắc mới sau thời điểm đó, dấu hiệu kích hoạt xuất hiện. Nhóm đánh giá phần thiết kế, lập trình và kiểm thử phải làm lại; sau đó xác định ảnh hưởng đến lịch Gantt, mốc 30/11 và ngân sách. Kết quả xử lý được ghi vào trạng thái rủi ro và báo cáo tiến độ.

**Cách kiểm tra sản phẩm:** Mỗi rủi ro phải có sự kiện và hậu quả rõ; điểm đánh giá phải theo cùng một thang; hành động phải giải quyết đúng nguyên nhân; người phụ trách phải biết khi nào cần hành động.

</details>
