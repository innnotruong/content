---
tags:
  - office-hours
  - ogif
  - discord
title: "OGIF Office Hours #24 - Go weekly, AI-Driven Workflows, Holistic Team AI Demo, and Figma to UI Component with Claude"
date: 2024-09-23
description: In our OGIF office hour 24 covers AI-driven workflows with Tom, a demo with the Holistic team, and Figma integration with Claude for UI components and Go commentary. Highlights include Agent Zero's data automation capabilities, Figma-to-code conversion, and the benefits of in-office collaboration for efficient knowledge transfer and AI/ML learning.
authors:
  - innno_
---

85 minutes

### Topics and Highlights
- Live coding demo showcased data engineering techniques.
- Introduced Agent Zero for automated data processing.
- Demonstrated data cleaning and analysis using CSV files.
- Generated infographics from backend technology data.
- Figma to code conversion for UI components.
- AI integration for automating repetitive tasks.
- Discussed team collaboration and knowledge sharing.

---

**Vietnamese Transcript**

**00:00** Ok, mọi người nghe rõ chưa? Chúng ta còn khoảng 12 phút nữa để Tom có thể demo live coding. Tuy nhiên, có lẽ sẽ không kịp hết phần này, nên mình sẽ chuẩn bị một phần demo về Data Engineering trước. Tom, bạn có thể bắt đầu được rồi đấy. Ok, chào mọi người, mình sẽ giới thiệu một phần demo liên quan đến Data Engineering. Phần này tập trung vào việc làm sạch dữ liệu với sự hỗ trợ của AI, để chúng ta có thể bắt đầu tiến hành phân tích dữ liệu hoặc chuẩn bị dữ liệu ban đầu.

**04:37** Mình sẽ chia sẻ màn hình nhé. Không cần dùng Zoom đâu. Ok, mọi người thấy màn hình rồi chứ? Ok, mình sẽ giới thiệu về dataset mà chúng ta sẽ làm việc hôm nay. Thực sự thì có rất nhiều loại dữ liệu mà chúng ta có thể làm sạch bằng một công cụ gọi là Agent Zero. Hôm nay mình sẽ sử dụng một dạng dataset kiểu như là lấy thông tin từ một nguồn nhất định, và sau đó đưa ra một file CSV. Cái CSV này thực sự rất lộn xộn, như là nó sắp xếp kiểu từng phần từng phần vậy, và việc làm sạch từng phần đó là khá khó. Thực tế, họ chia ra từng trang web, từng phần nhỏ. Vậy làm thế nào để chúng ta có một bộ dataset hoặc một infographic tổng hợp hết tất cả thông tin trên một file? Mình sẽ demo điều này cho mọi người xem.

<iframe width="560" height="315" src="https://www.youtube.com/embed/lAk1QSl7qS0?si=o-UbAP-JNwGuSrpm&amp;start=347" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

**06:22** Agent Zero là một công cụ AI Agent, và bạn chỉ cần nói với nó bằng ngôn ngữ tự nhiên, nó sẽ tự động viết code cho bạn. Ví dụ, vấn đề của mình nằm trong thư mục 'ph', thì mình sẽ chỉ nói với nó là: "Look into the ph folder and help me process all of the CSV files. I want to do some data analysis to understand what backend technologies all of these sites are using and aggregate all of them." Có vẻ như UI bị lỗi một chút, nhưng mình đang muốn phân tích các công nghệ backend mà các trang web này đang sử dụng. Agent Zero sẽ dùng GPT-4 hoặc GPT-4 mini để thực hiện tất cả công việc này.

**08:25** Nếu như nó gặp lỗi thì nó sẽ sửa lỗi đó thôi. Quy trình của Agent Zero có hai phần: một là nó sẽ chạy code, và phần còn lại là nó sẽ kiểm tra lại xem code đó chạy có ổn không. Ở đây, nó đã phát hiện ra lỗi rồi, nên nó sẽ tự động sửa lỗi đó cho mình. Hiện tại mình chỉ cần nói cho nó biết mục tiêu của mình là gì, và nó sẽ tự động viết code cho mình, từ đó mình có thể bắt đầu phân tích dữ liệu của những trang web mà mình đã tải về, chuyển đổi chúng thành các file CSV và làm sạch dữ liệu.

**09:06** Giờ thì mình sẽ yêu cầu nó tạo ra một infographic để tổng hợp tất cả các công nghệ backend mà các trang web đang sử dụng. Mình muốn một cái hình ảnh trực quan để dễ dàng phân tích. Vậy nên, mình sẽ yêu cầu nó là "Create me an infographic inside the 'ph' folder to aggregate all of the backend programming languages which are used across all CSV files." Sau đó nó sẽ tự động vẽ cho mình một biểu đồ bằng cách sử dụng thư viện matplotlib và xuất ra một hình ảnh PNG. Nếu nó gặp phải lỗi, nó sẽ tự động tải các thư viện cần thiết thông qua pip và tiếp tục quá trình. Quá trình này giúp tự động hóa hầu như tất cả những mong muốn của mình liên quan đến việc xử lý dữ liệu. Nó sẽ giữ lại tất cả những gì đã làm để mình có thể kiểm tra lại sau.

**09:58** Hiện tại, mình không muốn xem từng file kết quả nên mình sẽ yêu cầu Agent Zero đưa toàn bộ output vào thư mục 'ph' để mình dễ dàng quản lý. Sau đó, nếu mình cần sử dụng lại sau này, mình chỉ cần quay lại thư mục đó thôi. Giả sử mình cần thực hiện thêm các bước xử lý khác thì nó cũng sẽ rất tiện lợi.

**10:56** Bạn có thể thấy là với các bài toán như kiểu tạo một trình duyệt crawler, thực ra mình cũng có thể sử dụng cách tương tự để làm. Agent Zero sẽ đọc cấu trúc trang web, sau đó tải kết quả lên cho mình, và mình chỉ cần chỉ định các thẻ HTML, CSS mà mình muốn lấy dữ liệu từ đó. Thay vì phải tự viết code thủ công, giờ mình có thể nhờ nó làm luôn.

**11:42** Ví dụ như trong trường hợp này, mình thấy cách dễ nhất là mình chỉ cần xóa một vài cái entry không cần thiết, sau đó thêm một vài dòng mới để làm sạch dữ liệu. Nếu mình muốn tạo một đoạn code cho việc phân tích dữ liệu hoặc chỉ đơn giản là mình muốn tải một video YouTube và lấy 10 giây đầu tiên của nó, thì Agent Zero cũng có thể giúp mình làm việc đó. Ví dụ nhé, mình sẽ thử sao chép URL của một video YouTube và yêu cầu nó "Download this YouTube video and cut out the first 30 seconds of it." Agent Zero sẽ tự động code cho mình, sử dụng terminal, tải video xuống và cắt đúng 30 giây đầu tiên như yêu cầu.

**12:37** Trong quá trình thực hiện, nó sẽ tự động sử dụng terminal, tải video xuống và cắt phần cần thiết. Tuy nhiên, đôi lúc nó sẽ gặp phải một vài vấn đề nhỏ, như việc chọn module backend nào để xử lý quá trình này, chẳng hạn như nó đang dùng GPT-4 mini. Bạn có thể thấy nó thực sự đang sử dụng nhiều công cụ khác nhau để đảm bảo hoàn thành tác vụ một cách chính xác.

**13:41**  Có vẻ như nó đang gặp lỗi khi tải xuống hoặc cắt video. Lúc này, mình chỉ cần hướng dẫn lại cho nó một chút, hoặc yêu cầu nó xóa video đang tải về và thử lại. Đây là quá trình tự động hóa gần như hoàn toàn, và rất tiện lợi cho những tác vụ lặp đi lặp lại.

**14:54** Vì đây là một video dài, nên có thể demo sẽ hơi chậm. Mình có thể thử lại với một video ngắn hơn để xem nó hoạt động như thế nào. Giờ mình sẽ copy lại URL của video ngắn hơn, và yêu cầu "Download this YouTube video and get the first 30 seconds." Quá trình này đôi khi sẽ chạy hơi lâu, nên mình chỉ cần chờ đợi một chút, hệ thống AI sẽ xử lý và hoàn thành.

**16:01** Có một số vấn đề nhỏ, ví dụ như phòng làm việc hiện tại của mình có thể không cho phép tải xuống YouTube video, nên quá trình sẽ chậm một chút. Nhưng về cơ bản, nếu bạn muốn làm những tác vụ như phân tích dữ liệu trên web, hoặc cần một công cụ auto agent để xử lý các tác vụ phức tạp, thì Agent Zero là một lựa chọn tuyệt vời.

**17:43** Mình có thể tạo ra một auto agent để xử lý những trường hợp như thế này, ví dụ như việc tải video, phân tích dữ liệu, hoặc xử lý các tác vụ từ phía backend. Agent Zero sử dụng GPT-4 mini hoặc các mô hình khác tùy theo yêu cầu, và có thể thực hiện các tác vụ phức tạp một cách hiệu quả.

**19:00** Đến đây, nếu bạn muốn đi sâu hơn về việc sử dụng Agent Zero để tạo ra code, hoặc tạo các infographic trực quan từ dữ liệu, bạn hoàn toàn có thể yêu cầu nó xuất ra các định dạng khác như CSV, JSON, hoặc thậm chí là biểu đồ dạng Parquet. Nếu dữ liệu của bạn quá lớn và không muốn sử dụng AI vì tốn token, bạn có thể tương tác với hệ thống thông qua các database như Dgraph DB hoặc các hệ thống khác. Agent Zero sẽ giúp bạn tạo ra các câu lệnh query cần thiết, và bạn có thể tương tác với cơ sở dữ liệu mà không cần phải tự viết code từ đầu.

**20:09** Dữ liệu hoặc là Data Engineer, mình có thể yêu cầu nó viết cho dạng Pandas (Pandas DataFrame) chẳng hạn. Ồ, hình như nó bị chặn rồi thì phải [âm nhạc vang lên]. À, đúng rồi, chắc là do văn phòng này bị chặn rồi, vì vậy có thể nó không tải được từ mạng bên ngoài. Nhưng nếu mình muốn đi sâu hơn vào việc viết code hay tạo một infographic để mình có thể hình dung dữ liệu dễ hơn, thì mình có thể cho nó xuất ra một cái file CSV hoặc JSON. Điều tuyệt nhất là nó cũng có thể biên dịch dữ liệu sang định dạng Parquet nếu cần thiết.

**21:13** Nếu mình có một bộ dữ liệu khá lớn và không muốn dùng AI để xử lý vì sẽ tốn nhiều token, thì mình có thể nhờ Agent Zero tạo ra code cho mình và nó sẽ sắp xếp dữ liệu thành các cấu trúc theo yêu cầu. Ví dụ như lúc đó mình có thể tương tác với một cơ sở dữ liệu như DgraphDB hoặc là bất kỳ dạng cơ sở dữ liệu nào, Agent Zero sẽ giúp mình query dữ liệu đó mà không cần phải viết quá nhiều code thủ công. Như vậy, mình có thể tương tác với dữ liệu mà không cần can thiệp trực tiếp nhiều.

