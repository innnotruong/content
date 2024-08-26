---
tags:
  - office-hours
  - ogif
  - discord
title: "OGIF Office Hours #20 - Golang weekly, Modeling dynamic object properties, Devbox demo, LLM tracing, Cursor AI editor"
date: 2024-08-26
description: Our latest OGIF session covers key topics such as Go 1.23 and the introduction of Go Notebook, dynamic object modeling inspired by Notion, advanced LLM tracing techniques, Devbox demo and a hands-on look at the Cursor AI code editor. By sharing weekly topics chosen through tags, we foster a collaborative learning environment for our community to grow.
authors:
  - innno_
---

97 minutes

### Topics & Highlights

**00:00 - Introduction and Setup**

Kickoff of the session with attendance check and agenda setup.

**00:10:57 - Golang Commentary**

Discussion on Go 1.23, including Go Notebook, a Jupyter-like environment for Go, and performance optimization techniques.

**00:17:54 - Modeling Dynamic Object Properties**

Analysis of structuring dynamic properties inspired by Notion, focusing on separating model and field data into distinct database tables.

**00:40:11 - LLM Tracing**

Exploration of tracing and evaluating large language models (LLMs) with tools like phonic, ensuring outputs meet user expectations with metrics like latency and relevance.

**01:18:34 - Tooling: Cursor AI Editor**

Introduction to Cursor AI, an AI-powered code editor offering advanced features for code generation and project context management.

**01:36:07 - Summary and Concluding Thoughts**

Wrap-up of the session with key takeaways and final thoughts.

---

### Vietnamse Transcript 

**00:00** - Ok, chắc đủ rồi, bắt đầu nhé. Anh em khác chắc sẽ vào dần. Phát ơi, bắt đầu phần Go của em đi. Ok, mọi người nghe rõ chưa? Nghe rồi đúng không? Ok, vậy thì em sẽ bắt đầu như thế này. Đầu tiên là tuần này em có thấy một vài cái tool khá hay. Về tin tức thì cũng không có gì mới, chỉ có việc Go 1.23 đã release thôi. Đầu tiên là có cái Go Notebook, nó giống như thằng Jupyter mà mọi người biết, Jupyter là một công cụ đã ra mắt từ lâu bên Python, thường dùng cho mấy anh em hay làm machine learning hoặc data analysis. Bây giờ, Go cũng có một phiên bản tương tự, cho phép mình sử dụng Go ngay trong môi trường notebook như vậy. Mọi người có thể chạy nó local, thậm chí có thể build Docker container và chạy nó trong đó.

**10:57** - Go Notebook cũng có một số tính năng như vẽ biểu đồ (widget plot), khá giống với Jupyter, thậm chí còn nhanh hơn khi build và chạy Go local. Em đã test thử và thấy khá nhanh, thậm chí nhanh hơn Jupyter luôn. Hồi trước em có thử Jupyter thì thấy nó khá chậm. Tool thứ hai là "kuam", một công cụ hỗ trợ cho anh em dùng bên Nexttop. Kuam có chức năng stream những file cấu hình (config) không cần thiết trong project. Bình thường, nếu không có kuam, khi list ra các config mà không được sử dụng hoặc không kết nối được, mình phải tự xóa bằng tay trong file. Còn với kuam, nó sẽ tự động loại bỏ những cấu hình không cần thiết đó cho mình, và cũng có tùy chọn để quyết định có lưu vào file config hay không.

<iframe width="560" height="315" src="https://www.youtube.com/embed/S_y5IrBhfNQ?si=ys80zw6NTvFBIotT&amp;start=620" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

**11:44** - Tuần trước thì em có xem qua một số video từ bên UK, khá hay. Tình hình chung bên châu Âu, cộng đồng Go vẫn đang tập trung vào các vấn đề như testing performance, họ không chỉ đơn giản là đo đạc hiệu năng mà còn kiểm tra cách hệ thống hoạt động ra sao, có cả những đoạn liên quan đến CPU và GPU performance. Bên cạnh đó, có một bài về Software Design Complexity, bài này nói về việc thiết kế hệ thống sao cho đơn giản mà vẫn hiệu quả. Đối với những hệ thống lớn, cần nhiều component khác nhau, họ phải cân nhắc giữa độ phức tạp và hiệu quả của nó. Ý cuối cùng trong các bài này là về AI, nói chung, mấy bác Goer vẫn đang dùng AI ở mức cơ bản. Có một bài của một bác bên Microsoft cũng ok, nói về việc sử dụng AI để hỗ trợ code, nhưng cũng chỉ dừng lại ở mức cơ bản.

**14:56** - Ok, anh em có câu hỏi gì cho phần review của Phát không? Có ai muốn hỏi gì không?

**15:44** - À, về cái Oscar thì sao nhỉ? Tuần trước hay hai tuần trước mình có nói về nó rồi mà, còn nhớ không? Con Oscar và con Gasp, Oscar là một dự án lớn nha. Bài tuần trước có liên kết đến kiến trúc (architecture) của nó. Nó là một cái agent, giống như mấy cái của anh Tom làm, nhưng chủ yếu là bên Dr. By chỉ mới show cái architecture thôi, chưa chi tiết lắm. Để em kiếm lại rồi gửi link post lên sau. Còn code thì có, nhưng code của con Gasp thì không có public, nó nằm trong repo internal của Google, em sẽ gửi link sau nếu cần.

**16:53** - Việc bên đó rồi, chắc sẽ viết xong sớm thôi. Em đang chuẩn bị viết một cái module hoặc một cái OS theo cách hướng dẫn đó, giống như cái anh đã nói, có lẽ sẽ hoàn thành vào tuần sau đúng không? Có gì cần thì anh em cứ sẵn sàng thôi. Em nghe nói Phát đang phải code vô kích đấy, hơi bất ngờ nhưng mà kiểu như mấy cái start thì cũng tạm ổn thôi. Ok, cảm ơn Phát nhé. Rồi, tiếp theo chúng ta sẽ đến với một chủ đề liên quan đến việc lập hồ sơ. Cái này em đã share với anh em trong team một lần rồi thì phải. Đây là liên quan đến việc tạo ra dynamic object trong project.

**17:54** - Giống như bên Notion. Dạ, đúng rồi. Ok, đợi chút nhé. Cái này chắc bên đó làm được, để xem nào. Sẵn sàng chưa? Chắc là bên đó có thể lên production được rồi đúng không? Lên rồi, kiểu như mình đang dùng bản product thôi mà. Ok, vậy chắc để em chia sẻ màn hình cho mọi người xem. Mọi người thấy màn hình em chưa? Thấy rồi đúng không? Ok, chủ đề này là về việc mô hình hóa (modeling) các object động (dynamic objects). Về cơ bản, mục tiêu là chúng ta muốn tạo ra một object có khả năng mở rộng (extendable) như trong Notion, tức là có các field mà chúng ta có thể mở rộng hoặc thay đổi.

