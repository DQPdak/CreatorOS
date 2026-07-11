# Project Glossary

**Document ID:** PRJ-007

**Version:** 1.0.0

**Status:** Active

---

# 1. Purpose

Tài liệu này định nghĩa các thuật ngữ được sử dụng xuyên suốt trong dự án CreatorOS.

Mục tiêu:

- Thống nhất cách hiểu giữa Developer và AI.
- Tránh sử dụng nhiều thuật ngữ cho cùng một khái niệm.
- Làm tài liệu tham chiếu cho toàn bộ dự án.

Nếu một thuật ngữ xuất hiện trong tài liệu khác, ý nghĩa của nó phải tuân theo tài liệu này.

---

# 2. General Terms

## CreatorOS

Hệ điều hành hỗ trợ người sáng tạo nội dung bằng AI Workflow.

CreatorOS không phải là một AI, mà là một nền tảng điều phối nhiều AI để thực hiện các quy trình làm việc.

---

## User

Người sử dụng hệ thống.

Một User có thể sở hữu hoặc tham gia nhiều Workspace.

---

## Workspace

Không gian làm việc độc lập.

Mỗi Workspace có:

- Thành viên
- Channel
- Workflow
- AI Configuration
- Dashboard
- Dữ liệu riêng

---

## Member

Người tham gia một Workspace.

Mỗi Member có một hoặc nhiều Role.

---

## Role

Tập hợp các quyền của một Member trong Workspace.

Ví dụ:

- Owner
- Admin
- Editor
- Viewer

---

# 3. Content Terms

## Channel

Một kênh nội dung trên một nền tảng.

Ví dụ:

- YouTube Channel
- TikTok Account
- Facebook Page
- Instagram Account

Một Workspace có thể quản lý nhiều Channel.

---

## Platform

Nền tảng xuất bản nội dung.

Ví dụ:

- YouTube
- TikTok
- Facebook
- Instagram
- Podcast
- Blog

---

## Content

Đơn vị nội dung được tạo ra bởi hệ thống.

Ví dụ:

- Video
- Short Video
- Podcast
- Blog
- Newsletter

---

## Asset

Tài nguyên phục vụ tạo nội dung.

Ví dụ:

- Image
- Audio
- Video
- Subtitle
- Thumbnail
- Prompt
- Script

---

# 4. Workflow Terms

## Workflow

Chuỗi các bước để hoàn thành một quy trình.

Workflow là trung tâm của CreatorOS.

---

## Stage

Một giai đoạn trong Workflow.

Ví dụ:

- Research
- Script Writing
- Review
- Voice Generation
- Video Rendering
- Publishing

---

## Task

Một công việc cụ thể trong một Stage.

Task có thể được thực hiện bởi AI hoặc con người.

---

## Review

Quá trình kiểm tra kết quả của một Task.

Review có thể do AI hoặc con người thực hiện.

---

## Approval

Bước xác nhận cuối cùng trước khi chuyển sang Stage tiếp theo.

Người dùng luôn có quyền Approval cuối cùng.

---

# 5. AI Terms

## AI Provider

Đơn vị cung cấp mô hình AI.

Ví dụ:

- OpenAI
- Google
- Anthropic
- DeepSeek

---

## AI Model

Mô hình AI cụ thể.

Ví dụ:

- GPT
- Gemini
- Claude

---

## AI Agent

Một thành phần trong hệ thống sử dụng AI để thực hiện một nhiệm vụ cụ thể.

Ví dụ:

- Research Agent
- Script Agent
- SEO Agent

AI Agent không hoạt động độc lập mà phải nằm trong Workflow.

---

## Prompt

Dữ liệu đầu vào gửi cho AI Model.

Prompt được quản lý như một tài nguyên của hệ thống.

---

## Response

Kết quả do AI trả về sau khi xử lý Prompt.

---

# 6. Analytics Terms

## Dashboard

Giao diện tổng hợp dữ liệu và trạng thái hệ thống.

---

## Analytics

Quá trình thu thập và phân tích dữ liệu.

---

## Insight

Thông tin hoặc đề xuất được rút ra từ dữ liệu.

Insight hỗ trợ người dùng ra quyết định nhưng không tự động thay thế quyết định của người dùng.

---

## KPI

Chỉ số đánh giá hiệu quả.

Ví dụ:

- Views
- Watch Time
- Revenue
- CTR

---

# 7. Development Terms

## Module

Một nhóm chức năng độc lập của hệ thống.

Mỗi Module có tài liệu và mã nguồn riêng.

---

## Service

Một thành phần cung cấp chức năng cho Module hoặc hệ thống.

---

## API

Giao diện giao tiếp giữa các thành phần của hệ thống.

---

## Documentation

Nguồn thông tin chính thức mô tả hệ thống.

Documentation luôn được ưu tiên hơn mã nguồn khi xác định Requirement hoặc Design.

---

# 8. Future Terms

Các thuật ngữ mới chỉ được bổ sung khi:

- Được sử dụng trong ít nhất một Module.
- Có ý nghĩa rõ ràng.
- Không trùng với thuật ngữ hiện có.

Nếu thay đổi định nghĩa của một thuật ngữ, phải cập nhật tất cả tài liệu liên quan.

---

# Related Documents

- README.md
- PRJ-001 Project Bootstrap
- PRJ-002 Project Vision
- PRJ-003 Project Principles
- PRJ-004 Documentation Standard
- PRJ-005 Folder Structure
- PRJ-006 Technology Stack

---

# End of Document
