# 🎵 Dự án Đoàn Doanh Audio 🎵

## I. TỔNG QUAN DỰ ÁN
"Đoàn Doanh Audio" là siêu loa di động Hi-End công suất 4000W, là một kiệt tác DIY hội tụ những công nghệ tối tân nhất từ kỹ thuật âm học, tản nhiệt nước, vi mạch điện tử đến Trí tuệ nhân tạo (AI) và Hệ thống Robot tự hành (AMR). 
Dự án tập trung 100% vào **Loa Chính (Main Unit)** đóng vai trò là não bộ và trung tâm công suất. Hệ thống loa vệ tinh chỉ là phụ kiện mở rộng ngoại vi.

## II. 10 TÍNH NĂNG AI & DSP ĐỘC QUYỀN ĐẲNG CẤP THẾ GIỚI (10 KỲ QUAN CÔNG NGHỆ)
Nhờ sức mạnh của lõi AI và chip DSP ADAU, hệ thống sở hữu 10 tính năng "World-First" trên một chiếc loa All-in-one:

1. **AI Live Stem Splitter (Tách nhạc 4 Track thời gian thực):** Dùng AI bóc tách trực tiếp bài hát thành 4 kênh: Vocals, Bass, Drums, Other. Có thể tạo beat Karaoke lập tức từ mọi nguồn phát.
2. **Thermal-Adaptive AI DSP (Phân tần thích ứng nhiệt độ):** AI theo dõi nhiệt độ tản nhiệt nước. Khi Overheat, hệ thống không giảm Volume mà tự động can thiệp DSP (cắt Sub cao lên, dùng Multiband Compression) để giảm 25% công suất tiêu thụ vô hình.
3. **AI Psychoacoustic Bass (Bass ảo & Rung chấn 15Hz):** Ở chế độ Party, tạo sóng hài đánh lừa não bộ cảm nhận dải 20Hz. Ở chế độ Hi-End, mở khóa giới hạn dùng Linkwitz Transform ép Sub đánh thẳng xuống 15Hz tạo rung chấn vật lý.
4. **Auto Room Correction (Cân chỉnh phòng tự động):** Mic MEMS I2S gắn nổi mặt trước (ẩn dưới ê-căng) tự động quét RTA hiện sóng, bù trừ dội âm phòng thời gian thực.
5. **AI-SAM (Speaker Active Matching):** Giới hạn cơ học ảo (Excursion Limit). DSP tính toán biên độ màng loa, ép củ loa hoạt động 100% giới hạn vật lý để tạo áp lực bạo lực nhất mà không bao giờ rách màng hay chạm đáy.
6. **Predictive Dynamic BMS:** Ép xung ngược âm học. AI đọc UART từ BMS, nếu pin có nguy cơ sập giữa Party, hệ thống từ từ nới lỏng công suất Bass một cách tinh tế không ai nhận ra, kéo dài tuổi thọ pin thêm hàng giờ.
7. **Acoustic Hologram Upmixer:** Triệt tiêu xuyên âm (Crosstalk Cancellation) tạo sân khấu 3D giả lập, mở rộng âm hình ra không gian gấp 10 lần kích thước thật của loa.
8. **Active Cabinet Resonance Suppression:** Dùng cảm biến rung (Piezo Sensor) dán vào vách gỗ & DSP ép củ Bass tạo sóng cơ học ngược pha. "Khóa chết" mọi rung chấn, biến vỏ nhôm nguyên khối thành tảng đá tĩnh lặng tuyệt đối.
9. **Dynamic FIR/IIR Phase-Morphing:** Tự động "biến hình" Crossover. Dùng IIR (Độ trễ = 0) khi cắm Mic hát Karaoke/Live, và lập tức chuyển sang FIR 65,536-taps (Hoàn hảo về Pha thời gian) khi nghe nhạc Hi-End.
10. **AI Asymmetric Pneumatic Overdrive (Dẫn động Khí nén Bất đối xứng - Đỉnh cao Buồng nén):** 
    - *Vấn đề:* Thùng 32L ép 2 củ Sub Dayton tạo ra lò xo không khí phi tuyến tính. Khi màng loa thụt **vào trong**, khối khí bị nén tạo áp suất kháng cự khổng lồ. Khi màng loa bung **ra ngoài**, nó tạo ra áp suất thấp (lực hút chân không). Dùng dòng điện đối xứng thông thường sẽ sinh ra méo hài bậc 2 cực nặng và xé rách nhện loa do lố đà văng.
    - *Giải pháp AI & DSP:* NPU liên tục phân tích lực đàn hồi khí nén. Thay vì đẩy điện đối xứng, amply TPA3255 tung ra dòng điện **bất đối xứng**: Ở chu kỳ *thụt vào*, amply bơm nhồi thêm 40% công suất để "đạp" dứt khoát vào khối khí áp suất cao. Ở chu kỳ *bung ra* (bị lò xo khí nén đẩy bật dội ngược), amply lập tức chuyển sang chế độ **Phanh điện từ (Electromagnetic Braking)**. Nó tính toán hãm dòng điện lại sao cho màng loa chỉ vượt qua hành trình cân bằng một khoảng vừa đủ để thắng lực hút (vacuum) mà không bị văng lố đà (overshoot).
    - *Kết quả:* Vũ khí hóa hoàn toàn áp suất nén 32L. Hai màng loa Dayton dao động tịnh tiến sắc lẹm, cân bằng tuyệt đối kể cả ở Max Peak 4000W. Tạo ra cú nện Bass căng, tàn bạo, dứt khoát dội thẳng vào lồng ngực mà không hệ thống thùng hở nào làm được.

