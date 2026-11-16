---
name: bespoke-visual-craft
description: >-
  Use this skill to create custom, high-craft visual elements in code (technical SVG schematics, generative patterns, tactile noise shaders, editorial photo treatments, and architectural markers) instead of generic icon-in-a-box tropes and lifeless stock imagery.
---

# Bespoke Visual Craft & Code-Generated Art

Dấu hiệu tố cáo rõ rệt nhất của một trang web do AI làm ra là **"Icon đặt trong hộp màu nhạt"**: một chiếc icon thư viện (Lucide/FontAwesome) nằm trong ô vuông `44x44px`, bo góc `8px`, nền `rgba(accent, 0.1)`.

Khi sử dụng kỹ năng này, bạn **TUYỆT ĐỐI CẤM** dùng công thức "icon trong hộp màu nhạt". Mọi yếu tố đồ hoạ trên trang phải mang tính thủ công cao cấp (Bespoke Craft).

---

## 1. Thay Thế Icon Đại Trà Bằng "Technical SVG Schematics" (Bản Vẽ Kỹ Thuật)

Thay vì đặt một chiếc icon nhỏ xíu vô hồn trên đầu đoạn văn, hãy tự vẽ các **Sơ đồ hình học / Bản vẽ kỹ thuật bằng SVG thuần**:

- **Đặc điểm nhận diện**:
  - Sử dụng đường nét cực mảnh (`stroke-width="1"` hoặc `0.75`), kết hợp đường nét liền và nét đứt (`stroke-dasharray="3 3"`).
  - Có các dấu cộng định vị (crosshairs `+`), vòng tròn đồng tâm, toạ độ góc (`45°`, `0.024mm`), hoặc sơ đồ luồng dữ liệu có chấm sáng chạy dọc theo đường dẫn (`<animateMotion>` hoặc `stroke-dashoffset`).
- **Tác dụng**: Biến mỗi khối tính năng thành một bản thiết kế cơ khí/kiến trúc đầy thuyết phục.

---

## 2. Xử Lý Hình Ảnh Chuẩn Giám Đốc Nghệ Thuật (Editorial Media Treatment)

Không bao giờ quăng một bức ảnh stock nguyên bản vào khung bo tròn `border-radius: 16px`. Hãy áp dụng các kỹ thuật xử lý ảnh nghệ thuật:

### A. Tỷ lệ cắt cúp điện ảnh & tạp chí (Intentional Aspect Ratios)
- Sử dụng tỷ lệ `4:5` hoặc `3:4` (chân dung tạp chí), `21:9` (panorama điện ảnh), hoặc cắt hình học bất đối xứng (`clip-path: polygon(...)`).
- Kèm theo dòng chú thích kỹ thuật nhỏ bên dưới hoặc dọc cạnh ảnh (ví dụ: `FIG. 02 — ARCHIVE STUDIO, TOKYO [35MM]`).

### B. Bộ lọc màu đồng nhất (Chromatic Image Grading)
Dùng CSS filter hoặc SVG `<feColorMatrix>` để toàn bộ ảnh trên web hoà nhập tuyệt đối vào bảng màu thương hiệu:
```css
/* Hiệu ứng High-Contrast Monochrome có chiều sâu, khi hover mới trả lại màu gốc */
.editorial-image {
  filter: grayscale(100%) contrast(1.12) brightness(0.96);
  transition: filter 0.6s cubic-bezier(0.16, 1, 0.3, 1);
}
.editorial-image:hover {
  filter: grayscale(0%) contrast(1.02) brightness(1);
}
```

---

## 3. Tạo Chất Liệu Xúc Giác Bằng Code (Procedural Surface Textures)

Màn hình kỹ thuật số mặc định rất phẳng và lạnh. Hãy thêm lớp chất liệu vật lý siêu nhẹ bằng SVG hoặc CSS:

### A. Lớp hạt nhiễu phim Analog (SVG Film Grain Overlay)
Tạo một lớp phủ toàn trang cố định (`pointer-events: none; z-index: 9999; opacity: 0.035`) bằng bộ lọc `<feTurbulence type="fractalNoise" baseFrequency="0.8" numOctaves="3">` nhúng trực tiếp dưới dạng Data URI để tạo cảm giác như giấy in cao cấp hoặc phim nhựa.

### B. Hệ thống dấu neo kiến trúc (Architectural Grid Markers)
Tại các điểm giao nhau của đường kẻ lưới (Grid intersections), đặt các dấu cộng mảnh (`+`) hoặc góc vuông nhỏ (`┌ ┐ └ ┘`) kích thước `7px x 7px` để tạo cảm giác bề mặt được đo đạc tỉ mỉ.

### C. Typography như một Tác Phẩm Điêu Khắc (Typographic Sculpture)
Khi không có hình ảnh minh hoạ phù hợp, đừng dùng ảnh giả. Hãy dùng chính những con chữ khổng lồ (`12rem - 20rem`), chữ viền rỗng (`-webkit-text-stroke: 1px currentColor; color: transparent`), hoặc ma trận ký tự tương tác làm điểm nhấn thị giác chính.
