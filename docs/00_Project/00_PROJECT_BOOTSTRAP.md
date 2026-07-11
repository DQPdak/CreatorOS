# Project Bootstrap

**Document ID:** PRJ-001

**Version:** 1.0.0

**Status:** Active

---

# 1. Purpose

Tài liệu này định nghĩa nền tảng của dự án CreatorOS.

Đây là tài liệu đầu tiên mà mọi thành viên và AI phải đọc trước khi tham gia phát triển dự án.

Tài liệu này trả lời các câu hỏi:

- CreatorOS là dự án gì?
- Dự án được phát triển theo định hướng nào?
- Quy trình phát triển ra sao?
- Quy tắc làm việc là gì?
- Tài liệu được tổ chức như thế nào?

Tài liệu này không mô tả chi tiết sản phẩm, kiến trúc hay cơ sở dữ liệu.

---

# 2. Project Information

| Field             | Value                                 |
| ----------------- | ------------------------------------- |
| Project Name      | CreatorOS                             |
| Project Type      | AI Workflow Operating System          |
| Development Model | Documentation First                   |
| Repository Type   | Monorepo                              |
| Primary Language  | English (Documentation & Source Code) |
| Current Phase     | Documentation & System Design         |

---

# 3. Project Mission

CreatorOS được xây dựng nhằm chuẩn hóa và tự động hóa quy trình sản xuất nội dung số bằng AI.

Thay vì phụ thuộc vào một AI duy nhất, hệ thống sử dụng nhiều AI Agent chuyên trách được điều phối thông qua Workflow nhằm tạo ra quy trình làm việc ổn định, dễ mở rộng và có khả năng thay thế AI Provider khi cần.

---

# 4. Development Philosophy

CreatorOS tuân theo triết lý:

> **Design First. Documentation First. Code Last.**

Mọi quyết định kỹ thuật đều phải được mô tả bằng tài liệu trước khi được triển khai thành mã nguồn.

Code chỉ là kết quả của quá trình thiết kế.

---

# 5. Project Objectives

Các mục tiêu chính của dự án:

- Chuẩn hóa quy trình sản xuất nội dung.
- Hỗ trợ nhiều nền tảng nội dung.
- Điều phối nhiều AI Agent.
- Giảm thao tác thủ công.
- Quản lý nhiều Workspace và nhiều Channel.
- Hỗ trợ phân tích dữ liệu và ra quyết định.
- Có khả năng mở rộng thành nền tảng SaaS.

---

# 6. Development Workflow

CreatorOS được phát triển theo quy trình sau:

```text
Project

↓

Product

↓

Architecture

↓

Database

↓

API

↓

Workflow

↓

AI

↓

UI

↓

Module Specification

↓

Implementation

↓

Testing

↓

Deployment
```

Không được bỏ qua bất kỳ giai đoạn nào.

---

# 7. Documentation Policy

Toàn bộ dự án được điều khiển bằng tài liệu.

Mọi thay đổi đều phải bắt đầu từ tài liệu.

Các tài liệu là nguồn thông tin chính thức (Single Source of Truth).

Nếu có sự khác biệt giữa Code và Documentation thì Documentation được ưu tiên xem xét trước để xác định đâu là hành vi mong muốn của hệ thống.

---

# 8. Human In The Loop

AI chỉ đóng vai trò hỗ trợ.

Con người luôn là người:

- Phê duyệt yêu cầu.
- Phê duyệt thiết kế.
- Phê duyệt kiến trúc.
- Phê duyệt mã nguồn.
- Phê duyệt phát hành.

Không có bước nào được phép tự động bỏ qua sự kiểm tra của con người.

---

# 9. AI Strategy

CreatorOS không phụ thuộc vào bất kỳ AI Provider nào.

Mọi AI được xem là một Provider có thể thay thế.

Ví dụ:

- OpenAI
- Google Gemini
- Anthropic Claude
- DeepSeek
- Local LLM

Việc thay đổi AI Provider không được làm thay đổi kiến trúc của hệ thống.

---

# 10. Repository Strategy

Repository được tổ chức theo mô hình Monorepo.

Các thành phần chính:

- Backend
- Frontend
- Documentation
- Scripts
- Tools

Mỗi thành phần có trách nhiệm riêng và được phát triển độc lập nhưng tuân theo cùng một bộ tài liệu.

---

# 11. Project Lifecycle

Một chức năng mới phải trải qua các giai đoạn sau:

```text
Requirement

↓

Analysis

↓

Architecture

↓

Database

↓

API

↓

Workflow

↓

Module Specification

↓

Implementation

↓

Testing

↓

Review

↓

Release
```

Không được triển khai trực tiếp từ ý tưởng sang mã nguồn.

---

# 12. Success Criteria

CreatorOS được xem là thành công khi:

- Có thể quản lý nhiều dự án nội dung.
- Có thể quản lý nhiều Channel.
- Có thể thay thế AI Provider.
- Có Workflow rõ ràng.
- Có kiến trúc dễ mở rộng.
- Có tài liệu đầy đủ.
- Có khả năng thương mại hóa.

---

# 13. Related Documents

- README.md
- PRJ-002 Project Vision
- PRJ-003 Project Principles
- PRJ-004 Documentation Standard
- PRD-001 Product Requirements

---

# End of Document
