# Project Principles

**Document ID:** PRJ-003

**Version:** 1.0.0

**Status:** Active

---

# 1. Purpose

Tài liệu này định nghĩa các nguyên tắc cốt lõi trong quá trình thiết kế, phát triển và bảo trì CreatorOS.

Mọi quyết định về kiến trúc, mã nguồn, cơ sở dữ liệu, giao diện và AI đều phải tuân thủ các nguyên tắc trong tài liệu này.

Nếu có nhiều phương án thiết kế khác nhau, phương án phù hợp với các nguyên tắc dưới đây sẽ luôn được ưu tiên.

---

# 2. Core Philosophy

CreatorOS được xây dựng dựa trên ba triết lý nền tảng:

- Design First
- Documentation First
- Code Last

Mọi dòng code đều phải xuất phát từ thiết kế.

---

# 3. Documentation First

Documentation là nguồn thông tin chính thức của toàn bộ dự án.

Quy trình bắt buộc:

```text
Requirement

↓

Documentation

↓

Review

↓

Implementation
```

Không được phép viết code trước tài liệu.

---

# 4. Architecture Before Coding

Kiến trúc luôn được thiết kế trước.

Không được thiết kế kiến trúc trong quá trình viết code.

Mọi thay đổi lớn phải được phản ánh trong tài liệu Architecture trước khi triển khai.

---

# 5. Human In The Loop

AI là công cụ hỗ trợ.

Con người luôn chịu trách nhiệm cuối cùng đối với:

- Requirement
- Architecture
- Database
- API
- Workflow
- Code Review
- Release

Không có quyết định quan trọng nào được thực hiện hoàn toàn tự động.

---

# 6. AI Provider Independent

CreatorOS không phụ thuộc vào bất kỳ AI Provider nào.

Hệ thống phải có khả năng thay thế:

- OpenAI
- Claude
- Gemini
- DeepSeek
- Local LLM

mà không làm thay đổi kiến trúc tổng thể.

---

# 7. Workflow First

Workflow là trung tâm của hệ thống.

AI không tự hoạt động.

Mọi AI Agent đều phải thực hiện nhiệm vụ thông qua Workflow đã được định nghĩa.

---

# 8. Modular Design

Hệ thống được chia thành các Module độc lập.

Mỗi Module:

- Có mục tiêu riêng.
- Có tài liệu riêng.
- Có API riêng.
- Có khả năng phát triển độc lập.
- Có thể kiểm thử độc lập.

Module chỉ giao tiếp với nhau thông qua các giao diện đã được định nghĩa.

---

# 9. Single Responsibility

Mỗi thành phần chỉ nên có một trách nhiệm chính.

Áp dụng cho:

- Module
- Service
- Controller
- Repository
- React Component
- AI Agent

Không để một thành phần đảm nhiệm nhiều vai trò khác nhau.

---

# 10. Separation of Concerns

Tách biệt rõ ràng giữa:

- Business Logic
- Presentation
- Data Access
- Infrastructure
- AI Logic

Không trộn nhiều tầng trong cùng một thành phần.

---

# 11. Single Source of Truth

Mỗi loại thông tin chỉ có một nguồn chính thức.

Ví dụ:

- Requirement → Product Documents
- Architecture → Architecture Documents
- Database → Database Documents
- API → API Documents
- Workflow → Workflow Documents

Không sao chép cùng một nội dung ở nhiều nơi.

---

# 12. Traceability

Mọi thành phần phải có khả năng truy vết.

Ví dụ:

Requirement

↓

Module

↓

Database

↓

API

↓

Code

↓

Test

↓

Release

Bất kỳ thay đổi nào cũng phải xác định được nguồn gốc.

---

# 13. Review Before Merge

Không được Merge khi chưa hoàn thành:

- Documentation Review
- Architecture Review
- Code Review
- Testing

Review là bước bắt buộc.

---

# 14. Consistency

Toàn bộ dự án phải thống nhất về:

- Cấu trúc thư mục.
- Quy tắc đặt tên.
- Coding Style.
- Documentation Style.
- Git Convention.

Không tạo ngoại lệ nếu không thực sự cần thiết.

---

# 15. Simplicity

Ưu tiên giải pháp:

- Đơn giản.
- Dễ đọc.
- Dễ bảo trì.
- Dễ mở rộng.

Không tối ưu hóa sớm.

Không sử dụng thiết kế phức tạp khi chưa cần.

---

# 16. Scalability

Mọi thiết kế phải xem xét khả năng mở rộng.

Bao gồm:

- Nhiều người dùng.
- Nhiều Workspace.
- Nhiều Channel.
- Nhiều AI Provider.
- Nhiều Workflow.
- Nhiều Module.

Không thiết kế chỉ cho nhu cầu hiện tại.

---

# 17. Security by Design

Bảo mật phải được xem xét ngay từ giai đoạn thiết kế.

Bao gồm:

- Authentication
- Authorization
- Input Validation
- Secret Management
- Audit Log

Không bổ sung bảo mật sau khi hệ thống hoàn thành.

---

# 18. Data Driven

Mọi quyết định tối ưu hệ thống nên dựa trên dữ liệu.

Hệ thống cần có khả năng:

- Thu thập dữ liệu.
- Phân tích dữ liệu.
- Đưa ra Insight.
- Hỗ trợ quyết định.

---

# 19. Continuous Improvement

CreatorOS là dự án phát triển lâu dài.

Tài liệu và mã nguồn được phép cải tiến liên tục nhưng phải đảm bảo:

- Không phá vỡ kiến trúc.
- Không phá vỡ tài liệu.
- Không làm mất khả năng truy vết.

---

# 20. Related Documents

- README.md
- PRJ-001 Project Bootstrap
- PRJ-002 Project Vision
- PRJ-004 Documentation Standard
- ARC-001 System Overview

---

# End of Document
