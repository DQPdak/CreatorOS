# CreatorOS

> **AI Workflow Operating System for Content Creators**

CreatorOS là một nền tảng giúp xây dựng, quản lý và tự động hóa toàn bộ quy trình sản xuất nội dung số bằng AI.

Mục tiêu của dự án không phải là tạo ra một AI duy nhất, mà là xây dựng một **AI Workflow Operating System**, nơi nhiều AI Agent chuyên trách phối hợp với nhau thông qua các Workflow chuẩn hóa để hỗ trợ người sáng tạo nội dung.

---

# Project Status

Current Phase

```
Documentation & System Design
```

Hiện tại toàn bộ dự án đang tập trung vào việc thiết kế hệ thống.

Chúng tôi tuân thủ nguyên tắc:

> **Documentation First • Architecture First • Code Last**

Toàn bộ tài liệu sẽ được hoàn thiện trước khi bắt đầu phát triển mã nguồn.

---

# Vision

CreatorOS hướng tới việc trở thành một nền tảng có thể hỗ trợ:

- YouTube
- TikTok
- Facebook
- Instagram
- Podcast
- Blog
- Newsletter

đồng thời có khả năng mở rộng thành nền tảng SaaS dành cho nhiều người dùng trong tương lai.

---

# Repository Structure

```
CreatorOS/

├── backend/
├── frontend/
├── docs/
├── scripts/
└── tools/
```

| Folder   | Description                |
| -------- | -------------------------- |
| backend  | Backend source code        |
| frontend | Frontend source code       |
| docs     | Project documentation      |
| scripts  | Automation scripts         |
| tools    | Internal development tools |

---

# Documentation

Toàn bộ tài liệu của dự án được lưu trong thư mục:

```
docs/
```

Cấu trúc:

```
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

---

# Reading Order

Để hiểu dự án, hãy đọc tài liệu theo đúng thứ tự:

```
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

Việc đọc đúng thứ tự sẽ giúp hiểu được toàn bộ hệ thống mà không bỏ sót ngữ cảnh.

---

# Development Workflow

CreatorOS được phát triển theo quy trình sau:

```
Requirement

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

Code luôn là bước cuối cùng.

---

# Core Principles

CreatorOS được xây dựng dựa trên các nguyên tắc sau:

- Documentation First
- Architecture Before Coding
- Human In The Loop
- AI Provider Independent
- Modular Design
- Data Driven Decision
- Single Source of Truth

Chi tiết được định nghĩa trong:

```
docs/00_Project/
```

---

# Repository Rules

Mọi thành viên và AI tham gia dự án đều phải tuân thủ các quy tắc sau:

- Không viết code khi chưa có tài liệu.
- Không thay đổi kiến trúc nếu chưa được phê duyệt.
- Không để một AI đảm nhiệm nhiều vai trò nếu có thể tách thành nhiều Agent chuyên trách.
- Mọi chức năng đều phải có Specification trước khi triển khai.
- Mọi thay đổi phải có khả năng truy vết.
- Con người luôn là người đưa ra quyết định cuối cùng.

---

# Commit Convention

Các commit được thực hiện theo từng Package thay vì từng file.

Ví dụ:

```
docs(project): complete project foundation

docs(product): complete product definition

docs(architecture): complete system architecture

feat(workflow): implement workflow engine

fix(api): resolve authentication bug
```

---

# Technology Stack

Tech Stack chi tiết được định nghĩa tại:

```
docs/00_Project/05_TECH_STACK.md
```

---

# Roadmap

```
Phase 0
Project Foundation

↓

Phase 1
Product Definition

↓

Phase 2
Architecture Design

↓

Phase 3
Database Design

↓

Phase 4
API Specification

↓

Phase 5
Workflow Design

↓

Phase 6
AI Design

↓

Phase 7
UI/UX Design

↓

Phase 8
Module Specification

↓

Phase 9
Implementation

↓

Phase 10
Testing

↓

Phase 11
Deployment
```

---

# License

License sẽ được bổ sung khi dự án bước sang giai đoạn phát hành chính thức.

---

# Philosophy

CreatorOS không được xây dựng xoay quanh một AI cụ thể.

Mọi AI chỉ là **Provider** có thể thay thế.

Workflow mới là trung tâm của hệ thống.

Điều này giúp dự án có thể hoạt động lâu dài ngay cả khi một AI Provider không còn khả dụng trong tương lai.

---

**CreatorOS**

> _Design First. Documentation First. Code Last._