**18:54** - Vậy làm sao để chúng ta có thể mô hình hóa (model) được điều này? Bên đây, em đã có một cái database setup sẵn. Khi bắt đầu, chúng em đã đưa ra hai quyết định quan trọng trong việc mô hình hóa (modeling) hệ thống này. Thứ nhất, bản thân model chính và các field của nó phải được tách ra thành hai bảng (table) riêng biệt. Điều này là cần thiết vì nếu chúng ta muốn mở rộng danh sách các thuộc tính (property), chúng ta cần lưu các field này trong một bảng riêng.

<iframe width="560" height="315" src="https://www.youtube.com/embed/S_y5IrBhfNQ?si=R079FoyaHgmzrKsO&amp;start=1118" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

**19:44** - Ví dụ, giả sử chúng ta có một task, task này sẽ không chứa bất kỳ field nào trực tiếp. Thay vào đó, chúng ta sẽ có một bảng field riêng biệt. Trong bảng field này, sẽ có các thông tin như field type (kiểu dữ liệu của field), ví dụ như text, checkbox, hay select (multi-select). Tên (name) của field và các tùy chọn (option) của nó sẽ được lưu trữ trong một bảng riêng khác. Điều này cho phép chúng ta linh hoạt hơn trong việc thêm các option cho field một cách động (dynamic).

**20:23** - Nếu mọi người nhìn vào thì sẽ thấy hiện tại task và field này không có mối quan hệ trực tiếp nào với nhau. Thay vì tạo ra một quan hệ (relationship) trực tiếp giữa task và field, chúng em đã chọn cách sử dụng một bảng trung gian là bảng value. Bảng value này đóng vai trò là cầu nối giữa task và danh sách các field. Điều đó có nghĩa là khi thêm một field vào task, chúng ta không thực sự thêm field đó trực tiếp vào task, mà là thêm một record (bản ghi) vào bảng value. Record này sẽ liên kết task với field tương ứng.

**21:00** - Ở trong bảng value này, chúng em cũng đã mô hình hóa (model) theo kiểu linh hoạt bởi vì field type có rất nhiều dạng khác nhau như em đã nói: text, boolean, select, hay user. Mỗi loại value sẽ có một cột riêng biệt trong bảng value, ví dụ như cột dành cho text, cột dành cho boolean, cột dành cho select hay cột dành cho user. Điều này cho phép chúng ta linh hoạt hơn trong việc xử lý các loại dữ liệu khác nhau trong hệ thống của mình.

**21:33** - Đối với mỗi loại giá trị (value) khác nhau như text, boolean, và các loại khác, tụi em đều tạo một cột (column) riêng biệt trong bảng value. Ví dụ, cột cho text, cột cho boolean, cột cho select, hay cột cho user. Điều này có nghĩa là mình cũng hoàn toàn có thể kết nối các giá trị này với các bảng khác trong database của mình. Đây là quyết định đầu tiên mà tụi em đưa ra khi thiết kế hệ thống này.

Tại sao tụi em lại không tạo mối quan hệ trực tiếp (direct relationship) giữa task và field? Lý do là vì tụi em muốn các field này hoạt động như một cấu hình toàn cầu (global configuration). Khi một field mới được tạo ra, tất cả các task có thể sử dụng lại field này mà không cần phải tạo ra một mối quan hệ chặt chẽ. Mối quan hệ giữa task và field sẽ rất lỏng lẻo và tất cả các thao tác đều được xử lý thông qua bảng value. Khi xóa một giá trị trong bảng value, field trong task tương ứng cũng sẽ biến mất, nhưng field đó vẫn tồn tại cho các task khác.

**22:46** - Em nghĩ là vậy thôi. Ví dụ, nếu em tạo một task mới và muốn thêm một field select, khi em gõ chữ 'tag', hệ thống sẽ hiện lên các field đã tồn tại, và em có thể thêm field 'tag' đã tồn tại này vào task mới, đồng thời kế thừa luôn các option mà field này đã có. Nhìn chung thì hệ thống này cũng hoạt động khá nhanh.

**23:32** - Còn về các thao tác khác thì sao? Ví dụ như trong Notion, nó sẽ có các thao tác như sorting (sắp xếp), filtering (lọc) các field. Do các field này được lưu trữ trong một bảng riêng (table riêng), nếu muốn sắp xếp (sort) thì chỉ cần thêm một cột sort order vào bảng field. Khi điều chỉnh sort order này, nó sẽ tự động cập nhật cho toàn bộ workspace. Thực tế, hiện tại hệ thống của em chưa có task cụ thể để thử nghiệm, nhưng em nghĩ rằng nó sẽ hoạt động cho toàn bộ workspace.

**24:20** - Hiện tại, tụi em chưa nghĩ đến việc lưu sort order riêng cho từng task, vì điều này sẽ rất phức tạp. Sort order này hiện tại là toàn cục (global). Có một số thách thức khi sử dụng mô hình này, đó là lúc query, tụi em phải join rất nhiều bảng (tables) khác nhau và cần phải xử lý việc lọc (filter) và phân trang (pagination) các dữ liệu này. Với hạ tầng hiện tại của tụi em, sử dụng Prisma không thể xử lý được, nên tụi em phải viết raw SQL để thực hiện các truy vấn phức tạp này. Đây là một khó khăn lớn.

**24:59** - Một vấn đề khác là khi làm việc cross-organization hoặc cross-workspace, như khi mời guest từ tổ chức khác vào, việc quản lý các field này, đặc biệt là liên quan đến quyền truy cập (permission), rất phức tạp. Các field này chỉ thuộc về một tổ chức cụ thể, nên khi mời guest vào, vấn đề quản lý quyền truy cập trở nên rất rối rắm. Khi tụi em thiết kế hệ thống này, chưa tính đến việc cross-space, nên hiện tại đang phải tìm cách giải quyết tạm thời để nó hoạt động. Tuy nhiên, đây vẫn là một vấn đề tồn tại trong hạ tầng hiện tại của dự án.

**25:33** - Một vấn đề khác là giống như trong Notion, khi mình muốn di chuyển hoặc copy một trang từ bảng này sang bảng khác, bảng mới sẽ có một set property khác so với bảng gốc. Hiện tại, các field được lưu trữ ở cấp độ workspace hoặc organization, không phải ở cấp độ bảng (table). Điều này có nghĩa là các field này được dùng chung cho toàn bộ workspace.

**26:08** - Một cách để giải quyết vấn đề này là chuyển đổi giữa các workspace trong cùng một organization, như trong Notion. Khi guest vào, họ vẫn có thể thấy các task trong workspace của họ và các task từ các workspace khác nếu chúng được chia sẻ chung. Tuy nhiên, vấn đề xuất hiện khi hệ thống chia sẻ cùng một set field cho nhiều workspace khác nhau trong cùng một organization, gây ra sự xung đột về quyền truy cập và quản lý.