**22:04** Rồi, các bạn có câu hỏi gì cho phần này không? Nếu không thì chúng ta sẽ chuyển sang phần tiếp theo nhé. Ồ, mọi người thắc mắc là Agent Zero này khác gì với mấy cái Framework mà chúng ta đã từng show trước đây nhỉ? Thực ra, khác biệt ở chỗ Framework thì mình phải viết code rất nhiều. Còn với Agent Zero, mình không cần phải code bất kỳ thứ gì. Cụ thể là nó sẽ tự động tạo công cụ và xử lý các yêu cầu. Trong khi với các Framework thông thường, bạn phải tạo một Agent, thêm công cụ và thiết lập một Runner để nó có thể thực hiện các đầu ra từ công cụ đó. Agent Zero sẽ tự động tạo công cụ luôn, mình không phải làm gì cả. Để mình kiểm tra xem nó lưu dữ liệu ở đâu nhé.

**22:44** Nó có một thư mục riêng bên trong Agent Zero, khi nó hoàn thành một tác vụ, nó sẽ lưu lại vào bộ nhớ của mình, cụ thể là trong SQLite. Bộ nhớ này sẽ lưu trữ tất cả các công cụ đã được tạo ra và các đoạn code liên quan. Ví dụ, nếu mình chưa có công cụ để tải xuống video từ YouTube, thì nó sẽ tự tạo ra. Nếu mình muốn đào dữ liệu từ Facebook chẳng hạn, nó cũng sẽ tự động tạo ra công cụ để làm việc đó. Và khi mình yêu cầu lại, nó sẽ dùng lại bộ nhớ Cache của công cụ đó. Thỉnh thoảng, nếu quá lâu không sử dụng, Cache có thể sẽ bị xóa, nhưng nói chung nó sẽ lưu lại cho mình. Nó hơi khác với Auto-GPT ngày xưa.

**23:21** Trước đây, khi sử dụng Auto-GPT, nếu bạn muốn tạo ra một ứng dụng kiểu như để phục vụ phỏng vấn hoặc lấy thông tin từ web, bạn phải tạo một công cụ trước, viết code cụ thể cho từng tác vụ đó. Với Agent Zero, bạn không cần code gì cả, nó sẽ làm tất cả cho bạn. Như khi anh Ngọc Thành từng làm, anh ấy phải code tay mọi thứ, còn mình thì không cần làm gì cả và đã có kết quả rồi. Chính vì thế, môi trường và cách tiếp cận của Agent Zero là một công cụ tự động thực sự, không cần bạn phải can thiệp quá nhiều như các Framework khác.

**24:05** Vậy cấu trúc kiến trúc của Agent Zero có gì đặc biệt so với các công cụ khác? Thực ra, mình thấy nó đặc biệt ở chỗ mình có thể dùng nó cho các tác vụ liên quan đến Data Analysis hoặc Data Engineering một cách rất đơn giản. Ví dụ, nếu bạn có một file MP3 và muốn lọc ra các âm thanh lạ, thì nó có thể giúp bạn thực hiện điều đó. Mình còn nhớ là khi có một file PDF lớn, mình cần chia nhỏ nó ra hoặc gom lại, Agent Zero cũng làm điều này rất tốt.

**24:59** Tuy nhiên, nếu yêu cầu phức tạp hơn thì có lẽ nó chưa thực hiện một cách hoàn hảo, ví dụ như nếu mình muốn tạo một biểu đồ 3D Plot hoặc một Scale Plot thì nó sẽ hiểu nhưng chưa chính xác lắm. Vì vậy, Agent Zero chỉ đóng vai trò như một "starting point," tức là một trợ lý Junior, và từ đó bạn sẽ tiếp tục hoàn thiện các tác vụ trên nền tảng này.

**25:49** Ồ, mình vừa thấy có yêu cầu xử lý một file PDF tiếp theo. Ok, để thử xem nhé. Bạn muốn nó làm gì với file PDF này? Chuyển đổi sang Markdown à, hay bạn muốn nó tạo ra một file Altic? Điều này sẽ khá thú vị để xem khả năng xử lý của Agent Zero. Có vẻ bị chồng chéo (trùng lặp) dữ liệu hay sao ấy? Bây giờ mình sẽ thử tải xuống lại một lần nữa. Để nó tự tải xuống cho mình hoặc mình sẽ tự điều chỉnh menu này để nó tự động. Mình sẽ thử điều chỉnh thêm.

**27:11** Được rồi, mình sẽ đặt tên cho thư mục là "Fusion." Ok, để xem bên trong có gì không. Ồ, hình như có cái ảnh trong đó. Bây giờ yêu cầu Agent Zero trích xuất ảnh ra từ file PDF này. Bạn muốn lấy cái ảnh nào trước nhỉ? À, hình ảnh trước nhé. Được rồi. “Help me grab the images inside the Fusion PDF into a separate folder.” Ok, đây là những hình ảnh này rồi. Chúng đã được tách ra. Nhưng có vẻ nó đã biết cách cắt đúng vị trí.

**29:25** Chắc chắn rồi, mình nghĩ nó đã lấy được hình ảnh đó từ thư viện (Library). Chúng ta cần phải tinh chỉnh lại một chút để chuyển đổi từ định dạng JPEG sang PNG. Nó sẽ loại bỏ được phần nền trong suốt nữa. Xong rồi, tất cả đã hoàn thành. Tuyệt vời, tuyệt vời, mọi thứ đều ổn định.

**29:39** Bây giờ chúng ta mở thử file Preview xem sao, liệu có ổn định và chính xác không nhé. Thật sự là uy tín hơn, hơn là khi mình làm thủ công mà tốn rất nhiều thời gian. Nhờ có Agent Zero, mình đã không phải viết code từ đầu, nó đã làm tất cả cho mình rồi. Tuy nhiên, một nhược điểm là nếu có các đoạn bảng (table) trong file PDF thì nó sẽ chỉ trích xuất chúng dưới dạng hình ảnh thôi. Không thể giữ được format của bảng như trong file PDF gốc. Nhưng cũng tạm được, không vấn đề gì.

**30:37** Ok, có ai có câu hỏi gì không? Nếu không có thì chúng ta sẽ chuyển sang phần tiếp theo nhé. Đối với bài demo về Data thì có lẽ chúng ta sẽ tiếp tục vào thứ tư, đúng không? Đây cũng chỉ là phần đầu của công việc liên quan đến Data Engineering thôi. Nếu muốn một bài demo chi tiết hơn và sâu hơn, chúng ta sẽ phải đi sâu vào các khái niệm như MapReduce, và những kỹ năng chuyên môn khác. Đó là những kỹ năng cơ bản của một Data Engineer. Vậy thứ tư chúng ta sẽ tiếp tục, phải không? Hình như có bạn Nam Bùi đã nhắc đến một bài trước đó liên quan đến việc tóm tắt sách hoặc đọc file PDF hay truyện gì đó đúng không nhỉ?

**31:28** Nam Bùi, chuẩn bị lên giới thiệu một chút về tính năng AI của bên Figma nhé. Nam Bùi sẽ trình bày tiếp theo. Hôm nay, chúng ta còn có bạn Thông từ Holistic nữa, lát nữa mình sẽ mời bạn Thông lên để giao lưu và chia sẻ một chút.

**32:07**  Phần của mình là về việc tạo ra code từ file Figma bằng cách sử dụng AI. Ok, mình sẽ bắt đầu luôn. Đây là màn hình Figma, mọi người thấy rõ chưa?

**33:07** Đây là màn hình Figma của mình. Mình muốn chuyển một số thành phần (components) thành code và đảm bảo rằng nó có thể hoạt động đúng với các hành động cuối cùng (final action). Figma có một công cụ (tool) là "Figma to Code," và mình sẽ chọn plugin này. Sau đó, mình sẽ dùng chức năng "copy code," chọn tất cả các tùy chọn có sẵn và copy hết. Mình sẽ dán đoạn code này vào trong "flow AI" và bắt đầu chạy thử.

<iframe width="560" height="315" src="https://www.youtube.com/embed/lAk1QSl7qS0?si=AUJTYXNZZSAVCX5B&amp;start=2033" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

**33:53** Hiện tại, mình không chắc code này có đúng hay không, nhưng mình sẽ chạy thử và thấy nó hoạt động khá ổn. Thế là mình muốn chia sẻ lại cho mọi người. Đây là giao diện UI mà nó tạo ra, nhưng vẫn chưa hoàn thiện. Mình sẽ tinh chỉnh lại một chút để nó hoạt động đúng. Giờ mình sẽ thiết lập các component cần thiết và cấu hình chúng.

**36:11** Giả sử như mình sẽ thiết lập ngày tháng, hiện tại là ngày nào đó, nhưng mình sẽ đổi thành ngày mới cho phù hợp. Nó sẽ hiện thị chính xác ở đây. Giờ mình sẽ thực hiện bước tiếp theo để làm cho nó tương tác đúng với dữ liệu. Ví dụ như mình thiết lập để nó phản hồi chính xác với những giá trị mình đưa vào. Mình sẽ yêu cầu AI hoàn tất phần này.

**39:39** Như vậy là mình đã thử với một component rồi. Bằng cách sử dụng công cụ này, mình có thể chuyển đổi thiết kế từ Figma sang code và dán vào trong "flow AI" để nó hoạt động. Mình đã thử nghiệm với một component và thấy khá ổn.

Nam, bạn đã thử phần animation chưa? Animation à? Chưa thử, nhưng đó là một vấn đề mà mình cũng muốn tìm hiểu. Trước đây, sau khi thiết kế UI xong, việc chuyển đổi các phần animation thường mất rất nhiều thời gian. Nếu có thể chuyển được cả animation một cách tự động thì sẽ rất tuyệt vời.

**41:39** Dạ, thử làm việc với hướng đi đó nhé. Nếu như mình có thể convert đúng cái style hoặc chuyển đổi cả animation ở mức độ component, thì sẽ đẩy nhanh quá trình rất nhiều. Trước giờ, việc thiết kế thường phải dừng lại ở chỗ này, và chi phí cũng như thời gian cho đội ngũ ngồi làm phần đó là khá cao.

Dạ, ok. Em hiểu rồi. Em sẽ chuẩn bị cho lần demo sau.

Ừ, rồi ok. Chắc phần này mình tạm dừng ở đây trước đã, tranh thủ còn thời gian thì mời Thông lên chia sẻ một chút nhé. Thông, cái đề tài hôm qua mà bạn có gửi cho anh đó, bạn đã chuẩn bị kỹ chưa?

**42:22** Ok, có Thông lên rồi. Để giới thiệu nhanh một chút, bạn Thông là một thành viên của team Holistic, và họ có một sản phẩm BI Dashboard rất nổi tiếng. Đây là một trong những team mà mình rất tôn trọng trong việc làm sản phẩm. Thông ơi, hôm qua anh thấy có trao đổi về một vài đề tài mà em đưa ra. Anh chưa có dịp giới thiệu lại với mọi người, nhưng anh thấy rằng đó có thể là một đề tài rất thú vị. Em có thể thử chia sẻ về nó được không?

Có được không nhỉ? Thử xem lại một chút. Chắc bình thường là được thôi mà.

