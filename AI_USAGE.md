# AI Usage Log

## 1. Công cụ AI
**ChatGPT (OpenAI).**

## 2. Mục đích sử dụng
- Phân tích giao diện và trải nghiệm người dùng trên website Hasaki.vn dựa trên ảnh khảo sát.
- Đề xuất phương án cải tiến thẻ sản phẩm trong trang danh mục.
- Hỗ trợ xây dựng mã HTML5/CSS3 và hướng dẫn kiểm tra giao diện responsive.

## 3. Prompt đã sử dụng

**Prompt 1 – Đề xuất phương án thiết kế:**

> Tôi đang thực hiện bài tập cải tiến giao diện website thương mại điện tử Hasaki.vn bằng HTML5 và CSS3. Qua khảo sát, các thẻ sản phẩm tại trang danh mục hiển thị nhiều thông tin khuyến mãi, khiến bố cục khá dày đặc và khó so sánh sản phẩm. Tôi muốn thiết kế lại thẻ sản phẩm để hiển thị rõ hình ảnh, tên, giá gốc, giá khuyến mãi, phần trăm giảm giá và nút thêm vào giỏ hàng. Đối tượng sử dụng là khách hàng mua sắm mỹ phẩm trực tuyến tại Việt Nam. Hãy đề xuất bố cục, thành phần HTML, cách tổ chức CSS, cách hiển thị trên máy tính và điện thoại, cùng các điểm cần kiểm tra khả năng sử dụng. Chỉ giải thích phương án, chưa viết toàn bộ mã nguồn.

**Prompt 2 – Hỗ trợ tạo mã nguồn (yêu cầu triển khai tiếp theo):**

> Dựa trên phương án cải tiến thẻ sản phẩm Hasaki.vn, hãy tạo trang mẫu bằng HTML5 và CSS3 với tối thiểu 4 sản phẩm, mỗi sản phẩm có hình, tên, giá khuyến mãi, giá gốc, mức giảm giá và nút thao tác. Tách HTML vào `index.html`, CSS vào `css/style.css`; sử dụng CSS Grid, Flexbox và Media Queries để hiển thị 4 cột trên máy tính, 2 cột trên điện thoại. Không sử dụng JavaScript, backend hoặc cơ sở dữ liệu. Giải thích cách chạy và các mục cần kiểm tra.

## 4. Kết quả AI đề xuất
- Đề xuất thẻ sản phẩm có cấu trúc từ trên xuống: hình ảnh, nhãn giảm giá, thương hiệu, tên, giá bán, giá gốc và nút thao tác.
- Sử dụng `section` cho khu vực danh sách, `article` cho từng thẻ, `img`, `h3`, `strong`, `del` và `button` cho thông tin sản phẩm.
- Dùng CSS Grid cho danh sách 4/2 cột, Flexbox để căn chỉnh nội dung và Media Queries để tối ưu màn hình nhỏ.
- Tạo bản demo 4 sản phẩm và ảnh SVG minh họa, không sao chép hình ảnh có bản quyền từ trang tham khảo.

## 5. Kiểm tra và điều chỉnh
- **Đã đối chiếu:** Nhận xét về mật độ thông tin khuyến mãi tại trang danh mục với ảnh Hasaki thực tế; lựa chọn giản lược thành một nhãn giảm giá trên thẻ.
- **Đã kiểm tra trong mã:** Đường dẫn `css/style.css`, các ảnh trong `images/`, đủ 4 thẻ sản phẩm và quy tắc responsive 4/2 cột.
- **Sinh viên cần tự kiểm tra trước khi nộp:** Mở `index.html` trong trình duyệt, thử màn hình máy tính và điện thoại, kiểm tra chữ dài, ảnh, giá, khoảng cách và nút thao tác.
- **Chi tiết tự điều chỉnh (điền sau khi thực hiện):** [Ghi rõ một thay đổi bản thân phát hiện và sửa, ví dụ chỉnh kích thước nút hoặc khoảng cách trên điện thoại; nêu file và thuộc tính CSS đã sửa].
- **Minh chứng (tùy chọn):** [Đường dẫn hoặc tên ảnh chụp giao diện trước/sau khi tự sửa].

## 6. Phần tôi hiểu và có thể giải thích
- `index.html` chứa nội dung và cấu trúc hiển thị của trang.
- `css/style.css` chứa màu sắc, bố cục, khoảng cách và định dạng responsive.
- `.product-grid` dùng `display: grid` để chia cột sản phẩm.
- `.product-card` và `.product-details` dùng Flexbox để các phần trong thẻ được sắp xếp theo chiều dọc.
- `@media` thay đổi bố cục khi chiều rộng màn hình thu nhỏ.
- Thuộc tính `alt` giúp mô tả ảnh, `button` tạo nút thao tác; nút chưa hoạt động vì bài tập chỉ có HTML/CSS.

> **Quan trọng:** Không ghi rằng sinh viên đã tự thử hoặc tự sửa mã nếu chưa thực hiện. Hoàn thành các mục trong dấu `[...]` sau khi kiểm tra thực tế.
