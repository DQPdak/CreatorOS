# CreatorOS - Project Bootstrap

**Version:** 1.0.0
**Status:** Active
**Sprint:** Sprint 0 - Foundation
**Commit:** #0001
**Owner:** Product Team

---

# Purpose

Đây là tài liệu đầu tiên và quan trọng nhất của dự án.

Mọi AI, lập trình viên hoặc cộng tác viên mới **bắt buộc** phải đọc tài liệu này trước khi thực hiện bất kỳ công việc nào.

Tài liệu này **không mô tả chi tiết chức năng**.

Nó giúp người đọc hiểu:

- CreatorOS là gì.
- Dự án đang hướng tới điều gì.
- Cách làm việc của dự án.
- Các tài liệu phải đọc tiếp theo.
- Vai trò của bản thân trong dự án.

---

# Project Overview

Tên dự án:

**CreatorOS**

CreatorOS là một **AI Workflow Operating System** dành cho Content Creator.

Đây không phải một AI.

Đây không phải một công cụ tạo video.

Đây là một hệ thống điều phối (Orchestration System) giúp quản lý toàn bộ quy trình sản xuất nội dung bằng nhiều AI khác nhau.

AI chỉ là một module trong hệ thống.

Workflow mới là trung tâm của hệ thống.

---

# Why This Project Exists

Dự án được tạo ra vì ba lý do chính.

## 1. Giải quyết bài toán thực tế

Người phát triển muốn xây dựng một hệ thống hỗ trợ phát triển các kênh nội dung (bắt đầu từ YouTube) nhằm tạo nguồn thu nhập bền vững.

---

## 2. Xây dựng một sản phẩm kỹ thuật chất lượng cao

CreatorOS không được xây dựng như một bài tập hay một project demo.

Đây là một sản phẩm thực tế, có khả năng sử dụng hằng ngày, bảo trì lâu dài và có thể trở thành Portfolio chính.

---

## 3. Chuẩn bị cho khả năng thương mại hóa

Kiến trúc của CreatorOS sẽ được thiết kế ngay từ đầu theo hướng mở rộng thành SaaS nhiều người dùng.

Việc thương mại hóa không phải mục tiêu hiện tại, nhưng kiến trúc phải luôn sẵn sàng.

---

# Development Philosophy

CreatorOS được phát triển theo các nguyên tắc sau:

- Documentation First.
- Human First.
- Architecture Before Coding.
- Workflow Before AI.
- Vendor Independent.
- Incremental Development.
- Long-term Maintainability.

Chi tiết được mô tả trong tài liệu `PROJECT_PRINCIPLES`.

---

# Project Development Strategy

CreatorOS sẽ không được phát triển theo kiểu:

Requirement → Code → Fix.

CreatorOS sẽ được phát triển theo quy trình:

Requirement

↓

Architecture

↓

Database

↓

Workflow

↓

API

↓

UI

↓

Ticket

↓

Code

↓

Testing

↓

Review

↓

Release

Mỗi bước đều phải có tài liệu trước khi chuyển sang bước tiếp theo.

---

# AI Collaboration Strategy

Trong dự án này, AI được xem là các thành viên của một nhóm phát triển phần mềm.

Không có AI nào được phép thực hiện toàn bộ công việc.

Một AI chỉ đảm nhiệm một vai trò.

Ví dụ:

- Research
- Requirement
- Architecture Review
- Backend Development
- Frontend Development
- Documentation
- Testing
- Code Review

Các AI có thể phản biện lẫn nhau.

Người phát triển chỉ xem kết quả cuối cùng.

---

# Human Responsibilities

Người phát triển giữ quyền quyết định cuối cùng.

Vai trò của người phát triển gồm:

- Product Owner
- Software Architect
- Technical Reviewer
- Decision Maker

AI không được tự ý thay đổi định hướng dự án.

---

# Current Phase

Hiện tại dự án đang ở:

**Sprint 0 - Foundation**

Mục tiêu của Sprint 0:

- Hoàn thiện toàn bộ tài liệu nền tảng.
- Chuẩn hóa quy trình phát triển.
- Thiết kế sản phẩm.
- Chưa viết code.

---

# Repository Structure

Trong giai đoạn hiện tại repository gồm ba thư mục chính.

```text
CreatorOS/

backend/
frontend/
docs/
```

Chi tiết sẽ được định nghĩa trong tài liệu `FOLDER_STRUCTURE`.

---

# Documents Reading Order

Mọi AI hoặc thành viên mới phải đọc tài liệu theo đúng thứ tự sau:

1. PROJECT_BOOTSTRAP
2. PROJECT_VISION
3. PROJECT_PRINCIPLES
4. PRODUCT_REQUIREMENTS
5. PRODUCT_SCOPE
6. MODULE_MAP
7. DOCUMENTATION_STANDARD
8. FOLDER_STRUCTURE
9. TECH_STACK
10. GLOSSARY

Không được bỏ qua thứ tự này.

---

# AI Working Rules

Trước khi thực hiện bất kỳ Ticket nào, AI phải:

1. Đọc PROJECT_BOOTSTRAP.
2. Đọc các tài liệu liên quan.
3. Đọc Ticket.
4. Xác định phạm vi công việc.
5. Chỉ thực hiện đúng phạm vi được giao.

Sau khi hoàn thành, AI phải:

- cập nhật tài liệu liên quan;
- cập nhật CHANGELOG;
- cập nhật MODULE_REGISTRY (nếu có thay đổi);
- sinh Commit Message;
- sinh Pull Request Description.

---

# Definition of Sprint 0 Success

Sprint 0 được xem là hoàn thành khi:

- Tất cả tài liệu nền tảng hoàn chỉnh.
- Kiến trúc tổng thể được thống nhất.
- Danh sách module được xác định.
- Quy trình phát triển được chuẩn hóa.
- Mọi AI mới có thể tham gia dự án chỉ bằng cách đọc tài liệu.

Lưu ý:

Sprint 0 không có mục tiêu viết code.

Nếu kết thúc Sprint 0 mà chưa có một dòng code nhưng toàn bộ thiết kế đã hoàn chỉnh thì Sprint 0 vẫn được xem là thành công.

---

# End of Document
