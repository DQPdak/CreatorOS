# CreatorOS - Project Principles

**Document ID:** DOC-PRINCIPLES-001
**Version:** 1.0.0
**Status:** Active

---

# 1. Purpose

Tài liệu này định nghĩa các nguyên tắc bắt buộc trong quá trình phát triển CreatorOS.

Mọi thành viên và mọi AI tham gia dự án đều phải tuân thủ các nguyên tắc này.

Nếu có xung đột giữa một quyết định và tài liệu này thì phải ưu tiên tài liệu này cho đến khi Product Owner phê duyệt thay đổi.

---

# 2. Core Philosophy

CreatorOS được xây dựng như một sản phẩm thực tế.

Mục tiêu không phải là hoàn thành nhanh nhất.

Mục tiêu là tạo ra một hệ thống:

- Chất lượng cao.
- Có thể bảo trì nhiều năm.
- Có thể mở rộng.
- Có thể thương mại hóa.

---

# 3. Documentation First

Mọi thay đổi đều bắt đầu từ tài liệu.

Không được:

- Viết code trước rồi mới bổ sung tài liệu.
- Thay đổi chức năng mà không cập nhật tài liệu.
- Bỏ qua bước thiết kế.

Mỗi tài liệu là một phần của "Single Source of Truth".

---

# 4. Architecture Before Coding

Không được viết mã nguồn khi chưa hoàn thành:

- Requirement.
- Architecture.
- Database Design.
- Workflow Design.
- API Design (nếu có).

Code chỉ là bước hiện thực hóa thiết kế.

---

# 5. Human in the Loop

Con người luôn giữ quyền quyết định cuối cùng.

Các bước quan trọng như:

- Chốt Requirement.
- Chốt Workflow.
- Chốt Script.
- Xuất bản nội dung.

đều phải có sự phê duyệt của người dùng.

---

# 6. AI as Specialized Agents

CreatorOS không sử dụng một AI làm mọi việc.

Mỗi AI chỉ đảm nhận một nhiệm vụ rõ ràng.

Ví dụ:

- Research Agent.
- Script Writer.
- Script Reviewer.
- SEO Agent.
- Analytics Agent.

Việc chia nhỏ giúp:

- Dễ thay thế AI.
- Dễ đánh giá chất lượng.
- Dễ mở rộng hệ thống.

---

# 7. AI Provider Independence

Không phụ thuộc vào một nhà cung cấp AI.

Ví dụ:

- OpenAI
- Google
- Anthropic
- DeepSeek
- Các Local Model

Thay đổi Provider không được làm thay đổi Business Logic.

---

# 8. Modular Design

Hệ thống được chia thành các module độc lập.

Mỗi module:

- Có mục đích rõ ràng.
- Có tài liệu riêng.
- Có thể phát triển độc lập.
- Có thể kiểm thử độc lập.

Không tạo các module đa chức năng.

---

# 9. Single Responsibility

Một thành phần chỉ nên có một trách nhiệm chính.

Áp dụng cho:

- Module.
- Service.
- Controller.
- Component.
- AI Agent.

---

# 10. Incremental Development

Dự án được phát triển theo Sprint.

Mỗi Sprint phải tạo ra Deliverable hoàn chỉnh.

Không phát triển nhiều tính năng lớn cùng lúc.

---

# 11. Review Before Merge

Mọi thay đổi phải trải qua các bước:

1. Thiết kế.
2. Thực hiện.
3. Tự kiểm tra.
4. Kiểm tra bởi người phát triển.
5. Merge.

Không merge trực tiếp.

---

# 12. Data Driven Decision

Các quyết định tối ưu nội dung phải dựa trên dữ liệu.

Ví dụ:

- CTR.
- Watch Time.
- Audience Retention.
- RPM.
- Engagement.
- Conversion.

Không tối ưu chỉ dựa trên cảm nhận.

---

# 13. Version Everything

Mọi thành phần đều phải có phiên bản.

Bao gồm:

- Prompt.
- Workflow.
- Module.
- API.
- Database.
- Documentation.

Điều này giúp dễ theo dõi lịch sử thay đổi.

---

# 14. Ticket Driven Development

Mọi công việc đều phải có Ticket.

Một Ticket tối thiểu cần có:

- Mục tiêu.
- Phạm vi.
- Tiêu chí hoàn thành.
- Tài liệu tham khảo.

Không làm việc dựa trên mô tả miệng.

---

# 15. Documentation Maintenance

Sau mỗi thay đổi, phải cập nhật:

- README (nếu cần).
- Tài liệu liên quan.
- CHANGELOG.
- MODULE_REGISTRY (khi áp dụng).

Tài liệu luôn phải phản ánh đúng trạng thái hiện tại của hệ thống.

---

# 16. Security by Design

Các vấn đề về bảo mật phải được xem xét ngay từ giai đoạn thiết kế.

Không coi bảo mật là bước xử lý sau cùng.

---

# 17. Scalability by Design

Mọi quyết định kiến trúc phải cân nhắc khả năng mở rộng.

Không tối ưu cho một kênh duy nhất nếu điều đó làm hạn chế khả năng phát triển sau này.

---

# 18. Definition of Done

Một Deliverable chỉ được xem là hoàn thành khi:

- Requirement rõ ràng.
- Thiết kế hoàn chỉnh.
- Được Product Owner chấp thuận.
- Tài liệu đầy đủ.
- Code (nếu có) hoạt động đúng.
- Kiểm thử đạt yêu cầu.

---

# 19. Project Decision Authority

Quyền quyết định được phân chia như sau:

**Product Owner**

- Định hướng sản phẩm.
- Quyết định tính năng.
- Phê duyệt cuối cùng.

**Technical Lead**

- Kiến trúc hệ thống.
- Tiêu chuẩn kỹ thuật.
- Kế hoạch triển khai.

**AI Agents**

- Thực hiện nhiệm vụ được giao.
- Đề xuất giải pháp.
- Không tự ý thay đổi định hướng dự án.

---

# 20. Guiding Principle

Nếu có nhiều giải pháp, hãy ưu tiên giải pháp:

1. Dễ hiểu.
2. Dễ bảo trì.
3. Dễ mở rộng.
4. Dễ kiểm thử.
5. Ít phụ thuộc.
6. Có tài liệu rõ ràng.

Đây là tiêu chí mặc định cho mọi quyết định kỹ thuật trong CreatorOS.

---

# End of Document
