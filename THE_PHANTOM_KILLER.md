# 🎵 Dự án Đoàn Doanh Audio - The Phantom Killer 🎵

## I. TỔNG QUAN DỰ ÁN
Dự án siêu loa di động Hi-End công suất 4000W, tích hợp AI, tản nhiệt nước và công nghệ tối tân nhất từ âm học đến vi mạch tử. Hệ thống chia làm 2 phần chính: **Main Unit** (Loa chính tích hợp não bộ) và **Loa Vệ Tinh** (Active 3-Way).

## II. HỆ THỐNG CỦ LOA HI-END (Cấu hình 4-Way Active)
- **Subwoofer (Khoang giữa 32L, Thùng kín):** 2 x Dayton Audio RSS265HE-22 (10"). Ứng dụng công nghệ **Force-Canceling (Đối đỉnh)**, gông chặt bằng trục Inox M20 để triệt tiêu toàn bộ rung chấn.
- **Bass (Khoang trước kín):** 4 x B&C 5FG44 (5") - Từ Neo Pro-Audio, đánh upper-bass cực rát.
- **Mid (Khoang trước kín):** 4 x Scan-Speak Discovery 10F/4424G00 (4").
- **Treble:** 4 x BlieSMa T34A-4 (1.3") màng Alu-Magnesium.
*Lưu ý: Cụm Mid/Treble lắp ngoài mặt thùng, vát nghiêng 10 độ tối ưu âm hình Stereo và Time-Alignment.*

## III. NĂNG LƯỢNG & KHUẾCH ĐẠI (4000W)
- **Nguồn Điện:** 2 x Mean Well RSP-2000-48 (2000W siêu sạch).
- **Pin & BMS:** 12S4P Samsung 40T + BMS JK 100A (Giới hạn công suất xả 80%).
- **Sạc Thông Minh:** Tự chế, đọc data UART từ BMS. Tự động chuyển 3 mode, ngắt sạc nhường 100% công suất cho Amply khi đánh lớn.
- **Amply Class-D:** 8 bo TPA3255 (tổng 12 chip). Sub: 4 bo Mono (8 chip); Bass: 2 bo Mono (2 chip); Mid/Treble: 2 bo Stereo (2 chip).
- **Cách Ly Nhiễu:** Mass Nổi (Floating Ground) đi dây Star-Ground và dùng mạch cách ly DC-DC.

## IV. BỘ NÃO XỬ LÝ SỐ & TRÍ TUỆ NHÂN TẠO
- **Phần Cứng:** Orange Pi 5 Plus (NPU 6 TOPS) + XMOS XU208 + Cụm DSP (ADAU1452/1467) + Mạch DAC/Mixer rời.
- **Màn Hình UI:** 14 inch cảm ứng, nắp gập khung nhôm CNC, kính cường lực.
- **Hệ Điều Hành:** Bản phân phối Linux (Ubuntu/Debian) chạy Custom UI. 
- **AI & DSP Thực Thời:** Đo đạc RTA hiện sóng, tự động load profile DSP theo thể tích phòng (m3), tự động cắt hú (Anti-Feedback) qua AI (NPU).
- **Chế Độ Âm Thanh:** Các mode linh hoạt (Karaoke, Hi-End, Music, Party, Cinema). Cắt tần (Crossover) linh hoạt (VD: Mode Party ép Bass gánh đến 1.5kHz bảo vệ Mid; Mode Cinema gom loa chính thành Center+Sub, đẩy vệ tinh 5 kênh ra HDMI eARC/I2S).

## V. TẢN NHIỆT NƯỚC & THẨM MỸ (Water Cooling & ARGB)
- **Kiến Trúc:** Bơm kép Dual DDC đẩy song song (Parallel Loop) qua Distro-plate tới 8 Block TPA3255.
- **Két Làm Mát:** 2 Radiator Đồng nguyên chất ở 2 vách hông thùng loa.
- **Tản Nhiệt Khí:** 8 Quạt ARGB áp suất tĩnh, cấu hình Push-Pull qua két nước và màng ê-căng từ tính lọc bụi.
- **Bảo Vệ Điện Tử:** Phủ keo Conformal Coating toàn bộ board mạch chống ẩm.

## VI. KẾT NỐI & NGOẠI VI
- **Cổng vào:** HDMI eARC, Optical, Coaxial, USB-C, Wi-Fi Audio, Bluetooth QCC5125.
- **Kết nối Loa Vệ Tinh:** Truyền Nguồn + Tín hiệu Balanced Analog qua cáp Aviation/Speakon chuyên dụng chống nhiễu tuyệt đối.
- **Micro hát Live/Karaoke:** Box Micro rời cắm qua cổng XLR/6.35mm.

---
*Dự án được nghiên cứu và phát triển bởi itdoanh.*