## III. THIẾT KẾ CƠ KHÍ HI-END & BUỒNG ÂM (MAIN UNIT)
- **Vật liệu vỏ Box:** Nhôm nguyên tấm hợp kim Hàng không (6061-T6), độ dày đồng nhất **15mm** cho tất cả các vách. Các vách được ráp ghép bằng mộng ngàm CNC, dán keo cấu trúc và xiết chặt bằng bu-lông lục giác chìm Inox.
- **Xử lý Âm học mặt trong:** Phay CNC rãnh caro (Asymmetric Grid) sâu 3mm. Phủ toàn bộ bằng lớp keo giảm chấn/chống ồn (Bitumen hoặc Polyurea) dày 2-3mm giúp "tịt âm" kim loại hoàn toàn. Bắn khối nhôm CNC vuốt góc cong (Fillet blocks) tại các góc vuông để triệt tiêu sóng đứng.
- **Kích thước Chuẩn Phong Thủy Lỗ Ban (Phủ bì):** Ngang 432 mm x Cao 366 mm x Sâu 504 mm (Đại Cát trên cả 3 thước).
- **Cấu trúc Quai xách kiêm Roll-Cage (Nóc Loa):** Phay CNC nhôm 4 quai xách chữ U ngược ở 4 góc mặt trên (không làm tăng chiều rộng). Cấu trúc này không chỉ giúp bưng bê dễ dàng, mà còn làm Khung bảo vệ (Roll-cage) cho màn hình cảm ứng 14 inch gập ở giữa.
- **Cấu trúc 3 Khoang Độc Lập:**
  1. **Khoang Trước - Buồng Mid/Bass (~10.8L, Sâu 80mm):** Lắp đặt cụm củ loa mặt trước theo kiến trúc Bán Nguyệt Flush-Mount. 2 loa Bass B&C 5" nằm sát 2 góc dưới (lắp thẳng ngang). 2 loa Mid Scan-Speak 4" dịch vào tâm, nhô cao hơn và CNC phay họng nghiêng **hướng ra ngoài 10° và hếch lên trên 5°**. 2 loa Treble BlieSMa 1.3" đặt cạnh nhau ở chóp đỉnh vòm, CNC phay họng vát nghiêng **hướng ra ngoài 10° và hếch lên trên 10°**. Sự kết hợp vát góc (Compound Tilt) này đồng pha thời gian tuyệt đối và phát tán góc rộng như loa Line-Array sân khấu. Khoang được bịt kín và nhồi bông tiêu âm.
  2. **Khoang Giữa - Boong-ke Sub (~33.1L, Sâu 245mm):** Buồng nén nguyên khối không vách ngăn giữa. Hai củ Sub Dayton 10" nằm đối đỉnh ở 2 mặt bên hông (khoét lỗ giật cấp Flush-mount, bắt từ ngoài lọt lòng vào trong). Gông chặt bằng trục thép ren Inox M20 nối đít 2 củ loa (cách nhau 28mm) giúp tự triệt tiêu toàn bộ lực nén và rung chấn 4000W. Phay khoét lõm 2 bên hông dưới để gắn bánh xe 8-inch tự hành.
  3. **Khoang Sau - Vi mạch & Tản nhiệt (~16.3L, Sâu 124mm):** Không gian sâu 124mm ôm trọn 2 két tản nhiệt nước Radiator 240mm dọc 2 bên hông, quạt tạt gió ra ngoài. Chứa 2 cục nguồn Mean Well, 8 khối amply TPA3255. Mặt lưng là Mica/Kính cường lực 10mm lộ toàn bộ nội thất tản nhiệt nước PC trong suốt.

