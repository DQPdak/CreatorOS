# CreatorOS - Project Principles

> Version: 1.0.0
> Status: Draft
> Sprint: 0 - Foundation
> Document Type: Project Principles
> Last Updated: 2026-07-10

---

# 1. Mục đích

Tài liệu này định nghĩa toàn bộ nguyên tắc phát triển CreatorOS.

Đây là tài liệu bắt buộc đối với:

- Người phát triển
- AI
- Thành viên mới của dự án

Nếu có bất kỳ xung đột nào giữa một quyết định kỹ thuật và tài liệu này thì tài liệu này được ưu tiên.

---

# 2. Triết lý dự án

CreatorOS không phải là một project học tập.

CreatorOS là một sản phẩm thực tế.

Mọi quyết định đều phải hướng tới việc:

- Có thể sử dụng mỗi ngày.
- Có thể bảo trì nhiều năm.
- Có thể mở rộng.
- Có thể thương mại hóa.

---

# 3. Nguyên tắc số 1

## Documentation is the Source of Truth

Code không phải nguồn sự thật.

AI không phải nguồn sự thật.

Trí nhớ của người phát triển cũng không phải nguồn sự thật.

Tài liệu mới là nguồn sự thật.

Mọi thay đổi đều phải bắt đầu từ tài liệu.

Sau đó mới đến code.

---

# 4. Human First

AI chỉ là trợ lý.

Người phát triển là người chịu trách nhiệm cuối cùng.

Không có AI nào được phép:

- tự quyết định
- tự merge
- tự publish
- tự thay đổi kiến trúc

---

# 5. Architecture Before Coding

Không được viết code nếu chưa có:

Requirement

Flow

Entity

API

Review

---

# 6. Workflow Before AI

Workflow là tài sản quan trọng nhất.

AI chỉ là công cụ.

Nếu thay AI mà Workflow bị hỏng thì kiến trúc đã sai.

---

# 7. Modular Design

Mỗi module chỉ giải quyết một nhóm vấn đề.

Không được tạo module đa chức năng.

Ví dụ:

Không nên có

AIService

thực hiện:

- Research
- Story
- Voice
- SEO

Mỗi chức năng phải là module độc lập.

---

# 8. Single Responsibility

Một class.

Một service.

Một controller.

Một component.

Chỉ nên có một trách nhiệm chính.

---

# 9. Small Increment

Không phát triển 20 module cùng lúc.

Mỗi Sprint chỉ tập trung hoàn thành một số module nhỏ.

Module hoàn thành phải:

- có tài liệu
- có test
- có README
- có changelog

---

# 10. Human Approval

Workflow tiêu chuẩn luôn có bước xác nhận.

Ví dụ

Research

↓

Approve

↓

Outline

↓

Approve

↓

Script

↓

Approve

↓

Publish

Không được bỏ qua.

---

# 11. AI Collaboration

Không sử dụng một AI làm mọi việc.

Mỗi AI có một vai trò.

Ví dụ:

Research Agent

↓

Research Reviewer

↓

Story Writer

↓

Story Reviewer

↓

SEO Reviewer

↓

Human

Toàn bộ quá trình phản biện diễn ra nội bộ.

Người dùng chỉ xem kết quả cuối cùng.

---

# 12. AI Provider Independence

Không phụ thuộc vào:

ChatGPT

Gemini

Claude

DeepSeek

Nếu một Provider ngừng hoạt động thì chỉ cần thay Provider.

Không thay Workflow.

Không thay Business Logic.

---

# 13. Review First

Không Merge ngay sau khi AI sinh code.

Quy trình chuẩn:

AI

↓

Self Check

↓

Documentation Update

↓

Developer Review

↓

Merge

---

# 14. Documentation Standard

Mọi module đều phải có tài liệu.

Ví dụ

Requirement

Flow

Entity

API

README

CHANGELOG

Không có ngoại lệ.

---

# 15. Ticket Driven Development

AI không được code theo yêu cầu miệng.

Mọi công việc đều phải có Ticket.

Một Ticket gồm:

- Mục tiêu
- Phạm vi
- Tài liệu tham khảo
- Tiêu chí hoàn thành
- Tiêu chí kiểm thử

---

# 16. No Scope Creep

Không thêm tính năng vì "hay".

Trước khi thêm tính năng phải trả lời:

- Giải quyết vấn đề gì?
- Có đúng Vision không?
- Có đúng Scope không?
- Có cần ở Sprint hiện tại không?

Nếu không trả lời được thì không phát triển.

---

# 17. Data First

Mọi quyết định tối ưu đều dựa trên dữ liệu.

Không dựa trên cảm tính.

Ví dụ:

Không nói

"Tôi nghĩ video này hay."

Mà phải có dữ liệu:

- CTR
- Retention
- View
- RPM
- Engagement

---

# 18. Version Everything

Mọi thứ đều có Version.

Bao gồm:

- Prompt
- Workflow
- Agent
- Requirement
- API
- Database
- Module

Không ghi đè.

Luôn có lịch sử.

---

# 19. AI Must Update Documentation

Sau khi hoàn thành một Ticket AI bắt buộc:

- cập nhật README
- cập nhật CHANGELOG
- cập nhật MODULE_REGISTRY
- cập nhật tài liệu liên quan

Không chỉ sinh code.

---

# 20. Long-Term Thinking

CreatorOS được thiết kế cho vòng đời nhiều năm.

Không ưu tiên giải pháp nhanh nếu làm giảm:

- chất lượng
- khả năng mở rộng
- khả năng bảo trì

---

# 21. Quy trình phát triển chuẩn

Requirement

↓

Review

↓

Architecture

↓

Review

↓

Database

↓

Review

↓

Workflow

↓

Review

↓

API

↓

Review

↓

UI

↓

Review

↓

Ticket

↓

AI Development

↓

Testing

↓

Developer Review

↓

Merge

---

# 22. Quy trình làm việc với AI

Mọi AI trước khi thực hiện công việc phải:

1. Đọc PROJECT_BOOTSTRAP

2. Đọc PROJECT_VISION

3. Đọc PROJECT_PRINCIPLES

4. Đọc tài liệu Module liên quan

5. Đọc Ticket

Sau đó mới được bắt đầu.

---

# 23. Definition of Done

Một module chỉ được xem là hoàn thành khi:

✓ Requirement hoàn chỉnh

✓ Flow hoàn chỉnh

✓ Entity hoàn chỉnh

✓ API hoàn chỉnh

✓ Code hoàn chỉnh

✓ Test đạt

✓ README đầy đủ

✓ CHANGELOG cập nhật

✓ MODULE_REGISTRY cập nhật

✓ Được Developer Review

---

# End of Document
