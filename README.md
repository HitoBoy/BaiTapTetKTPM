# BaiTapTetKTPM
**Bài tập Tết môn KTPM**

1. Docker là gì?
  - Docker là nền tảng phần mềm cho phép bạn dựng, kiểm thử và triển khai ứng dụng. Docker cho phép bạn tạo các môi trường độc lập và tách biệt để khởi chạy và phát triển ứng dụng một cách nhanh chóng. Bằng Docker, bạn có thể quản lý môi trường của bạn cũng như cách bạn quản lý các ứng dụng. Bằng cách tận dụng các phương pháp của Docker cho việc vận chuyển, kiểm thử và triển khai code, bạn có thể giảm đáng kể thời gian trễ giữa việc viết mã và chạy nó.

2. Docker-composer là gì?
  - Docker-composer là một công cụ dùng để định nghĩa và chạy các chương trình Docker sử dụng nhiều container (multi-container). Với Docker-composer, bạn có thể sử dụng một file YAML để thiết lập các service cần thiết cho chương trình. Cuối cùng, với một câu lệnh, bạn có thể create và start tất cả service từ các thiết lập đó. Gồm 3 bước chính:
    1. Khai báo các môi trường của chương trình trong Dockerfile.
    2. Khai báo các service cần thiết cho chương trình trong file docker-compose.yml để các service có thể chạy cùng với nhau trong một môi trường.
    3. Chạy câu lệnh docker-compose up để start Compose và chạy chương trình.
  - Một trong những ưu điểm khi sử dụng docker-composer là bạn có thể định nghĩa ngăn xếp ứng dụng của bạn trong 1 file, đặt nó tại root của repo của project của bạn, và dễ dàng cho phép người khác tham gia vào project của bạn. Người khác chỉ cần clone repo của bạn và chạy ứng dụng bằng composer.

3. So sánh giữa Linux, Unix, BSD và *nix:

  - Unix, Linux, BSD và *nix (đại diện cho "hệ điều hành dựa trên Unix") đều là các hệ điều hành có nguồn gốc từ hệ điều hành Unix ban đầu và chia sẻ nhiều đặc điểm chung, nhưng cũng có những khác biệt quan trọng:

    - Unix:
      - Unix là hệ điều hành gốc và được phát triển bởi AT&T Bell Labs vào cuối những năm 1960 và đầu những năm 1970.
      - Unix không phải là mã nguồn mở, mà là một hệ điều hành thương mại.
      - Unix đưa ra nền tảng cho nhiều hệ điều hành dựa trên Unix khác, như Linux và BSD.

    - Linux:
      - Linux là một hạt nhân (kernel) hệ điều hành mã nguồn mở được tạo ra bởi Linus Torvalds vào những năm 1990.
      - Linux không chỉ là hạt nhân mà còn là tên gọi chung cho các bản phân phối hệ điều hành dựa trên hạt nhân Linux cùng với các công cụ hệ thống và ứng dụng mở rộng khác.
      - Linux phát triển nhanh chóng và hiện đang được sử dụng rộng rãi từ các máy tính cá nhân đến các hệ thống máy chủ và nhúng.

    - BSD (Berkeley Software Distribution):
      - BSD là một dòng hệ điều hành dựa trên Unix được phát triển tại Đại học California, Berkeley.
      - BSD bắt đầu từ mã nguồn của Unix và sau đó đã phát triển thành các hệ điều hành độc lập.
      - BSD có một số biến thể như FreeBSD, OpenBSD, và NetBSD, mỗi biến thể có mục tiêu và điểm mạnh riêng.

    - Hệ điều hành dựa trên Unix (Unix-like OS hoặc nix):
      - *nix là thuật ngữ dùng để mô tả bất kỳ hệ điều hành nào có nguồn gốc từ Unix hoặc chia sẻ nhiều đặc điểm với Unix.
      - Nó bao gồm cả Unix, Linux, BSD và các hệ điều hành dựa trên Unix khác như macOS (dựa trên Darwin, một BSD variant) và Solaris.
      - Các hệ điều hành *nix chia sẻ một số triết lý và cơ sở kỹ thuật, bao gồm việc sử dụng shell, hệ thống file hệ thống, cơ chế quyền truy cập và các công cụ hệ thống.


4. macOS thuộc loại hệ điều hành nào? 
  - macOS thuộc loại hệ điều hành dựa trên Unix (*nix)