**26:51** - Các field này hiện đang được kết nối trực tiếp với tổ chức (organization) thay vì với workspace, cho nên các field này được sử dụng chung cho toàn bộ workspace. Có thể có cách giải quyết vấn đề này là cho phép người dùng chuyển đổi trực tiếp giữa các workspace, giống như trong Notion. Điều này có nghĩa là khi người dùng truy cập vào, về bản chất thì toàn bộ organization vẫn thuộc quyền quản lý của mình. Nhưng hiện tại, hệ thống đang cho phép guest truy cập vào và thấy tất cả các task trong tổ chức của họ, cũng như các task từ các tổ chức khác mà họ được mời tham gia. Điều này dẫn đến việc các dữ liệu bị chia sẻ chung giữa các tổ chức, gây ra sự xung đột.

**27:31** - Nếu mình sử dụng cách tiếp cận riêng biệt thì sẽ không gặp vấn đề này. Nhưng thực chất, điều này bắt nguồn từ việc các task chỉ là một thực thể của hệ thống lịch (calendar entity), đúng không?

**28:26** - So với các block trong Notion, thì các block của Notion được xây dựng dựa trên kiến trúc từ block lên (bottom-up architecture). Còn hệ thống này thì chỉ là một mô phỏng đơn giản (mockup) chứ không thực sự có liên quan nhiều đến block. Đây chỉ là một mô phỏng để hệ thống có thể hoạt động theo cách riêng của nó.

**29:54** - Để hệ thống hoạt động một cách hợp lý, chúng ta cần đảm bảo rằng mối quan hệ giữa các field và các giá trị (value) là rõ ràng và không bị nhầm lẫn. Điều này bao gồm việc tránh các vòng lặp (loops) trong thiết kế dữ liệu. Một vòng lặp trong thiết kế chỉ nên tồn tại khi nó thực sự cần thiết để tối ưu hóa truy vấn (query) hoặc các tác vụ khác. Tuy nhiên, phải nhận thức được rằng vòng lặp này có thể dẫn đến nhiều khó khăn trong việc bảo trì và phát triển hệ thống. Khi người khác nhìn vào thiết kế này, họ cần phải hiểu được mục đích của vòng lặp là gì và nó không nên bị nhầm lẫn với các mục đích khác.

**35:03** - Nếu mình muốn loại bỏ vòng lặp này, mình cần phải tái cấu trúc lại hệ thống để đảm bảo rằng các quan hệ trong hệ thống là minh bạch và dễ hiểu. Thực tế, đã có nhiều bài viết và thảo luận về chủ đề này, và mình sẽ cần phải nghiên cứu thêm để đưa ra quyết định cuối cùng.

**35:51** - Một phần mình còn đang băn khoăn là nếu giữ vòng lặp như hiện tại, khi người dùng xóa một option của một field, thì tất cả các task đang sử dụng option này sẽ tự động được cập nhật và loại bỏ option đó khỏi database. Điều này có nghĩa là mình không cần phải thực hiện lại việc kiểm tra tính hợp lệ (revalidation) cho các task đó. Nếu giữ vòng lặp này, việc quản lý sẽ trở nên đơn giản hơn, nhưng nó có thể dẫn đến các vấn đề khác về lâu dài.

**37:07** - Cần cân nhắc kỹ lưỡng xem liệu có nên giữ vòng lặp này hay không, hoặc nên tái cấu trúc lại để tránh các vấn đề phức tạp trong tương lai. Việc quyết định giữ vòng lặp hay loại bỏ nó có thể phụ thuộc vào cách mà hệ thống được sử dụng và quản lý. Nếu quyết định giữ vòng lặp, chúng ta cần đảm bảo rằng nó được thiết kế một cách rõ ràng và có thể dễ dàng quản lý và bảo trì.

**39:03** - Một phần khác của buổi thảo luận hôm nay sẽ tập trung vào việc giới thiệu một số công cụ mới để theo dõi và kiểm tra hệ thống (tracing tools). Điều này rất cần thiết trong quá trình phát triển và bảo trì các phần mềm lớn, đặc biệt là khi chúng ta cần theo dõi từng bước hoạt động của hệ thống để đảm bảo mọi thứ diễn ra suôn sẻ.

<iframe width="560" height="315" src="https://www.youtube.com/embed/S_y5IrBhfNQ?si=z8OG5iFWwefkGDBj&amp;start=2388" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

**40:11** - Khi phát triển một hệ thống sử dụng machine learning (ML), quá trình thường sẽ bao gồm các bước như lên ý tưởng, lựa chọn mô hình, tùy chỉnh (customization), sau đó là triển khai (deploy). Bước cuối cùng, giống như với phần mềm truyền thống, là giám sát (monitoring) và thu thập phản hồi (feedback) để cải tiến hệ thống. Đối với phần mềm truyền thống, sự khác biệt nằm ở chỗ chúng ta đã biết trước đầu ra (output) sẽ như thế nào và có thể xác định được nó dựa trên đầu vào (input). Tuy nhiên, đối với phần mềm tích hợp machine learning, kết quả đầu ra thường mang tính xác suất. Điều này có nghĩa là khi người dùng nhập liệu (input), kết quả trả về (output) có thể thay đổi tùy thuộc vào mô hình hoặc cấu hình mô hình mà chúng ta sử dụng. Vì vậy, việc theo dõi (tracing) trở nên cực kỳ quan trọng sau khi triển khai, để đảm bảo rằng các kết quả đầu ra của phần mềm đáp ứng được kỳ vọng của người dùng.

**40:50** - Một điểm đặc trưng của hệ thống tích hợp ML là sự không chắc chắn trong kết quả đầu ra. Ví dụ, khi người dùng nhập liệu vào hệ thống, kết quả trả về có thể khác nhau tùy thuộc vào cách mô hình được tùy chỉnh (customized) hoặc cấu hình (tuned). Do đó, hệ thống theo dõi (tracing) cần phải giúp chúng ta hiểu rõ hơn về quá trình xử lý và xác định xem liệu các kết quả có đáp ứng kỳ vọng không, có vi phạm các quy tắc không, và liệu kết quả đó có liên quan (relevant) đến câu hỏi hay yêu cầu của người dùng hay không.

**41:31** - Hệ thống theo dõi này có thể mở rộng hơn nữa bằng cách thêm vào các bước đánh giá (evaluating). Ví dụ, trong một kiến trúc hệ thống đã phát triển, quá trình xử lý dữ liệu sẽ đi qua nhiều bước, từ khi người dùng gửi yêu cầu, hệ thống tiếp nhận, xử lý qua các mô hình ML, rồi trả về kết quả. Trong quá trình này, mỗi bước có thể mang một tỷ lệ sai số nhất định. Vì vậy, chúng ta cần theo dõi từng bước để xác định được phần nào trong quá trình xử lý có vấn đề, chẳng hạn như kết quả trả về chậm hoặc không chính xác.

