# Memo Teardown — Notion

**Nhóm:** Hello world      
| Họ và tên | Mã sinh viên |
|---|---|
| Nguyễn Minh Hiếu | 2A202601154 |
| Nguyễn Ngọc Chi | 2A202602024 |
| Trần Thanh Huyền | 2A202601578 |
| Thiều Thị Ngọc Ánh | 2A202601864 |
 

**Phạm vi phân tích:** Notion như một **AI-powered workspace** — nơi lưu trữ tài liệu, dự án, meeting notes và tri thức của cá nhân/đội nhóm, sau đó dùng AI để tìm kiếm, tổng hợp và thực hiện công việc.

**Vì sao chọn sản phẩm này:** Notion có chuỗi quyết định sản phẩm rõ: từ workspace linh hoạt, đến AI viết/chỉnh sửa, Q&A trên dữ liệu nội bộ, kết nối các công cụ khác, rồi chuyển sang AI Meeting Notes, Enterprise Search và Agents. Sản phẩm cũng có hai tệp user dễ so sánh: power users/nhóm startup ban đầu và các team/doanh nghiệp hiện tại.

## §1. Timeline các cập nhật lớn

| Thời điểm | Cập nhật | Context lúc đó | Nguyên lý |
|---|---|---|---|
| 2018 | **Notion 2.0 ra mắt trên Product Hunt**, trở thành một lần relaunch quan trọng của sản phẩm. [Nguồn](https://www.producthunt.com/stories/the-makings-of-a-notion-product-and-launching-it-on-product-hunt?comment=1446291) | Notion cần tìm lại traction và tiếp cận nhóm người dùng thích tự xây công cụ làm việc. Product Hunt tạo kênh tiếp cận early adopters có khả năng thử sản phẩm mới và chia sẻ lại cho cộng đồng. | **Composable primitives → workflow moat:** thay vì bán một công cụ đơn chức năng, Notion cung cấp các building block có thể ghép thành wiki, task manager, project tracker hoặc CRM nhẹ. Càng nhiều workflow được xây trên đó, chi phí rời đi càng tăng. |
| 11/2022 | **Notion AI private alpha** được mở, đưa AI trực tiếp vào workspace. [Nguồn](https://www.notion.com/blog/introducing-notion-ai) | GPT-4 và làn sóng generative AI làm thay đổi kỳ vọng về phần mềm năng suất. Notion có sẵn nơi người dùng viết và lưu dữ liệu, nên không cần bắt đầu bằng một chatbot độc lập. | **Context before generation:** AI có giá trị hơn khi nằm ngay trong nơi user đang làm việc và có sẵn context; wrapper chỉ có sức mạnh khi tận dụng được workflow/data riêng. |
| 02/2023 | **Notion AI mở cho mọi người**, đồng thời chuyển trọng tâm từ tạo nội dung mới sang cải thiện nội dung người dùng đã viết. [Nguồn](https://www.notion.com/blog/notion-ai-is-here-for-everyone) | Alpha cho thấy người dùng không thường xuyên yêu cầu AI viết mọi thứ từ đầu; hành vi lặp lại nhiều nhất là highlight nội dung và chọn “Improve writing”. | **Learning loop / definition of good:** không cố chấp với giả định ban đầu về use case; dùng hành vi thực tế để định nghĩa “AI tốt” là cộng tác viên chỉnh sửa, tóm tắt và khai mở ý tưởng — không nhất thiết thay thế người viết. |
| 11/2023 | **Notion Q&A beta** ra mắt, cho phép hỏi đáp trên tài liệu, dự án, meeting notes và dữ liệu trong workspace. [Nguồn](https://www.notion.com/blog/introducing-q-and-a?slug=introducing-q-and-a) | Khi workspace đã tích lũy nhiều trang và database, vấn đề lớn không còn là tạo nội dung mà là tìm đúng thông tin. Notion chuyển AI từ writing assistant sang knowledge assistant. | **Data gravity / context moat:** dữ liệu càng được lưu có cấu trúc trong sản phẩm, AI càng hữu ích; AI trở thành lý do để quay lại workspace và củng cố giá trị của dữ liệu đã tích lũy. |
| 01/2024 | **Notion Calendar** ra mắt, liên kết lịch, deadline trong database, tài liệu và meeting context. [Nguồn](https://www.notion.com/releases/2024-01-17) | Notion đã sở hữu tài liệu và project context nhưng thời gian, lịch họp và deadline vẫn nằm ở công cụ khác. Calendar là bước mở rộng sang workflow liền kề thay vì chỉ cải thiện editor. | **Own the adjacent workflow:** mở rộng sang bước kế bên trong cùng công việc để giảm context switching; tài liệu, task, deadline và meeting có thể tạo thành một hệ thống thống nhất. |
| 07/2024 | **Notion AI hợp nhất chat/search**, bổ sung one-click AI skills, tìm thông tin từ Notion/Slack và gọi AI từ ngoài ứng dụng bằng global shortcut. [Nguồn](https://www.notion.com/releases/2024-07-29) | User không muốn học prompt phức tạp hoặc rời ứng dụng đang làm việc. Notion đưa AI gần hơn với hành động hằng ngày và bắt đầu mở rộng context ra các công cụ khác. | **AI as the interface to the system of work:** AI không chỉ là một nút viết; nó trở thành lớp giao diện để truy vấn và biến dữ liệu trong nhiều công cụ thành hành động. |
| 05/2025 | **Notion 2.51** đưa AI Meeting Notes, Enterprise Search, Research Mode và các connector vào trung tâm; Business/Enterprise có gói AI bao gồm các khả năng này. [Nguồn](https://www.notion.com/releases/2025-05-13) | Notion chuyển rõ từ công cụ cá nhân/team nhỏ sang hạ tầng tri thức cho doanh nghiệp. Các công ty cần tìm thông tin xuyên Slack, Drive, Microsoft, Jira… và cần kiểm soát quyền truy cập. | **Vertical AI / land-and-expand:** bắt đầu từ workflow quen thuộc của một nhóm, sau đó bán giá trị ở cấp doanh nghiệp bằng dữ liệu, governance, connector và use case cụ thể như onboarding, research, meeting memory. |
| 09/2025 | **Notion 3.0 đưa AI Agents vào trung tâm**, cho phép Agent tạo docs, xây database, tìm kiếm qua công cụ và thực hiện workflow nhiều bước. [Nguồn](https://www.notion.com/blog/introducing-notion-3-0) | Khi AI đã có quyền truy cập vào workspace, bước tiếp theo là để AI không chỉ trả lời mà còn thực hiện các phần việc lặp lại. Đây là chuyển dịch từ assistant sang execution. | **Assist → execute:** khi model đủ tốt, giá trị chuyển từ “giúp tôi viết” sang “giúp tôi hoàn thành outcome”; moat nằm ở context, permission và workflow chứ không chỉ ở model. |

### Vì sao chọn những mốc này

Nhóm chọn các mốc thể hiện thay đổi về **định vị, workflow, user segment hoặc mô hình AI**, thay vì liệt kê các bản sửa lỗi và cập nhật giao diện. Có thể loại các mốc như template mới, cải thiện mobile hoặc thay đổi nhỏ của database vì chúng không làm thay đổi đáng kể câu trả lời cho ba câu hỏi: Notion phục vụ ai, giải quyết việc gì và tạo moat ở đâu. Chuỗi mốc cho thấy ba lần chuyển quan trọng: từ workspace linh hoạt → AI cộng tác trong nội dung → AI truy cập và thực hiện trên hệ thống tri thức của team.

## §2. Tệp user & JTBD

| | Early adopters | Tệp hiện tại |
|---|---|---|
| **Đặc điểm** | Founder, product manager, designer hoặc engineer ở startup nhỏ; thường dùng nhiều công cụ, thích tự thiết kế workflow, chấp nhận bỏ thời gian học database/template để đổi lấy sự linh hoạt. Họ dễ xuất hiện ở Product Hunt, cộng đồng startup, template community và các kênh chia sẻ workflow. | Team 10–1.000+ người trong Product, Marketing, HR, Sales, Support và Operations; cần một nơi chung cho docs, project, meeting notes và company knowledge. Cá nhân/student/creator vẫn là nhóm lớn, nhưng hướng AI/enterprise hiện tại tập trung vào team và tổ chức. G2 hiện phân loại Notion cho project management, enterprise search, note-taking và AI writing, với review từ small business đến enterprise. [Nguồn](https://www.g2.com/products/notion/reviews) |
| **JTBD chính** | “Khi công cụ hiện tại quá rời rạc hoặc cứng nhắc, tôi muốn tự xây một hệ thống ghi chú–project–database phù hợp với cách làm việc của mình để mọi thứ nằm cùng một nơi.” | “Khi thông tin và quyết định bị phân tán trong docs, Slack, email, lịch và các công cụ project, tôi muốn tìm câu trả lời, tóm tắt context và biến nó thành hành động nhanh để team không phải làm ‘work about work’.” |
| **Trước đó họ làm bằng cách nào** | Kết hợp Google Docs/Drive, Trello hoặc Asana, spreadsheets, Evernote và các công cụ riêng lẻ; thường tự nối bằng link, folder và template. | Google Docs/Drive cho tài liệu, Slack để hỏi người khác, Asana/Jira/Linear để theo dõi dự án, Google Calendar cho lịch và ghi chú họp rải rác. Case study của Remote mô tả Notion được dùng như một “single source of truth” thay cho nhiều công cụ, trong đó Q&A giúp nhân viên tìm thông tin nhanh hơn. [Nguồn](https://www.notion.com/blog/remote-notion) |

### Dịch chuyển tệp

Mốc **Notion 2.0/Product Hunt (2018)** giúp Notion thu hút power users và startup builders — những người sẵn sàng tự lắp ghép workspace. Từ mốc **Q&A (2023)**, **Enterprise Search/AI Meeting Notes (2025)** và **Agents (2025)**, sản phẩm chuyển thêm giá trị sang team/doanh nghiệp: không chỉ “tôi tổ chức ghi chú thế nào” mà là “cả công ty tìm và sử dụng tri thức thế nào”. Notion Calendar và Notion Mail cũng mở rộng phạm vi từ tài liệu sang thời gian và giao tiếp.

### Switching cost — 4 forces

| Lực | Phân tích với Notion |
|---|---|
| **Push — vấn đề với giải pháp hiện tại** | Tài liệu, task, meeting notes và quyết định nằm ở nhiều nơi; tìm thông tin tốn thời gian; team lặp lại cùng một câu hỏi; người mới khó biết context. Đây là “work about work” mà Q&A, Enterprise Search và Research Mode nhắm tới. |
| **Pull — sức hút của giải pháp mới** | Một workspace linh hoạt, template/database có thể tùy biến, AI viết–tóm tắt–tìm kiếm–nghiên cứu, Meeting Notes và Agent. Người dùng không chỉ nhận câu trả lời mà còn giữ câu trả lời trong cùng nơi họ quản lý công việc. |
| **Habit — thói quen cũ** | Team đã quen với cấu trúc page, database, template, shortcut và quy ước ghi chép trong Notion. Những thói quen này tạo ra “muscle memory”, đồng thời khiến việc chuyển sang công cụ khác đòi hỏi đào tạo lại cả team. |
| **Anxiety — nỗi lo khi chuyển đổi** | Mất dữ liệu hoặc link giữa các page; tốn công migrate và thiết kế lại workspace; learning curve cao; lo về quyền truy cập, dữ liệu AI, hiệu năng của database lớn và khả năng offline. Các review cộng đồng cũng nhắc tới setup overhead, performance và offline như trade-off của sự linh hoạt. [Nguồn](https://www.producthunt.com/products/notion/reviews) |

**Lực giữ user mạnh nhất:**  habit. Khi docs, database, project history, meeting notes và template của cả team đã ở trong Notion, sản phẩm không còn chỉ là một app ghi chú; nó trở thành bộ nhớ vận hành của tổ chức. Nếu lực này biến mất — ví dụ dữ liệu được di chuyển dễ dàng, quyền truy cập và liên kết không còn tốt hơn đối thủ — Notion sẽ phải cạnh tranh nhiều hơn bằng tính năng AI thuần túy, nơi moat mỏng hơn.

## §3. Ba dự đoán hướng đi (6–12 tháng tới)

### Dự đoán 1 — Mở rộng tính năng

- **Dự đoán:** Notion sẽ phát triển AI Agent từ trợ lý cá nhân thành các **Custom Agents cho từng team/workflow**, có thể tự động xử lý công việc xuyên Notion, email, lịch và các công cụ bên ngoài.
- **Lập luận:** §1 cho thấy Notion đi từ AI viết/chỉnh sửa → Q&A → Search/Connectors → Agents. §2 cho thấy user hiện tại cần giảm việc tìm kiếm và phối hợp giữa nhiều công cụ. Vì vậy bước hợp lý tiếp theo là đóng gói các quy trình lặp lại như onboarding, weekly update, research brief hoặc triage thành Agent dùng chung cho team.

### Dự đoán 2 — Mở rộng segment

- **Dự đoán:** Notion sẽ đẩy mạnh nhóm khách hàng **doanh nghiệp và các phòng ban chuyên biệt** như Product, Sales, Customer Support, HR và Operations.
- **Lập luận:** §1 ghi nhận Enterprise Search, AI Meeting Notes, Research Mode và connector được đưa vào Business/Enterprise; §2 cho thấy tệp hiện tại cần một knowledge hub thay cho việc hỏi người khác hoặc tìm ở nhiều ứng dụng. Khi Notion có context và quyền truy cập của từng phòng ban, họ có thể bán outcome cụ thể như onboarding nhanh hơn, trả lời khách hàng nhất quán hơn và giảm thời gian chuẩn bị báo cáo.

### Dự đoán 3 — Mô hình kiếm tiền và phòng thủ trước Big Tech

- **Dự đoán:** Notion sẽ kiếm tiền và phòng thủ trước Google/Microsoft chủ yếu bằng **AI cấp doanh nghiệp**: governance, permission-aware search, connector, auditability và Agent theo workflow — thay vì cố thắng bằng một model nền tảng riêng.
- **Lập luận:** §1 cho thấy Notion đã gắn AI với dữ liệu workspace, connector và kế hoạch Business/Enterprise; §2 cho thấy switching cost mạnh nhất là dữ liệu có cấu trúc và workflow của team. Google/Microsoft có thể cung cấp AI trong từng app, nhưng Notion có lý do để tập trung vào lớp context xuyên công cụ và cách team tổ chức tri thức. Đây là hướng moat mà model tốt hơn một chút không dễ thay thế ngay.

**Dự đoán tự tin nhất:** Dự đoán 1. Giả định có thể làm dự đoán này gãy là Agent không đủ đáng tin để tự thực hiện workflow, hoặc chi phí kiểm tra/sửa output cao hơn thời gian tiết kiệm được. Nếu giả định đó sai, Notion có thể quay lại ưu tiên Search, Meeting Notes và các AI copilot có human-in-the-loop thay vì tự động hóa nhiều bước.

## §4. AI Log

| Việc | AI làm hay nhóm làm? | Nhóm kiểm chứng/phán đoán lại thế nào? |
|---|---|---|
| Đề xuất các sản phẩm phù hợp với đề bài | AI hỗ trợ đề xuất; **nhóm quyết định chọn Notion** | Nhóm đối chiếu ba tiêu chí của đề: AI đóng vai trò lớn, có ít nhất 6 mốc công khai và JTBD rõ. |
| Tìm và tóm tắt các mốc timeline | AI hỗ trợ tìm kiếm/tổng hợp từ changelog và blog | Nhóm mở lại từng link nguồn gốc của Notion, giữ các mốc làm thay đổi định vị/workflow/segment và loại các cập nhật nhỏ. |
| Viết context và gợi ý nguyên lý cho từng mốc | AI tạo bản nháp | Nhóm đọc chéo để chuyển nhãn chung chung thành nguyên lý có tên như “context before generation”, “learning loop”, “data gravity” và “assist → execute”. |
| Xác định early adopters, tệp hiện tại và JTBD | AI tổng hợp giả thuyết từ Product Hunt, G2 và case study của Notion | Nhóm phân biệt dữ kiện nguồn với suy luận: segment và JTBD được viết cụ thể, đồng thời nối segment-shift về các mốc Q&A, Enterprise Search và Agents. |
| Viết 3 dự đoán 6–12 tháng | AI đề xuất các hướng có thể xảy ra | **Nhóm chịu trách nhiệm phán đoán cuối cùng**; mỗi dự đoán được giữ lại chỉ khi dẫn được về ít nhất một mốc ở §1 và một nhận định user/JTBD ở §2. |
| Biên tập memo theo template và kiểm tra checklist | AI hỗ trợ định dạng | Nhóm kiểm tra lại đủ 6–8 mốc, link nguồn, 4 forces, 3 dự đoán, phần kiểm chứng và các placeholder tên nhóm/thành viên trước khi nộp. |
