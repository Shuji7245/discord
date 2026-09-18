# 💬 Discord Clone Project

Một ứng dụng nhắn tin và giao tiếp thời gian thực mô phỏng các chức năng cốt lõi của Discord, bao gồm quản lý máy chủ (Servers), kênh trò chuyện (Channels), và đính kèm đa phương tiện.

## Công nghệ sử dụng

* **Frontend:** NextJS, ReactJS, Tailwind CSS
* **Backend Core & Real-time:** NodeJS (REST API & WebSocket)
* **Background Workers:** Python (Xử lý hàng đợi, render/nén video)
* **Database:** PostgreSQL (Lưu trữ user, server, message, metadata)
* **Cache & Message Broker:** Redis (Quản lý session, Pub/Sub cho real-time socket)
* **Object Storage:** MinIO (Lưu trữ vật lý hình ảnh, video và tệp đính kèm)

## Tính năng giai đoạn 1 (MVP)

* **Xác thực:** Đăng ký, đăng nhập và bảo mật phiên bằng JWT.
* **Quản lý Server (Guild):** Tạo server, tạo kênh (channel) và tạo mã mời (invite code).
* **Giao tiếp Real-time:** Nhắn tin tức thời trong các kênh thông qua socket.
* **Lưu trữ Media:** Upload, lưu trữ và stream video/ảnh từ bucket chuyên dụng.

## 🛠 Yêu cầu hệ thống

* Node.js (v18+)
* Python (v3.10+)
* Docker & Docker Compose (Dành cho database và storage nội bộ)
* Git

## Hướng dẫn cài đặt (Local Development)

**1. Clone kho lưu trữ**
```bash
git clone [https://github.com/Shuji7245/discord.git](https://github.com/Shuji7245/discord.git)
cd discord