**43:09** Ủa, bình thường không vấn đề gì đúng không? Ừm, kiểm tra lại thử xem nhé, có lẽ là vấn đề về permission (quyền truy cập). Để xem lại nào. Chắc trước giờ chưa từng kết nối với bạn bè trên đây bao giờ, không biết có vấn đề gì không. Theo lý thuyết thì phải kết nối được rồi. Để kiểm tra lại phần quyền truy cập nhé. Nếu đang ở chế độ "newbie" trên đây, thì có thể cần kết nối lại.

Rồi, thử kiểm tra lại quyền truy cập trên trình duyệt xem sao.

Thông ơi, nếu dùng trình duyệt Chrome hoặc Safari, thì phần quyền truy cập nằm ở đâu nhỉ? Nếu là Safari thì nó sẽ nằm gần ô tìm kiếm (search bar) đó. Còn nếu dùng Windows thì…

**44:27** Mình cũng không chắc lắm nếu dùng Windows. Có ai biết không nhỉ? Dùng trình duyệt thì chắc là không phức tạp đâu, thường thì nó sẽ hỏi phần quyền truy cập thôi. Alo, alo? Ok, được rồi. Thông đã kết nối được rồi đó.

Tiếp tục câu chuyện nhé, mấy anh em trước đó có trao đổi với nhau và Thông hiện là thành viên của team Holistic. Chúng ta có nói chuyện về việc gặp gỡ, chia sẻ với nhau một lần. Hôm qua có trao đổi thêm một chút và Thông đã đề cập đến hai ba vấn đề mà team đang thử nghiệm. Mình không kỳ vọng nhiều lắm, nhưng nếu Thông có thể trình bày về các đề tài đó, thì chắc chắn sẽ rất thú vị. Đội Data Research (DR) của mình cũng đang khám phá những xu hướng hiện tại và những khả năng mới, và cũng muốn xem giới hạn của chúng ở đâu.

**45:24** Nếu tiện thì Thông có thể chia sẻ thêm về các đề tài và cách ứng dụng AI hiện tại. Nếu có thể thì đề cập đến hai đề tài đó để anh em nghe thử xem, nếu hứng thú thì chúng ta có thể gặp gỡ và giao lưu thêm lần khác.

Ồ, Nam, lên tiếp tục đi nào.

Xin chào mọi người, cảm ơn anh đã giới thiệu. Thật ra, hôm nay team em cũng có một buổi chia sẻ, nên em đã kéo vài bạn qua đây cùng tham gia. Đa số là team Product đang ngồi nghe chung rồi. Ok, em chia sẻ luôn nhé.

**46:02** Cảm ơn anh đã giới thiệu. Em và team em sẽ chia sẻ một chút về những bài toán mà tụi em đang làm. Thật ra, vì phần BI (Business Intelligence) rất rộng và cần nhiều kiến thức nền tảng, nên tụi em vẫn chưa tập trung nhiều vào AI. Chủ yếu là đang thử nghiệm một vài use case nhỏ để demo trước. Hiện tại tụi em đang có hai bài toán chính. Để dễ hiểu, em sẽ chia sẻ màn hình và nói thử xem mọi người hiểu được không.

Mọi người có nghe về tính năng Dashboard ESC chưa? Tụi em đang thử triển khai một tính năng lớn có tên là Dashboard ESC.

<iframe width="560" height="315" src="https://www.youtube.com/embed/lAk1QSl7qS0?si=SBLyM6MPgRgfAwUQ&amp;start=2918" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

**47:31** Nếu mọi người có sử dụng BI (Business Intelligence), thì thường các công cụ BI chủ yếu là các công cụ GUI (Graphical User Interface) để kéo thả và tạo ra các biểu đồ trực quan, đúng không? Bên team em muốn đẩy nó xa hơn một chút, đó là khi tạo ra một dashboard, nó sẽ sinh ra code tương đương với giao diện UI. Tức là mình có thể tạo một dashboard bằng code hoặc bằng UI, và hai cái này sẽ tự động đồng bộ với nhau. Mục đích là để có thể lưu trữ tất cả các phân tích này trong một Git repository, thực hiện CI/CD, refactoring, và làm cho việc tạo dashboard và visualization trở nên có thể lập trình được (programmable). Thêm vào đó là tính tái sử dụng (reusability).

**48:58** Vậy là cái mà anh em đang làm là chuyển đổi toàn bộ dashboard thành dạng code, đúng không? Tức là biến tất cả mọi thứ trên dashboard thành dạng văn bản (text) hết?

Đúng rồi anh, chính xác là như vậy. Khi biến nó thành code, mình có thể thực hiện version control, đẩy lên Git, làm branching các kiểu luôn. Điều này cũng giúp nhiều team có thể cùng nhau phát triển, kiểm soát môi trường dev/prod tốt hơn. Đó chính là cách mà tụi em muốn áp dụng cho dự án này.

Khi code được sinh ra từ UI, tụi em có thể dùng OpenAI để generate toàn bộ phần code này để tạo ra dashboard. Ví dụ như, ở trường hợp này, em sẽ dựa trên dataset đã được định nghĩa sẵn và từ đó sinh ra dashboard.

**49:35** Không biết mọi người có thấy màn hình được không nhỉ? Bên anh vẫn thấy được bình thường nhé. Ok, ví dụ em tạo một dashboard mới ở đây. Em có một nút AI, bên trong đó là một con Bot mà tụi em đã tạo sẵn với những chỉ dẫn (instructions) rõ ràng. Tuy nhiên, tụi em cũng giới hạn quyền lựa chọn của người dùng để tránh việc trả lời sai câu hỏi. Để em thử chọn ví dụ "User" với nhóm "City" xem sao. Bên dưới, nó sẽ chạy một prompt để sinh ra code bên tay trái này.

Thật ra, ở giữa có một file JSON để xác định xem nó sinh ra phần tử code nào (code elements). Em không phải là Engineer trực tiếp làm phần này, nhưng nếu mọi người muốn biết rõ hơn, tụi em có thể nhờ kỹ sư của tụi em lên trình bày chi tiết. Hiện tại nó đang ở giai đoạn beta, nên thỉnh thoảng có lúc work, có lúc không. Lúc nãy nó hoạt động tốt, nhưng bây giờ có vẻ không được.

**51:16** Nếu nó hoạt động bình thường, thì nó sẽ sinh ra hai filter ở đây và ba chart bên dưới. Điều này có nghĩa là từ UI, nó sẽ chuyển qua một lớp JSON rồi qua prompt, sau đó sinh ra giao diện UI cuối cùng. Cả quá trình đó đang cố gắng tự động hóa hoàn toàn.

Đúng vậy, nó sẽ sinh ra các đoạn text, rồi tự động lựa chọn dimension và measure phù hợp để tạo ra kết quả bên phải này dựa trên một số quy tắc mà tụi em thiết lập. Nó sẽ tự động sinh ra tiêu đề (title), mô tả (description), và các thành phần khác. Giống như việc bạn show một artifact trên hệ thống CL vậy, nhưng ở đây là từ text biến thành UI.

**51:58** Tất cả các thành phần UI là tụi em đã quy định trước, phải không? Đúng vậy, em không nhớ chính xác, nhưng nó dựa trên tổ hợp của số lượng dimension và measure. Mỗi measure sẽ kết hợp với một số dimension nhất định, ví dụ như một measure với ba dimension sẽ sinh ra khoảng sáu biểu đồ (chart). Mỗi dimension sẽ tạo ra hai biểu đồ.

Thật ra, tụi em cũng có option cho nó generate bất kỳ thứ gì, nhưng vì như vậy sẽ rất khó kiểm soát nên tụi em giới hạn lại, ví dụ như tạo ra một layout, một page với một bảng để hiển thị dimension và measure ở đây.

**53:20** Hiện tại thì tụi em vẫn đang trong giai đoạn thử nghiệm (testing). Mức độ hoàn thiện về mặt user experience (UX) vẫn chưa được kiểm chứng. Ban đầu, hy vọng là việc sử dụng code generation bằng LLM (Large Language Model) sẽ tăng tốc độ cho team phát triển (development team). Ban đầu chỉ muốn gây ấn tượng (impress) thôi. Muốn cho mọi người thấy rằng việc này hoàn toàn có thể được thực hiện bởi AI.

Nếu nhìn xa hơn, chúng ta có thể mong muốn rằng đoạn code này sẽ được hoàn thiện và tối ưu hơn.

**54:04** Khi sinh ra dữ liệu, nó nên có ý nghĩa hơn, phải có sự phù hợp và ngữ cảnh tốt hơn. Ví dụ như, nó có thể hiểu được rằng trong dataset này có những field nào liên quan để đưa ra các câu hỏi mà người dùng mong muốn. Để người dùng có thể nhập câu hỏi bằng ngôn ngữ tự nhiên, ví dụ như hỏi "Doanh thu ở Việt Nam là bao nhiêu?" thì nó sẽ tự động chọn field "revenue" và "country" là Việt Nam để tạo ra hai biểu đồ. Đó là hướng đi xa hơn trong tương lai, còn hiện tại thì nó vẫn còn khá cơ bản.

Điểm mạnh nhất của công cụ này là mọi thứ đều được chuyển thành code

**54:38** Bên tay trái này là phần syntax của YAML mà em vừa đề cập, đúng không? Đây là phần Editor ở phía bên trái?

Đúng rồi anh, chính xác.

Vậy hiện tại nó chưa ổn định là do phần chuyển đổi sang YAML chưa chính xác, phải không?

Đúng rồi, việc nó có chính xác hay không phụ thuộc nhiều vào cách mình kiểm soát kỳ vọng và outcome (kết quả). Quan trọng nhất là cái prompt (hướng dẫn) mà mình viết và cung cấp cho AI.

**55:22** Vậy hiện tại ai đang xây dựng các agent cho việc này? Là team Engineer hay team Product của em?

Hiện tại, cả team Engineer và team Product đều đang làm việc cùng nhau. Người trực tiếp viết các system prompts là một kỹ sư kết hợp với người bên Product. Product sẽ quản lý nhiều hơn về hành vi, tức là muốn nó hiển thị như thế nào, kết quả ra sao.

Ồ, hiểu rồi. Vậy là chất lượng phần output phụ thuộc vào người viết prompt đúng không?

Chính xác là vậy.

**56:08** Vậy dự án này tiến triển đến bao nhiêu phần trăm rồi em?

Thực ra, ban đầu team em cũng chưa có kế hoạch gì quá cụ thể. Chủ yếu là đang thử nghiệm thôi, chưa thật sự đầu tư nhiều. Nếu muốn làm đến nơi đến chốn thì phải đầu tư thời gian và nguồn lực nhiều hơn. Nếu làm nửa chừng rồi không work, mọi người sẽ quay lại trách mình.

À, vậy cái file YAML đó là đặc trưng của bên em hay là một dạng chuẩn?

Nó là do team em tạo ra, tụi em đã phát triển hai loại ngôn ngữ: một cái gọi là "Modeling Language" là YAML, và một cái là "Query Language" là AQL. Toàn bộ file này là YAML, nó sẽ khai báo các block (khối) cần thiết. AQL thì tương đương với SQL nhưng có một vài khác biệt về cú pháp và cách sử dụng.

