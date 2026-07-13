---
description: >-
  Tài liệu dành cho người dùng client: cài đặt, đăng nhập, kích hoạt bản quyền
  và sử dụng toàn bộ tính năng Vidora.
---

# Hướng dẫn sử dụng Vidora

Vidora là ứng dụng desktop để tải, xử lý và quản lý video, âm thanh, hình ảnh và phụ đề. Tài liệu này dành cho người dùng bản client thương mại của Vidora.

> Vidora cần kết nối Internet và máy chủ bản quyền hoạt động. Ứng dụng chính chỉ mở sau khi tài khoản, thiết bị và mã bản quyền được máy chủ xác minh.

### Bắt đầu nhanh

1. Tải đúng bộ cài Vidora do nhà cung cấp gửi.
2. Cài đặt rồi mở Vidora.
3. Đăng nhập bằng email và mật khẩu.
4. Nếu thiết bị chưa được kích hoạt, nhập mã bản quyền và chọn **Kích hoạt bản quyền**.
5. Khi trạng thái bản quyền hợp lệ, chọn **Khởi chạy ứng dụng**.
6. Vào **Cài đặt > Phụ thuộc** để kiểm tra FFmpeg, yt-dlp và các công cụ cần thiết.
7. Chọn **YouTube** hoặc **Đa nền tảng**, thêm URL vào hàng đợi và bắt đầu tải.

### 1. Yêu cầu hệ thống

Vidora hỗ trợ các nền tảng sau:

* Windows 10 trở lên, kiến trúc x64.
* macOS 10.15 trở lên, Intel hoặc Apple Silicon tùy gói cài.
* Linux x64 hiện đại qua gói `.deb`, `.AppImage` hoặc `.flatpak` tùy bản phát hành.
* Kích thước cửa sổ mặc định là 1280 × 720; kích thước tối thiểu là 1100 × 620.
* Cần Internet, quyền truy cập máy chủ Vidora, tài khoản hợp lệ và mã bản quyền.

Các công cụ Vidora sử dụng:

* **yt-dlp**: engine tải video; được đóng gói hoặc quản lý trong ứng dụng.
* **FFmpeg**: cần cho ghép video và âm thanh, chất lượng cao, xử lý video, cắt file và phụ đề.
* **Deno**: được Vidora tự quản lý khi cần.
* **gallery-dl**: phải được cài ở cấp hệ thống nếu sử dụng trang Gallery.
* **aria2c**: tùy chọn để tăng khả năng tải; người dùng tự cài rồi bật trong Cài đặt.

### 2. Cài đặt Vidora

Chỉ tải Vidora từ liên kết chính thức do nhà cung cấp công bố trong Launcher hoặc kênh hỗ trợ. Không dùng bản cài từ nguồn không xác định vì mỗi bản production được cấu hình để kết nối với một máy chủ bản quyền cụ thể.

#### Windows

1. Mở file `.msi` hoặc `.exe`.
2. Làm theo trình cài đặt.
3. Mở **Vidora** từ Start Menu hoặc shortcut trên Desktop.

#### macOS

1. Mở file `.dmg`.
2. Kéo Vidora vào thư mục Applications.
3. Mở Vidora từ Applications.

#### Linux

Cài gói `.deb`, `.AppImage` hoặc `.flatpak` tương ứng với bản phân phối. Với AppImage, hãy cấp quyền thực thi trước khi mở.

### 3. Đăng nhập và đăng ký

Khi mở Vidora, Launcher xuất hiện trước ứng dụng chính.

#### Đăng nhập

1. Chọn **Đăng nhập**.
2. Nhập email và mật khẩu.
3. Bật **Ghi nhớ đăng nhập** nếu muốn lưu email cho lần sau. Vidora không lưu mật khẩu trong tùy chọn này.
4. Chọn **Đăng nhập**.

Bản client hiện yêu cầu xác thực lại khi khởi động tiến trình mới. Nếu thiết bị đã kích hoạt và vẫn hợp lệ, thông thường bạn không cần nhập lại mã bản quyền.

#### Đăng ký

1. Chọn **Đăng ký**.
2. Nhập email, mật khẩu và xác nhận mật khẩu.
3. Mật khẩu phải dài từ 12 đến 128 ký tự.
4. Chọn **Tạo tài khoản** hoặc nút đăng ký được hiển thị.