**43:03** - Để thực hiện việc theo dõi này, hệ thống cần các chỉ số (metrics) cơ bản như độ trễ (latency), tỷ lệ lỗi (error rate), và thời gian phản hồi (execution time). Đối với các phần mềm truyền thống, các chỉ số này đã đủ để đánh giá hiệu suất hệ thống. Tuy nhiên, khi thêm vào yếu tố đánh giá (evaluating), chúng ta cần các chỉ số phức tạp hơn như độ chính xác (accuracy), độ liên quan (relevance), thiên vị (bias), hoặc mức độ rủi ro (risk). Những chỉ số này thường được đánh giá thông qua một mô hình khác, ví dụ như chúng ta có thể sử dụng một mô hình khác để đánh giá kết quả của GPT-4, xác định xem kết quả đó có liên quan hay chính xác không.

**45:40** - Để minh họa, em đang sử dụng công cụ phonic để thực hiện việc theo dõi (tracing) cho hệ thống. Công cụ này có giao diện người dùng thân thiện và cho phép tích hợp dễ dàng với các mô hình ML như GPT-4. Em đã tạo một bộ chỉ mục (index) cho một file chứa các thông tin liên quan đến dự án và stakeholders. Sau đó, hệ thống sẽ sử dụng GPT-4 để trả lời các câu hỏi dựa trên dữ liệu này.

**46:32** - Khi hệ thống đã được thiết lập và tải lên chỉ mục, em sẽ thử nghiệm với một số câu hỏi để kiểm tra phản hồi từ mô hình GPT-4. Các câu hỏi đơn giản nằm trong dữ liệu sẽ được mô hình xử lý tốt, nhưng các câu hỏi phức tạp hoặc không có trong dữ liệu sẽ không được mô hình trả lời đúng. Kết quả trả về sẽ được tổng hợp và đánh giá.

**47:50** - Hệ thống sẽ chỉ đánh giá dựa trên các chỉ số cơ bản như độ trễ và số token đã sử dụng. Tuy nhiên, để có đánh giá chính xác hơn, em sẽ cấu hình thêm phần đánh giá (evaluating) bằng cách sử dụng một mô hình khác như GPT-4 hoặc Cloud 3.5. Khi mô hình khác này đánh giá, nó sẽ cung cấp cho mình các thông số chi tiết hơn như độ chính xác hay độ liên quan của các câu trả lời.

**48:42** - Sau khi chạy thử, hệ thống sẽ cho phép chúng ta chọn những chỉ số nào cần theo dõi, như độ liên quan (relevance), độ chính xác (correctness), và độ độc hại (toxicity). Đa số các mô hình sẽ không trả lời các câu hỏi liên quan đến nội dung độc hại, nhưng hệ thống vẫn kiểm tra để đảm bảo an toàn.

**49:28** - Kết quả đánh giá sẽ được hiển thị trên giao diện dưới dạng các ma trận (matrix). Mỗi câu trả lời sẽ được kiểm tra xem nó có chính xác không hay chỉ là dự đoán vô căn cứ từ mô hình. Những đánh giá này rất quan trọng trong việc cải thiện và tinh chỉnh các mô hình ML để đảm bảo chúng hoạt động hiệu quả và đáng tin cậy.

**50:48** - Format của hệ thống sẽ hiển thị dữ liệu và yêu cầu trả về giá trị tương ứng. Sau đó, chúng ta có thể trực quan hóa (visualize) dữ liệu này. Hệ thống sẽ đánh giá xem dữ liệu trả về có liên quan (relevant) hay không. Ví dụ, có hai câu hỏi cuối trong thử nghiệm trước đó không có trong tài liệu. Do đó, hệ thống đánh giá rằng các câu trả lời này không liên quan. Cụ thể, câu hỏi về chiến lược giao dịch của trader không có trong tài liệu, vì vậy mô hình đánh giá xác định rằng câu trả lời của hệ thống là không liên quan.

**51:34** - Khi hệ thống đánh giá các câu trả lời, nó sẽ xác định rằng các câu trả lời có liên quan đến tài liệu hay không. Ví dụ, mô hình đánh giá có thể xác định rằng câu trả lời của hệ thống là chính xác về mặt cú pháp, nhưng nếu nó không nằm trong tài liệu tham khảo, thì độ liên quan sẽ được đánh giá là không có. Điều này rất quan trọng để đảm bảo rằng hệ thống không chỉ cung cấp câu trả lời chính xác về mặt hình thức mà còn phải phù hợp với ngữ cảnh và tài liệu hiện có.

**52:15** - Đánh giá liên quan đến việc xác định xem các thông tin trong tài liệu tham khảo có khớp với câu trả lời mà mô hình cung cấp hay không. Nếu thông tin không được tìm thấy trong tài liệu tham khảo, hệ thống sẽ đánh giá rằng câu trả lời không có độ liên quan (unrelated). Đây là một công cụ quan trọng để theo dõi (tracing) và đánh giá hệ thống sau khi triển khai.

**53:14** - Sau khi triển khai, một trong những vấn đề quan trọng là đánh giá chất lượng của mô hình. Chúng ta có thể sử dụng một mô hình cao cấp hơn để đánh giá mô hình hiện tại hoặc sử dụng mô hình miễn phí hoặc tự huấn luyện. Đánh giá này có thể áp dụng cho cả các mô hình có sẵn (pre-trained models) hoặc các mô hình tự tùy chỉnh (custom models). Ví dụ, nếu mô hình chính của chúng ta không phải là GPT-4, chúng ta có thể sử dụng một mô hình khác để đánh giá chất lượng.

**54:09** - Hệ thống đánh giá có thể được sử dụng để kiểm tra chất lượng của các mô hình ML hoặc cách chúng ta kết hợp (combine) các thành phần trong hệ thống. Điều này đảm bảo rằng đầu ra của hệ thống phù hợp và đáp ứng được yêu cầu của người dùng. Đánh giá này là một phần bổ sung (extra) nhưng rất quan trọng trong việc theo dõi và cải thiện hệ thống.

**55:31** - Bản chất của hệ thống này vẫn là theo dõi (tracing) từng bước và debug khi cần thiết. Đối với các chỉ số cơ bản như độ trễ (latency), hệ thống sẽ theo dõi các thông số như thời gian thực hiện, lỗi, và kiểm tra từng bước để đảm bảo rằng hệ thống hoạt động đúng.

**56:12** - Hệ thống này có thể rất hữu ích trong việc quản lý các truy vấn lớn, đặc biệt là khi cần đánh giá đầu ra của hàng loạt người dùng. Sau khi chạy các truy vấn, chúng ta có thể lọc các câu trả lời được đánh giá là có điểm số thấp và xử lý chúng để cải thiện hệ thống.

