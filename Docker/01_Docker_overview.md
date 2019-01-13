## Docker

Docker ra đời 2013. Nó được kỹ sư trẻ Solomon Hykes người Pháp lập trình bằng Golang, một ngôn ngữ được Google giới thiệu năm 2009.

Docker nhanh chóng được cộng đồng CNTT đón nhận với tốc độ chóng mặt. Docker là phương thức, công cụ, hạ tầng để hiện thực hoá xây dựng Microservice, triển khai ứng dụng lên điện toán đám mây nhanh, gọn, tự động, chính xác. Docker có nhiều ưu điểm so với công nghệ ảo hoá, Virtualization:

* Tiết kiệm tài nguyên hệ thống: dung lượng ổ cứng, bộ nhớ, CPU time

* Khởi động nhanh và tắt cũng nhanh hơn rất nhiều

* Lập trình thành script tự động được

* Kết nối thành cụm cluster (Docker Swarm, Kubernetes)

* Dễ dàng quản lý (manage), quan sát (monitor)

<img src="/img/1.jpg">


* Docker Engine: Dùng để tạo ra Docker image và chạy Docker container.

* Docker Hub: Dịch vụ lưu trữ giúp chứa các Docker image.

* Docker Machine: Tạo ra các Docker engine trên máy chủ.

* Docker Compose: Chạy ứng dụng bằng cách định nghĩa cấu hình các Docker container thông qua tệp cấu hình

* Docker image: Một dạng tập hợp các tệp của ứng dụng, được tạo ra bởi Docker engine. Nội dung của các Docker image sẽ không bị thay đổi khi di chuyển. Docker image được dùng để chạy các Docker container.

* Docker container: Một dạng runtime của các Docker image, dùng để làm môi trường chạy ứng dụng.