5. So sánh giữa Alpine và Ubuntu:

  - Alpine và Ubuntu là hai bản phân phối Linux phổ biến được sử dụng cho các mục đích khác nhau.

    - Kích thước và cấu trúc:
      - Alpine: Alpine Linux rất nhỏ gọn và nhẹ, với kích thước cài đặt cơ bản chỉ khoảng vài chục MB. Điều này làm cho Alpine thích hợp cho việc triển khai các ứng dụng container hoặc các hệ thống nhúng yêu cầu tài nguyên ít.
      - Ubuntu: Ubuntu có kích thước cài đặt lớn hơn, thường từ vài trăm MB đến vài GB, phụ thuộc vào phiên bản cụ thể và các gói phần mềm được cài đặt. Ubuntu thích hợp cho nhiều mục đích sử dụng, từ máy chủ đến máy tính cá nhân.

    - Hệ thống quản lý gói:
      - Alpine: Alpine sử dụng apk, một hệ thống quản lý gói nhẹ và nhanh chóng, cho phép người dùng cài đặt, cập nhật và gỡ bỏ các gói phần mềm dễ dàng.
      - Ubuntu: Ubuntu sử dụng apt (Advanced Packaging Tool) hoặc apt-get, cung cấp một hệ thống quản lý gói mạnh mẽ và phổ biến, cho phép quản lý gói phần mềm một cách linh hoạt và hiệu quả.

    - Tiêu chuẩn hóa và hỗ trợ:
      - Alpine: Alpine thường được sử dụng trong các môi trường container do kích thước nhỏ và tính nhẹ. Nó thường được ưa chuộng trong các môi trường microservices và DevOps.
      - Ubuntu: Ubuntu thường được sử dụng cho các mục đích đa dạng, từ máy chủ đến máy tính cá nhân và máy trạm. Nó cung cấp sự ổn định, hỗ trợ lâu dài và một cộng đồng lớn với nhiều tài liệu và hỗ trợ sẵn có.

    - Bảo mật:
      - Alpine: Alpine được biết đến với hệ thống bảo mật mạnh mẽ và phần nhỏ gọn của nó. Do đó, nó thường được sử dụng trong các môi trường yêu cầu bảo mật cao như container.
      - Ubuntu: Ubuntu cũng có một hệ thống bảo mật đáng tin cậy và nhận được sự hỗ trợ từ một cộng đồng lớn trong việc cung cấp các bản cập nhật và vá lỗi bảo mật.

6. VNC là gì?
  - VNC, viết tắt của "Virtual Network Computing", là một hệ thống được sử dụng để chia sẻ màn hình giữa các thiết bị khác nhau với mục đích điều khiển từ xa. Điều này cho phép người dùng từ xa có thể xem và điều khiển màn hình, bàn phím và chuột của một máy tính khác như thể họ đang ngồi trước máy tính đó.

  - VNC hoạt động dựa trên mô hình client/server. Máy tính cần được cài đặt thành một máy chủ VNC, trong khi máy tính khác muốn điều khiển từ xa cần cài đặt một trình xem VNC, hoặc còn gọi là client. Khi hai thành phần này được kết nối, máy chủ VNC sẽ chuyển gửi hình ảnh màn hình từ xa đến trình xem VNC.

  - Ngoài việc xem màn hình từ xa, VNC cũng cho phép người dùng điều khiển máy tính từ xa bằng cách sử dụng bàn phím và chuột của thiết bị điều khiển. Điều này mang lại khả năng kiểm soát đầy đủ các hoạt động trên máy tính từ xa sau khi được cấp phép từ máy tính đó.

  - VNC được phát triển tại Cambridge vào cuối những năm 1990 bởi những người sáng lập của RealVNC và đã trở thành một công nghệ phổ biến trong việc truy cập và điều khiển máy tính từ xa.

**Bài tập tự thực hành:**

https://github.com/HitoBoy/BaiTapTetKTPM/assets/100589413/4f808b8d-44a6-4ec3-a5ac-d7b5cd6cb335

  - Chạy máy ảo bằng VMWare với hệ điều hành là Ubuntu.
  - Khi đó DE của máy là GNOME
  - Cài LightDM qua Terminal và restart lại máy ảo
  - Cài X11VNC qua Terminal rồi config user password của x11vnc.service để lúc sau đăng nhập.
  - Sau khi cài đặt thành công xong, em sử dụng lệnh start để chạy x11vnc.service và dùng lệnh status để lấy port cho ip address lúc sau
  - Tại terminal em dùng lệnh ip addr để lấy luôn địa chỉ ip address cho máy ảo
  - Tạo 1 tệp rỗng rồi tạo Dockerfile với file index.html cho web
  - Ở Dockerfile em đã sử dụng 2 lệnh là FROM và COPY
  - Lệnh FROM ở đây dùng để... vì khi tạo image mới thì image nào cũng cần xuất phát từ một image khác
  - Lệnh COPY ở đây dùng để...
  - Còn file index.html chứa hello world đơn giản
  
  - Để khởi chạy docker image em đã sử dụng lệnh docker build để xây dựng image rồi dùng lệnh run để khởi chạy.
  - Tại máy tính gốc thì em có tải TightVNC để sử dụng VNC Viewer để remote lên máy ảo.
  - Khởi động VNC Viewer lên, điền ip address và số port vào ô remote host để connect tới máy ảo.
  - Phía máy ảo yêu cầu máy chính nhập mật khẩu là mật khẩu đã thay đổi lúc config x11vnc.service
  - Nhập đúng mật khẩu thì màn hình ứng dụng sẽ tạo ra màn hình mới là màn hình đang sử dụng của máy ảo
  - Như trong ảnh thì có thể thấy 2 con trỏ chuột ở màn hình vnc viewer và màn hình máy ảo

