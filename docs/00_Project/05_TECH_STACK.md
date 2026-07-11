# Technology Stack

**Document ID:** PRJ-006

**Version:** 1.0.0

**Status:** Active

---

# 1. Purpose

Tài liệu này định nghĩa bộ công nghệ (Technology Stack) được sử dụng trong CreatorOS.

Mục tiêu của tài liệu không phải là lựa chọn công nghệ "tốt nhất", mà là lựa chọn công nghệ phù hợp với từng giai đoạn phát triển của dự án.

CreatorOS được phát triển theo chiến lược:

> **Free First, Scale Later**

Điều này có nghĩa là:

- Giai đoạn đầu ưu tiên công nghệ miễn phí hoặc Free Tier.
- Khi hệ thống có doanh thu sẽ nâng cấp dần.
- Việc nâng cấp không được yêu cầu viết lại kiến trúc.

---

# 2. Technology Principles

Mọi công nghệ được lựa chọn phải đáp ứng các tiêu chí sau:

- Miễn phí hoặc có Free Tier.
- Có cộng đồng lớn.
- Được duy trì lâu dài.
- Có tài liệu đầy đủ.
- Dễ học.
- Dễ bảo trì.
- Dễ thay thế.
- Phù hợp với AI Code Generation.
- Có lộ trình mở rộng.

Không lựa chọn công nghệ chỉ vì xu hướng.

---

# 3. Development Phases

CreatorOS được chia thành ba giai đoạn phát triển.

## Phase 1 - MVP

Mục tiêu:

- Hoàn toàn miễn phí hoặc chi phí rất thấp.
- Có thể phát triển bởi một người.
- Có thể triển khai nhanh.
- Tạo ra sản phẩm đầu tiên.

---

## Phase 2 - Growth

Sau khi có người dùng hoặc doanh thu.

Có thể bổ sung:

- Redis
- Queue
- Docker
- Monitoring
- Logging
- Background Jobs

---

## Phase 3 - Scale

Khi CreatorOS trở thành nền tảng SaaS.

Có thể bổ sung:

- Kubernetes
- Load Balancer
- CDN
- Object Storage
- Message Queue
- Microservices
- Distributed Cache

---

# 4. Current Technology Stack (MVP)

## Frontend

| Category         | Technology    |
| ---------------- | ------------- |
| Language         | TypeScript    |
| Framework        | React         |
| Build Tool       | Vite          |
| Router           | React Router  |
| State Management | Redux Toolkit |
| HTTP Client      | Axios         |
| Styling          | CSS Modules   |

---

## Backend

| Category  | Technology           |
| --------- | -------------------- |
| Language  | TypeScript           |
| Runtime   | Node.js              |
| Framework | Express.js (Current) |
| API       | REST API             |

Lưu ý:

Framework Backend có thể thay đổi trong tương lai mà không ảnh hưởng đến kiến trúc tổng thể.

---

## Database

| Category            | Technology |
| ------------------- | ---------- |
| Relational Database | PostgreSQL |

Trong giai đoạn đầu có thể sử dụng:

- PostgreSQL Local
- Supabase Free

Không khóa chặt vào một nhà cung cấp dịch vụ.

---

## Authentication

- JWT

---

## Storage

Giai đoạn hiện tại:

- Cloudinary Free

Trong tương lai:

- AWS S3
- Cloudflare R2
- MinIO

---

## Deployment

Frontend:

- Vercel Free

Backend:

- Render Free

Database:

- Supabase Free hoặc PostgreSQL Local

---

# 5. AI Technology

CreatorOS không phụ thuộc vào một AI Provider.

AI chỉ là một thành phần có thể thay thế.

Các Provider có thể sử dụng:

- OpenAI
- Google Gemini
- Anthropic Claude
- DeepSeek
- Groq
- OpenRouter
- Local LLM

Workflow không được phụ thuộc vào bất kỳ AI nào.

---

# 6. Development Tools

Các công cụ phục vụ phát triển:

| Category        | Tool               |
| --------------- | ------------------ |
| IDE             | Visual Studio Code |
| Version Control | Git                |
| Repository      | GitHub             |
| API Testing     | Postman            |
| Documentation   | Markdown           |
| Diagram         | Mermaid            |

---

# 7. Future Technologies

Các công nghệ dưới đây không nằm trong phạm vi MVP nhưng kiến trúc phải hỗ trợ tích hợp trong tương lai.

Ví dụ:

- Redis
- Docker
- Kubernetes
- RabbitMQ
- Kafka
- Elasticsearch
- Qdrant
- pgvector
- S3
- Cloudflare R2
- Electron
- React Native

---

# 8. Technology Upgrade Strategy

Việc nâng cấp công nghệ phải đảm bảo:

- Không thay đổi Requirement.
- Không thay đổi Workflow.
- Không thay đổi Business Logic.
- Không yêu cầu viết lại toàn bộ hệ thống.

Ví dụ:

```text
Cloudinary Free
        ↓
AWS S3
```

```text
Render Free
        ↓
AWS EC2
```

```text
Supabase Free
        ↓
PostgreSQL Cluster
```

```text
Gemini Free
        ↓
OpenAI
```

Việc nâng cấp chỉ nên thay đổi lớp Infrastructure.

---

# 9. Technology Review

Việc thay đổi Tech Stack phải trả lời được các câu hỏi sau:

- Công nghệ mới giải quyết vấn đề gì?
- Có phù hợp với kiến trúc hiện tại không?
- Có làm tăng chi phí không?
- Có ảnh hưởng đến Workflow không?
- Có cần thay đổi Database không?
- Có cần thay đổi AI Layer không?

Nếu câu trả lời không rõ ràng thì không nên thay đổi.

---

# Related Documents

- README.md
- PRJ-001 Project Bootstrap
- PRJ-002 Project Vision
- PRJ-003 Project Principles
- PRJ-005 Folder Structure
- ARC-001 System Overview

---

# End of Document