Nhà vận hành có thể tắt đăng ký công khai trên production. Nếu không đăng ký được, hãy dùng tài khoản do nhà cung cấp cấp hoặc liên hệ hỗ trợ.

Các nút Google, Discord và Quên mật khẩu chỉ hoạt động khi nhà vận hành đã cấu hình liên kết tương ứng.

### 4. Kích hoạt bản quyền

Mã bản quyền Vidora có dạng `VIDORA-XXXXXX-XXXXXX-XXXXXX-XXXXXX-XXXXXX-XXXXXX`.

1. Đăng nhập trong Launcher.
2. Mở phần **Bản quyền** hoặc màn hình **Kích hoạt Vidora**.
3. Nhập mã vào ô **Mã bản quyền**.
4. Chọn **Kích hoạt bản quyền**.
5. Chờ máy chủ xác minh tài khoản, key và thiết bị.

Kích hoạt sẽ liên kết một mã bản quyền với một tài khoản và một thiết bị. Không chia sẻ email, mật khẩu hoặc key cho người khác.

Các lỗi thường gặp:

* **Mã không hợp lệ**: kiểm tra ký tự, dấu gạch ngang và nguồn cấp key.
* **Bản quyền hết hạn hoặc bị thu hồi**: liên hệ nhà cung cấp.
* **Key đã gắn với thiết bị khác**: hủy kích hoạt máy cũ trước khi chuyển máy.
* **Thiết bị đã liên kết tài khoản khác**: liên hệ hỗ trợ để kiểm tra binding.
* **Không đọc được ID phần cứng**: khởi động lại ứng dụng; nếu vẫn lỗi, gửi Nhật ký cho hỗ trợ.
* **Quá nhiều lần thử**: chờ một lúc rồi thử lại.

Vidora không hiển thị HWID thô. Machine ID trong giao diện chỉ là mã nhận diện rút gọn phục vụ hỗ trợ.

### 5. Sử dụng Launcher

Launcher chính gồm các mục:

* **Tổng quan**: trạng thái bản quyền, thông báo, banner và liên kết nhanh.
* **Tin tức**: bản cập nhật và changelog do nhà vận hành công bố.
* **Tải xuống**: liên kết tải phiên bản chính thức.
* **Hàng đợi**: trạng thái các tác vụ đã lưu.
* **Bản quyền**: kích hoạt và xem thông tin key hiện tại.
* **Cài đặt**: tùy chọn Launcher.
* **Hỗ trợ**: Discord, website, tài liệu và kênh hỗ trợ đã cấu hình.
* **Giới thiệu**: phiên bản Launcher và thông tin build.

Nút **Khởi chạy ứng dụng** chỉ bật khi bản quyền hợp lệ, backend trực tuyến và không có bảo trì hoặc cập nhật bắt buộc. Mỗi lần bấm, Launcher gọi máy chủ để cấp quyền lần cuối rồi mới mở client.

Khi client đang chạy, Vidora tiếp tục xác minh quyền sử dụng khoảng mỗi 30 giây và nhận lệnh vô hiệu hóa trực tiếp từ máy chủ. Nếu key bị thu hồi, tài khoản bị khóa hoặc phiên không còn hợp lệ, client sẽ quay lại Launcher.

### 6. Giao diện chính

Thanh bên của Vidora có 12 màn hình:

* **YouTube**
* **Đa nền tảng**
* **Gallery**
* **Kênh**
* **Tóm tắt AI**
* **Xử lý video**
* **Phụ đề**
* **Dịch video**
* **Xuất dữ liệu**
* **Thư viện**
* **Nhật ký**
* **Cài đặt**

Bạn có thể đổi ngôn ngữ, giao diện sáng/tối và thu gọn thanh bên ở khu vực điều hướng.

### 7. Thiết lập ban đầu

Trước lần tải đầu tiên:

