## Tổng quan về Docker Swarm

Docker Engine v1.12.0 và mới hơn cho phép lập trình viên triển khai container trong chế độ Swarm. Một Swarm cluster bao gồm Docker Engine được triển khai trên nhiều node. Node "Manager" thực hiện sắp xếp và quản lý cluster. Các node "Worker" nhận và thi hành nhiệm vụ từ node "manager". Mỗi service, có thể được khai báo, bao gồm nhiệm vụ có thể chạy trong Swarm node. Services có thể được sao chép để chạy trên nhiều node. Trong mô hình sao chép service, cân bằng tải nội bộ và DNS nội bộ có thể được sử dụng để cung cấp sẵn sàng các endpoint dịch vụ.

<img src="/img/4.png">

Kiến trúc Docker Swarm bao gồm các "manager" và các "worker". Người dùng có thể khai báo trạng thái mong muốn của nhiều service để chạy trong Swarm cluster sử dụng YAML files. Đây là vài thuật ngữ thông dụng liên quan đến Docker Swarm:

* Node: Một node là một thực thể của Swarm, các node có thể được phân phối tại chỗ hoặc trên cloud.

* Swarm: một cluster của các node. Trong chế độ Swarm, bạn sắp đặt các service, thay vì chạy các container bằng câu lệnh.

* Manager node: Là node nhận các định nghĩa service từ người dùng, và gửi công việc đến các node Worker. Node Manager có thể cũng thực hiện công việc của các node Worker.

* Worker node: là node nhận và chạy các nhiệm vụ từ node Manager.

* Service: Một service xác định images của container mà số lượng các bản lặp lại. Đây là một câu lệnh ví dụ sẽ được đặt trên 2 node có sẵn:

`docker service create --replicas 2 --name mynginx nginx`

* Task: một task là một nhiệm vụ của service trong một node worker.

## Kubernetes vs. Docker Swarm: Technical Capabilities


| <img src="/img/5.png"> | <img src="/img/6.png"> |
|------------------------|------------------------|
|Application Definition| |



