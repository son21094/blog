---
title: "Giới thiệu về Hệ thống phân tán"
---

# Hệ thống phân tán là gì?

Hệ thống phân tán là tập hợp các máy tính độc lập phối hợp với nhau để người dùng cảm nhận như một hệ thống duy nhất. Các thành phần của hệ thống thường nằm ở nhiều địa điểm vật lý khác nhau và giao tiếp thông qua mạng máy tính.

# Các ứng dụng của hệ thống phân tán

Hệ thống phân tán được sử dụng rộng rãi trong nhiều lĩnh vực:
- Dịch vụ web như Google, Facebook, Amazon.
- Hệ thống thanh toán điện tử.
- Dữ liệu lớn (Big Data) như Hadoop.
- Điện toán đám mây (cloud computing).
- Các ứng dụng IoT và hệ thống cảm biến phân tán.
- Trò chơi trực tuyến đa người chơi.

# Các khái niệm chính của hệ thống phân tán

## Các thuật ngữ:

- **Scalability (Khả năng mở rộng):** Khả năng hệ thống tiếp tục hoạt động hiệu quả khi quy mô tăng (người dùng, dữ liệu, xử lý...).
- **Fault Tolerance (Chịu lỗi):** Khả năng tiếp tục hoạt động dù có một hoặc vài thành phần gặp lỗi.
- **Availability (Khả dụng):** Mức độ sẵn sàng phục vụ của hệ thống.
- **Transparency (Tính trong suốt):** Người dùng không thấy sự phức tạp của hệ thống phân tán (ví dụ: không biết có bao nhiêu máy chủ xử lý).
- **Concurrency (Tính đồng thời):** Cho phép nhiều người dùng tương tác cùng lúc.
- **Parallelism (Tính song song):** Chia nhỏ công việc để xử lý đồng thời nhằm tăng tốc độ.
- **Openness (Tính mở):** Hệ thống có thể tích hợp các thành phần khác nhau (ngôn ngữ, nền tảng...).
- **Vertical Scaling (Mở rộng theo chiều dọc):** Nâng cấp phần cứng (RAM, CPU) của một máy chủ đơn lẻ.
- **Horizontal Scaling (Mở rộng theo chiều ngang):** Thêm nhiều máy chủ để chia tải.
- **Load Balancer (Cân bằng tải):** Phân phối yêu cầu giữa nhiều máy chủ để tránh quá tải.
- **Replication (Nhân bản):** Sao chép dữ liệu sang nhiều máy để tăng độ tin cậy.

## Ví dụ:

Một hệ thống đặt vé máy bay trực tuyến sử dụng:
- **Horizontal Scaling**: Thêm nhiều máy chủ web để xử lý người dùng đồng thời.
- **Load Balancer**: Chuyển người dùng đến máy chủ ít tải nhất.
- **Replication**: Sao lưu dữ liệu chuyến bay và đặt chỗ trên nhiều máy.
- **Fault Tolerance**: Nếu một máy chủ web bị lỗi, các máy còn lại tiếp tục phục vụ.
- **Transparency**: Người dùng không biết mình đang tương tác với nhiều máy khác nhau.
- **Scalability**: Khi nhu cầu tăng, hệ thống có thể mở rộng dễ dàng.

# Kiến trúc của hệ thống phân tán

## Một số mô hình kiến trúc phổ biến:
- **Client-Server:** Máy khách gửi yêu cầu, máy chủ xử lý.
- **3-tier architecture:** Phân lớp rõ ràng: giao diện - logic - dữ liệu.
- **Microservices:** Hệ thống chia thành nhiều dịch vụ nhỏ, độc lập, có thể triển khai riêng biệt.
- **Event-driven architecture:** Các thành phần giao tiếp bằng sự kiện (Event Queue).
- **Peer-to-peer (P2P):** Các nút trong mạng vừa là client vừa là server.
- **Service-Oriented Architecture (SOA):** Các dịch vụ được đóng gói và giao tiếp qua giao thức chung (SOAP, REST).

## Ví dụ:

Hệ thống Netflix sử dụng kiến trúc **microservices**:
- Mỗi dịch vụ xử lý một chức năng như đăng nhập, danh sách phim, thanh toán...
- Dùng **load balancer** để phân tải.
- Mỗi microservice có thể **replicate** để chịu lỗi và đảm bảo **availability**.
- Sử dụng **event-driven architecture** để xử lý các hành vi người dùng như play/pause, chọn phim...

---