**57:12** - Việc sử dụng các công cụ như tracing có thể tiêu tốn chi phí, đặc biệt là khi đánh giá nhiều truy vấn phức tạp. Các công cụ đánh giá này có thể sử dụng các mô hình phức tạp, dẫn đến chi phí cao. Tuy nhiên, việc theo dõi và đánh giá sau khi triển khai vẫn là cần thiết để đảm bảo hệ thống hoạt động hiệu quả.

**58:51** - Các công cụ như vậy cho phép theo dõi và đánh giá toàn bộ quy trình xử lý của hệ thống. Chúng có thể giúp tính toán chi phí và xác định các bước nào trong quy trình xử lý cần cải thiện. Việc tích hợp các công cụ này có thể giúp theo dõi từng bước và đảm bảo rằng hệ thống hoạt động theo đúng cách mà chúng ta mong muốn.

**01:03:21** - Việc triển khai hệ thống mới với các công cụ như debox có thể giúp quản lý các dịch vụ một cách dễ dàng mà không cần đến container hoặc Docker. Điều này có thể hữu ích trong việc tối ưu hóa hiệu suất và giảm tải hệ thống. Tuy nhiên, việc thiết lập và cấu hình ban đầu có thể gặp một số khó khăn, đặc biệt là khi cần tương thích với nhiều môi trường khác nhau.

<iframe width="560" height="315" src="https://www.youtube.com/embed/S_y5IrBhfNQ?si=sCTdtk_6L69pWZiK&amp;start=3736" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

**01:05:58** - Việc quản lý hệ thống thông qua debox giúp đơn giản hóa quy trình, nhưng cũng có những thách thức nhất định như cần phải tùy chỉnh các gói cài đặt. Điều này đòi hỏi người dùng phải có kiến thức sâu về hệ thống và các gói phần mềm được sử dụng. Tuy nhiên, lợi ích của việc này là giảm bớt sự phụ thuộc vào Docker và cải thiện hiệu suất hệ thống.

**01:08:07** - Cộng đồng sử dụng debox còn khá nhỏ, vì vậy việc tìm kiếm hỗ trợ có thể hơi khó khăn. Tuy nhiên, đối với các dự án nhỏ hoặc khi cần tối ưu hóa tài nguyên hệ thống, debox có thể là một giải pháp hữu hiệu. Chúng ta cần cân nhắc kỹ lưỡng trước khi áp dụng để đảm bảo rằng hệ thống sẽ hoạt động hiệu quả trong môi trường phát triển và triển khai.

**01:17:10** - Có gì thêm không? Em clean up lại rồi, em chia lại cho mọi người. Hiện tại, em đang chạy chung tất cả các service lên cùng một lúc. Nếu muốn chạy từng cái riêng lẻ thì cũng được.

**01:18:34** - Hôm nay, em sẽ demo một công cụ mới mà mọi người có thể đã nghe đến gần đây, đó là Cursor. Đây là một IDE mới nổi trong cộng đồng lập trình, và em thấy nó khá hữu ích. Cursor thực ra giống VS Code về mặt giao diện, nhưng điểm đặc biệt là nó có hai tính năng chính: một là "comk" - dùng để chỉnh sửa code, và hai là "coml" - dùng để chat và hỗ trợ phát triển trực tiếp.

**01:18:34** Bây giờ em sẽ thử demo một số tính năng của nó. Ví dụ, với "comk," em có thể yêu cầu Cursor tạo ra một tính năng mới. Giả sử, em muốn tạo một lệnh "standup" để tag tất cả mọi người trong một channel. Em sẽ yêu cầu nó tạo lệnh này với một số tùy chọn như thêm hoặc loại bỏ người mình muốn tag, hoặc chọn channel mà lệnh này sẽ được thực thi.

Cursor sẽ generate code dựa trên yêu cầu của mình, nhưng có một nhược điểm nhỏ là nó không tự động tạo file hay folder, mà mình phải tự tạo thủ công. Sau đó, mình mới có thể dùng code mà nó generate ra. Ở đây, nó đã generate ra một đoạn code, nhưng không theo cấu trúc project của em, vì vậy em cần phải chỉ định thêm ontext cho nó.

**01:19:29** Mình có thể hỏi nó một số thứ về bối cảnh hiện tại. Ví dụ như mình đang cần tìm hiểu về một số khía cạnh của project, thì lúc chat, Cursor sẽ có hai tùy chọn: một là chat với AI trong môi trường tổng quát, hai là chat trong một context cụ thể của project. Điều này cho phép mình có được cái nhìn tổng quan về cấu trúc và cách thức hoạt động của project này.

Giả sử mình muốn Cursor giúp mình triển khai một tính năng mới, ví dụ như tạo một lệnh mới trong bot Discord. Mình có thể yêu cầu nó tạo một lệnh "standup" để nhắc tất cả mọi người trong một kênh nhất định. Lệnh này sẽ có một số tùy chọn như cho phép thêm hoặc loại bỏ những người mà mình không muốn nhắc, hoặc chọn một kênh cụ thể để gửi thông báo.

<iframe width="560" height="315" src="https://www.youtube.com/embed/S_y5IrBhfNQ?si=NzvG59yE_qbbipPJ&amp;start=4731" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

**01:21:01** Tuy nhiên, một nhược điểm của Cursor là nó không thể tự tạo file hay thư mục mới, mình phải tự tạo thủ công. Mặc dù vậy, Cursor  có thể generate code theo yêu cầu của mình. Nhưng đôi khi, code nó tạo ra không theo đúng cấu trúc của project mình. Nếu muốn nó bám sát hơn với context hiện tại, mình có thể import các file và thư mục liên quan vào để nó hiểu rõ hơn về cấu trúc project.

Cursor cũng cho phép mình import một số tài nguyên như file, thư mục, hoặc đoạn code cụ thể từ web hay các nguồn khác. Ví dụ, mình có thể yêu cầu nó sử dụng một thư mục có tên là "commands" và import các file liên quan vào đó. Khi đó, Cursor AI sẽ generate code và cấu trúc theo đúng format mà project mình đang sử dụng, như tạo ra các file `base`, `interface`, và `implementation` cho lệnh "standup" mới này.

**01:23:25** Sau khi tạo xong code, nó còn chỉ mình cách cập nhật những phần khác của project như việc thêm lệnh mới vào giao diện của bot Discord. Thông thường, khi làm việc với Cursor, nó sẽ cung cấp những giải pháp cụ thể và chi tiết hơn, đặc biệt là khi mình có thể import các file mẫu có sẵn theo convention của project mình.

**01:24:28** Ví dụ, mình có thể yêu cầu Cursor tạo một unit test cho một file cấu hình như `config.go`. Đây là một ví dụ đơn giản, sử dụng những unit test có sẵn của Go. Nếu mình muốn sử dụng thêm một thư viện khác hoặc thêm chi tiết vào phần test, mình có thể yêu cầu Cursor AI điều chỉnh theo ý mình.

Nếu project của mình đã có sẵn các file test theo một convention nhất định, mình có thể import các file đó vào để Cursor học theo, từ đó tạo ra các test cases chuẩn hơn. Điều này giúp mình tiết kiệm thời gian và đảm bảo các test cases tạo ra phù hợp với convention của team.

