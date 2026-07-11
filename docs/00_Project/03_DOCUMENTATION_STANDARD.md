# Documentation Standard

**Document ID:** PRJ-004

**Version:** 1.0.0

**Status:** Active

---

# 1. Purpose

Tài liệu này định nghĩa tiêu chuẩn viết tài liệu của toàn bộ dự án CreatorOS.

Mục tiêu:

- Thống nhất cách tổ chức tài liệu.
- Giúp tài liệu dễ đọc và dễ bảo trì.
- Giúp AI và Developer dễ tìm kiếm thông tin.
- Đảm bảo mọi tài liệu có cấu trúc nhất quán.

Mọi tài liệu trong dự án phải tuân thủ tiêu chuẩn này.

---

# 2. Scope

Tiêu chuẩn này áp dụng cho:

- Project Documents
- Product Documents
- Architecture Documents
- Database Documents
- API Documents
- Workflow Documents
- AI Documents
- UI Documents
- Deployment Documents
- Testing Documents
- Development Documents
- Module Documents

Không áp dụng cho mã nguồn (Source Code).

---

# 3. Documentation Hierarchy

Tài liệu của CreatorOS được tổ chức theo cấu trúc sau:

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

Mỗi nhóm tài liệu chỉ chịu trách nhiệm cho đúng phạm vi của mình.

---

# 4. Document Metadata

Mọi tài liệu đều phải bắt đầu bằng phần Metadata.

Cấu trúc chuẩn:

```text
Document ID:
Version:
Status:
```

Ví dụ:

```text
Document ID: ARC-001

Version: 1.0.0

Status: Active
```

---

# 5. Document Template

Mọi tài liệu sử dụng cùng một Template.

```md
# Document Title

**Document ID:** XXX-001

**Version:** 1.0.0

**Status:** Active

---

# 1. Purpose

...

---

# 2. Main Content

...

---

# Related Documents

...

---

# End of Document
```

Template này được sử dụng cho toàn bộ tài liệu trong dự án.

---

# 6. Document ID Convention

Quy tắc đặt Document ID:

| Category     | Prefix |
| ------------ | ------ |
| Project      | PRJ    |
| Product      | PRD    |
| Architecture | ARC    |
| Database     | DB     |
| API          | API    |
| Workflow     | WF     |
| AI           | AI     |
| UI           | UI     |
| Deployment   | DEP    |
| Testing      | TEST   |
| Development  | DEV    |
| Module       | MOD    |

Ví dụ:

```text
PRJ-001

PRD-001

ARC-002

DB-003

API-001

MOD-015
```

---

# 7. Version Convention

Tài liệu sử dụng Semantic Versioning.

| Version | Meaning          |
| ------- | ---------------- |
| Major   | Thay đổi lớn     |
| Minor   | Bổ sung nội dung |
| Patch   | Sửa lỗi nhỏ      |

Ví dụ:

```text
1.0.0

1.0.1

1.1.0

2.0.0
```

---

# 8. Document Status

Mỗi tài liệu phải có một trạng thái.

| Status     | Meaning                   |
| ---------- | ------------------------- |
| Draft      | Đang soạn                 |
| Review     | Đang được xem xét         |
| Active     | Đang sử dụng              |
| Deprecated | Không khuyến nghị sử dụng |
| Archived   | Đã lưu trữ                |

---

# 9. File Naming Convention

Quy tắc đặt tên file:

- Viết bằng tiếng Anh.
- Không dùng khoảng trắng.
- Sử dụng dấu gạch dưới (\_).
- Tên file viết HOA.
- Đánh số theo thứ tự.

Ví dụ:

```text
00_PROJECT_BOOTSTRAP.md

01_PROJECT_VISION.md

02_SYSTEM_OVERVIEW.md

05_DATABASE_DESIGN.md
```

---

# 10. Writing Guidelines

Khi viết tài liệu cần tuân thủ các nguyên tắc sau:

- Mỗi tài liệu chỉ giải quyết một chủ đề.
- Không sao chép nội dung từ tài liệu khác.
- Ưu tiên nội dung rõ ràng và chính xác.
- Không sử dụng văn phong hội thoại.
- Không đưa ý kiến cá nhân vào tài liệu.
- Giải thích thuật ngữ khi cần thiết.
- Sử dụng danh sách và bảng khi phù hợp.

---

# 11. Cross References

Nếu tài liệu liên quan đến tài liệu khác, sử dụng phần:

```text
Related Documents
```

Ví dụ:

```text
PRJ-001 Project Bootstrap

PRJ-003 Project Principles

ARC-001 System Overview
```

Không sao chép nội dung giữa các tài liệu.

---

# 12. AI Compatibility

Mọi tài liệu phải đảm bảo:

- Có cấu trúc ổn định.
- Có Heading rõ ràng.
- Có khả năng đọc độc lập.
- Không phụ thuộc lịch sử cuộc trò chuyện.
- Có thể được AI phân tích và sử dụng làm ngữ cảnh.

Mục tiêu là bất kỳ AI nào cũng có thể hiểu tài liệu chỉ bằng cách đọc chính tài liệu đó.

---

# 13. Documentation Lifecycle

Một tài liệu sẽ trải qua các giai đoạn sau:

```text
Draft

↓

Review

↓

Active

↓

Deprecated (nếu có)

↓

Archived (nếu có)
```

---

# 14. Documentation Review Checklist

Trước khi chuyển sang trạng thái **Active**, tài liệu phải đạt các tiêu chí sau:

- Nội dung đúng mục đích.
- Không trùng lặp với tài liệu khác.
- Đúng Template chuẩn.
- Có Document ID.
- Có Version.
- Có Status.
- Có Related Documents (nếu cần).
- Không có lỗi chính tả.
- AI có thể đọc và hiểu mà không cần ngữ cảnh bổ sung.

---

# Related Documents

- README.md
- PRJ-001 Project Bootstrap
- PRJ-002 Project Vision
- PRJ-003 Project Principles

---

# End of Document
