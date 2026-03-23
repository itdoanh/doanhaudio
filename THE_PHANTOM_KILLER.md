# 🎵 Dự án Đoàn Doanh Audio - The Phantom Killer 🎵

## I. TỔNG QUAN DỰ ÁN
"The Phantom Killer" là siêu loa di động Hi-End công suất 4000W, là một kiệt tác DIY hội tụ những công nghệ tối tân nhất từ kỹ thuật âm học, tản nhiệt nước, vi mạch điện tử đến Trí tuệ nhân tạo (AI). 
Dự án tập trung 100% vào **Loa Chính (Main Unit)** đóng vai trò là não bộ và trung tâm công suất. Hệ thống loa vệ tinh chỉ là phụ kiện mở rộng ngoại vi.

## II. THIẾT KẾ CƠ KHÍ & BUỒNG ÂM (MAIN UNIT)
- **Kích thước & Chất liệu:** Dáng Capsule nằm ngang (Ngang 46cm x Cao 38cm x Sâu 52cm). Gỗ Plywood Nga (Vỏ 30mm, vách 20mm).
- **Cấu trúc 3 Khoang Độc Lập:**
  1. **Khoang Giữa (Boong-ke Sub - 32L):** Thiết kế thùng kín (16L/củ). Hai củ Sub nằm quay lưng vào nhau, gông chặt bằng trục Inox M20 đối đỉnh (công nghệ Force-canceling / Isobaric) triệt tiêu hoàn toàn rung chấn thân vỏ.
  2. **Khoang Trước (11.5L):** Buồng kín, chia vách độc lập cho củ Bass và cụm Mid/Treble.
  3. **Khoang Sau (15.3L):** Chứa toàn bộ vi mạch, trạm nguồn và hệ thống tản nhiệt nước. Mặt lưng Mica 10mm trong suốt khoe linh kiện.

## III. HỆ THỐNG CỦ LOA HI-END (4-Way Active trên Main Box)
- **Subwoofer:** 2 x Dayton Audio RSS265HE-22 (10") - 800W RMS/1600W Peak.
- **Bass:** 2 x B&C 5FG44 (5") - Củ Pro-Audio từ Neo.
- **Mid:** 2 x Scan-Speak Discovery 10F/4424G00 (4").
- **Treble:** 2 x BlieSMa T34A-4 (1.3") - Màng hợp kim nhôm-magie.
- **Đặc điểm Âm học:** Cụm Mid và Treble được phay lắp nổi ở mặt ngoài ván, vát nghiêng 10 độ hướng tâm để tối ưu âm hình Stereo và Time-Alignment (Đồng pha thời gian).

## IV. NĂNG LƯỢNG & KHUẾCH ĐẠI (4000W)
- **Trạm Nguồn:** 2 x Mean Well RSP-2000-48 (Tổng 4000W) + Dàn tụ bù áp xả tức thời 150.000uF 80V.
- **Pin & BMS:** Khối pin 12S4P Samsung 40T (48 cell) + BMS JK 100A (Set giới hạn xả 80% công suất để an toàn).
- **Sạc Thông Minh (Custom):** Đọc data UART từ BMS để điều dòng sạc. 3 Mode: Chạy Pin / Vừa cắm điện vừa sạc / Tự động ngắt sạc nhường 100% công suất cho amply khi mở âm lượng lớn.
- **Amply (8 Bo mạch - 12 Chip TPA3255):**
  - *Sub:* 4 bo Mono (8 chip) đánh độc lập 4 coil.
  - *Bass:* 2 bo Mono (2 chip).
  - *Mid/Treble:* 2 bo Stereo (2 chip).
- **Xử lý Nhiễu (Floating Ground):** Hệ thống không nối đất được thiết kế theo chuẩn Star-Grounding (Mass hình sao). Vỏ khung nối mass qua mạch tụ/trở (1000V/1 MegaOhm). Các mạch tín hiệu dùng module cách ly nguồn DC-DC và cách ly quang/từ tính (Digital Isolator).

## V. BỘ NÃO ĐIỀU KHIỂN, DSP & AI
- **Phần Cứng Xử Lý:** Orange Pi 5 Plus (tích hợp NPU 6 TOPS) + XMOS XU208 + Mạch DSP (ADAU1452/1467) + Mạch DAC/Mixer chuyên dụng.
- **Màn Hình Điều Khiển:** Màn hình cảm ứng 14 inch (tháo laptop), dán kính cường lực, thiết kế khung nhôm CNC gập/dựng linh hoạt ở mặt trên loa.
- **Hệ Điều Hành:** Linux (Debian/Ubuntu) chạy Custom UI toàn màn hình. Tối ưu Real-time Audio với độ trễ siêu thấp.
- **Công Nghệ Trí Tuệ Nhân Tạo (AI) trên NPU:** 
  - Phân tích RTA hiện sóng, tự động Load profile DSP theo thể tích phòng (m3) do người dùng nhập.
  - Nhận diện và cắt hú (Anti-Feedback) thời gian thực bằng mô hình AI học sâu kết hợp phần cứng, cực kỳ hữu dụng khi hát Live/Karaoke.
- **Các Chế Độ Âm Thanh & Dynamic Crossover:** Đo đạc chi tiết từng Hz, Pha, Độ trễ.
  - *Chế độ Party:* Ép công suất đỉnh, Sub cắt dưới 40Hz -> 100Hz. Bass gánh từ 100Hz -> 1.5kHz để bảo vệ củ Mid yếu. Mid đánh từ 1.5kHz -> dải Treble.
  - *Chế độ Rạp Phim (Cinema):* Loa Main gộp thành kênh Center + Sub. Giải mã Dolby chuẩn, đẩy tín hiệu 5 kênh Surround/Atmos ra các loa vệ tinh bên ngoài.
  - *Các chế độ khác:* Karaoke, Hi-End, Music, Thuyết trình.

## VI. TẢN NHIỆT NƯỚC & THẨM MỸ CÔNG NGHIỆP
- **Kiến Trúc Làm Mát:** Dùng 2 Bơm DDC khỏe nối tiếp/song song đẩy nước qua Distro-plate (Ống góp) chia thành 2 nhánh song song làm mát cho 8 block TPA3255, tránh nghẽn dòng.
- **Két Nước (Radiator):** 2 Két tản nhiệt Đồng nguyên chất (240/280mm, dày 30-45mm) đặt ở 2 vách hông.
- **Quạt ARGB & Push-Pull:** 8 Quạt áp suất tĩnh cao kẹp 2 bên két nước theo mô hình Push-Pull ép gió xuyên qua lớp ê-căng từ tính lọc bụi.
- **Bảo Vệ Điện Tử:** Phủ keo Conformal Coating toàn bộ board mạch chống hơi ẩm và chập cháy.

## VII. KẾT NỐI & NGOẠI VI
- **I/O Đa Dạng:** HDMI eARC (nhận luồng Dolby), Optical, Coaxial, USB-C, LAN RJ45, Wi-Fi Audio (DLNA/AirPlay), Bluetooth QCC5125.
- **Hệ Thống Micro:** Sử dụng Box Micro rời kết nối qua cổng XLR/6.35mm Combo, giúp linh hoạt nâng cấp bộ thu phát không dây bên ngoài.
- **Xuất Loa Vệ Tinh (Phụ kiện rời):** Tín hiệu Analog Balanced và nguồn điện được truyền qua Jack hàng không (Aviation Plug) hoặc Neutrik Speakon cực kỳ chắc chắn và chống nhiễu tuyệt đối.

---
*Bản thiết kế hệ thống được nghiên cứu, tinh chỉnh và phát triển bởi itdoanh.*