**01:25:02** Nếu mình muốn thêm một tính năng phức tạp hơn, chẳng hạn như load dữ liệu từ một file JSON, Cursor có thể giúp mình cập nhật phần code để thực hiện điều này. Nó sẽ thêm phần code cần thiết vào trong file của mình, giúp tự động hóa các công việc lặp lại và giảm thiểu sai sót khi làm việc thủ công.

**01:26:40** Mình có thể có câu hỏi rằng liệu Cursor có index toàn bộ code của mình lên server của họ hay không. Theo quảng cáo của họ, Cursor sẽ chạy hoàn toàn trên máy tính của mình, tạo ra một môi trường riêng để xử lý và index toàn bộ source code, không gửi dữ liệu lên server của họ trừ khi mình chọn sử dụng API key của họ.

**01:27:56** Tuy nhiên, vẫn có một số lo ngại về việc dữ liệu có thể được gửi lên server của Cursor trong quá trình xử lý, đặc biệt khi mình sử dụng API key của họ thay vì key của chính mình. Dù vậy, nếu sử dụng key riêng, mình có thể kiểm soát dữ liệu của mình tốt hơn và biết được ai đang sử dụng nó.

**01:29:03** Về giao diện, Cursor có vẻ tiện lợi hơn khi giúp mình import file và code từ nhiều nguồn khác nhau, điều này giúp cải thiện khả năng hiểu context của nó. Ví dụ, mình có thể import một project từ GitHub để Cursor AI học theo convention của project đó và generate code phù hợp hơn.

**01:31:19** Em đã thử nghiệm việc import một project từ GitHub và yêu cầu Cursor AI chỉnh sửa code theo convention của project đó. Kết quả là nó hiểu và áp dụng các convention một cách khá hiệu quả, mặc dù đôi khi vẫn cần phải làm một số tinh chỉnh thủ công. Cursor AI có thể không chỉ generate code mà còn giúp quản lý và chỉnh sửa code một cách hiệu quả hơn.

**01:33:16** Một điểm mạnh khác của Cursor là khả năng giúp mình import và làm việc với context nhanh chóng, đặc biệt hữu ích khi làm việc với các project lớn hoặc khi cần đảm bảo tính nhất quán trong codebase. Mặc dù vẫn có một số giới hạn, nhưng Cursor thực sự là một công cụ mạnh mẽ và đáng thử nghiệm trong quá trình phát triển phần mềm.

**01:36:07** Tóm lại, Cursor không chỉ là một công cụ generate code mà còn giúp hiểu rõ và quản lý codebase lớn hiệu quả. Nó có thể thay thế hoặc bổ sung cho các công cụ khác như Codex hay GitHub Copilot trong các dự án đòi hỏi sự chính xác và khả năng hiểu sâu về context. Nếu có điều kiện, em khuyến khích mọi người nên thử nghiệm công cụ này để tận dụng tối đa các tính năng của nó.

---

### English Transcript

**00:00** - Ok, that's probably enough, let's start. Others will join in gradually. Phat, go ahead with your Go section. Ok, can everyone hear me? You can hear me, right? Ok, so I'll start like this. First, this week I found a few interesting tools. As for news, there's nothing new, just the release of Go 1.23. First off, there's this Go Notebook, which is similar to Jupyter that you're all familiar with. Jupyter is a tool that has been around for a long time in Python, typically used for machine learning or data analysis. Now, Go also has a similar version that allows us to use Go within a notebook environment. You can run it locally or even build a Docker container and run it in there.

**10:57** - Go Notebook also has some features like plotting (widget plot), quite similar to Jupyter, and it might even be faster when building and running Go locally. I’ve tested it and found it to be quite fast, even faster than Jupyter. I used to find Jupyter quite slow. The second tool is "kuam," a tool that supports those using Nexttop. Kuam streams unnecessary configuration files (configs) in your project. Normally, without kuam, when listing out unused or unconnected configs, you'd have to manually delete them from the file. With kuam, it automatically removes those unnecessary configurations, and you have the option to decide whether to save this change to the config file or not.

**14:56** - Ok, does anyone have any questions about Phat's review? Does anyone want to ask anything?

**15:44** - Ah, about Oscar, how is that? We mentioned it last week or two weeks ago, do you remember? The Oscar and Gasp projects—Oscar is a big one. Last week's article linked to its architecture. It’s an agent, similar to what Tom has done, but mainly on Dr. By, where they only showed the architecture, not in detail. I'll find it and post the link later. There is code, but the Gasp code is not public; it's in Google's internal repo. I’ll send the link if needed.

**16:53** - That work over there will probably be done soon. I'm preparing to write a module or an OS based on that guide, like you mentioned, and it should be ready by next week, right? If anything comes up, you guys should be ready. I heard Phat is coding quite a bit, which is a bit surprising, but it seems the start is quite stable. Ok, thanks, Phat. Alright, next, we'll move on to a topic related to creating dynamic objects in a project.

**17:54** - Similar to Notion. Yes, that's right. Ok, wait a moment. This could probably be done over there, let's see. Are you ready? They should be able to go into production, right? They have already gone live, as we're using the product version. Ok, let me share my screen for everyone. Can you see my screen? You can, right? Ok, this topic is about modeling dynamic objects. Essentially, we want to create an object that is extendable, like in Notion, where you have fields that can be extended or modified.

**18:54** - So how can we model this? Over here, I've set up a database. When we started, we made two important decisions in modeling this system. First, the main model itself and its fields need to be separated into two different tables. This is necessary because if we want to extend the list of properties, we need to store these fields in a separate table.

**19:44** - For example, suppose we have a task, this task will not directly contain any fields. Instead, we will have a separate field table. In this field table, there will be information such as the field type (the data type of the field), for example, text, checkbox, or select (multi-select). The name of the field and its options will be stored in another separate table. This allows us to be more flexible in adding options to the field dynamically.

**20:23** - If you look at it, you'll see that currently, the task and the field don’t have a direct relationship. Instead of creating a direct relationship between the task and the field, we chose to use an intermediate table called the value table. This value table acts as a bridge between the task and the list of fields. This means that when you add a field to a task, you’re not actually adding that field directly to the task, but rather adding a record to the value table. This record will link the task to the corresponding field.

**21:00** - In this value table, we’ve also modeled it flexibly because field types can vary, as I mentioned: text, boolean, select, or user. Each value type has its own column in the value table, for example, a column for text, a column for boolean, a column for select, or a column for user. This gives us more flexibility in handling different data types in our system.

**21:33** - For each different value type like text, boolean, and others, we created a separate column in the value table. For instance, a column for text, a column for boolean, a column for select, or a column for user. This means we can also connect these values to other tables in our database. This was the first decision we made when designing this system.