## IV. HỆ THỐNG CỦ LOA HI-END (4-Way Active trên Main Box)
- **Subwoofer:** 2 x Dayton Audio RSS265HE-22 (10") - 800W RMS/1600W Peak.
- **Bass:** 2 x B&C 5FG44 (5") - Củ Pro-Audio từ Neo. Đánh upper-bass cực rát.
- **Mid:** 2 x Scan-Speak Discovery 10F/4424G00 (4"). (Nhỏ nhưng tái tạo Vocal siêu mượt).
- **Treble:** 2 x BlieSMa T34A-4 (1.3") - Màng hợp kim nhôm-magie đắt giá.
- **Đặc điểm Âm học:** Cụm Mid/Treble được phay lọt lòng mặt ngoài vỏ nhôm, vát nghiêng 3D đa hướng (Compound Angle Waveguides) để tối ưu âm hình Stereo 3D, đồng pha thời gian và bao phủ góc rộng (Wedge Dispersion).

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
- **Bộ não Trung tâm (Robot & AI):** NVIDIA Jetson Orin Nano (40 TOPS) chạy hệ điều hành ROS 2. Gánh vác xử lý tự hành SLAM, Camera 3D và xử lý Audio lõi.
- **Phần Cứng Audio:** XMOS XU208 + Mạch DSP (ADAU1452/1467) + Mạch DAC/Mixer.
- **UI & Màn Hình:** Màn hình cảm ứng 14 inch tháo laptop, dán kính cường lực, khung nhôm CNC gập/dựng trên đỉnh loa. Tích hợp AI chống hú (Anti-Feedback) thời gian thực.
- **Các Chế Độ Âm Thanh (Crossover Động):**
  - *Party Mode:* Ép Max SPL (Peak ~125-127dB). Sub thùng kín cắt ở 40Hz để tối ưu nén pháo kích. Bass gánh lên 1.5kHz để bảo vệ củ Mid yếu.
  - *Cinema / Hi-End Mode:* Gom Loa Main thành Center + Sub, tự động giải mã luồng Dolby chuẩn. Sub đánh thả ga xuống 15Hz rung sàn nhà. Đẩy kênh Surround ra các cổng vệ tinh.

## VII. TẢN NHIỆT NƯỚC & THẨM MỄ
- **Kiến Trúc Làm Mát:** Bơm kép Dual DDC đẩy song song (Parallel Loop) qua Distro-plate tới 8 block nước TPA3255 tránh suy giảm áp lực.
- **Két & Quạt:** 2 Két tản nhiệt Đồng nguyên chất (240/280mm) ở 2 vách hông. 8 Quạt ARGB áp suất tĩnh cao, chạy cấu hình Push-Pull.
- **Bảo Vệ Điện Tử:** Phủ keo Conformal Coating toàn bộ board mạch chống ẩm mốc/chập cháy.

## VIII. KẾT NỐI & NGOẠI VI
- **I/O Đa Dạng:** HDMI eARC (nhận Dolby), Optical, Coaxial, USB-C, LAN RJ45, Wi-Fi Audio (DLNA/AirPlay), Bluetooth QCC5125.
- **Box Micro Rời:** Để tinh gọn Main Unit, hệ thống thu phát Micro không dây được đẩy ra Box riêng, cắm qua cổng XLR/6.35mm.
- **Xuất Loa Vệ Tinh:** Truyền tín hiệu Balanced Analog và Nguồn qua Jack hàng không (Aviation Plug) hoặc Neutrik Speakon cực kỳ chắc chắn, chống nhiễu tuyệt đối.

## IX. CYBERTRUCK MINI - HỆ THỐNG GẦM TỰ HÀNH & AI ROBOTICS
Do khối lượng Kẻ Hủy Diệt xấp xỉ 100kg (Tải trọng thiết kế 150kg), chiếc loa này được nâng cấp thành một cỗ xe Cybertruck tự hành thu nhỏ (AMR - Autonomous Mobile Robot).
- **Kiến trúc gầm hạ trọng tâm:** Phay khoét lõm 2 bên hông vỏ nhôm để gắn **2 Bánh Hub Motor BLDC 8-inch (Trục đơn Single-Shaft)**. Mâm vỏ ôm trọn hệ thống giúp toàn bộ thân loa xệ lọt thỏm xuống giữa 2 bánh, cách mặt đất chỉ khoảng 3cm, triệt tiêu lật và rung chấn.
- **Hệ thống dẫn động & Tank-Turn:** Động cơ 350W-500W/bánh, điều khiển qua mạch ODrive/VESC (Giao tiếp CAN Bus). Kết hợp với **4 bánh Caster PU lõi thép 3-inch** xoay 360 độ giấu dưới gầm. Hệ thống dư sức đẩy 150kg leo dốc 20 độ và xoay múa tròn 360 độ (Tank-Turn) tại chỗ cực êm.
- **Đôi mắt AI & Follow-Me:** Tích hợp Camera độ sâu **Intel RealSense D435** và Lidar ẩn sau ê-căng. NVIDIA Jetson chạy mô hình YOLO/Pose nhận diện khung xương để loa tự động né chướng ngại vật và lẳng lặng lăn bánh bám theo gót chân chủ nhân ở khoảng cách 2 mét.

## X. DỰ TOÁN CHI PHÍ & VẬT TƯ (BOM - BILL OF MATERIALS)
*Đây là bài toán chi phí được tối ưu hóa theo chiến lược "Smart Procurement" (Gom đơn Đại lý B2B - Vận chuyển Đường biển) và khoán trọn gói gia công CNC.*

### 1. HỆ THỐNG CỦ LOA (Speaker Drivers)
**Chiến lược Order:** Gom toàn bộ 8 củ loa tại một đại lý âm thanh quốc tế (VD: SoundImports Châu Âu). Sử dụng tài khoản B2B để hưởng chiết khấu. Vận chuyển **Đường Thủy (Sea Freight)** về Việt Nam.
*   **2 x Treble BlieSMa T34A-4:** ~20.000.000 VNĐ.
*   **2 x Sub Dayton Audio RSS265HE-22 10":** ~16.000.000 VNĐ.
*   **2 x Bass B&C 5FG44 5":** ~5.500.000 VNĐ.
*   **2 x Mid Scan-Speak Discovery 10F/4424G00:** ~5.000.000 VNĐ.
**=> Tổng chi phí Củ loa: ~ 46.500.000 VNĐ**

### 2. CHI PHÍ GIA CÔNG BOX NHÔM CNC & CƠ KHÍ
*   **Gói Gia công Nhôm nguyên khối 6061-T6 (Bao gồm phay quai xách đỉnh, họng kèn nghiêng, ngàm gắn bánh xe hông):** Ước tính khoảng ~15.000.000 - 18.000.000 VNĐ.
*   **Vật tư phụ gia (Kính cường lực 10mm, Keo Epoxy, Keo Bitumen chống ồn, trục thép ren M20):** ~2.500.000 VNĐ.
**=> Tổng chi phí Vỏ Box Nhôm hoàn thiện: ~ 20.500.000 VNĐ**

### 3. HỆ THỐNG MẠCH ĐIỆN & NĂNG LƯỢNG
*   **Nguồn, Pin & BMS (Mean Well, Samsung 40T, JK BMS):** ~11.000.000 VNĐ.
*   **Amply TPA3255 (8 Bo mạch) & Phụ kiện:** ~9.000.000 VNĐ.
**=> Tổng chi phí Năng lượng & Amply: ~ 20.000.000 VNĐ**

### 4. BỘ NÃO, DSP & TỰ HÀNH (CYBERTRUCK MODULE)
*   **NVIDIA Jetson Orin Nano + Intel RealSense D435:** ~12.000.000 VNĐ.
*   **2 Motor Hub 8-inch trục đơn + Mạch ODrive + 4 Bánh Caster lõi thép:** ~6.000.000 VNĐ.
*   **Mạch DSP ADAU + DAC/Mixer + Màn hình cảm ứng 14 inch:** ~7.500.000 VNĐ.
**=> Tổng chi phí Não bộ AI & Gầm xe: ~ 25.500.000 VNĐ**

### 5. HỆ THỐNG TẢN NHIỆT NƯỚC (Water-Cooling)
*   **Bơm & Tank (2 x DDC, Distro-plate CNC):** ~3.500.000 VNĐ.
*   **Két & Quạt (2 Radiator Đồng 240mm, 8 Quạt ARGB):** ~3.000.000 VNĐ.
*   **8 x Block nước TPA3255 & Fitting:** ~3.000.000 VNĐ.
**=> Tổng chi phí Tản nhiệt: ~ 9.500.000 VNĐ**

### 💰 TỔNG DỰ TOÁN CHI PHÍ (ESTIMATED TOTAL BOM)
**=> Khoảng 122.000.000 VNĐ (~ 4.880 USD)**

---
*Bản thiết kế hệ thống được nghiên cứu, tinh chỉnh và phát triển bởi itdoanh.*
