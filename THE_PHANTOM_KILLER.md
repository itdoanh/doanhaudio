# 🎵 Dự án Đoàn Doanh Audio - The Phantom Killer 🎵

## I. TỔNG QUAN DỰ ÁN
"The Phantom Killer" là siêu loa di động Hi-End công suất 4000W, là một kiệt tác DIY hội tụ những công nghệ tối tân nhất từ kỹ thuật âm học, tản nhiệt nước, vi mạch điện tử đến Trí tuệ nhân tạo (AI). 
Dự án tập trung 100% vào **Loa Chính (Main Unit)** đóng vai trò là não bộ và trung tâm công suất. Hệ thống loa vệ tinh chỉ là phụ kiện mở rộng ngoại vi.

## II. 4 TÍNH NĂNG AI & DSP ĐỘC QUYỀN ĐẲNG CẤP THẾ GIỚI
Nhờ sức mạnh của lõi NPU 6 TOPS (Orange Pi 5 Plus) và chip DSP ADAU, hệ thống sở hữu 4 tính năng "World-First" trên một chiếc loa All-in-one:

1. **AI Live Stem Splitter (Tách nhạc 4 Track thời gian thực):** Dùng AI học sâu bóc tách trực tiếp bài hát (bất kỳ nguồn nào) thành 4 kênh: Vocals, Bass, Drums, Other. Người dùng chỉnh Volume từng track bằng thanh trượt trên màn hình (VD: Kéo Vocal về 0 để tạo beat Karaoke lập tức từ nhạc Spotify/YouTube).
2. **Thermal-Adaptive AI DSP (Phân tần thích ứng nhiệt độ):** AI theo dõi nhiệt độ dung dịch tản nhiệt nước và amply. Nếu hệ thống chạm ngưỡng Overheat, AI không giảm Volume mà tự động can thiệp DSP (Cắt Sub cao lên khoảng 5Hz, áp dụng Multiband Compression). Kết quả: Áp lực âm thanh giữ nguyên 100% nhưng công suất tiêu thụ giảm 25%, hệ thống tự động mát lại.
3. **AI Psychoacoustic Bass & Tactile Subsonic (Bass ảo & Rung chấn vật lý):** Ứng dụng linh hoạt theo chế độ:
   - *Chế độ Party:* Khi Sub bị cắt ở 40Hz để ép Max SPL, DSP tự động tạo sóng hài bậc 2/bậc 3 (Harmonics) trộn vào nhạc. Não bộ sẽ tự "tưởng tượng" ra dải 20Hz sâu thẳm mà màng loa không cần thụt thò quá mức, giúp loa kêu to nứt vách nhưng tiếng vẫn sâu.
   - *Chế độ Hi-End / Cinema:* Tắt Bass ảo. Mở khóa toàn bộ giới hạn, dùng DSP can thiệp sâu (Linkwitz Transform) ép 2 củ Sub Dayton đánh thẳng xuống tần số thực **15Hz - 20Hz**. Với thiết kế thùng kín đối đỉnh, người nghe sẽ thực sự "cảm nhận" được sự rung lắc của sàn nhà và tức ngực về mặt vật lý.
4. **Auto Room Correction (Cân chỉnh âm học phòng tự động):** 
   - Tích hợp trực tiếp mạch Micro MEMS I2S (Knowles / InvenSense) thu tín hiệu phẳng 20Hz-20kHz. Mạch mic được **gắn nổi ngay trên mặt trước** của ván loa (nằm ẩn dưới lớp ê-căng từ tính), chỉ khoan một lỗ siêu nhỏ để luồn dây tín hiệu vào trong và bít kín bằng silicon nhằm bảo toàn áp suất buồng nén.
   - Khi chọn chế độ "Trong Nhà", loa tự động phát tiếng Sweeping/Pink Noise. NPU phân tích biểu đồ RTA thời gian thực, sau đó can thiệp FIR Filter/DSP (Auto EQ & Delay) để cắt dội âm, bù dải khuyết. Lưu Profile tự động theo từng không gian.

## III. THIẾT KẾ CƠ KHÍ & BUỒNG ÂM (MAIN UNIT)
- **Kích thước & Chất liệu:** Dáng Capsule nằm ngang (Ngang 46cm x Cao 38cm x Sâu 52cm). Gỗ Plywood Nga (Vỏ 30mm, vách 20mm).
- **Cấu trúc 3 Khoang Độc Lập:**
  1. **Khoang Giữa (Boong-ke Sub - 32L):** Thiết kế thùng kín (16L/củ). Hai củ Sub nằm quay lưng vào nhau, gông chặt bằng trục Inox M20 đối đỉnh (Force-canceling) triệt tiêu hoàn toàn rung chấn thân vỏ.
  2. **Khoang Trước (11.5L):** Buồng kín, chia vách độc lập cho cụm Bass và cụm Mid/Treble.
  3. **Khoang Sau (15.3L):** Chứa vi mạch, trạm nguồn và tản nhiệt nước. Lưng Mica 10mm khoe linh kiện.