1. Vào **Cài đặt > Phụ thuộc**.
2. Kiểm tra trạng thái yt-dlp, FFmpeg và Deno.
3. Cài FFmpeg nếu Vidora báo thiếu.
4. Vào **Cài đặt > Tải xuống** và chọn thư mục mặc định.
5. Chọn định dạng, chất lượng, số lượt tải đồng thời và giới hạn tốc độ phù hợp.
6. Nếu cần tải nội dung đăng nhập, cấu hình cookies tại **Cài đặt > Mạng & Xác thực**.
7. Chỉ bật proxy khi mạng của bạn thực sự cần proxy.

### 8. Tải video YouTube

1. Chọn **YouTube** trên thanh bên.
2. Chọn chế độ **Đơn**, **Nhiều** hoặc **Từ khóa**.
3. Dán một hay nhiều URL hoặc nhập từ khóa tìm kiếm.
4. Chọn **Thêm vào hàng đợi**.
5. Mở **Cài đặt nhanh** cho từng mục nếu cần.
6. Chọn **Video** hoặc **Âm thanh**, chất lượng, định dạng, codec, FPS, phụ đề và thư mục lưu.
7. Với playlist, bật chế độ playlist và kiểm tra phạm vi mục cần tải.
8. Chọn **Bắt đầu tải**.

Vidora còn hỗ trợ:

* Tải playlist và live stream.
* Tải một khoảng thời gian cụ thể của video.
* Hẹn giờ tải.
* Tải phụ đề và thumbnail.
* SponsorBlock khi đã bật.
* Tự thử lại theo cấu hình.
* Phát hiện video trùng từ Thư viện; bạn có thể bỏ qua hoặc thêm lại.

Nếu cần video riêng tư, giới hạn tuổi hoặc nội dung yêu cầu đăng nhập, hãy cấu hình cookies đúng trình duyệt trong **Mạng & Xác thực**.

### 9. Tải đa nền tảng

Trang **Đa nền tảng** dùng yt-dlp để xử lý TikTok, Instagram, Facebook, X/Twitter, Bilibili, Youku và hơn 1.800 website được hỗ trợ.

1. Mở **Đa nền tảng**.
2. Dán URL nội dung.
3. Thêm vào hàng đợi.
4. Chọn video hoặc âm thanh và các tùy chọn đầu ra.
5. Chọn **Bắt đầu tải**.

URL video Douyin được xử lý ở trang Đa nền tảng. Hiện Vidora chưa hỗ trợ theo dõi hồ sơ Douyin trong trang Kênh.

Một số nền tảng thay đổi cơ chế thường xuyên. Khi lỗi, hãy cập nhật yt-dlp, kiểm tra cookies và thử lại với URL gốc trên trình duyệt.

### 10. Tải Gallery

Gallery dùng để tải bộ sưu tập ảnh, feed creator, chương truyện tranh và các gallery được gallery-dl hỗ trợ.

1. Cài `gallery-dl` ở cấp hệ thống.
2. Vào **Cài đặt > Phụ thuộc** để xác nhận Vidora nhận diện được công cụ.
3. Mở **Gallery**.
4. Dán URL bộ sưu tập.
5. Chọn thư mục lưu và bắt đầu tải.

Nếu thấy thông báo **Cần có gallery-dl**, chọn **Mở Dependencies** và hoàn tất cài đặt trước.

### 11. Kênh và tự động tải

Trang **Kênh** hiện hỗ trợ theo dõi 9 nền tảng:

* YouTube
* Bilibili
* Youku
* TikTok
* Vimeo
* Dailymotion
* Twitch
* SoundCloud
* Niconico

Cách duyệt và theo dõi:

1. Dán URL hồ sơ hoặc URL kênh, không dán URL video riêng lẻ.
2. Chọn **Lấy danh sách video**.
3. Chọn từng video hoặc **Chọn tất cả**.
4. Chọn **Tải đã chọn** để tải ngay.
5. Chọn **Theo dõi** nếu muốn lưu kênh.
6. Mở cài đặt kênh để bật **Tự động tải**, đặt chu kỳ kiểm tra, chất lượng và bộ lọc từ khóa.
7. Dùng **Kiểm tra ngay** để tìm nội dung mới mà không chờ chu kỳ.

Khi bỏ theo dõi, dữ liệu video đã lưu của kênh có thể bị xóa khỏi cơ sở dữ liệu Vidora; các file media đã tải trên ổ đĩa không bị xóa theo thao tác này.