**56:53** Để em ví dụ AQL, nó giống như SQL nhưng có một vài phần khác biệt. Ví dụ ở đây... (Em chỉ phần code trên màn hình). Không biết mọi người có câu hỏi gì thêm không nhỉ?

Ngoài bài toán này ra, còn bài toán nào nữa không? Hôm trước em có nói về hai bài toán mà.

Dạ, tụi em có nhiều bài toán nhỏ lẻ, em chưa đi qua hết được. Nhưng có một bài toán khá lớn là ngôn ngữ AQL này. Dù tụi em đã có documentation (tài liệu hướng dẫn) đầy đủ, nhưng việc người dùng áp dụng ngôn ngữ này có một learning curve (độ khó khi học). Tụi em đang tìm cách làm sao để người dùng có thể học và sử dụng AQL dễ dàng hơn. Ví dụ như, liệu AI có thể tự động tạo ra các câu lệnh AQL dựa trên tài liệu mà tụi em cung cấp hay không?

**57:59** Ồ, hiểu rồi, cái đó hoàn toàn khả thi nha. Nếu có đủ ví dụ, có thể dùng fine-tuning để hướng dẫn AI làm điều đó, đúng không?

Dạ, đúng vậy. Hiện tại tụi em đang tìm hiểu thêm. Em đang viết tài liệu hướng dẫn để người dùng hiểu được cách sử dụng AQL. Việc áp dụng AQL cũng hơi khó vì nó khác với mindset (cách suy nghĩ) của SQL. Trừ khi team Holistic đứng ở vị trí buộc người dùng phải sử dụng, sẽ khó để họ thay đổi cách suy nghĩ quen thuộc.

**58:37** Dù AQL có nhiều tính năng mạnh mẽ hơn SQL, nhưng cần phải thay đổi mindset của người dùng. Đó là lý do việc áp dụng cũng có phần thử thách. Hiện tại, tụi em đang viết thêm các ví dụ, nhưng số lượng ví dụ hiện nay cũng chưa đủ nhiều.

Nếu ví dụ đủ nhiều, thì AI có thể học và tạo ra các câu lệnh chính xác hơn đúng không?

Đúng rồi. Hiện tại, em đang cố gắng làm cho việc học ngôn ngữ AQL này trở nên dễ dàng hơn bằng cách sử dụng AI.

**59:25** Nếu AI có thể chuyển đổi từ ngôn ngữ tự nhiên sang AQL thì chắc chắn sẽ tiết kiệm rất nhiều thời gian cho người dùng.

Dạ đúng rồi, nếu AI có thể chuyển đổi từ ngôn ngữ tự nhiên sang AQL thì sẽ không cần phải học cú pháp AQL nữa.

Vậy trong quá trình triển khai, nếu AI hỗ trợ được chuyển đổi từ câu hỏi tiếng Anh sang câu lệnh AQL, thì mình có thể bỏ qua phần trung gian phải không?

Chính xác anh, nếu AI có thể làm được điều đó, chúng ta có thể bỏ qua bước trung gian.

**01:00:14** Nhưng nếu bỏ qua bước đó, liệu việc tạo ra một ngôn ngữ lập trình mới có còn cần thiết không?

Không hẳn là một Domain-Specific Language (DSL) đơn thuần, mà nó là một ngôn ngữ lập trình mới dành riêng cho việc truy vấn (query). Để nói rõ hơn, có lẽ nên nhờ một bạn khác trong team em trình bày thì sẽ chi tiết hơn.

**01:00:54** Ví dụ, trong SQL, tính tái sử dụng (reusability) rất kém, khó để tạo ra các hàm (function) hoặc mô-đun (module) có tính linh hoạt. Nhưng với AQL, nó có đầy đủ các khái niệm như function, variable, và nhiều tính năng lập trình khác. Điều này giúp nó trở nên maintainable (dễ bảo trì) hơn, reusable (có tính tái sử dụng) hơn, và hoạt động ở một cấp độ cao hơn SQL.

Ồ, ok. Vậy ngoài hai bài toán này, team em còn bài toán nào khác nữa không?

**01:01:36** Khi được áp dụng AI, thì giá trị thực sự của nó sẽ được thể hiện rõ hơn. Em nghĩ có hai bài toán chính ở đây. Thứ nhất là làm sao để tối ưu hóa trải nghiệm của người dùng (experience) bằng AI. Ví dụ như khi anh tạo một truy vấn (query), nó có thể đề xuất (suggest) cho anh xem là truy vấn đó có sai không, hoặc nên refactor (tái cấu trúc) như thế nào. Nó cũng có thể tự động thêm các mô tả (description) hoặc metadata để những người khác có thể dễ dàng khám phá hơn. Đây là bài toán liên quan đến việc cải thiện trải nghiệm của người dùng.

Bài toán thứ hai là bài toán về dịch vụ (service). Trong tương lai, làm sao để người dùng doanh nghiệp chỉ cần nhập một prompt mà có thể ra được kết quả mà không cần phải thông qua data analyst. Em nghĩ bài toán này cũng có rất nhiều người đang cố gắng giải quyết, nhưng nó vẫn có khá nhiều thách thức.

**01:02:17** Ví dụ như, thay vì yêu cầu một analyst phải ngồi xây dựng dashboard, thì người dùng doanh nghiệp chỉ cần hỏi "Revenue năm nay là bao nhiêu?" là hệ thống tự động đưa ra kết quả mà không cần phải hiểu rõ dữ liệu hoặc cách truy vấn nó. Bài toán này nhiều đội ngũ về BI (Business Intelligence) đang cố gắng giải quyết.

Thách thức chính là làm sao đảm bảo dữ liệu chính xác (data accuracy), làm sao để truy vấn đúng những gì cần thiết. Ví dụ, cách tính doanh thu (revenue) có thể khác nhau giữa các công ty, và việc đảm bảo rằng người dùng này chỉ truy cập được vào dữ liệu của họ, không truy cập chéo (cross-access) sang dữ liệu của người khác cũng là một vấn đề.

**01:02:52** Vậy các bạn Tom và Thành nghĩ sao? Vì team của mình cũng đang gặp những vấn đề tương tự.

Bên em thì thực ra cũng biết từ lâu là thị trường (market) hơi tương tự trong lĩnh vực của Prol, nhưng Prol không áp dụng được cho phân tích dữ liệu (analytics). Nếu có một giải pháp như vậy thì em nghĩ sẽ rất hay.

Câu chuyện về việc sử dụng ngôn ngữ tự nhiên (natural language) để truy vấn SQL thì có nhược điểm là cần phải đi vào chi tiết về dimension (kích thước) và measure (chỉ số). Nhưng nếu trên ngôn ngữ truy vấn của em đã chia sẵn dimension rồi thì có thể tiết kiệm được nhiều bước hơn.

**01:04:26** Thông, em nghĩ bài toán này có thể giải quyết một cách nghiêm túc không? Nếu có cơ hội thì chúng ta có thể ngồi lại một buổi khác để thảo luận sâu hơn.

Em thấy nó có vẻ cũng khá dễ làm dựa trên những gì em đã trình bày. Ý anh là bài nào?

Bài đầu tiên là về việc viết Custom System Prompt. Đây là bài dễ nhất mà team đang làm nhiều. Bài thứ hai cần xem ví dụ có đủ hay không, và cần kiểm tra kỳ vọng nữa. Anh thấy bài này nếu làm tốt thì có thể bỏ qua bước học AQL và sử dụng ngôn ngữ tự nhiên để truy vấn.

**01:05:07** Hiện tại, các bạn đang muốn dùng ngôn ngữ tự nhiên để sinh ra AQL thay vì đi thẳng qua SQL, đúng không?

Đúng rồi. Nếu mà người dùng doanh nghiệp không cần phải học mà vẫn có thể truy vấn một cách tự nhiên, thì đoạn code AQL sẽ tự động chạy.

Đúng rồi, mục tiêu là như vậy. Để chuyển từ việc yêu cầu một người làm analytics phải biết AQL, giờ đây người dùng doanh nghiệp bình thường có thể tự truy vấn và tạo ra dashboard (bảng điều khiển) của họ. Công cụ mà team đang xây dựng hướng đến mục đích này, phải không?

**01:05:55** Đúng vậy. Nghe có vẻ hợp lý, nhưng cũng có nhiều thách thức nhỏ bên trong. Ví dụ như, khi một người dùng doanh nghiệp hỏi "Active users của tháng này là bao nhiêu?" thì việc làm sao để AI hiểu và trả lời chính xác vẫn còn là một bài toán.

**01:06:33** Tháng này. Dạ, vấn đề là AI cần phải hiểu định nghĩa của "active user" vì mỗi nhóm, mỗi team có định nghĩa khác nhau. Cho nên, AI phải có khả năng hiểu đúng định nghĩa mà người dùng đang đề cập dựa trên dữ liệu hiện có trong dataset, trong modeling code của tụi em. Điều này tương đương với một bài toán mà team của anh cũng đang làm, đó là team đang có một bài toán về truy vấn thông tin du lịch.

Nghĩa là mỗi người dùng sẽ hỏi: "Link booking của tôi đâu?" hay "Lịch trình của tôi đâu?" Thì thông tin ngữ cảnh của người dùng đã được gói gọn trong hệ thống rồi. Nó chỉ là phần context đi kèm thôi, không phải là vấn đề chính. Vậy, mỗi hệ thống khi sử dụng giải pháp này đều bắt buộc phải bao gồm thông tin context đó, đúng không?

**01:07:54** Dạ đúng rồi, bước tiếp theo là nếu muốn giải quyết bài toán này một cách nghiêm túc, thì cần phải sắp xếp lại để đảm bảo rằng yêu cầu và dữ liệu kèm theo được hiểu rõ ràng. Giờ mới nói chuyện với nhau khoảng 10 phút thôi, nên mới hiểu sơ sơ. Chi tiết thì còn cần phải xem xét thêm các luồng demo để đảm bảo nó hoạt động đúng như mong đợi. Có thể cần nhiều ví dụ hơn, kiểu như các bài test để mô phỏng quá trình làm việc thực tế.

Dạ đúng rồi, sau này nếu thấy thú vị thì có thể ngồi lại để hai team mình cùng nghiên cứu thêm.

**01:08:33** Dạ, anh cứ báo em nếu cần sắp xếp. Hiện tại, ai đang định hướng cho phần này? Anh Huy ạ?

Thực ra là cả team đang cùng làm thôi, không chỉ riêng anh Huy. Nguyên cả team leadership đang cùng tham gia định hướng.

Vậy là team có nhiều co-founder?

Đúng rồi, có 5 người lận.

Ok, vậy ngoài các bài toán này, còn có vấn đề nào khác mà em muốn chia sẻ không?

Thật ra, em cũng chưa chuẩn bị nhiều lắm, chỉ mới có được chừng đó thôi.

**01:09:25** Tom với Thành, các anh còn câu hỏi nào về đề tài này không? Chắc là chưa đâu, để hôm nào setup một buổi khác rồi mình bàn tiếp.

Ok, cảm ơn Thông nhiều. Chúng ta còn đủ thời gian để tiếp tục bài của Thành hay là chuyển qua lịch trình khác?

Chắc là kịp bài ngắn của em đó, xem thử bài nào.

