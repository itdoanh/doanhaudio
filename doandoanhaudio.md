# 🎵 Dự án Đoàn Doanh Audio 🎵

## I. TỔNG QUAN DỰ ÁN
"Đoàn Doanh Audio" là siêu loa di động Hi-End công suất 4000W, là một kiệt tác DIY hội tụ những công nghệ tối tân nhất từ kỹ thuật âm học, tản nhiệt nước, vi mạch điện tử đến Trí tuệ nhân tạo (AI) và Hệ thống Robot tự hành (AMR). 
Dự án tập trung 100% vào **Loa Chính (Main Unit)** đóng vai trò là não bộ và trung tâm công suất. Hệ thống loa vệ tinh chỉ là phụ kiện mở rộng ngoại vi. Với tổng khối lượng tĩnh lên tới **100kg**, đây là một cỗ máy cơ khí hạng nặng mang linh hồn của nghệ thuật âm thanh.

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
  1. **Khoang Trước - Buồng Mid/Bass (~10.8L, Sâu 80mm):** Lắp đặt cụm củ loa mặt trước theo kiến trúc Bán Nguyệt Flush-Mount. 2 loa Bass Purifi 5.25" nằm sát 2 góc dưới (lắp thẳng ngang). 2 loa Mid BlieSMa M74B-6 dịch vào tâm, nhô cao hơn và CNC phay họng nghiêng **hướng ra ngoài 10° và hếch lên trên 5°**. 2 loa Treble BlieSMa T34B-4 đặt cạnh nhau ở chóp đỉnh vòm, CNC phay họng vát nghiêng **hướng ra ngoài 10° và hếch lên trên 10°**. Sự kết hợp vát góc (Compound Tilt) này đồng pha thời gian tuyệt đối và phát tán góc rộng. Khoang được bịt kín và nhồi bông tiêu âm.
     - *Cơ cấu SPINE BRACING (Khóa lưng nam châm B&W):* Củ loa Purifi được khóa chết bằng cơ cấu Spine Bracing. Sử dụng một **Cốc kẹp CNC (Magnet Yoke)** ôm sát vòng ngoài nam châm (hở tâm để không bịt lỗ thoát khí tản nhiệt của Voice Coil). Cốc này nối với một trục Inox M12 đâm xuyên qua vách ngăn phía sau. Bằng cách dùng cờ-lê xiết đai ốc từ phía boong-ke sau, trục Inox kéo ngược và kẹp chặt củ Purifi vào vách nhôm mặt trước với lực nén cực lớn. Phản lực giật lùi (Backlash force) $\pm$9.8mm của màng loa Purifi sẽ truyền thẳng qua trục Inox vào khối lượng 100kg của loa, giữ mặt trước tĩnh lặng tuyệt đối để củ Beryllium tái tạo không gian tĩnh như chân không.
  2. **Khoang Giữa - Boong-ke Sub (~33.1L, Sâu 245mm):** Buồng nén nguyên khối không vách ngăn giữa. Hai củ Sub Dayton 10" nằm đối đỉnh ở 2 mặt bên hông (khoét lỗ giật cấp Flush-mount, bắt từ ngoài lọt lòng vào trong). Gông chặt bằng trục thép ren Inox M20 nối đít 2 củ loa (cách nhau 28mm) giúp tự triệt tiêu toàn bộ lực nén và rung chấn 4000W. Phay khoét lõm 2 bên hông dưới để gắn bánh xe 8-inch tự hành.
  3. **Khoang Sau - Vi mạch & Tản nhiệt (~16.3L, Sâu 124mm):** Không gian sâu 124mm ôm trọn 2 két tản nhiệt nước Radiator 240mm dọc 2 bên hông, quạt tạt gió ra ngoài. Chứa 2 cục nguồn Mean Well, dàn Amply 6-Layer PCBs. Mặt lưng là Mica/Kính cường lực 10mm lộ toàn bộ nội thất tản nhiệt nước PC trong suốt.