### 12. Tóm tắt AI

1. Vào **Cài đặt > Tính năng AI**.
2. Chọn nhà cung cấp như Gemini, OpenAI, DeepSeek, Qwen, Ollama, LM Studio hoặc endpoint tương thích được hỗ trợ.
3. Nhập API key hoặc địa chỉ dịch vụ cục bộ theo nhà cung cấp.
4. Mở **Tóm tắt AI**.
5. Dán URL YouTube, chọn kiểu tóm tắt và ngôn ngữ.
6. Chọn **Tóm tắt**.
7. Sao chép kết quả hoặc **Lưu vào thư viện**.

Với video không có transcript phù hợp, Vidora có thể cần Whisper và FFmpeg để tạo nội dung đầu vào. Dịch vụ AI bên ngoài có thể tính phí theo tài khoản của bạn.

### 13. Xử lý video

Trang **Xử lý video** cho phép mô tả thao tác bằng ngôn ngữ tự nhiên, chẳng hạn cắt đoạn, nén, đổi kích thước, tách âm thanh, tạo GIF, chèn watermark hoặc ghép file.

1. Chọn file nguồn.
2. Nhập yêu cầu rõ ràng.
3. Kiểm tra kế hoạch và lệnh FFmpeg Vidora tạo ra.
4. Xác nhận chạy.
5. Theo dõi tiến trình và mở file đầu ra khi hoàn tất.

Luôn kiểm tra đường dẫn, định dạng và thao tác trước khi xác nhận. Tác vụ này cần FFmpeg.

### 14. Phụ đề

Trang **Phụ đề** là Subtitle Workshop tích hợp.

Bạn có thể:

* **Mở File Phụ Đề**, **Tải từ URL** hoặc **Tạo Mới**.
* Tạo phụ đề bằng Whisper.
* Chỉnh nội dung và thời gian từng câu.
* Tìm và thay thế, tách hoặc gộp câu.
* Kiểm tra QC, tốc độ đọc và lỗi chồng thời gian.
* Dịch bằng AI và sửa ngữ pháp.
* Đồng bộ với video, waveform và cảnh cắt.
* Xuất SRT, VTT hoặc ASS.
* Chuyển đổi hàng loạt.

Hãy lưu bản sao trước khi chạy sửa hàng loạt hoặc dịch toàn bộ dự án.

### 15. Dịch video bằng OCR

Trang **Dịch video** dùng OCR để trích phụ đề cháy trong khung hình.

1. Chọn video.
2. Khoanh vùng chỉ chứa phụ đề.
3. Chọn ngôn ngữ nguồn.
4. Chọn chế độ **Nhanh**, **Tự động** hoặc **Chính xác**.
5. Chọn **Trích xuất phụ đề**.
6. Kiểm tra kết quả và mở trong Subtitle Workshop để sửa.
7. Xuất SRT hoặc TXT.

Vùng OCR càng sát dòng phụ đề thì tốc độ và độ chính xác càng tốt.

### 16. Xuất dữ liệu và Assets

Trang **Xuất dữ liệu** có hai nhóm chính:

* **Dữ liệu**: lấy metadata từ playlist, kênh, từ khóa hoặc danh sách URL rồi xuất CSV, Excel, JSON, Markdown, XML, YAML, SQLite, Word và các định dạng hỗ trợ khác.
* **Assets**: tải thumbnail, phụ đề, bình luận và tài nguyên liên quan khi nguồn hỗ trợ.

Kiểm tra số lượng mục và trường dữ liệu trước khi chạy tác vụ lớn.

### 17. Thư viện

**Thư viện** là nguồn lịch sử lâu dài của nội dung đã tải. Dữ liệu được giữ cho đến khi bạn tự xóa hoặc dọn Thư viện.

Bạn có thể:

* Tìm kiếm và lọc lịch sử.
* Gắn tag và tạo bộ sưu tập.
* Phát media.
* Đổi tên hoặc mở vị trí file.
* Tải lại.
* Tách hoặc cắt file media.
* Tạo tóm tắt AI.
* Xóa chỉ bản ghi hoặc xóa cả bản ghi và file tùy lựa chọn.