**01:10:40** Mọi người thấy màn hình chưa? Bài này chủ yếu có mấy tools thôi. Em sẽ giới thiệu sơ qua về lý do tại sao em chọn những tools này.

Tool đầu tiên là K9s. K9s giống như một tool để xem community logs, và nhìn chung nó cũng dễ sử dụng, khá giống với `kubectl logs`. Cơ bản là liên hệ được với cluster rồi namespace, và nó trông đẹp hơn, có tính tương tác (interactive) cao hơn một chút. Nó có một số lệnh menu như thế này để chọn và xem, khá trực quan. Nếu ai thích xài `kubectl logs` thì có thể tiếp tục xài, còn nếu không thì có thể thử dùng cái này.

**01:11:39** Tool thứ hai mà em thấy hay là HTTPie. HTTPie khá giống với `curl`, nhưng nó tốt hơn vì nó hỗ trợ rất nhiều tính năng mà `curl` hoặc những tool HTTP khác không có. Ví dụ như, HTTP/2, HTTP/3 by default đều có hỗ trợ, còn `curl` thì không. HTTPie cũng hỗ trợ nhiều tính năng khác nữa mà em không tiện liệt kê ở đây. Mọi người có thể tự tìm hiểu thêm.

**01:13:12** Tool thứ ba là Bat. Bat là một tool để đọc file giống như `cat`, nhưng nó hỗ trợ thêm tính năng syntax highlighting trên terminal. Tool này hữu ích cho những ai thường xuyên làm việc trên terminal, đặc biệt là những người dùng Linux.

Em nghĩ rằng mấy tool này chủ yếu dành cho những người thích sử dụng terminal-based app, kiểu như mình đang quay trở lại với việc sử dụng các ứng dụng trên terminal vậy. Ban đầu là từ CLI, chuyển qua GUI desktop app, rồi tới web app, và giờ là quay về terminal app.

<iframe width="560" height="315" src="https://www.youtube.com/embed/lAk1QSl7qS0?si=wlwOvmE6pIrFwH0A&amp;start=4410" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

**01:13:54** Bây giờ, kiểu như là có quá nhiều công cụ GUI rồi, có vẻ như đã bão hòa. Thế nên mọi người quay lại làm những cái tool CLI (command-line interface) để cảm thấy nó mượt hơn, dễ sử dụng hơn. Có lẽ là như vậy.

Vừa rồi, em điểm qua các công cụ tuần trước, chỉ có vậy thôi. Còn công cụ này là `searx-lobster` à?

Dạ, cái nào cũng được anh. Ý là anh có thể đưa link nào cũng được, không nhất thiết phải dùng link này. Nếu muốn, thay vì mở web, anh có thể dùng trực tiếp qua đây.

Ồ, tính ra mấy ông dev giờ hết việc để làm rồi nhỉ?

**01:14:36** Dạ đúng rồi. Tuần trước em cũng nói rồi, em có theo dõi một chút về câu chuyện này. Trong bài tuần trước, cách đây khoảng ba tuần, bên Golang cũng có một công cụ riêng, gọi là `genkit`. Mọi người có thể thử, nó khá dễ xài. Chỉ cần xài như những công cụ mà em vừa giới thiệu thôi. Chắc là nó mới xuất hiện, em cũng không rõ cộng đồng đang dùng như thế nào, nên phải đợi thêm thời gian để xem tình hình. Nếu mọi người muốn thử thì cứ thử, nó cũng dễ dùng.

Ý là nếu anh muốn code thử cái phần API trên terminal thì có thể dùng tool này, đúng không?

**01:15:20** Đúng rồi anh, nó gom lại từ nhiều công cụ khác thôi. Thực ra, công cụ này còn nhiều tính năng khác mà em không liệt kê hết. Chắc là phải đợi một thời gian nữa xem có thêm tính năng nào không. Hiện tại, Python vẫn là ngôn ngữ chủ đạo. Nó tương thích với mọi ngôn ngữ, miễn là có example thì nó sẽ chạy.

Ừ, đúng rồi. Ok, chắc là hết rồi. Cảm ơn mọi người.

Theo lịch trình, team mình sẽ nghe thêm một phần nữa về việc làm Data Reprocessing mà Tom làm hồi nãy trong cái folder 'bx'. Nếu tuần sau có thời gian thì chúng ta sẽ đi sâu hơn vào phần này. Còn không thì chúng ta sẽ quay lại những bài trước mà ba team đã làm.

**01:16:16** Nếu được thì mọi người nên xem trước trong tuần này, sau đó tuần sau chúng ta thử nghiệm một chút về YouTube transcription hoặc thử với Bin, một công cụ AI assistant đang dùng. Coi xem chúng ta có thể demo như thế nào và chia nhau tổng kết lại từng phần.

Ngoài ra, các bài toán về việc đưa dữ liệu vào, viết Custom Regex thì trước sau gì team mình cũng sẽ cần những tool để thực hiện. Nếu mọi người không có thời gian làm hoặc chưa kịp, thì cứ để cho team Linh ngồi làm và đẩy phần đó luôn. Chắc là tool gần nhất mình cần phát triển là một Project Reporter.

**01:17:02** Reporter kiểu tổng hợp thông tin từ nhiều nguồn và tạo ra một báo cáo (report template) về tình trạng dự án. Cái này sẽ khá hữu ích trong việc theo dõi dự án, đúng không?

Đúng rồi, em nghĩ vậy. Tom đang làm thêm một dự án là tạo comic script. Hôm trước mình có đề cập đến việc tạo một dự án tên là "WM Comic," tập trung vào các chủ đề liên quan đến tài chính và công nghệ. Mỗi chủ đề sẽ có khoảng ba đến năm comic strips theo phong cách hài hước.

**01:17:46** Tuần sau, Tom sẽ bắt đầu từ từ, có thể train một mô hình LoRA để vẽ mèo (cat drawing). Mục tiêu là những meme (grama) mà team mình thường thấy online sẽ được chuyển thành một comic strip giống như trang Monkey User hoặc XKCD. Nếu ai biết trang đó thì mình sẽ làm tương tự.

Trên nền đó, mình sẽ vẽ nhân vật theo phong cách của riêng mình, và đây cũng là cách để team làm PR, truyền thông ra bên ngoài.

**01:18:30** Vậy đó là kế hoạch cơ bản nhé. Ngoài ra, chắc mình sẽ điểm qua tình hình check-in của team mình sau khi kích hoạt lại việc đến văn phòng (office) một chút. Tuần trước, hay hai tuần trước gì đó, mình có nói về việc triển khai chiến dịch khuyến khích mọi người quay lại văn phòng.

Hiện nay, trang thiết bị cơ bản đã sẵn sàng, có khoảng ba bạn từ team Holistic đã quay lại văn phòng rồi. Bé Vi hôm trước cũng phỏng vấn trên Techy Story. Tình hình là các trang thiết bị đang dần được thiết lập lại.

**01:19:21** Mình có một kênh trên Slack để kiểm tra xem ai check-in ở văn phòng và ai không có mặt ở đó. Có một vài bạn check-in nhưng lại không có mặt ở văn phòng. Kỳ vọng của mình là mọi người sẽ cố gắng dành nhiều thời gian tại văn phòng hơn trong thời gian tới, để chúng ta có thể phối hợp và chia sẻ thông tin hiệu quả hơn.

**01:20:06** Hiện nay, về trang thiết bị thì đang trang bị cơ bản rồi, có khoảng ba bạn từ team Holistic cũng đến đây, giống như trước kia bé Vi có phỏng vấn trên Techy Story. Tình hình trang thiết bị cũng đã được khôi phục. Mình có một channel đang ẩn ở đây để theo dõi ai check-in vào văn phòng. Có một số bạn check-in nhưng thực tế không có mặt tại văn phòng, mọi người có thấy không?

Kỳ vọng là trong thời gian tới, anh hy vọng mọi người có thể lên văn phòng, ngồi cùng nhau nhiều hơn để trao đổi, chia sẻ công việc.

**01:20:41** Nhất là về workflow, căn bản là trong giai đoạn này workflow khi xây dựng sản phẩm sẽ thay đổi rất nhiều. Việc ngồi cạnh nhau sẽ giúp chuyển giao kiến thức (knowledge transfer) nhanh hơn so với ngồi online. Hiện tại, mấy buổi họp online chỉ giúp show nhanh kết quả, còn quá trình tìm ra giải pháp thì khó chia sẻ hơn. Việc ngồi cùng nhau một hoặc hai ngày một tuần sẽ giúp mọi người nắm bắt nhanh hơn, đặc biệt là với Tom và những bạn đã có kinh nghiệm, sẽ hỗ trợ nhanh hơn rất nhiều. Anh vẫn hy vọng mọi người chủ động quay trở lại văn phòng nhé.

**01:21:16** Channel check-in ở đây cũng có vài anh em check-in rồi. Mỗi tuần danh sách sẽ được post lại trong lobby để mọi người thấy, và đúng là danh sách này vẫn là những gương mặt cũ. Thật ra, cũng có thêm vài bạn mới, như bạn Cát, bạn Biên đã lên. Trước đây, Biên không hay lên văn phòng lắm, thường thì chỉ lên chơi thôi, chứ không phải lên làm việc. Nhưng bây giờ cũng bắt đầu xuất hiện những gương mặt quen thuộc hơn, đó là dấu hiệu tích cực.

Hy vọng mọi người có thể bắt đầu lại việc đến văn phòng một ngày trong tuần, tìm góc làm việc riêng của mình. Văn phòng hiện tại có thể chứa tối đa khoảng 12 người, không nhiều hơn. Mọi người cố gắng sắp xếp thời gian, đặc biệt trong giai đoạn này việc chuyển giao kiến thức là quan trọng nhất.

**01:21:50** Anh muốn thúc đẩy việc này vì muốn chuyển giao kiến thức về AI/ML, ngồi cùng nhau sẽ tạo ra nhiều ý tưởng hơn. Việc chỉ ngồi xem tutorial trên mạng thì không thể nào có được sự hiệu quả như khi ngồi cạnh nhau. Nhìn Tom làm việc mới thấy được sự dã man, mình còn thích nữa huống chi anh em khác.

Vậy là về việc quay lại văn phòng, anh cũng muốn Tom tham gia. Tom thì có một số công việc khác nữa nên có thể lúc lên lúc không, nhưng anh hy vọng Tom sẽ dành thời gian lên văn phòng cùng anh em để chia sẻ kinh nghiệm, vì đó là cách học nghề nhanh nhất.

**01:23:13** Ngoài ra, mỗi lần check-in thì mọi người sẽ nhận được 5 ICY. Nghe qua thì có vẻ không nhiều, nhưng khi cộng dồn thì số tiền này có thể dùng để trang trải tiền ăn uống mỗi tháng, có thể khoảng 3-4 triệu đồng, không ít đâu. Anh đã ngồi nhẩm tính rồi, những bạn trước giờ thường xuyên lên văn phòng sẽ được nhận khá nhiều.

Mỗi lần check-in, các bạn sẽ nhận ICY. Hiện nay, số ICY chưa được công bố ra ngoài vì sợ spam quá. Nhưng khi cộng dồn lại, số ICY này cũng đáng kể. Đây không phải là mục đích chính, nhưng sẽ là động lực khuyến khích mọi người lên văn phòng.

