# 💌 Website Thư Tình & Hệ Thống Quà Tặng 20/10/2026

Website chúc mừng ngày Phụ nữ Việt Nam 20/10/2026 dành riêng cho người yêu, được thiết kế theo phong cách **Love Letter, Romantic, Soft Pink & Minimalist**.

Tất cả đã được tối ưu hóa gói gọn trong **CHỈ 1 FILE HTML DUY NHẤT** (`index.html`), không cần cài đặt Node.js hay backend phức tạp, có thể mở trực tiếp bằng trình duyệt trên máy tính/điện thoại hoặc deploy miễn phí lên GitHub Pages chỉ trong vài giây!

---

## ✨ Điểm nổi bật & Tính năng đã hoàn thiện

1. **Hiệu ứng phong bì rơi & mở thư 3D chân thực**:
   - Khi vào trang, phong bì từ trên cao rơi xuống trung tâm màn hình với gia tốc trọng trường và độ nảy (gravity & bounce).
   - Khi chạm vào phong bì: Con dấu sáp trái tim bung nở, nắp phong bì mở 180° bằng CSS 3D transform, lá thư trượt ra ngoài và phóng to mượt mà sang bố cục đọc thư.
   - Có âm thanh mở giấy sột soạt nhẹ nhàng (được tổng hợp trực tiếp bằng Web Audio API, không lo phụ thuộc file ngoài).

2. **Nội dung thư tình chuẩn xác từng câu chữ**:
   - Dòng tiêu đề `20102026` thanh lịch.
   - Giữ nguyên vẹn 100% nội dung thư của bạn.
   - Chữ ký `Thương em nhiều.` và `Anh.` theo font chữ viết tay nghệ thuật.

3. **Bộ đếm thời gian yêu nhau từ 27/06/2026**:
   - Ngày mốc cố định: **27.06.2026**.
   - Hiển thị dòng: *“Từ ngày 27.06.2026, chúng mình đã bên nhau được… ♡”*
   - Tự động tính toán chuẩn xác theo thời gian thực (năm, tháng, ngày và tổng số ngày).

4. **Âm nhạc Lofi / Piano lãng mạn (Web Audio API)**:
   - Tích hợp bộ phát nhạc giao hưởng ballad / Canon in D ấm áp sinh ra từ Web Audio API.
   - Mặc định tắt âm thanh, nút bật/tắt đĩa than xoay ở góc trên bên phải.

5. **Hệ thống nhận quà & Theo dõi lộ trình ("App giao hàng cao cấp")**:
   - Nút *“Nhận món quà của anh ♡”* với hộp thoại xác nhận.
   - Tạo mã đơn duy nhất (ví dụ: `DH-2010-8386`) và lưu vào `localStorage`.
   - **Bản đồ Leaflet & OpenStreetMap**:
     - **Điểm xuất phát (A)**: `18 Nguyễn Ngọc Nhựt, Phú Thọ Hòa, Hồ Chí Minh, Vietnam`
     - **Điểm đến (B - Nhà em)**: `490B/48C đường Bá Trạc, Chánh Hưng, Hồ Chí Minh, Vietnam`
     - Vẽ chính xác lộ trình xe chạy (12.5 km) với 279 tọa độ GPS chuẩn xác từ OSRM.
   - **Thanh tiến trình 3 giai đoạn**:
     - `1. 🎁 Đã nhận quà`: *“Anh biết em đã nhận quà rồi nè ♡ - Chờ anh chuẩn bị một chút nhé…”*
     - `2. 🚚 Đang giao quà`: *“Quà của em đang trên đường đến rồi! ♡…”* (với animation xe giao hàng di chuyển trên thanh tiến trình).
     - `3. 🏠 Quà đã đến nơi`: Toàn màn hình chúc mừng **“TING TONG! ♡ Quà của em đang ở dưới nhà rồi nè! Em ra nhận quà nhé, anh chờ em đó.”** kèm hộp quà mở ra và pháo hoa trái tim rực rỡ!

6. **Cơ chế cập nhật trạng thái nhanh (Admin Controls)**:
   - **Qua đường dẫn (URL)**:
     - `index.html?admin=oce` hoặc `index.html#oce` -> Tự động chuyển đơn sang **Đang giao quà**.
     - `index.html?admin=done` hoặc `index.html#done` -> Tự động chuyển đơn sang **Quà đã đến nơi (TING TONG)**.
   - **Qua giao diện bí mật**:
     - Bấm vào biểu tượng ổ khóa nhỏ `🔒` ở góc dưới cùng bên phải.
     - Nhập mã PIN: `20102026` (hoặc `love`).
     - Bảng điều khiển sẽ hiện ra cho phép bạn: chuyển đổi trạng thái bằng 1 click, nhập Discord Webhook URL, gửi tin nhắn test, hoặc reset đơn để thử lại từ đầu!
   - **Đồng bộ thời gian thực**: Sử dụng cơ chế lắng nghe sự kiện `storage` giữa các tab, khi bạn cập nhật trạng thái thì tab của bạn gái sẽ tự động đổi ngay mà không cần reload.

7. **Tích hợp Discord Webhook**:
   - Gửi thông báo đến Discord kèm mention tài khoản `<@463969672967094272>`.
   - Cấu hình an toàn trong bảng quản trị hoặc biến cục bộ.

---

## 🚀 Cách chạy thử nghiệm trên máy (Local)

### Cách 1: Mở trực tiếp file HTML
Bạn chỉ cần click đúp vào file `index.html` trong thư mục [love-letter-20-10/index.html](file:///C:/Users/hoangkiet/.gemini/antigravity-ide/scratch/love-letter-20-10/index.html) để mở trên bất kỳ trình duyệt nào (Chrome, Edge, Firefox, Cốc Cốc, Safari).

### Cách 2: Chạy server local (Khuyên dùng)
Mở terminal tại thư mục này và chạy lệnh:
```bash
python -m http.server 5173
```
Sau đó truy cập trình duyệt:
- Xem trang người yêu: `http://localhost:5173/`
- Cập nhật đang giao quà: `http://localhost:5173/?admin=oce`
- Cập nhật quà đã đến nơi: `http://localhost:5173/?admin=done`

---

## 🌐 Hướng dẫn Deploy miễn phí lên GitHub Pages

Vì toàn bộ ứng dụng chỉ gói gọn trong **1 file `index.html`**, việc deploy lên GitHub Pages cực kỳ đơn giản và miễn phí 100%:

1. Tạo một repository mới trên GitHub (ví dụ: `love-letter-20-10`).
2. Tải file `index.html` lên thư mục gốc của repository (root).
3. Vào mục **Settings** của repository -> chọn thẻ **Pages** ở thanh menu bên trái.
4. Tại mục **Build and deployment** -> **Branch**: Chọn nhánh `main` (hoặc `master`) và thư mục `/(root)`, sau đó nhấn **Save**.
5. Sau 1-2 phút, GitHub sẽ cung cấp cho bạn một đường link HTTPS công khai (ví dụ: `https://your-username.github.io/love-letter-20-10/`).
6. Bạn có thể gửi link này cho bạn gái bất cứ lúc nào!