## IV. BẢNG TÍNH TOÁN CÂN NẶNG CHI TIẾT (~100 KG)
Đây là một cỗ máy bạo lực về mặt vật lý, khối lượng tĩnh lên tới 100kg giúp triệt tiêu hoàn toàn nội chấn:
- **Khung vỏ Nhôm CNC 15mm & Vách ngăn:** ~45.0 kg
- **Hệ thống 8 Củ loa:** ~18.0 kg *(2x Dayton: 13kg, 2x Purifi: 3kg, 4x BlieSMa: 2kg)*
- **Hệ thống Gầm tự hành (2 Hub Motor 8", Bánh Caster, Trục Inox):** ~10.0 kg
- **Hệ thống Tản nhiệt nước (Rad đồng, Bơm Dual, Block, Nước Coolant):** ~8.0 kg
- **Nguồn Mean Well RSP-2000 (2 cục):** ~4.0 kg
- **Khối Pin Samsung 40T 12S4P + BMS:** ~4.0 kg
- **Khối Vi mạch (PCB 6-layer, Busbar đồng khối, Jetson AI, Màn hình):** ~6.0 kg
- **Cơ cấu Spine Bracing & Ốc vít Inox/Cáp kết nối:** ~5.0 kg
=> **TỔNG KHỐI LƯỢNG THIẾT KẾ DỰ KIẾN: ~100.0 KG**

## V. HỆ THỐNG CỦ LOA HI-END (4-Way Active trên Main Box)
- **Subwoofer:** 2 x Dayton Audio RSS265HE-22 (10") - 800W RMS/1600W Peak.
- **Bass:** 2 x Purifi PTT5.0X04-NFA-01 (5.25") - Quái vật hành trình siêu dài ($\pm$9.8mm), độ méo tiệm cận 0%, gánh vác dải Kick-drum bạo lực (80Hz - 450Hz).
- **Mid:** 2 x BlieSMa M74B-6 (3") - Dome Beryllium nguyên chất siêu nhẹ (1.8g). Tốc độ chớp nhoáng, giọng hát nổi khối 3D siêu thực (450Hz - 3kHz).
- **Treble:** 2 x BlieSMa T34B-4 (1.3") - Dome Beryllium nguyên chất. Dải siêu âm vươn tới 40kHz, tĩnh lặng và tàng hình tuyệt đối.
- **Đặc điểm Âm học:** Cụm Mid/Treble được phay lọt lòng mặt ngoài vỏ nhôm, vát nghiêng 3D đa hướng (Compound Angle Waveguides) để tối ưu âm hình Stereo 3D, đồng pha thời gian và bao phủ góc rộng (Wedge Dispersion).

## VI. NĂNG LƯỢNG & KHUẾCH ĐẠI (4000W)
- **Trạm Nguồn:** 2 x Mean Well RSP-2000-48 (Tổng 4000W) + Dàn tụ xả dòng tức thời 150.000uF.
- **Pin & BMS:** Khối pin 12S4P Samsung 40T + BMS JK 100A (Set giới hạn an toàn 80%).
- **Sạc Thông Minh:** Tự chế, đọc UART từ BMS. Tự động chuyển 3 Mode, ngắt sạc nhường 100% công suất cho amply khi mở âm lượng lớn.
- **Amply (8 Bo mạch - 12 Chip TPA3255 & IRS2092S):**
  - Sub: 2 bo Mono IRS2092S chạy SiC MOSFET.
  - Bass: 2 bo Mono TPA3255 (chế độ PBTL Interleaved).
  - Mid/Treble: 2 bo Stereo TPA3255.
- **Xử lý Nhiễu (Floating Ground):** Hệ thống đi dây Multi-Tier Star-Grounding. Vỏ nối mass qua tụ/trở (1000V/1 MegaOhm). Mạch tín hiệu dùng module cách ly nguồn DC-DC và cách ly quang/từ tính.

## VII. BỘ NÃO ĐIỀU KHIỂN & DSP
- **Bộ não Trung tâm (Robot & AI):** NVIDIA Jetson Orin Nano (40 TOPS) chạy hệ điều hành ROS 2. Gánh vác xử lý tự hành SLAM, Camera 3D và xử lý Audio lõi.
- **Phần Cứng Audio:** XMOS XU208 + Mạch DSP (ADAU1452/1467) + Mạch DAC/Mixer ESS.
- **UI & Màn Hình:** Màn hình cảm ứng 14 inch tháo laptop, dán kính cường lực, khung nhôm CNC gập/dựng trên đỉnh loa. Tích hợp AI chống hú (Anti-Feedback) thời gian thực.
- **Các Chế Độ Âm Thanh (Crossover Động):**
  - *Party Mode:* Ép Max SPL (Peak ~125-127dB). Sub thùng kín cắt ở 40Hz để tối ưu nén pháo kích. Bass gánh lên 450Hz để bảo vệ củ Mid Beryllium.
  - *Cinema / Hi-End Mode:* Gom Loa Main thành Center + Sub, tự động giải mã luồng Dolby chuẩn. Sub đánh thả ga xuống 15Hz rung sàn nhà. Đẩy kênh Surround ra các cổng vệ tinh.

## VIII. TẢN NHIỆT NƯỚC & THẨM MỄ
- **Kiến Trúc Làm Mát:** Bơm kép Dual DDC đẩy song song (Parallel Loop) qua Distro-plate tới các block nước TPA3255 và SiC MOSFET tránh suy giảm áp lực.
- **Két & Quạt:** 2 Két tản nhiệt Đồng nguyên chất (240/280mm) ở 2 vách hông. 8 Quạt ARGB áp suất tĩnh cao, chạy cấu hình Push-Pull.
- **Bảo Vệ Điện Tử:** Phủ keo Conformal Coating toàn bộ board mạch chống ẩm mốc/chập cháy.

## IX. KẾT NỐI & NGOẠI VI
- **I/O Đa Dạng:** HDMI eARC (nhận Dolby), Optical, Coaxial, USB-C, LAN RJ45, Wi-Fi Audio (DLNA/AirPlay), Bluetooth QCC5125.
- **Box Micro Rời:** Để tinh gọn Main Unit, hệ thống thu phát Micro không dây được đẩy ra Box riêng, cắm qua cổng XLR/6.35mm.
- **Xuất Loa Vệ Tinh:** Truyền tín hiệu Balanced Analog và Nguồn qua Jack hàng không (Aviation Plug) hoặc Neutrik Speakon cực kỳ chắc chắn, chống nhiễu tuyệt đối.

## X. CYBERTRUCK MINI - HỆ THỐNG GẦM TỰ HÀNH & AI ROBOTICS
Do khối lượng Kẻ Hủy Diệt xấp xỉ 100kg (Tải trọng thiết kế 150kg), chiếc loa này được nâng cấp thành một cỗ xe Cybertruck tự hành thu nhỏ (AMR - Autonomous Mobile Robot).
- **Kiến trúc gầm hạ trọng tâm:** Phay khoét lõm 2 bên hông vỏ nhôm để gắn **2 Bánh Hub Motor BLDC 8-inch (Trục đơn Single-Shaft)**. Mâm vỏ ôm trọn hệ thống giúp toàn bộ thân loa xệ lọt thỏm xuống giữa 2 bánh, cách mặt đất chỉ khoảng 3cm, triệt tiêu lật và rung chấn.
- **Hệ thống dẫn động & Tank-Turn:** Động cơ 350W-500W/bánh, điều khiển qua mạch ODrive/VESC (Giao tiếp CAN Bus). Kết hợp với **4 bánh Caster PU lõi thép 3-inch** xoay 360 độ giấu dưới gầm. Hệ thống dư sức đẩy 150kg leo dốc 20 độ và xoay múa tròn 360 độ (Tank-Turn) tại chỗ cực êm.
- **Đôi mắt AI & Follow-Me:** Tích hợp Camera độ sâu **Intel RealSense D435** và Lidar ẩn sau ê-căng. NVIDIA Jetson chạy mô hình YOLO/Pose nhận diện khung xương để loa tự động né chướng ngại vật và lẳng lặng lăn bánh bám theo gót chân chủ nhân ở khoảng cách 2 mét.

## XI. HỆ THỐNG KHUẾCH ĐẠI ĐA DẢI (THE ULTIMATE AMPLIFICATION CORE)
**Định hướng:** Ultra High-End Active DSP 4-Way Loudspeaker System (Hệ thống loa 4 đường tiếng chủ động).  
**Kiến trúc cốt lõi:** Task Segregation (Phân rã nhiệm vụ) & Aerospace-Grade Discrete Components (Linh kiện rời cấp độ Hàng không vũ trụ). Không bắt một linh kiện làm nhiều việc. Ép các khối Silicon Class-D (TPA3255, IRS2092S) hoạt động trong một môi trường sinh tồn lý tưởng tuyệt đối.

---

### 1. MODULE 1 (TREBLE): BLIESMA T34B-4 BERYLLIUM - "ULTRA-LINEAR AEROSPACE BTL"
**Tính chất củ loa:** Beryllium nguyên chất, siêu âm vươn tới 40kHz.  
**Mục tiêu thiết kế:** Méo hài tổng (THD+N) < 0.001% ở 40kHz. Nền âm tĩnh lặng tuyệt đối (Noise Floor < -125dB).
*   **Phân rã Nguồn điện:** PVDD qua Active Ripple Eater (Discrete Capacitance Multiplier). GVDD/AVDD qua tổ hợp Dual LT3045 LDO (Nhiễu siêu thấp 0.8 µVrms).
*   **Tầng xử lý Tín hiệu:** Tầng Buffer JFET & Error-Amp chạy bằng Discrete Op-Amp (Sparkos SS3602) Pure Class-A. OPA2188 DC-Servo liên tục ép DC Offset về 0.000V.
*   **Công suất & Hủy nhiễu:** TPA3255 BTL ép xung 600kHz. Pseudo-GaN SiC Clamping (8x Diode Silicon Carbide) mô phỏng sườn xung GaN, bóp chết méo hài bậc lẻ H3, H5.
*   **Mạng xuất âm:** PFFB dùng 100% điện trở Vishay Naked Z-Foil (sai số 0.005%). Bộ lọc LC (Cuộn cảm Air-Core + tụ WIMA FKP2) cắt 150kHz. RF Termination Zobel dùng điện trở Caddock Non-Inductive + tụ Silver Mica.

### 2. MODULE 2 (MID): BLIESMA M74B-6 BERYLLIUM - "DISCRETE HYBRID CLASS-A BTL"
**Tính chất củ loa:** Dome Beryllium 3-inch, siêu nhẹ 1.8g, cực kỳ nhạy cảm với méo giao điểm.
*   **Nguồn điện & Tầng xử lý:** Kế thừa 100% nguồn tam lập cách ly của Treble. Sử dụng Discrete Pre-Amp Pure Class-A để bơm sự ấm áp và nhạc tính vào sự chính xác tàn nhẫn của màng Beryllium, bảo tồn hài âm bậc chẵn (H2).
*   **Bộ lọc Ultra Hi-End:** Nâng cấp cực đoan lên **Cuộn cảm Lá Đồng lõi không khí (Mundorf CFC)** 7.0 µH + **Tụ màng Bạc/Đồng ngâm dầu (Duelund/Mundorf)** 1.0 µF. Vật liệu xa xỉ này bóp chết 100% méo từ trễ (Magnetic Hysteresis), giải phóng sân khấu âm thanh 3D siêu thực.
*   **Z-Foil On-Board Kelvin Sense PFFB:** Khóa cứng thông số amply, bù trừ tàn nhẫn lực dội ngược (Back-EMF).

### 3. MODULE 3 (MID-BASS): PURIFI PTT5.25X04-NAA-05 - "AEROSPACE INTERLEAVED PBTL"
**Tính chất củ loa:** Hành trình Xmax $\pm$9.8mm, bị nhốt trong thùng nhôm nén kín tạo áp suất cực lớn.
*   **Kiến trúc Interleaved PBTL (BTL Lệch Pha):** 2 chip TPA3255 đánh PBTL. Can thiệp Clock ép 2 nửa cầu đóng/cắt lệch pha nhau chính xác 180°. Tần số băm xung biểu kiến đập vào màng Purifi lên tới **1.2 MHz**, tự động triệt tiêu nhiễu Ripple.
*   **Cuộn cảm Liên kết Từ tính (Bi-filar Coupled Nanocrystalline):** Quấn bằng dây dẹt trên cùng một lõi Nanocrystalline (Vật liệu Hàng không). Chống bão hòa từ tuyệt đối dù Peak giật lên 30 Ampe.
*   **Tụ Nguồn Bạo Chúa:** Phủ đồng nguyên khối Copper Pour sát chân PVDD. Tổ hợp tụ Low-ESR Rubycon ZLH + Gốm MLCC xả dòng cấp tốc để Purifi nện những cú Kick-bass bạo lực nhất. PFFB vi sai Z-Foil ép nội trở về 0 (Bỏ qua Zobel điện dung lớn).

### 4. MODULE 4 (SUBWOOFER): DAYTON 10" - "COMPOSITE GaN & PNEUMATIC OVERDRIVE"
**Tính chất củ loa:** DVC (2 Coil x 2 Ohms). Peak 1600W. Hoạt động như lò xo khí nén phi tuyến tính (Buồng 32L).
*   **Mạch Nâng Áp 1MHz GaN:** Boost 4-Phase dùng **GaN FETs (Gallium Nitride)** và biến áp phẳng PCB đưa 48V lên $\pm$75V DC siêu phẳng. Mạch phản ứng với sụt áp trong 1 micro-giây.
*   **Khuếch đại Composite SiC:** IC IRS2092S lái sò **SiC MOSFET (Wolfspeed)** thông qua BJT Totem-Pole. Khối công suất 1600W này nằm gọn trong vòng lặp hồi tiếp tổng của Sparkos Op-Amp Class-A để ép THD < 0.001%.
*   **Cảm Biến Dòng Điện Hàng Không & Phanh Động Học AI:** Dây loa Sub luồn qua Cảm biến từ trường hiệu ứng Hall (Allegro ACS37002) báo dòng Peak 50A về DSP với nội trở 0 Ohm. Khi AI hãm phanh màng loa (Electromagnetic Braking), năng lượng dội ngược sinh Bus Pumping (vượt 82V) sẽ được xả qua mạch **Active Brake Chopper** vào Khối điện trở Sứ công suất cao ngâm trong khối Tản nhiệt nước.

### 5. QUY CHUẨN THIẾT KẾ PCB BẮT BUỘC (AEROSPACE ROUTING)
1.  **Vật liệu 6 Lớp (6-Layer Rogers):** Đặt in tại PCBWay. Sử dụng lõi **Rogers RO4350B** (cấp độ 5G/Radar).
2.  **Microwave Routing cho PFFB:** Tín hiệu hồi tiếp PFFB đi theo chuẩn đường truyền vi sai (Differential Stripline) chạy Via ngầm giữa 2 lớp Ground Plane để cách ly bức xạ từ khối nguồn 4000W.
3.  **Multi-Tier Star Grounding:** Mass tín hiệu, Mass số và Mass công suất phân bổ trên các Layer riêng biệt. Chập lại qua hạt Ferrite Bead chịu dòng cao để bóp chết vòng lặp nhiễu (Ground Loop).
4.  **Solid Copper Busbar:** Trên mạch Subwoofer SiC và Boost SMPS GaN, mở Solder Mask hàn đính trực tiếp các thanh **Đồng nguyên khối (Solid Copper Busbar)** lên mặt PCB để gánh dòng xả >50 Ampe.

## XII. DỰ TOÁN CHI PHÍ & VẬT TƯ (BOM - BILL OF MATERIALS)
*Lưu ý: Dự toán được bóc tách theo từng Bo mạch (Module) để phục vụ lộ trình R&D nhiều năm. Mức giá quy đổi tương đối dựa trên báo giá của Mouser, Digi-Key, PCBWay và các đại lý Hi-End Audio toàn cầu (Cập nhật hệ thống Beryllium và Purifi mới nhất).*

### 1. HỆ THỐNG CỦ LOA (TRANSDUCERS) - *Trái tim âm học*
| STT | Hạng mục Vật tư | Số lượng | Đơn giá (VNĐ) | Thành tiền (VNĐ) | Ghi chú |
| :--- | :--- | :---: | :--- | :--- | :--- |
| 1.1 | Treble: BlieSMa T34B-4 (Beryllium) | 2 | 22.000.000 | 44.000.000 | Dải siêu âm vươn tới 40kHz |
| 1.2 | Mid: BlieSMa M74B-6 (Beryllium 3") | 2 | 24.000.000 | 48.000.000 | Tàng hình, tốc độ chớp nhoáng |
| 1.3 | Bass: PURIFI PTT5.25X04-NAA-05 (5.25")| 2 | 6.500.000 | 13.000.000 | Xmax 9.8mm, bạo lực vô song |
| 1.4 | Sub: Dayton Audio RSS265HE-22 (10") | 2 | 6.500.000 | 13.000.000 | DVC 800W RMS/củ |
| **I** | **TỔNG HỆ THỐNG CỦ LOA** | | | **118.000.000**| |

### 2. CHI PHÍ CHẾ TẠO CÁC BO MẠCH (PCBs & PCBA COMPONENTS) - *Linh hồn đẳng cấp*
*Đã bao gồm chi phí in mạch PCB Rogers RO4350B tại PCBWay và toàn bộ linh kiện cắm/dán.*
| STT | Tên Bo Mạch (Board / Module) | Số lượng | Đơn giá (VNĐ) | Thành tiền (VNĐ) | Phân tích linh kiện chính trên Bo mạch |
| :--- | :--- | :---: | :--- | :--- | :--- |
| 2.1 | **Bo mạch Treble (Module 1)**<br>*Ultra-Linear Aerospace BTL* | 2 Bo (L/R) | 8.500.000 | 17.000.000 | - PCB 6-Lớp Rogers<br>- 1x TPA3255, 8x Diode SiC<br>- 2x Sparkos SS3602 (Discrete Op-Amp)<br>- 10x Điện trở Vishay Z-Foil (0.005%)<br>- Cuộn cảm Air-Core + Tụ WIMA FKP2 |
| 2.2 | **Bo mạch Mid (Module 2)**<br>*Discrete Hybrid Class-A BTL* | 2 Bo (L/R) | 14.500.000 | 29.000.000 | - PCB 6-Lớp Rogers<br>- 1x TPA3255, 8x Diode SiC<br>- 2x Sparkos SS3602<br>- **Cuộn cảm lá đồng Mundorf CFC**<br>- **Tụ ngâm dầu (Mundorf/Duelund)**<br>- Điện trở Vishay Z-Foil |
| 2.3 | **Bo mạch Mid-Bass (Module 3)**<br>*Interleaved PBTL* | 2 Bo (L/R) | 7.500.000 | 15.000.000 | - PCB 6-Lớp Rogers<br>- **2x TPA3255 (Chế độ PBTL lệch pha)**<br>- Cuộn cảm kép lõi Nanocrystalline<br>- Tụ nguồn Bulk Rubycon ZLH |
| 2.4 | **Bo mạch Subwoofer (Module 4)**<br>*Composite SiC BTL* | 2 Bo (C1/C2)| 6.000.000 | 12.000.000 | - PCB 4-Lớp (Copper Pour & Busbar)<br>- 1x IRS2092S + **Sò SiC MOSFETs**<br>- Cảm biến dòng Hall Allegro ACS37002<br>- Mạch phanh Chopper + Trở sứ tản nhiệt |
| 2.5 | **Bo mạch Nâng Áp (Boost SMPS)**<br>*1MHz GaN Multiphase* | 1 Bo tổng | 12.000.000 | 12.000.000 | - PCB 4-Lớp Đồng dày (2oz - 4oz)<br>- **Transistor GaN (Gallium Nitride)**<br>- Biến áp phẳng (Planar Transformer) |
| 2.6 | **Bo mạch Nguồn Cách ly Tuyến tính**<br>*Active Ripple Eater & LDOs* | 1 Bo tổng | 6.500.000 | 6.500.000 | - MOSFET công suất chịu tải tĩnh<br>- Mảng LDO LT3045/LT3094 (0.8 µVrms)<br>- Biến áp xuyến bọc nhiễu cho GVDD |
| **II** | **TỔNG CHI PHÍ CHẾ TẠO BO MẠCH** | | | **91.500.000** | |

### 3. BỘ NÃO AI, DSP & ROBOTICS (AMR) - *Trí tuệ nhân tạo*
| STT | Hạng mục Vật tư | Số lượng | Đơn giá (VNĐ) | Thành tiền (VNĐ) | Ghi chú |
| :--- | :--- | :---: | :--- | :--- | :--- |
| 3.1 | **Mạch Bộ não Trung tâm AI** | 1 Bo | 13.500.000 | 13.500.000 | NVIDIA Jetson Orin Nano (8GB) |
| 3.2 | **Mạch Xử lý Âm thanh số (DSP Board)**| 1 Bo | 6.500.000 | 6.500.000 | ADAU1467 + XMOS XU208 + DAC ESS SABRE |
| 3.3 | Camera 3D Intel RealSense D435 + Lidar | Bộ | 12.000.000 | 12.000.000 | Đôi mắt AI Follow-Me & Tránh vật cản |
| 3.4 | **Mạch Điều khiển Động cơ (Motor Driver)**| 2 Bo | 3.500.000 | 7.000.000 | Mạch ODrive/VESC CAN Bus lái Hub Motor |
| 3.5 | Hub Motor BLDC 8" (Động cơ bánh xe) | 2 Cụm| 1.500.000 | 3.000.000 | Hệ dẫn động gầm Tank-Turn tải 150kg |
| 3.6 | Màn hình cảm ứng 14" + Kính cường lực | 1 | 3.000.000 | 3.000.000 | Giao diện điều khiển (UI) gập nóc |
| **III**| **TỔNG HỆ THỐNG AI, DSP & ROBOTICS**| | | **45.000.000** | |

### 4. NĂNG LƯỢNG, BẢO VỆ & KẾT NỐI - *Sức mạnh 4000W*
| STT | Hạng mục Vật tư | Số lượng | Đơn giá (VNĐ) | Thành tiền (VNĐ) | Ghi chú |
| :--- | :--- | :---: | :--- | :--- | :--- |
| 4.1 | Nguồn Mean Well RSP-2000-48 (2000W) | 2 | 8.500.000 | 17.000.000 | Cấp nguồn khi cắm điện lưới |
| 4.2 | Khối Pin Samsung 40T (48 Cell) + Kẽm | Bộ | 6.000.000 | 6.000.000 | Khối 12S4P xả dòng siêu cao (Tự pack) |
| 4.3 | **Mạch Quản lý Pin (BMS Board)** | 1 Bo | 2.500.000 | 2.500.000 | Mạch JK BMS 100A + Active Balancer |
| 4.4 | Dây dẫn, Jack Neutrik, Aviation Plug | Bộ | 8.500.000 | 8.500.000 | Dây đồng mạ bạc Teflon, đầu cắm mạ vàng|
| **IV** | **TỔNG NĂNG LƯỢNG & KẾT NỐI** | | | **34.000.000** | |

### 5. KHUNG VỎ CNC & HỆ THỐNG TẢN NHIỆT NƯỚC - *Cơ khí chính xác*
| STT | Hạng mục Vật tư | Số lượng | Đơn giá (VNĐ) | Thành tiền (VNĐ) | Ghi chú |
| :--- | :--- | :---: | :--- | :--- | :--- |
| 5.1 | Nhôm 6061-T6 + Phay CNC nguyên khối | Bộ | 35.000.000 | 35.000.000 | Vách 15mm, cơ cấu Spine Bracing Inox |
| 5.2 | Bơm Dual DDC + Block nước làm mát | Bộ | 12.000.000 | 12.000.000 | Custom Distro-plate, Block đồng tản IC |
| 5.3 | Radiator Đồng (240/280mm) + Quạt ARGB| 2+8 | 6.000.000 | 6.000.000 | Cấu hình Push-Pull áp suất tĩnh |
| 5.4 | Phụ liệu (Polyurea, Ống Hard-tube, Ốc) | Bộ | 5.000.000 | 5.000.000 | Xử lý âm học, chống rung, bịt kín |
| **V** | **TỔNG CƠ KHÍ & TẢN NHIỆT NƯỚC** | | | **58.000.000** | |

---

### TỔNG CỘNG CHI PHÍ DỰ KIẾN (GRAND TOTAL)
*   **I. Hệ thống củ loa (Transducers):** 118.000.000 VNĐ
*   **II. Chi phí chế tạo các Bo mạch (PCBA):** 91.500.000 VNĐ
*   **III. Hệ thống AI, DSP & Robotics:** 45.000.000 VNĐ
*   **IV. Năng lượng & Kết nối:** 34.000.000 VNĐ
*   **V. Cơ khí & Tản nhiệt nước:** 58.000.000 VNĐ
*   *Dự phòng phát sinh (R&D, Test cháy mạch, Thuế quan - 10%):* ~34.500.000 VNĐ

=> **TỔNG LƯỢNG VỐN ĐẦU TƯ DỰ KIẾN (CAPEX): ~381.000.000 VNĐ (Khoảng 15.200 USD)**