**01:23:44** Tóm lại, trong đợt này nếu có vấn đề gì chính, thì đây là những điểm cần lưu ý. Ngoài ra, về việc liên quan đến Memo, kiến thức, hay chia sẻ thì Huy Nguyễn đang tổng kết xong đợt, nhưng chắc chưa đủ. Cũng phải xem lại xem như thế nào, có thể còn chưa xong.

Kỳ vọng là đến nửa năm sau sẽ có iPhone 16 để đổi thưởng, hoặc nhanh hơn là đổi MacBook, nhưng còn tùy vào sự đóng góp của mọi người. Về chính sách, team chỉ có thể đặt ra những chính sách như vậy, còn mọi người có hưởng ứng hay không thì tùy.

**01:24:30** Nếu không có gì khác, thì hẹn gặp anh em vào thứ tư tuần sau nhé, để tiếp tục các phần còn lại. Nhớ là đừng quên check-in nhé. Ok, vậy là hết rồi. Nếu có vấn đề gì thắc mắc, mọi người cứ hỏi. Nếu không thì mình sẽ kết thúc ở đây.

Tạm biệt mọi người.

---

**English Transcript**

**00:00** Okay, can you all hear me clearly? We have about 12 minutes left before Tom demonstrates some live coding, although we might not have enough time for a full live session. We’ll probably have a demo focusing on data engineering techniques. Alright, Tom, let’s start.

Let me begin. Hello everyone, I’ll introduce a demo that I usually use. This demo is typically employed for data engineering, especially for preparing and cleaning data before analysis. In this step, we use AI to help clean the data and get ready for either data analysis or preparing the data itself.

**04:37** Let me share my screen. There’s no need for everyone to use Zoom. Can you all see my screen now? Yes, okay, great. So, let’s begin by introducing the dataset we’ll be working with. There are many types of data we can clean using a tool called Agent Zero. Today, we’ll use a dataset that involves extracting information from some source, resulting in a CSV file.

The CSV data is quite raw, arranged in a basic columnar format extracted from a web player. They usually extract this data, indicating what technology they use, like jQuery or Next.js, and then arrange it in a format that's quite difficult to work with. The dataset is separated by web pages, making it challenging to begin with.

Our goal is to transform it into a more comprehensive format, such as an infographic, or create a consolidated dataset with all the relevant data in a centralized manner. So, let’s move forward with this now.

**05:41** Agent Zero is a tool that serves as an agent; I just need to tell it what to do, and it will write the code for me. For example, in this case, the problem lies in the `ph` folder. So, I’ll instruct it to “Look into the `ph` folder and help me process all the CSV files.” I want to analyze which backend technologies these sites are using.

**06:22** Agent Zero is an AI agent tool, and you just need to communicate with it in natural language; it will automatically write the code for you. For example, if I have an issue with data located in the 'ph' folder, I simply tell it: "Look into the ph folder and help me process all of the CSV files. I want to do some data analysis to understand what backend technologies all of these sites are using and aggregate all of them." It seems like the UI is a bit buggy at the moment, but my goal is to analyze which backend technologies these websites are using. Agent Zero will utilize GPT-4 or GPT-4 mini to handle all these tasks.

**08:25** If it encounters any errors, it will automatically fix them. The process of Agent Zero consists of two parts: one part is running the code, and the other part is checking whether that code runs correctly. Here, it has already detected an error, so it will automatically correct it for me. At this stage, I just need to define my objective, and Agent Zero will write the code for me. From there, I can start analyzing the data from the websites I've downloaded, converting them into CSV files, and cleaning the data.

**09:06** Now, I'll ask it to create an infographic to aggregate all the backend technologies used by the websites. I want a visual representation to make the analysis easier. Therefore, I instruct it: "Create me an infographic inside the 'ph' folder to aggregate all of the backend programming languages which are used across all CSV files." Then it will automatically draw a chart using the Matplotlib library and export a PNG image for me. If it encounters any errors, it will automatically download the necessary libraries through pip and continue the process. This automation covers almost all my needs related to data processing. It will also keep all the work saved so that I can review it later.

**09:58** Currently, I don't want to review each individual result file, so I'll ask Agent Zero to output everything into the 'ph' folder for easy management. Later, if I need to use it again, I just need to go back to that folder. This feature is quite convenient for any further processing steps I may need.

**10:56** You can see that for tasks like creating a web crawler, I can also use a similar method. Agent Zero will read the website structure, upload the results, and all I need to do is specify the HTML and CSS tags I want to extract data from. Instead of writing the code manually, I can now have Agent Zero handle it for me.

**11:42** For instance, in this case, the easiest way is for me to delete a few unnecessary entries and then add some new rows to clean the data. If I want to generate code for data analysis or simply download a YouTube video and extract the first 10 seconds of it, Agent Zero can handle that as well. For example, I'll copy the URL of a YouTube video and instruct it: "Download this YouTube video and cut out the first 30 seconds of it." Agent Zero will automatically code the task, using the terminal to download the video and cut out the first 30 seconds as requested.

**12:37** During this process, it will automatically utilize the terminal, download the video, and extract the required segment. However, sometimes it may face minor issues, such as choosing which backend module to use for this process; for instance, it might be using GPT-4 mini. As you can see, it's actually using various tools to ensure the task is completed accurately.

**13:41** It seems that it's encountering an error when downloading or cutting the video. At this point, I only need to give it a bit more guidance or ask it to delete the current video download and try again. This process is almost fully automated and is extremely convenient for repetitive tasks.

**14:54** Because this is a long video, the demo might be a bit slow. I can try again with a shorter video to see how it performs. Now I'll copy the URL of a shorter video and instruct: "Download this YouTube video and get the first 30 seconds." This process might sometimes take a bit longer to run, but I just need to wait a bit, and the AI system will handle it and complete the task.

**16:01** There are some minor issues, for example, the current office setup might not allow downloading YouTube videos, so the process might be a bit slow. But fundamentally, if you want to perform tasks such as web data analysis or need an auto agent to handle complex tasks, Agent Zero is an excellent choice.

**17:43**
I can create an auto agent to handle situations like this, for instance, downloading videos, data analysis, or processing backend tasks. Agent Zero utilizes GPT-4 mini or other models depending on the requirement and can perform complex tasks efficiently.

**19:00** From here, if you want to delve deeper into using Agent Zero to generate code or create visual infographics from data, you can fully instruct it to export in different formats like CSV, JSON, or even Parquet charts. If your data is too large and you don’t want to use AI due to token costs, you can interact with the system through databases such as Dgraph DB or others. Agent Zero will assist in generating the necessary query commands, allowing you to interact with the database without having to write code from scratch.

**20:09** For data or data engineering tasks, I can instruct it to generate code in Pandas (Pandas DataFrame), for example. Oh, it seems like it's being blocked now [music plays in the background]. Ah, that’s right, probably due to the office network restrictions, it might not be able to download from external networks. But if I want to go deeper into writing code or creating an infographic that helps visualize data more clearly, I can have it export a CSV or JSON file. The best part is that it can even compile the data into the Parquet format if needed.

**21:13** If I have a relatively large dataset and don’t want to use AI to process it because it would consume too many tokens, I can ask Agent Zero to generate code for me, and it will organize the data into the required structures. For instance, I could interact with a database like DgraphDB or any other type of database, and Agent Zero will help me query the data without requiring much manual coding. This way, I can interact with the data without needing to intervene directly.

**22:04** Alright, do you have any questions about this section? If not, we'll move on to the next part. Oh, someone asked how Agent Zero differs from the frameworks we’ve shown before? The main difference is that with a framework, you have to write a lot of code. With Agent Zero, you don't have to code anything. Specifically, it automatically creates the tools and handles the requests. In contrast, with traditional frameworks, you have to create an Agent, add the tools, and set up a Runner for it to execute the outputs from those tools. Agent Zero creates the tools automatically; you don’t have to do anything. Let me check where it stores the data.

**22:44 I**t has a dedicated folder within Agent Zero, and when it completes a task, it saves it into its memory, specifically in SQLite. This memory stores all the tools that have been created and the related code snippets. For example, if I don't have a tool to download videos from YouTube, it will create one for me. If I want to scrape data from Facebook, it will also automatically generate a tool to handle that. And when I ask for it again, it will use the cached memory of that tool. Occasionally, if it hasn’t been used for a while, the cache might be cleared, but in general, it will retain the data for me. This is quite different from the old Auto-GPT.

**23:21** In the past, when using Auto-GPT, if you wanted to create an application for interviews or extract information from the web, you had to create a tool first and write the specific code for each task. With Agent Zero, you don't need to code anything; it does everything for you. For instance, when Mr. Ngoc Thanh used to work on this, he had to code everything manually, while I didn’t have to do anything and still got the results. Therefore, the environment and approach of Agent Zero is truly an automated tool that doesn't require much intervention, unlike other frameworks.

**24:05** So, what’s special about Agent Zero's architectural structure compared to other tools? In fact, what I find unique is that you can use it for data analysis or data engineering tasks very simply. For example, if you have an MP3 file and want to filter out unusual sounds, it can help you do that. I also remember when I had a large PDF file, and I needed to split it or merge it, Agent Zero performed this task very efficiently as well.

**24:59** However, if the requirements are more complex, it might not perform perfectly. For example, if I want to create a 3D Plot or a Scale Plot, Agent Zero can understand but isn’t always accurate. Therefore, Agent Zero serves as more of a "starting point," like a junior assistant, from which you’ll need to continue refining the tasks on this foundation.

**25:49** Oh, I just saw a new request to process a PDF file. Okay, let’s try it out. What would you like it to do with the PDF file? Convert it to Markdown, or would you prefer it to create an Altic file? This will be interesting to see how Agent Zero handles it. It seems there might be some data overlap or duplication, doesn’t it? Let me try downloading it again. I can either let it download for me or adjust this menu manually for it to be automatic. I’ll make some further adjustments.

**27:11** Alright, I’ll name the folder "Fusion." Let’s check what’s inside. Oh, it looks like there are some images in there. Now I’ll instruct Agent Zero to extract the images from the PDF file. Which image do you want to extract first? Ah, let’s go with the images first, okay. "Help me grab the images inside the Fusion PDF into a separate folder." Alright, here are the images, and they’ve been extracted. It seems like Agent Zero knew how to cut them out correctly.

**29:25** It seems to have successfully extracted the images from the library. We need to fine-tune it a bit to convert them from JPEG to PNG format. This will also allow us to keep the transparency intact. Done, everything is completed. Great job, this is excellent.

**29:39** Now, let’s open the Preview file and see if everything is stable and accurate. It’s honestly much more reliable than when I do it manually, which takes a lot of time. Thanks to Agent Zero, I didn’t have to write any code; it did everything for me. However, one drawback is that if there are tables in the PDF file, it will only extract them as images. It can’t maintain the original table format from the PDF. But still, it’s quite acceptable.

**30:37** Okay, does anyone have any questions? If not, we’ll move on to the next section. As for the Data demo, I think we’ll continue on Wednesday, right? This is just the initial part of the work related to Data Engineering. If we want a more detailed and in-depth demo, we’ll need to dive into concepts like MapReduce and other specialized skills. These are the fundamental skills of a Data Engineer. So, we’ll continue on Wednesday, correct? I believe Nam Bui mentioned an earlier topic about summarizing books or reading PDF files or some kind of story, didn’t he?

