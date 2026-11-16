---
name: anti-template-web-architecture
description: >-
  Use this skill whenever designing or coding websites, landing pages, web apps, or portfolios to break free from the repetitive AI SaaS layout skeleton. Provides 12+ Awwwards/Godly-inspired spatial architectures, broken grids, split-screen pinned layouts, editorial spreads, and interactive index structures.
---

# Anti-Template Web Architecture (Breaking the AI Skeleton)

Nguyên nhân lớn nhất khiến các trang web do AI tạo ra nhìn "na ná nhau" — dù đã đổi màu và đổi font — là vì chúng dùng chung **một bộ khung xương DOM duy nhất**:
`Navbar ngang -> Hero căn giữa -> Dải logo đối tác -> 3 cột tính năng (icon + chữ) -> Bento Grid -> Bảng giá 3 cột -> FAQ Accordion -> Footer 4 cột`.

Khi kỹ năng này được kích hoạt, bạn **BỊ CẤM** sử dụng trình tự cấu trúc trên trừ khi người dùng yêu cầu đích danh. Thay vào đó, bạn phải chọn một trong các **Kiến trúc Không gian (Spatial Architectures)** dưới đây.

---

## 1. 8 Kiến trúc Trang Đột Phá (Awwwards / Godly Archetypes)

### Kiến trúc A: Split-Screen Pinned Narrative (Bố cục Đôi Ghim Cố Định)
- **Cấu trúc**: Màn hình chia làm 2 cột bất đối xứng (ví dụ `42% / 58%` hoặc `35% / 65%`) bằng CSS Grid.
- **Cơ chế**:
  - Một cột được ghim cố định (`position: sticky; top: 0; height: 100vh`) chứa tiêu đề lớn, điều hướng chương mục, hoặc một khung Canvas/Visual biến đổi theo vị trí cuộn.
  - Cột còn lại cuộn tự do qua các phân đoạn nội dung chi tiết, hình ảnh khổ dọc, và thông số kỹ thuật.
- **Khi nào dùng**: Portfolio, trang giới thiệu sản phẩm thiết kế, kiến trúc, studio sáng tạo, tài liệu tương tác.

### Kiến trúc B: Editorial Magazine Spread (Bố cục Tạp Chí Đa Cột Lệch Nhịp)
- **Cấu trúc**: Hệ thống lưới 12 cột có đường kẻ chia cột mảnh (`border-right: 1px solid`) hoặc khoảng trống bất đối xứng lớn.
- **Cơ chế**:
  - Mở đầu không phải bằng nút bấm CTA, mà bằng một **Tuyên ngôn thị giác (Visual Manifesto)**: Chữ Display cỡ cực lớn chiếm trọn chiều ngang (`100vw`), theo sau là đoạn dẫn nhập lệch sang cột thứ 7–12.
  - Hình ảnh có tỷ lệ đa dạng (`4:5` dọc, `21:9` điện ảnh, `1:1` vuông nhỏ) được đặt lệch hàng (staggered vertical offsets) tạo nhịp điệu như trang báo giấy nghệ thuật.
- **Khi nào dùng**: Thời trang, ẩm thực, thương hiệu cao cấp, văn hoá, blog chuyên sâu, sự kiện.

### Kiến trúc C: Interactive Archive / Index Table (Giao diện Danh Mục Tương Tác)
- **Cấu trúc**: Toàn bộ trang chủ là một bảng danh mục sống động (Index-first UI) gồm các hàng ngang sắc nét (`border-bottom: 1px solid`).
- **Cơ chế**:
  - Mỗi hàng hiển thị thông tin cô đọng theo cột: `[Mã số] — [Tên hạng mục/Dự án] — [Danh mục] — [Năm/Thông số]`.
  - Khi di chuột (hover) qua từng hàng: một cửa sổ preview ảnh/video nổi lên đi theo trỏ chuột, hoặc mở rộng mượt mà ngay tại dòng đó (accordion reveal), hoặc đổi hình nền toàn trang.
- **Khi nào dùng**: Agency, danh mục sản phẩm, kho lưu trữ dự án, phòng trưng bày nghệ thuật, danh sách tính năng kỹ thuật.