Why didn’t we create a direct relationship between the task and the field? The reason is that we wanted these fields to act as a global configuration. When a new field is created, all tasks can reuse this field without needing to create a tight relationship. The relationship between the task and the field will be very loose, and all operations are handled through the value table. When you delete a value in the value table, the corresponding field in the task will also disappear, but the field will still exist for other tasks.

**22:46** - That’s about it. For example, if I create a new task and want to add a select field, when I type 'tag', the system will show the existing fields, and I can add this existing 'tag' field to the new task, inheriting all the options that this field already has. Overall, this system works quite quickly.

**23:32** - What about other operations? For example, in Notion, you have operations like sorting and filtering fields. Since these fields are stored in a separate table, if you want to sort, you just need to add a sort order column to the field table. When you adjust this sort order, it will automatically update for the entire workspace. In practice, my system doesn't have a specific task to test this yet, but I think it will work across the entire workspace.

**24:20** - Currently, we haven't considered saving a separate sort order for each task because that would be very complex. The sort order is currently global. There are some challenges when using this model, which is during queries, we have to join many different tables and deal with filtering and pagination of the data. With our current infrastructure, using Prisma cannot handle this, so we have to write raw SQL to execute these complex queries. This is a major difficulty.

**24:59** - Another issue is when working cross-organization or cross-workspace, such as inviting guests from other organizations. Managing these fields, especially related to access permissions, is very complicated. These fields belong to a specific organization, so when inviting guests, managing access permissions becomes very tangled. When we designed this system, we didn’t account for cross-space, so now we're working around it to make it functional. However, this is still a problem in our current infrastructure.

**25:33** - Another issue is similar to Notion, where when you want to move or copy a page from one table to another, the new table will have a different set of properties from the original table. Currently, the fields are stored at the workspace or organization level, not at the table level. This means that these fields are shared across the entire workspace.

**26:08** - One way to solve this issue is by allowing users to switch directly between workspaces within the same organization, as in Notion. When a guest enters, they can still see tasks in their workspace and tasks from other workspaces if they are shared. However, the issue arises when the system shares the same set of fields for multiple workspaces within the same organization, causing conflicts in access and management.

**26:51** - These fields are currently directly connected to the organization rather than the workspace, so these fields are shared across the entire workspace. There could be a solution to this by allowing users to switch directly between workspaces, like in Notion. This means that when users access it, the entire organization is still under their control. But currently, the system allows guests to enter and see all tasks within their organization and tasks from other organizations they’ve been invited to. This leads to data being shared across organizations, causing conflicts.

**27:31** - If we use a separate approach, we won’t face this issue. But actually, this issue originates from the fact that tasks are just an entity of the calendar system, right?

**28:26** - Compared to blocks in Notion, Notion's blocks are built on a bottom-up architecture. This system, however, is just a simple mockup and doesn’t have much relation to blocks. It's merely a mockup to make the system operate in its own way.

**29:54** - To make the system operate reasonably, we need to ensure that the relationship between fields and values is clear and not confusing. This includes avoiding loops in data design. A loop in design should only exist if it is truly necessary to optimize queries or other tasks. However, we must be aware that this loop can lead to many difficulties in maintaining and developing the system. When others look at this design, they need to understand the purpose of the loop and not confuse it with other purposes.

**35:51** - One part I’m still pondering is if we keep the loop as it is, when a user deletes an option of a field, all tasks using that option will automatically update and remove that option from the database. This means we won’t need to revalidate those tasks. If we keep this loop, management will become simpler, but it may lead to other issues in the long run.

**37:07** - We need to carefully consider whether to keep this loop or restructure it to avoid future complexities. Deciding to keep or remove the loop may depend on how the system is used and managed. If we decide to keep the loop, we need to ensure that it’s designed clearly and can be easily managed and maintained.

**39:03** - Another part of today’s discussion will focus on introducing some new tools for system tracing and monitoring. This is crucial in the development and maintenance of large software, especially when we need to monitor each step of the system's operation to ensure everything runs smoothly.

**40:11** - When developing a system that uses machine learning (ML), the process usually involves steps like ideation, model selection, customization, and then deployment. The last step, like traditional software, is monitoring and gathering feedback to improve the system. For traditional software, the difference lies in that we already know what the output will be and can determine it based on the input. However, for software integrated with machine learning, the output is often probabilistic. This means that when a user inputs data, the output may vary depending on the model or model configuration we use. Therefore, tracing becomes extremely important after deployment to ensure that the software's outputs meet user expectations.

**40:50** - A characteristic of ML-integrated systems is the uncertainty in the output. For example, when a user inputs data into the system, the output may vary depending on how the model is customized or tuned. Therefore, the tracing system needs to help us better understand the process and determine whether the outputs meet expectations, whether they violate any rules, and whether the outputs are relevant to the user’s questions or requests.

**41:31** - This tracing system can be expanded further by adding evaluation steps. For example, in a developed system architecture, the data processing process will go through many steps, from when the user submits a request, the system receives it, processes it through ML models, and then returns the result. In this process, each step may carry a certain degree of error. Therefore, we need to trace each step to identify where in the processing chain there is an issue, such as the result being returned slowly or inaccurately.

**43:03** - To perform this tracing, the system needs basic metrics like latency, error rate, and execution time. For traditional software, these metrics are sufficient to evaluate system performance. However, when adding the evaluation factor, we need more complex metrics like accuracy, relevance, bias, or risk. These metrics are often evaluated through another model. For example, we might use another model to evaluate the results of GPT-4 to determine if the results are relevant or accurate.

**45:40** - To illustrate, I’m using a tool called phonic to perform tracing for the system. This tool has a user-friendly interface and allows easy integration with ML models like GPT-4. I’ve created an index for a file containing information related to the project and stakeholders. The system will then use GPT-4 to answer questions based on this data.

**46:32** - Once the system is set up and the index is loaded, I will experiment with some questions to check the responses from the GPT-4 model. Simple questions within the data will be handled well by the model, but complex questions or those not found in the data will not be answered correctly. The results will be aggregated and evaluated.

**47:50** - The system will only evaluate based on basic metrics like latency and the number of tokens used. However, for a more accurate assessment, I will configure additional evaluation by using another model, such as GPT-4 or Cloud 3.5. When this other model evaluates, it will provide more detailed metrics such as accuracy or relevance of the answers.

**48:42** - After running the tests, the system will allow us to choose which metrics to monitor, such as relevance, correctness, and toxicity. Most models won’t answer questions related to toxic content, but the system still checks to ensure safety.

**49:28** - The evaluation results will be displayed on the interface as matrices. Each answer will be checked to see if it is accurate or just a baseless guess from the model. These evaluations are crucial in improving and fine-tuning ML models to ensure they operate effectively and reliably.

**50:48** - The system's format will display the data and require the corresponding value to be returned. Then, we can visualize this data. The system will evaluate whether the returned data is relevant. For example, there were two final questions in the previous test that were not in the document. Therefore, the system evaluates that these answers are not relevant. Specifically, the question about the trader's trading strategy was not in the document, so the evaluation model determined that the system's answer was irrelevant.

