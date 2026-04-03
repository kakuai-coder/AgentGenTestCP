# 🚀 AICodeGen 2.0 - Trợ lý Tự động hóa Lập trình Thi đấu (Competitive Programming)

**AICodeGen 2.0** là công cụ GUI mạnh mẽ trên Windows, giúp tự động hóa toàn bộ quy trình: từ phân tích đề bài (ảnh/chữ) bằng AI, sinh mã nguồn lời giải, tạo bộ test case địa phương, cho đến việc tự động đăng bài lên Online Judge (OJ).

---

## ✨ Tính năng nổi bật (Version 2.0)

### 🤖 1. Phân tích & Sinh Test bằng AI (Sinh Test Tab)
- **Hỗ trợ Ảnh & Clipboard**: Chỉ cần chụp ảnh đề bài (Win+Shift+S) và nhấn `Ctrl+V` để nạp vào phần mềm.
- **AI Đỉnh cao **: Tự động phân tích logic, giới hạn bài toán và sinh code giải chuẩn xác.
- **Tự động sinh Test Data**: Tạo bộ dữ liệu đầu vào `.in` và đầu ra `.out` phong phú, bao gồm cả các trường hợp biên (edge cases).
- **Cơ chế Retry thông minh**: Tự động thử lại khi gặp lỗi giới hạn API (Quota 429), giúp quá trình sinh không bị gián đoạn.

### 🌐 2. Tự động hóa Upload OJ (OJ & Đăng Bài Tab)
- **Kết nối Trực tiếp ptcoding.edu.vn (Hoặc các DMOJ khác)**: Tự động Đăng nhập -> Tạo bài mới -> Upload ZIP -> Ghép cặp (Apply). Hiện tại chỉ hoạt động tốt nhất với ptcoding.
- **Phát hiện Ghi đè**: Tự động kiểm tra nếu bài đã tồn tại và hỏi ý kiến người dùng trước khi cập nhật.
- **Tối ưu hóa Giao diện OJ**: 
  - Nếu AI sinh ra mô tả văn bản, chương trình tự động xóa tệp đề bài cũ (ảnh/PDF) để tránh trùng lặp.
  - Tự động điền Giới hạn thời gian (Time Limit) và bộ nhớ (Memory Limit).
- **Theo dõi Tiến độ**: Log chi tiết từng bước (Login, Uploading, Polling, Applying).

### 🛠 3. Các cải tiến Kỹ thuật Quan trọng
- **Sửa lỗi ZIP Bloat**: Khắc phục triệt để lỗi nén đệ quy (từng gây ra file 2GB). File ZIP giờ đây chỉ nặng vài chục KB.
- **Hỗ trợ Zip64**: Tương thích với các bộ test case lớn (dung lượng thực tế >4GB).
- **Giao diện Hiện đại**: Sử dụng `customtkinter` mang lại trải nghiệm mượt mà, chuyên nghiệp.

---

## 🚀 Hướng dẫn Sử dụng (Quick Start)

### Cài đặt ban đầu
1. Đi tới mục [**Releases**](https://github.com/) của kho lưu trữ này và tải xuống tệp `AICodeGen_Release.zip` mới nhất.
2. Giải nén thư mục, click đúp vào file `AICodeGen.exe` để khởi chạy ứng dụng.
3. Trong lần đầu sử dụng, phần mềm sẽ yêu cầu nhập **Gemini API Key** (Sẽ được lưu an toàn tại `~/.ai_cp_config.json`).
   - Truy cập trang chủ [Google AI Studio](https://aistudio.google.com/app/apikey) để tạo API Key của bạn (Hoàn toàn miễn phí 100%).
   - Sao chép dòng mã bí mật đó và dán vào ứng dụng, AICodeGen sẽ cất chìa khóa an toàn vào ổ cứng để các lần sau không cần nhờ bạn nữa.
5. Gõ mã bài thi, chụp ảnh đề đưa vào, và uống nước để thư giãn!
---

## 📂 Cấu trúc Thư mục Kết quả
Khi thực hiện sinh bài, kết quả được lưu tại:
- `solutions/<mã_bài>/`: Chứa code giải `solution.cpp` và bộ test.
- `solutions/<mã_bài>/<mã_bài>.zip`: File nén để nộp thủ công (nếu cần).

---

## ⚠️ Lưu ý
- Đảm bảo tài khoản OJ có quyền tạo/chỉnh sửa bài toán.
- Kiểm tra lại định dạng file `Time/Memory Limit` cho đúng với yêu cầu của từng trang OJ cụ thể.
  
## 💖 Ủng Hộ (Donate)
Toàn bộ dự án này được viết ra để phục vụ cho sự nghiệp giáo dục, giúp các giáo viên bộ môn và các bạn học sinh chuyên bớt đi gánh nặng của hàng chục giờ sinh test đầy gian khổ. Nếu tiện ích nhỏ bé này đã cất đi gánh nặng lớn của bạn, mong bạn hãy mời tôi một tách trà nhẹ nhàng nhé! ☕

- **Ngân Hàng / Ví Điện Tử:** 
  - Ngân hàng: `(MB Bank)` - Số TK: `(0357794112)` - Chủ TK: `(Ngo Viet Tinh)`

*Những đóng góp chân tình sẽ đảm bảo rằng ứng dụng này không những sống hiên ngang mà còn liên tục được trang bị các tính năng vô giá ở những phiên bản trong tương lai. Cảm ơn bạn!* 😊

---
<div align="center">
  <i>Được làm bằng 💻 và ❤️.</i>
</div>
