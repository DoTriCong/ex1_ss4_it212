# BÀI 1: Phân tích & Lựa chọn (Thực hành thiết kế prompt tối ưu hóa mã nguồn)

**Đáp án lựa chọn:** **B**

---

## Phân tích chi tiết phương án B
Phương án B là tối ưu nhất vì nó áp dụng đầy đủ **5 thành phần cốt lõi của Prompt**:

- **Role (Vai trò):** "Hãy đóng vai trò là một Java Senior Developer" → xác định rõ AI phải hành xử như một lập trình viên giàu kinh nghiệm, có khả năng refactor chuẩn Clean Code.  
- **Goal (Mục tiêu):** "Nhiệm vụ của bạn là tái cấu trúc logic rẽ nhánh lồng nhau phức tạp của class DiscountService" → mục tiêu cụ thể, rõ ràng.  
- **Context (Ngữ cảnh):** "Dự án sử dụng Java 11" → cung cấp bối cảnh công nghệ chính xác để AI sinh code phù hợp.  
- **Constraint (Ràng buộc):** "Giữ nguyên logic nghiệp vụ tính chiết khấu ban đầu, không thay đổi kiểu dữ liệu đầu vào/đầu ra, sử dụng guard clauses" → ràng buộc nghiệp vụ và kỹ thuật chi tiết.  
- **Format (Định dạng):** "Trình bày kết quả dưới dạng khối mã nguồn Java hoàn chỉnh kèm giải thích ngắn bằng tiếng Việt" → định dạng đầu ra rõ ràng, dễ đọc và dễ hiểu.  

Nhờ có đủ 5 thành phần, AI sẽ sinh ra mã nguồn chuẩn xác ngay từ lần đầu, hạn chế việc phải chỉnh sửa thủ công.

---

## Tại sao phương án A chưa đạt chuẩn
- **Role:** Không xác định rõ vai trò AI.  
- **Goal:** Mục tiêu mơ hồ ("tái cấu trúc code cho đẹp hơn").  
- **Context:** Không nêu rõ phiên bản Java.  
- **Constraint:** Không yêu cầu cụ thể về guard clauses, dễ dẫn đến refactor sai hướng.  
- **Format:** Không yêu cầu định dạng cụ thể, dễ dẫn đến code thiếu chú thích hoặc không chuẩn Clean Code.  

→ Hệ quả: AI có thể sinh code sơ sài, thiếu chi tiết, cần chỉnh sửa nhiều.

---

## Tại sao phương án C chưa đạt chuẩn
- **Role:** Không xác định vai trò AI.  
- **Goal:** Chỉ yêu cầu bỏ bớt if-else, nhưng lại ép dùng Stream API → không phù hợp với nghiệp vụ tính toán chiết khấu.  
- **Context:** Không nêu rõ môi trường công nghệ.  
- **Constraint:** Không đảm bảo giữ nguyên logic nghiệp vụ, nguy cơ thay đổi cách tính.  
- **Format:** Chỉ yêu cầu code ngắn gọn, không có chú thích giải thích.  

→ Hệ quả: AI có thể sinh code ngắn nhưng khó đọc, khó bảo trì, và có thể sai logic nghiệp vụ.

---

## Kết luận
Phương án B là lựa chọn đúng đắn nhất vì nó **áp dụng đầy đủ 5 thành phần Prompt (Role, Goal, Context, Constraint, Format)**, đảm bảo AI sinh mã nguồn refactor chuẩn Clean Code, giữ nguyên logic nghiệp vụ và dễ hiểu ngay từ lần đầu.