## IV. HỆ THỐNG CỦ LOA HI-END (4-Way Active trên Main Box)
- **Subwoofer:** 2 x Dayton Audio RSS265HE-22 (10") - 800W RMS/1600W Peak.
- **Bass:** 2 x B&C 5FG44 (5") - Củ Pro-Audio từ Neo. Đánh upper-bass cực rát.
- **Mid:** 2 x Scan-Speak Discovery 10F/4424G00 (4"). (Nhỏ nhưng tái tạo Vocal siêu mượt).
- **Treble:** 2 x BlieSMa T34A-4 (1.3") - Màng hợp kim nhôm-magie đắt giá.
- **Đặc điểm Âm học:** Cụm Mid/Treble được phay lắp nổi ở mặt ngoài ván, vát nghiêng 10 độ hướng tâm để tối ưu âm hình Stereo và Time-Alignment.

## V. NĂNG LƯỢNG & KHUẾCH ĐẠI (4000W)
- **Trạm Nguồn:** 2 x Mean Well RSP-2000-48 (Tổng 4000W) + Dàn tụ xả dòng tức thời 150.000uF.
- **Pin & BMS:** Khối pin 12S4P Samsung 40T + BMS JK 100A (Set giới hạn an toàn 80%).
- **Sạc Thông Minh:** Tự chế, đọc UART từ BMS. Tự động chuyển 3 Mode, ngắt sạc nhường 100% công suất cho amply khi mở âm lượng lớn.
- **Amply (8 Bo mạch - 12 Chip TPA3255):**
  - Sub: 4 bo Mono (8 chip).
  - Bass: 2 bo Mono (2 chip).
  - Mid/Treble: 2 bo Stereo (2 chip).
- **Xử lý Nhiễu (Floating Ground):** Hệ thống đi dây Star-Grounding. Vỏ nối mass qua tụ/trở (1000V/1 MegaOhm). Mạch tín hiệu dùng module cách ly nguồn DC-DC và cách ly quang/từ tính.

## VI. BỘ NÃO ĐIỀU KHIỂN & DSP
- **Phần Cứng:** Orange Pi 5 Plus + XMOS XU208 + Mạch DSP (ADAU1452/1467) + Mạch DAC/Mixer.
- **UI & Màn Hình:** Màn hình cảm ứng 14 inch tháo laptop, dán kính cường lực, khung nhôm CNC gập/dựng trên đỉnh loa. Chạy Linux (Debian/Ubuntu) với Custom UI, tích hợp AI chống hú (Anti-Feedback) thời gian thực kết hợp mạch cứng.
- **Các Chế Độ Âm Thanh (Crossover Động):**
  - *Party Mode:* Ép Max SPL (Peak ~125-127dB). Sub thùng kín cắt ở 40Hz để tối ưu nén pháo kích. Bass gánh lên 1.5kHz để bảo vệ củ Mid yếu.
  - *Cinema / Hi-End Mode:* Gom Loa Main thành Center + Sub, tự động giải mã luồng Dolby chuẩn. Sub đánh thả ga xuống 15Hz rung sàn nhà. Đẩy kênh Surround ra các cổng vệ tinh.

## VII. TẢN NHIỆT NƯỚC & THẨM MỸ
- **Kiến Trúc Làm Mát:** Bơm kép Dual DDC đẩy song song (Parallel Loop) qua Distro-plate tới 8 block nước TPA3255 tránh suy giảm áp lực.
- **Két & Quạt:** 2 Két tản nhiệt Đồng nguyên chất (240/280mm) ở 2 vách hông. 8 Quạt ARGB áp suất tĩnh cao, chạy cấu hình Push-Pull.
- **Bảo Vệ Điện Tử:** Phủ keo Conformal Coating toàn bộ board mạch chống ẩm mốc/chập cháy.

## VIII. KẾT NỐI & NGOẠI VI
- **I/O Đa Dạng:** HDMI eARC (nhận Dolby), Optical, Coaxial, USB-C, LAN RJ45, Wi-Fi Audio (DLNA/AirPlay), Bluetooth QCC5125.
- **Box Micro Rời:** Để tinh gọn Main Unit, hệ thống thu phát Micro không dây được đẩy ra Box riêng, cắm qua cổng XLR/6.35mm.
- **Xuất Loa Vệ Tinh:** Truyền tín hiệu Balanced Analog và Nguồn qua Jack hàng không (Aviation Plug) hoặc Neutrik Speakon cực kỳ chắc chắn, chống nhiễu tuyệt đối.

---
*Bản thiết kế hệ thống được nghiên cứu, tinh chỉnh và phát triển bởi itdoanh.*