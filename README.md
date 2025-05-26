# ticket-backend
# Event Ticketing Backend

Đây là backend hệ thống quản lý vé sự kiện, gồm các microservices và các dịch vụ hỗ trợ như Kafka, Zookeeper, Redis.

---

## Yêu cầu

- Docker (phiên bản mới)
- Docker Compose (phiên bản 2+)

---

## Cấu trúc dịch vụ

- **Zookeeper:** dịch vụ quản lý cluster Kafka
- **Kafka:** message broker cho các service giao tiếp
- **Redis:** lưu trữ cache, session
- **AuthService:** dịch vụ xác thực người dùng
- **CheckinService:** dịch vụ check-in vé
- **TicketManagementService:** dịch vụ quản lý vé
- **ApiGateway:** cổng API tổng hợp các dịch vụ backend

---

## Cách chạy

1. Clone repo này về máy:

git clone https://github.com/tri-0412/ticket-backend.git
- cd event-ticketing-backend
- docker compose up -d
## Kiểm tra container đã chạy
docker ps