**51:34** - When the system evaluates the answers, it will determine whether the answers are relevant to the document. For example, the evaluation model may determine that the system's answer is syntactically correct, but if it is not in the reference document, the relevance will be evaluated as none. This is crucial to ensure that the system not only provides correct answers in form but also fits the context and available documentation.

**52:15** - Evaluation involves determining whether the information in the reference document matches the answer provided by the model. If the information is not found in the reference document, the system will evaluate that the answer is unrelated. This is an important tool for tracing and evaluating the system after deployment.

**53:14** - After deployment, one of the key issues is evaluating the quality of the model. We can use a higher-level model to evaluate the current model or use a free or self-trained model. This evaluation can be applied to both pre-trained models and custom models. For example, if our main model is not GPT-4, we can use another model to evaluate the quality.

**54:09** - The evaluation system can be used to check the quality of ML models or how we combine components in the system. This ensures that the system's output is appropriate and meets user requirements. This evaluation is an extra but very important part of tracing and improving the system.

**55:31** - The essence of this system is still to trace each step and debug when necessary. For basic metrics like latency, the system will monitor parameters like execution time, errors, and check each step to ensure that the system operates correctly.

**56:12** - This system can be very useful in managing large queries, especially when evaluating the output of a large number of users. After running the queries, we can filter out the answers that are rated as low and address them to improve the system.

**57:12** - Using tools like tracing can incur costs, especially when evaluating many complex queries. These evaluation tools may use complex models, leading to high costs. However, tracing and evaluation after deployment are still necessary to ensure that the system operates efficiently.

**58:51** - Tools like l smi allow for tracing and evaluating the entire system processing workflow. They can help calculate costs and identify which steps in the processing workflow need improvement. Integrating these tools can help trace each step and ensure that the system operates in the way we expect.

**01:03:21** - Deploying a new system with tools like debox can help manage services easily without needing containers or Docker. This can be useful in optimizing performance and reducing system load. However, the initial setup and configuration can encounter some difficulties, especially when needing to be compatible with multiple environments.

**01:05:58** - Managing the system through debox simplifies the process, but there are certain challenges, such as needing to customize installation packages. This requires users to have deep knowledge of the system and the software packages being used. However, the benefit is reducing reliance on Docker and improving system performance.

**01:08:07** - The community using debox is still quite small, so finding support can be a bit difficult. However, for small projects or when needing to optimize system resources, debox can be an effective solution. We need to carefully consider before applying it to ensure that the system will operate efficiently in the development and deployment environment.

**01:17:10** - Anything else? I cleaned up and shared it again for everyone. Currently, I’m running all the services together at once. If you want to run them individually, that’s also possible.

**01:18:34** - Today, I will demo a new tool that you may have heard of recently, called Cursor. This is a new IDE that has been gaining popularity in the programming community, and I find it quite useful. Cursor actually resembles VS Code in terms of interface, but what sets it apart is its two main features: "comk" - used for code editing, and "coml" - used for chatting and direct development support.

**01:18:34** Now, I will demo some of its features. For example, with "comk," I can ask Cursor to create a new feature. Suppose I want to create a "standup" command to tag everyone in a channel. I can ask it to create this command with some options like adding or removing people I want to tag, or choosing the channel where this command will be executed.

Cursor will generate code based on my request, but one downside is that it cannot automatically create files or folders; I have to create them manually. After that, I can use the code it generates. Here, it generated a piece of code, but not according to the structure of my project, so I need to provide more context for it.

**01:19:29** You can ask it about various aspects of the current project. For instance, if you need to understand certain parts of the project, when you chat, Cursor will give you two options: chat with the AI in a general environment, or chat within a specific project context. This allows you to get an overview of the structure and workings of this project.

Suppose you want Cursor to help you implement a new feature, such as creating a new command in a Discord bot. You can ask it to create a "standup" command to remind everyone in a specific channel. This command will have several options, like allowing the addition or removal of people you don’t want to remind, or selecting a specific channel to send the notification to.

**01:21:01** However, one drawback of Cursor is that it cannot automatically create new files or directories; you have to do it manually. Despite that, Cursor can generate code based on your request. But sometimes, the code it generates doesn’t follow the structure of your project. If you want it to stick more closely to the current context, you can import related files and directories to help it understand the project structure better.

Cursor also allows you to import resources like files, directories, or specific code snippets from the web or other sources. For example, you can ask it to use a folder named "commands" and import related files into it. Then, Cursor AI will generate code and structure it according to the format your project uses, such as creating `base`, `interface`, and `implementation` files for the new "standup" command.

**01:23:25** After generating the code, it also guides you on how to update other parts of the project, like adding the new command to the Discord bot interface. Typically, when working with Cursor, it provides more specific and detailed solutions, especially when you can import existing sample files that follow your project’s conventions.

**01:24:28** For example, you can ask Cursor to create a unit test for a configuration file like `config.go`. This is a simple example, using existing unit tests from Go. If you want to use an additional library or add details to the test, you can ask Cursor AI to adjust it according to your preferences.

If your project already has test files following a specific convention, you can import those files for Cursor to learn from, so it can create test cases that align with your team’s conventions. This helps save time and ensures that the generated test cases fit the team’s convention.

**01:25:02** If you want to add a more complex feature, such as loading data from a JSON file, Cursor can help you update the code to implement this. It will add the necessary code to your file, automating repetitive tasks and minimizing errors when working manually.

**01:26:40** You might have a question about whether Cursor indexes all your code to their server. According to their advertisement, Cursor runs entirely on your computer, creating a local environment to process and index all the source code, without sending data to their server unless you choose to use their API key.

**01:27:56** However, there are still some concerns about whether data might be sent to Cursor’s server during processing, especially if you use their API key instead of your own. However, if you use your own key, you can better control your data and know who is using it.

**01:29:03** In terms of the interface, Cursor seems more convenient as it helps you import files and code from various sources, improving its ability to understand the context. For example, you can import a project from GitHub for Cursor AI to learn the project’s conventions and generate more appropriate code.

**01:31:19** I’ve experimented with importing a project from GitHub and asking Cursor AI to edit the code according to the project’s conventions. The result is that it understands and applies the conventions quite effectively, though some manual tweaks may still be needed. Cursor AI can not only generate code but also help manage and edit the code more efficiently.

**01:33:16** Another strength of Cursor is its ability to help you quickly import and work with context, which is especially useful when working on large projects or when ensuring consistency across the codebase. While there are still some limitations, Cursor is indeed a powerful tool worth trying in software development.

**01:36:07** In conclusion, Cursor is not just a code generator but also helps to understand and manage large codebases effectively. It can replace or complement other tools like Codex or GitHub Copilot in projects that require precision and deep context understanding. If possible, I encourage everyone to try this tool to take full advantage of its features.