**31:28** Nam Bui, get ready to introduce a bit about the AI features of Figma on your side, alright? You’ll be presenting next. Today, we also have Thong from Holistic; later, I’ll invite Thong to join us for some sharing and interaction.

**32:07** My segment will be about generating code from a Figma file using AI. Okay, I’ll start now. Here’s the Figma screen, can everyone see it clearly?

**33:07** This is my Figma screen. I want to convert some components into code and ensure they work correctly with the final action. Figma has a tool called "Figma to Code," and I’ll select this plugin. Then I’ll use the "copy code" function, choose all available options, and copy everything. I’ll paste this code into "flow AI" and start running it.

**33:53** Currently, I’m not entirely sure if this code is correct, but I’ll run it and see that it works quite well. I wanted to share this with everyone. Here’s the UI interface it generated, although it’s not yet fully complete. I’ll tweak it a bit to make sure it works correctly. Now, I’ll set up the necessary components and configure them.

**36:11** For example, if I set up the date, and currently it’s set to a specific date, I’ll change it to the new date to make it suitable. It will display accurately here. Now, I’ll proceed to the next step to make it interact correctly with the data. For instance, I’ll configure it to respond precisely to the values I input. I’ll instruct the AI to complete this part.

**39:39** So, I’ve tried it with one component already. By using this tool, I can convert designs from Figma into code and paste it into "flow AI" to make it function. I tested it with one component, and it works quite well.

Nam, have you tried out the animation part yet? Animation? No, I haven’t tried that yet, but it’s something I want to explore. In the past, after completing the UI design, the step of converting animations usually took a lot of time. If we can automatically convert animations as well, that would be amazing.

**41:39** Yes, let's try working with that direction. If we can accurately convert the style or transition the animation at the component level, it will speed up the process significantly. Up to now, the design work often stops at this stage, and the cost as well as the time required for the team to handle this part is quite high.

Okay, I understand. I will prepare for the next demo session.

Alright, let’s pause this segment here for now. Since we still have some time left, let's invite Thong to share a bit. Thong, have you prepared for the topic you sent me yesterday?

**42:22** Okay, Thong is here. Let me quickly introduce him. Thong is a member of the Holistic team, and they have a very well-known BI (Business Intelligence) Dashboard product. It's one of the teams I highly respect in terms of product development. Thong, I noticed that yesterday you shared a couple of topics. I haven’t had a chance to introduce them to everyone yet, but I think they could be really interesting. Can you try sharing them with us?

Is that possible? Let’s check again. It should work fine.

**43:09** Oh, it seems to be working fine, right? Let’s check again, maybe it’s an issue with permissions. Let's take another look. I think it should connect without problems; I’ve never connected with friends here before, so I'm not sure if there might be any issues. In theory, it should work. Let’s review the access permissions. If you’re currently set as a "newbie" here, you might need to reconnect.

Okay, let's check the browser permissions.

Thong, if you're using Chrome or Safari, where would the access permissions be located? If it's Safari, it should be near the search bar. If you're using Windows, then…

**44:27** I’m not entirely sure about Windows. Does anyone know? When using a browser, it shouldn't be too complicated; usually, it prompts for access permissions. Hello, hello? Okay, it’s working now. Thong has successfully connected.

Let’s continue the discussion. The team had talked before, and Thong is currently a member of Holistic. We previously mentioned having a chance to sit down and share with each other. Yesterday, we discussed a bit more, and Thong mentioned two or three issues that the team is currently experimenting with. I’m not expecting too much, but if Thong could present those topics, they would definitely be interesting. Our Data Research (DR) team is also exploring current trends and new possibilities, and we’d like to see where the limits are.

**45:24** If it’s convenient, could you share more about those topics and how AI is being applied at the moment? Perhaps cover the two topics you mentioned earlier so that everyone can hear them. If there's enough interest, we could arrange another session to meet and explore further.

Oh, Nam, go ahead and continue.

Hello everyone, thank you for the introduction. In fact, my team also has a sharing session today, so I’ve brought a few team members here to join in. Most of the Product team is already here listening together. Okay, I’ll share now.

**46:02** Thank you for the introduction. My team and I will share a bit about the projects we're working on. In reality, since the BI (Business Intelligence) domain is vast and requires a lot of foundational knowledge, we haven’t fully focused on AI yet. Primarily, we’re experimenting with a few small use cases for demo purposes. Currently, we have two main projects. To make it easier to understand, I’ll share my screen and explain; let’s see if everyone can follow along.

Have you heard of the Dashboard ESC feature? We're trying to implement a major feature called Dashboard ESC.

**47:31** If you've worked with BI (Business Intelligence), you'll know that most BI tools are primarily GUI (Graphical User Interface) tools for dragging and dropping to create visual dashboards, right? Our team wants to take it a bit further, meaning that when you create a dashboard, it automatically generates code that corresponds with the UI. This means you can create a dashboard either via code or through the UI, and both will be automatically synchronized. The goal is to be able to store all these analytics in a Git repository, perform CI/CD, do refactoring, and make the process of creating dashboards and visualizations programmable. Additionally, it enhances reusability.

**48:58** So, what you’re working on is converting the entire dashboard into code, right? Essentially transforming everything on the dashboard into text format?

Yes, that's exactly right. When everything is converted into code, we can implement version control, push it to Git, and create branches. This also enables multiple teams to collaboratively develop and control both the development and production environments more effectively. That’s how we're applying this concept in our project.

When the code is generated from the UI, we can use OpenAI to generate all of this code to create the dashboard. For example, in this case, I will rely on a pre-defined dataset and generate the dashboard from that.

**49:35** Can everyone see the screen? From my side, it’s visible. Okay, let’s say I create a new dashboard here. I have an AI button that contains a bot we preconfigured with specific instructions. However, we’ve restricted user options to avoid incorrect responses. I’ll try selecting "User" and "City" as a group. It will then run a prompt to generate the code on the left side.

Actually, there’s an intermediate JSON file that determines which code elements are generated. I’m not the Engineer directly working on this, but if anyone wants more detailed information, we can have one of our engineers provide an in-depth explanation. Currently, it's in beta, so sometimes it works, and sometimes it doesn’t. Earlier it worked fine, but it seems to be having issues now.

**51:16** If it functions correctly, it will generate two filters here and three charts below. This means that from the UI, it transitions through a JSON layer, then through a prompt, and finally generates the UI interface. The whole process is trying to be fully automated.

Yes, it will generate text and automatically select the appropriate dimensions and measures to produce the result on the right based on some rules we've established. It will generate titles, descriptions, and other elements automatically. It’s similar to how you show an artifact in the CL system, but here, it’s converting from text to UI.

**51:58** All the UI components are pre-defined by your team, correct?

That’s right. I can’t recall all the details, but it’s based on combinations of dimensions and measures. For example, one measure with three dimensions will generate about six charts, with each dimension contributing two charts.

In reality, we have options that allow it to generate anything, but doing so makes it hard to control. Therefore, we limit it to generating a layout, a page, or a table to display the dimensions and measures here.

**53:20** Currently, we’re still in the testing phase. The level of completion regarding user experience (UX) hasn’t been fully validated. Initially, we hope that using code generation with LLM (Large Language Model) will accelerate the development team’s progress. Initially, the goal was just to impress, to show that this could be done entirely by AI.

If we look further ahead, the hope is that the generated code will be more complete and optimized.

**54:04** When generating data, it should be more meaningful, with better relevance and context. For example, it could identify which fields are related in a dataset to generate questions that users want. This way, users can input questions in natural language, like "What’s the revenue in Vietnam?" and it will automatically select the "revenue" and "country" fields to create two charts. That’s the direction we're aiming for in the future, but right now it’s still quite basic.

The most powerful aspect of this tool is that everything gets converted into code.

**54:38** The syntax on the left-hand side is the YAML part you mentioned, right? Is this the editor on the left side?

Yes, that’s correct.

So, the current instability is due to the conversion into YAML not being accurate, is that right?

Exactly. Whether it’s accurate or not depends a lot on how we control expectations and outcomes. The most crucial part is the prompt we write and provide to the AI.
**55:22** So, who is currently building the agents for this? Is it your Engineering or Product team?

Currently, both the Engineering and Product teams are working together. The person who writes the system prompts is an engineer working alongside someone from Product. The Product team will primarily manage the behavior, meaning how it should display and what the outcome should be.

Ah, I see. So the quality of the output depends on the person writing the prompt, correct?

Exactly.

**56:08** So, how far along is your project in terms of progress?

Actually, in the beginning, our team didn’t have a very specific plan. We’re mostly experimenting at this stage and haven't invested a lot of time or resources yet. If we want to do it properly, we would need to invest more effort. If we stop halfway and it doesn’t work out, people might come back and criticize us.

Oh, so the YAML file, is that something unique to your team or is it a standard format?

It was developed by our team. We’ve created two types of languages: one is called the "Modeling Language," which is YAML, and the other is the "Query Language," which is AQL. This entire file is in YAML, and it declares the necessary blocks. AQL is somewhat equivalent to SQL but has a few differences in syntax and usage.

**56:53** Let me give an example of AQL; it’s similar to SQL but with a few differences. For example, here... (I’m pointing to the code on the screen). Does anyone have any additional questions?

Besides this project, do you have any other projects you’re working on? You mentioned two earlier.

Yes, we have many smaller projects, but I haven't gone through all of them yet. However, one significant challenge we're facing is with the AQL language itself. Even though we have comprehensive documentation, there’s a learning curve for users to adopt this language. We're exploring ways to make it easier for users to learn and use AQL. For example, can AI automatically generate AQL queries based on the documentation we've provided?

**57:59** Ah, I see, that's entirely feasible. If there are enough examples, you could fine-tune the AI to do that, right?

Yes, exactly. We’re currently looking into that. I’m in the process of writing documentation to help users understand how to use AQL. The adoption of AQL can be challenging because it requires a different mindset compared to SQL. Unless Holistic is in a position where users are forced to use it, it will be tough to change their familiar way of thinking.

**58:37** Even though AQL has more powerful features than SQL, it requires a shift in mindset, making it challenging to adopt. Right now, we're adding more examples, but the number of examples isn't sufficient yet.

If there are enough examples, the AI could learn and generate more accurate queries, right?

Yes, that’s correct. Currently, I’m trying to make learning AQL easier by leveraging AI.

**59:25** If AI could translate from natural language to AQL, it would save users a lot of time.

Absolutely, if AI can handle the conversion from natural language to AQL, there would be no need to learn AQL syntax anymore.

So, during implementation, if AI can facilitate converting from English queries to AQL statements, can we bypass the intermediate step?

Exactly, if AI can do that, we can eliminate the intermediate step.

**01:00:14** But if we skip that step, would creating a new programming language still be necessary?

Not exactly—it’s not merely a Domain-Specific Language (DSL); it’s actually a new programming language dedicated to querying. To explain it better, I think it would be best if another team member could provide a more detailed presentation.

**01:00:54** For example, in SQL, reusability is quite limited, and it’s challenging to create flexible functions or modules. But with AQL, it incorporates all the concepts like functions, variables, and other programming features. This makes it more maintainable, reusable, and operates at a higher level than SQL.

