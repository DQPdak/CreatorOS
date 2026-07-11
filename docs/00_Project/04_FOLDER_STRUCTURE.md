# Folder Structure

**Document ID:** PRJ-005

**Version:** 1.0.0

**Status:** Active

---

# 1. Purpose

Tài liệu này định nghĩa cấu trúc thư mục chuẩn của dự án CreatorOS ở cấp độ Repository.

Mục tiêu:

- Thống nhất cách tổ chức dự án.
- Giúp dễ mở rộng.
- Giúp dễ bảo trì.
- Giúp AI và Developer nhanh chóng xác định vị trí tài liệu và mã nguồn.

Tài liệu này chỉ mô tả cấu trúc thư mục của Repository.

Cấu trúc chi tiết của Backend và Frontend sẽ được định nghĩa trong tài liệu Architecture.

---

# 2. Repository Structure

CreatorOS sử dụng mô hình **Monorepo**.

```text
CreatorOS/

├── backend/
├── frontend/
├── docs/
├── scripts/
├── tools/
│
├── .gitignore
├── README.md
└── LICENSE
```

---

# 3. Directory Description

## backend/

Chứa toàn bộ mã nguồn Backend của hệ thống.

Bao gồm:

- Business Logic
- API
- Database
- AI Integration
- Workflow Engine

---

## frontend/

Chứa toàn bộ mã nguồn Frontend.

Bao gồm:

- User Interface
- Dashboard
- Workflow Builder
- Analytics
- Administration

---

## docs/

Chứa toàn bộ tài liệu của dự án.

Đây là nguồn thông tin chính thức của CreatorOS.

Không lưu tài liệu kỹ thuật ở vị trí khác.

---

## scripts/

Chứa các Script phục vụ phát triển.

Ví dụ:

- Build Script
- Migration Script
- Generate Script
- Automation Script

---

## tools/

Chứa các công cụ nội bộ phục vụ phát triển.

Ví dụ:

- CLI
- Utilities
- AI Helper
- Internal Tool

---

# 4. Documentation Structure

Thư mục `docs/` được tổ chức như sau:

```text
docs/

00_Project/
01_Product/
02_Architecture/
03_Database/
04_API/
05_Workflows/
06_AI/
07_UI/
08_Deployment/
09_Testing/
10_Development/
11_Modules/
```

Ý nghĩa:

| Folder          | Description            |
| --------------- | ---------------------- |
| 00_Project      | Nền tảng dự án         |
| 01_Product      | Định nghĩa sản phẩm    |
| 02_Architecture | Kiến trúc hệ thống     |
| 03_Database     | Thiết kế cơ sở dữ liệu |
| 04_API          | Đặc tả API             |
| 05_Workflows    | Workflow nghiệp vụ     |
| 06_AI           | Thiết kế AI Agent      |
| 07_UI           | Thiết kế giao diện     |
| 08_Deployment   | Triển khai hệ thống    |
| 09_Testing      | Kiểm thử               |
| 10_Development  | Tiêu chuẩn phát triển  |
| 11_Modules      | Đặc tả từng Module     |

---

# 5. Documentation Reading Order

Tài liệu phải được đọc theo thứ tự:

```text
README

↓

00_Project

↓

01_Product

↓

02_Architecture

↓

03_Database

↓

04_API

↓

05_Workflows

↓

06_AI

↓

07_UI

↓

08_Deployment

↓

09_Testing

↓

10_Development

↓

11_Modules
```

Không nên bỏ qua các bước trước.

---

# 6. Source Code Organization

Backend và Frontend được phát triển độc lập.

Mỗi phần có:

- Kiến trúc riêng.
- Tiêu chuẩn riêng.
- Tài liệu riêng.

Hai phần chỉ giao tiếp thông qua API hoặc các giao thức đã được định nghĩa.

---

# 7. Documentation Ownership

Mỗi thư mục trong `docs/` chịu trách nhiệm cho một nhóm kiến thức riêng.

Không sao chép cùng một nội dung ở nhiều thư mục.

Ví dụ:

- Database chỉ mô tả Database.
- API chỉ mô tả API.
- Module chỉ mô tả Module.

Nếu cần tham chiếu, sử dụng phần **Related Documents**.

---

# 8. Future Expansion

Cấu trúc Repository phải hỗ trợ việc mở rộng trong tương lai.

Ví dụ:

- Mobile Application
- Desktop Application
- SDK
- Plugin
- Marketplace
- AI Models
- Infrastructure

Việc bổ sung các thành phần mới không được làm thay đổi cấu trúc hiện tại.

---

# 9. Repository Rules

Các quy tắc tổ chức Repository:

- Không lưu tài liệu ngoài thư mục `docs/`.
- Không lưu Script trong Backend hoặc Frontend.
- Không đặt nhiều mục đích khác nhau trong cùng một thư mục.
- Mỗi thư mục phải có trách nhiệm rõ ràng.
- Ưu tiên cấu trúc đơn giản và dễ tìm kiếm.

---

# Related Documents

- README.md
- PRJ-001 Project Bootstrap
- PRJ-003 Project Principles
- PRJ-004 Documentation Standard
- ARC-001 System Overview

---

# End of Document