### Kiến trúc D: Product-as-Hero / Live Sandbox (Sản Phẩm Là Màn Hình Đầu Tiên)
- **Cấu trúc**: Xoá bỏ hoàn toàn phần "Hero giới thiệu sáo rỗng". Ngay khi vào trang, 85% diện tích màn hình đầu tiên là một **bản mô phỏng tương tác trực tiếp (Interactive Playground / Live Tool)** của chính sản phẩm đó.
- **Cơ chế**:
  - Người dùng có thể bấm nút thật, kéo thanh trượt, gõ thử dữ liệu, chuyển đổi chế độ xem ngay lập tức.
  - Tiêu đề thương hiệu và nút điều hướng được thu gọn tinh tế vào một thanh Dock nổi ở cạnh dưới màn hình (`bottom: 24px`) hoặc góc trên bên trái.
- **Khi nào dùng**: Công cụ phần mềm, ứng dụng web, AI tool, tiện ích developer, fintech.

### Kiến trúc E: Asymmetric Broken Grid & Overlapping Collage (Lưới Phá Cách Xếp Lớp)
- **Cấu trúc**: Các phần tử không nằm ngoan ngoãn trong các ô bằng nhau mà giao thoa qua các cột lưới (`grid-column: 2 / 8` chồng một phần lên `grid-column: 6 / 12` với `z-index` có chủ đích).
- **Cơ chế**:
  - Chữ tiêu đề lớn đè một nửa lên rìa bức ảnh.
  - Các chú thích kỹ thuật (captions) nằm dọc theo cạnh ảnh (`writing-mode: vertical-rl`).
- **Khi nào dùng**: Nghệ thuật đương đại, âm nhạc, streetwear, chiến dịch ra mắt sản phẩm mới.

### Kiến trúc F: Scrollytelling Chapter Choreography (Kể Chuyện Phân Cảnh)
- **Cấu trúc**: Trang web được chia thành 4–5 phân cảnh toàn màn hình (`min-height: 100vh`), mỗi phân cảnh có bảng màu (theme) đảo ngược nhau (ví dụ: Cảnh 1 nền Đen Mực -> Cảnh 2 chuyển mượt sang nền Giấy Ngà -> Cảnh 3 nền Đỏ Vermilion).
- **Cơ chế**: Sử dụng bộ đếm chương cố định ở rìa màn hình (`[01 / 04]`) và chuyển tiếp bối cảnh rõ rệt.

---

## 2. Quy tắc Phá Bỏ Các Thành Phần Rập Khuôn (Component Detox)

### ❌ Tuyệt đối không làm điều hướng (Navbar) kiểu cũ mọi lúc:
Thay vì luôn dùng thanh `height: 64px; justify-content: space-between; backdrop-blur` ở đỉnh trang, hãy luân phiên sử dụng:
1. **Floating Bottom Pill Dock**: Thanh điều hướng nhỏ gọn nổi ở đáy màn hình như macOS/iOS.
2. **Corner Frame Navigation**: 4 mục điều hướng gắn ở 4 góc màn hình cố định (`top-left`, `top-right`, `bottom-left`, `bottom-right`), tạo khung ngắm máy ảnh bao quanh nội dung.
3. **Vertical Sidebar Spine**: Thanh gáy sách dọc bên trái rộng `48px - 64px` với chữ xoay dọc 90 độ.
4. **Minimal Editorial Header**: Dòng chữ giống đầu trang báo với ngày tháng, toạ độ, phiên bản, và danh mục ngăn cách bằng đường kẻ mảnh.

### ❌ Tuyệt đối không dùng "3-Column Feature Cards" lặp lại:
Khi cần trình bày 3–6 lợi ích hoặc tính năng, **CẤM** tạo 3 chiếc hộp bo tròn đặt cạnh nhau. Hãy thay bằng:
1. **Interactive Tabbed Showcase**: Cột trái là danh sách tiêu đề lớn; bấm hoặc hover vào mục nào thì cột phải hiển thị sơ đồ/giao diện chi tiết của mục đó.
2. **Staggered Zig-Zag Editorial**: Trình bày lệch dòng với tỷ lệ 1 lớn – 2 nhỏ không đối xứng.
3. **Horizontal Spec Sheet**: Bố cục bảng thông số kỹ thuật chuẩn công nghiệp với đường kẻ mảnh, số liệu thực tế và hình minh hoạ kỹ thuật đi kèm.

### ❌ Cấm Footer 4 cột nhàm chán:
Hãy biến Footer thành một **Monumental Closing (Cái kết đầy ấn tượng)**:
- Một dòng chữ Typography khổng lồ chạy tràn lề đáy màn hình (`font-size: 14vw; line-height: 0.85`).
- Một nút tương tác lớn hoặc lời mời hợp tác trực diện thay vì 20 đường link giả (`Privacy Policy`, `Terms`, `Blog`, `Careers`...) không dẫn đi đâu.