Okay, got it. So, aside from these two projects, does your team have any other projects you're working on?

**01:01:36** When AI is applied, its real value will become more apparent. I think there are two main challenges here. The first one is how to optimize the user experience using AI. For example, when you create a query, the AI can suggest whether the query is incorrect or needs refactoring. It can also automatically add descriptions or metadata so that others can explore it more easily. This is the problem related to enhancing the user experience.

The second challenge is a service-related problem. In the future, how can we enable business users to just enter a prompt and get results without needing to go through a data analyst? I think many people are trying to solve this problem, but there are still quite a few challenges.

**01:02:17** For example, instead of needing an analyst to sit down and build a dashboard, business users could simply ask, "What's the revenue this year?" and the system will automatically provide the result without requiring them to understand the data or how to query it. Many teams in Business Intelligence (BI) are working to solve this problem.

The main challenge is ensuring data accuracy and making sure the queries are correct. For example, calculating revenue can vary from company to company, and ensuring that one user accesses only their own data without cross-accessing another’s is also a concern.

**01:02:52** What do you think, Tom and Thanh? Our team is also dealing with similar issues.

Well, on our side, we've known for a while that there is a similar market for Prol, but Prol isn’t suitable for analytics. Having a solution like this would be very beneficial.

The issue with using natural language to query SQL is that you often need to get into the details of dimensions and measures. However, if your query language already has dimensions pre-defined, you can save quite a few steps.

**01:04:26** Thong, do you think this problem can be tackled seriously? If there’s an opportunity, maybe we could arrange another session to dive deeper.

I think it seems quite doable based on what I’ve demonstrated. But which problem are you referring to?

The first one is about writing custom system prompts. That’s the easiest, and the team is working on it extensively. The second one requires checking if there are enough examples and testing expectations. I feel that if this is done well, we could bypass the step of learning AQL and instead use natural language for querying.

**01:05:07** Currently, your team wants to generate AQL using natural language instead of going directly through SQL, correct?

Yes, exactly. If business users don't need to learn and can query naturally, then the AQL code will run automatically.

Right, that’s the goal. Instead of requiring someone with analytics knowledge to understand AQL, now a regular business user can query and generate their own dashboard. That’s the tool your team is building, isn’t it?

**01:05:55** Yes, that’s right. It sounds reasonable, but there are still a few small challenges. For instance, when a business user asks, "What are the active users for this month?" the AI needs to be able to understand and provide an accurate answer, which is still a challenge.

**01:06:33** For this month? Yes, the issue is that AI needs to understand the definition of "active user" because each group or team may define it differently. So, the AI must be able to grasp the correct definition the user is referring to, based on the available data in the dataset and modeling code. This corresponds to a problem our team is also working on, which is querying travel information.

This means that every user will ask, "Where's my booking link?" or "Where’s my itinerary?" The user context is already encapsulated in the system, so it’s just an accompanying context and not the main issue. Every system that uses this solution has to include that context information, right?

**01:07:54** Yes, exactly. The next step is if we want to tackle this problem seriously, we need to arrange things to ensure that the requirements and accompanying data are clearly understood. We've only been discussing this for about 10 minutes, so we only have a basic understanding. The details still need to be reviewed further, such as examining the demo flow to ensure it works as expected. We may need more examples, like test cases, to simulate real-world workflows.

Yes, that’s right. If we find it interesting later, both teams can come together and study it more.

**01:08:33** Alright, let me know if you need to arrange anything. Currently, who’s leading this part? Is it Anh Huy?

Actually, the entire team is working on it, not just Anh Huy. The whole leadership team is involved in guiding it.

Oh, so there are many co-founders on your team?

Yes, there are five of them.

Okay, apart from these challenges, is there anything else you'd like to share?

Not really; I haven't prepared much yet—just up to this point so far.

**01:09:25** Tom and Thanh, do you have any more questions about this topic? Probably not, so let's set up another session to discuss it further another time.

Okay, thank you so much, Thông. Do we have enough time to continue with Thành's presentation, or should we move on to the next agenda item?

I think we have enough time for a short presentation from me; let’s take a look at one of my topics.

**01:10:40** Can everyone see my screen? This presentation mainly involves a few tools. I’ll briefly go over why I chose these tools.

The first tool is K9s. It’s like a tool for viewing community logs, and overall, it's quite easy to use—quite similar to `kubectl logs`. Basically, you just connect it to your cluster and namespace, and it has a more visually appealing, interactive interface. It offers some menu commands like these, making it very intuitive. If anyone prefers using `kubectl logs`, you can stick with that, but if not, you might want to try this out.

**01:11:39** The second tool that I find useful is HTTPie. HTTPie is quite similar to `curl`, but it’s more advanced as it supports many features that `curl` or other HTTP tools don’t. For example, HTTPie supports HTTP/2 and HTTP/3 by default, while `curl` does not. There are many other features that HTTPie offers, but I won’t list them all here. You can explore it yourself.

**01:13:12** The third tool is Bat. Bat is like `cat` for reading files, but it adds syntax highlighting support directly in the terminal. This tool is especially useful for those who frequently work on the terminal, especially Linux users.

I think these tools are mainly intended for those who prefer using terminal-based apps. It's like we’re going back to using terminal applications again. We started with CLI, then moved to GUI desktop apps, then web apps, and now we’re returning to terminal apps.

**01:13:54** Now, it seems like there are so many GUI tools available that it's becoming saturated. So people are turning back to CLI (command-line interface) tools because they feel smoother and easier to use. Maybe that’s why.

That’s all I have for the tools this week. Is this `searx-lobster`?

Yes, that’s one option, but you can use any link. It doesn't have to be this one. Instead of opening a web page, you can use it directly here.

Wow, developers really seem to be running out of things to do these days, huh?

**01:14:36 Y**es, it does feel that way. Last week, I mentioned that I was following this trend a bit. About three weeks ago, in a previous session, Golang introduced its own tool called `genkit`. You can give it a try; it’s pretty straightforward. Just use it as you would with the tools I’ve just mentioned. It’s quite new, so I’m not sure how widely the community is using it yet. We’ll need more time to assess it. If you want to try it out, just go ahead.

So if I want to code the API part directly on the terminal, I can use this tool, right?

**01:15:20** Yes, exactly. This tool consolidates several others into one. In fact, there are many more features that I haven’t covered. We’ll have to wait and see if more features are added later on. For now, Python is still the main language. It's language-agnostic, and as long as you have examples, it will run.

Yes, that’s true. Okay, I think that’s all. Thank you, everyone.

As per the schedule, our team will listen to another session on Data Reprocessing that Tom presented earlier using the 'bx' folder. If there’s time next week, we’ll delve deeper into this. Otherwise, we’ll return to the topics the three teams covered previously.

**01:16:16** If possible, everyone should review it this week, so that next week we can experiment with YouTube transcription or try out Bin, the AI assistant we’re currently using. Let’s see how we can demo this and collectively summarize each part.

Additionally, for tasks involving data input and writing custom Regex, our team will eventually need such tools. If anyone doesn’t have the time to do it or isn’t ready, we can let Linh’s team handle it and move forward with that part. The closest tool we need to develop is a Project Reporter.

**01:17:02** The Reporter is designed to aggregate information from multiple sources and generate a report template on project status. This would be quite helpful in project monitoring, right?

Yes, I think so. Tom is also working on another project, which involves creating a comic strip. We previously mentioned starting a project called "WM Comic," focusing on finance and technology topics. Each topic will have about three to five comic strips in a humorous style.

**01:17:46** Next week, Tom will gradually start, perhaps training a LoRA model to draw cats. The goal is to convert the memes (grama) that our team often sees online into a comic strip, similar to websites like Monkey User or XKCD. If anyone knows those sites, we’re aiming for something like that.

On that foundation, we’ll create our characters in our own style, which will be a way for the team to do PR and communication externally.

**01:18:30** So that’s the basic plan. Besides that, I’ll quickly review our team’s check-in status after reactivating the office visits. Last week, or maybe two weeks ago, I mentioned the campaign to encourage everyone to return to the office.

Currently, the equipment setup is ready, and about three members from the Holistic team have already returned to the office. Vi also did an interview on Techy Story previously, and the office equipment is being set up again.

**01:19:21** We have a Slack channel to track who checks in at the office and who isn't physically there. Some people check in but aren’t actually present in the office. My hope is that everyone will start spending more time in the office soon so that we can coordinate and share information more effectively.

**01:20:06** Currently, about three members from the Holistic team are back in the office, similar to when Vi previously did the interview on Techy Story. The equipment setup is back in place. We have a hidden channel to monitor who checks in at the office. You can see that some people check in without being physically present.

I hope everyone can make an effort to spend more time in the office to work and share knowledge together.

**01:20:41** Especially regarding workflow, fundamentally, the workflow for building products will change during this period. Sitting together will facilitate faster knowledge transfer than working online. Currently, our online meetings only allow us to quickly show results, but sharing the process of finding solutions is more difficult. Sitting together for one or two days a week will help everyone catch up more quickly. Especially with Tom and those who have experience, they’ll be able to support everyone more effectively. I still hope everyone will proactively return to the office.

**01:21:16** The check-in channel here already has a few members who have checked in. Every week, the list will be posted in the lobby for everyone to see, and, as expected, it’s still the usual faces. However, there are some new additions like Cat and Biên. Previously, Biên rarely came to the office—usually just to hang out, not to work. But now, familiar faces are starting to appear more frequently, which is a good sign.

I hope everyone can start coming to the office at least one day a week, claiming your own workspace. Our office can host up to 12 people, no more. Please try to arrange your time, especially during this phase, as knowledge transfer is crucial.

**01:21:50** I want to promote this because knowledge transfer, especially on AI/ML, will yield more insights when working together. Watching tutorials online doesn't quite have the same impact. Seeing Tom in action will be eye-opening, even I am impressed.

So that’s the update on returning to the office. I also want Tom to participate. Tom has other side projects, so his attendance might be sporadic, but I hope he can spend time in the office with everyone to share experiences, as that's the fastest way to learn.

**01:23:13** Additionally, each check-in grants 5 ICY points. It might not seem like much, but accumulated, it can cover food expenses each month, which might be around 3-4 million VND—not insignificant. I’ve done some calculations, and those who frequently come to the office will receive quite a bit.

Each time you check in, you receive ICY points. Currently, it’s not publicly posted to avoid spam, but once accumulated, it’s quite significant. This isn’t the main incentive, but it serves as a motivation for everyone to come to the office.

**01:23:44** In summary, these are the main points to note for this period. Regarding memo-related topics, knowledge sharing, or other updates, Huy Nguyễn is finalizing the summaries, but they might not be complete yet. We'll have to see how it turns out.

The goal is that by mid-year, we might have enough points for an iPhone 16, or maybe even swap for a MacBook, but that depends on everyone’s contribution. As for policy, the team can only set up these incentives; it's up to everyone whether to participate.

**01:24:30** If there’s nothing else, I’ll see everyone next Wednesday to continue with the rest. Don’t forget to check in via "We." Okay, that’s all. If anyone has any questions, feel free to ask. If not, we’ll wrap up here.

Goodbye everyone. 