Vidora dùng chính Thư viện để phát hiện video tải trùng. Không nên xóa lịch sử nếu bạn vẫn muốn tính năng này nhận biết các lượt tải trước.

### 18. Nhật ký

Mở **Nhật ký** khi cần kiểm tra tác vụ hoặc gửi thông tin cho hỗ trợ.

Các bộ lọc gồm **Lệnh**, **Thông tin**, **Thành công** và **Lỗi**. Bạn có thể tìm kiếm, làm mới, xuất hoặc xóa nhật ký.

Khi báo lỗi, hãy gửi:

* Phiên bản Vidora.
* URL hoặc nền tảng gặp lỗi, nếu được phép chia sẻ.
* Thời điểm xảy ra lỗi.
* Thông báo hiển thị.
* File nhật ký đã xuất.

Xóa hoặc che cookies, token, API key và thông tin cá nhân trước khi gửi công khai.

### 19. Cài đặt

Vidora hiện có các nhóm cài đặt:

* **Chung**
* **Tài khoản & License**
* **Phụ thuộc**
* **Tải xuống**
* **Tính năng AI**
* **Mạng & Xác thực**
* **Plugin**
* **Tải từ xa**
* **Extension**
* **Giới thiệu**

Chỉ cài plugin `.ywp` từ nguồn tin cậy. Plugin có thể tham gia quy trình sau tải và tác động đến file của bạn.

### 20. Chuyển bản quyền sang máy khác

1. Trên máy cũ, mở **Cài đặt > Tài khoản & License**.
2. Chọn **Hủy kích hoạt thiết bị**.
3. Đăng xuất hoặc đóng Vidora.
4. Trên máy mới, cài đúng bản Vidora.
5. Đăng nhập cùng tài khoản và kích hoạt lại key.

Nếu không còn quyền truy cập máy cũ hoặc đã thay đổi phần cứng lớn, liên hệ nhà cung cấp để yêu cầu xử lý binding. Không cố kích hoạt liên tục vì hệ thống có giới hạn tần suất.

### 21. Khắc phục sự cố nhanh

#### Không đăng nhập được

* Kiểm tra email và mật khẩu.
* Xác nhận đang dùng đúng bản client do nhà cung cấp phát hành.
* Kiểm tra Internet và trạng thái Backend ở Launcher.
* Nếu tài khoản bị tạm ngưng, liên hệ hỗ trợ.

#### Không kích hoạt được key

* Nhập lại key, không thêm khoảng trắng.
* Kiểm tra key đã dùng trên máy khác hay chưa.
* Kiểm tra thời hạn và trạng thái key.
* Khởi động lại nếu không đọc được thông tin thiết bị.

#### Nút Khởi chạy ứng dụng bị khóa

* Bản quyền chưa hợp lệ.
* Backend đang ngoại tuyến.
* Hệ thống đang bảo trì.
* Phiên bản client thấp hơn phiên bản tối thiểu hoặc có cập nhật bắt buộc.

#### Tải thất bại

* Cập nhật yt-dlp.
* Cài hoặc kiểm tra FFmpeg.
* Kiểm tra cookies với nội dung cần đăng nhập.
* Thử tắt proxy hoặc aria2 nếu vừa thay đổi cấu hình.
* Mở Nhật ký để xem lỗi cụ thể.

#### Video không có âm thanh hoặc không ghép được

Kiểm tra FFmpeg tại **Cài đặt > Phụ thuộc**, sau đó tải lại.

#### Gallery không hoạt động

Cài gallery-dl trên hệ thống và mở lại Vidora.

### 22. An toàn và sử dụng có trách nhiệm

* Chỉ tải nội dung bạn sở hữu, được cấp quyền hoặc pháp luật cho phép.
* Tuân thủ điều khoản của từng nền tảng và quy định bản quyền.
* Không chia sẻ tài khoản, key, cookies, API key hoặc token.
* Chỉ dùng plugin, proxy và file cài từ nguồn đáng tin cậy.
* Sao lưu dữ liệu quan trọng trước khi xử lý hoặc xóa hàng loạt.

Tài liệu này mô tả dòng Vidora 0.20.0 hiện tại. Nhãn giao diện có thể thay đổi nhẹ theo ngôn ngữ, cấu hình của nhà vận hành và phiên bản được phát hành.
