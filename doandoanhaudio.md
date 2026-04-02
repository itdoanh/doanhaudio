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


## X. HỆ THỐNG KHUẾCH ĐẠI ĐA DẢI (THE ULTIMATE AMPLIFICATION CORE)
**Định hướng:** Ultra High-End Active DSP 4-Way Loudspeaker System (Hệ thống loa 4 đường tiếng chủ động).  
**Kiến trúc cốt lõi:** Task Segregation (Phân rã nhiệm vụ) & Aerospace-Grade Discrete Components (Linh kiện rời cấp độ Hàng không vũ trụ). Không bắt một linh kiện làm nhiều việc. Ép các khối Silicon Class-D (TPA3255, IRS2092S) hoạt động trong một môi trường sinh tồn lý tưởng tuyệt đối.

---

## 1. MODULE 1 (TREBLE): BLIESMA T34A-4 - "ULTRA-LINEAR AEROSPACE BTL"
**Tính chất củ loa:** Độ nhạy 97dB, trở kháng Le = 3.8 Ohms phẳng, màng nhôm-magie cực cứng dao động tuyến tính vượt 35kHz.  
**Mục tiêu thiết kế:** Méo hài tổng (THD+N) < 0.001% ở 35kHz. Nền âm tĩnh lặng tuyệt đối như không cắm điện (Noise Floor < -125dB). Đáp tuyến phẳng $\pm$0.1dB bất chấp tải. Chặn đứng 100% nguyên nhân vật lý sinh méo hài bậc lẻ (H3, H5).

### 1.1. Phân rã Nguồn điện Chuyên biệt (Triple-Isolated Power Supply)
Tuyệt đối không dùng chung nguồn trực tiếp để tránh nhiễu chéo (Cross-modulation) từ dàn Subwoofer.
*   **PVDD (Nguồn động lực 48V):** Đi qua mạch **Active Ripple Eater (Discrete Capacitance Multiplier)** chạy bằng MOSFET công suất. Mạch này biến nguồn pin đang bị dao động thành nguồn DC phẳng tuyệt đối (Ripple ~ 0.000V). Ngay tại chân PVDD của TPA3255, hàn trực tiếp dải tụ gốm **Ultra-Low ESL MLCC** (đảo cực Reverse Geometry) để cung cấp dòng xả nano-giây, chặn đứng sụt áp thời gian chết (Dead-time voltage sag).
*   **GVDD & VDD (Nguồn Lái cực cổng 12V):** Cắt đứt hoàn toàn mạch hạ áp (Buck converter) nội bộ của TPA3255. Sử dụng module nguồn cách ly riêng, chạy qua tổ hợp **Dual LT3045 LDO (Nhiễu siêu thấp 0.8 µVrms)**. Nguồn 12V phẳng như gương này ép khối Gate-Driver nội bộ đóng/cắt Mosfet với sườn xung sắc lẹm và tàn bạo nhất.
*   **AVDD (Nguồn Logic 3.3V):** Lọc qua một tầng LT3045 riêng biệt, bảo vệ tuyệt đối lõi so sánh (Comparator) khỏi nhiễu kỹ thuật số.

### 1.2. Phân rã Tầng xử lý Tín hiệu (Instrumentation Discrete Architecture)
Thay thế hoàn toàn IC Op-Amp tích hợp bằng Kiến trúc 2 tầng Op-Amp rời (Discrete Op-Amp) chạy Pure Class-A:
1.  **Tầng Buffer Cách ly (Outside PFFB Loop):** Sử dụng Discrete Op-Amp nền tảng JFET (Vd: Sparkos Labs SS3602 hoặc Burson V6). Nhiệm vụ: Cách ly trở kháng với DSP, chuyển đổi tín hiệu vi sai với CMRR > 100dB. Tầng này nằm ngoài vòng lặp hồi tiếp để bảo toàn biên độ pha (Phase Margin).
2.  **Tầng Error Amplifier (Inside PFFB Loop):** Sử dụng Discrete Op-Amp siêu tốc độ (High Slew-rate Bipolar). Đóng vai trò là "Trạm thu" (Summing Node), so sánh tín hiệu sạch từ Buffer với tín hiệu hồi tiếp PFFB dội về từ cọc loa, bơm dòng sửa lỗi trực tiếp vào TPA3255. 
*   **DC-Servo Độc lập:** Dùng Op-Amp OPA2188 (Zero-drift) liên tục quét và ép DC Offset về 0.000V tại đầu vào, giữ màng loa BlieSMa ở đúng tâm vật lý.

### 1.3. Cấu hình Công suất & Mạng xuất âm (Output Stage)
*   **IC Khuếch đại:** Texas Instruments TPA3255 (Chế độ BTL Direct-Coupled). Ép xung (Fsw) đồng bộ Master/Slave Clock **600kHz** để đẩy nhiễu switching ra khỏi phổ âm thanh.
*   **Pseudo-GaN SiC Clamping (Đột phá chống méo bậc lẻ):** Kẹp 8 Diode Schottky **Silicon Carbide (SiC)** siêu tốc (Qrr=0) từ 4 chân Output xuống GND và lên PVDD. Mô phỏng sườn xung vuông vức của amply GaN, triệt tiêu tận gốc lực dội ngược từ diode nội sinh chậm chạp, bóp chết méo hài H3, H5 từ trong trứng nước.
*   **Mạng PFFB Vishay Z-Foil Cực Đoan:** Sử dụng 100% điện trở **Vishay Naked Z-Foil (sai số 0.005%, TCR 0.05ppm/°C)** cho mạng hồi tiếp. Đạt độ cân bằng vi sai hoàn hảo toán học, khóa chết sai số hệ thống mà không cần vòng lặp quá phức tạp.
*   **Bộ lọc LC (Load-Invariant 150kHz):** Cuộn cảm 5.0 µH (Lõi không khí Air-Core, dây Litz đồng) + Tụ WIMA FKP2 0.22 µF / 100V. Điểm cắt 150kHz giúp đáp tuyến 35kHz là một đường thẳng tắp.
*   **RF Termination Zobel Hàng Không:** Bỏ trở/tụ thường. Dùng điện trở **Caddock Thick-Film TO-220 (Non-Inductive)** kết hợp tụ **Silver Mica (Mica Bạc)**. Nhiệm vụ duy nhất: Hấp thụ 100% sóng siêu cao tần thành nhiệt lượng mà không sinh ra từ trường ký sinh (ESL = 0).

---

## 2. MODULE 2 (MIDRANGE): SCAN-SPEAK 10F/4424G00 - "DISCRETE HYBRID & ZERO-INERTIA BTL"
**Tính chất củ loa:** Màng siêu nhẹ (Mms = 2.8g), tốc độ chớp nhoáng nhưng cực kỳ nhạy cảm với méo từ trễ (Hysteresis) và méo giao điểm (Crossover distortion).  
**Mục tiêu thiết kế:** Trễ pha 0 độ (300Hz - 3kHz). Trung âm mang linh hồn Analog của amply Pure Class-A (dày dặn, mọng nước, bảo tồn H2 tự nhiên) nhưng sở hữu Damping Factor tàn bạo của amply xung để kiểm soát Back-EMF.

### 2.1. Nguồn điện & Tầng xử lý (Bảo tồn Nhạc tính)
*   **Nguồn Tam lập (Triple-Isolated):** Kế thừa 100% kiến trúc cách ly PVDD (Ripple Eater), GVDD và AVDD (LT3045) của dải Treble.
*   **Discrete Pre-Amp Đậm Đặc Nhạc Tính:** Sử dụng module Op-Amp Rời (Discrete) phân cực Pure Class-A tĩnh cao để đón tín hiệu. Sự hoàn hảo của linh kiện rời cấp nguồn bởi LDO LT3094/LT3045 giúp dải trung âm bảo tồn trọn vẹn các hài âm bậc chẵn (H2) tự nhiên sinh ra từ bản thu, tái tạo giọng ca sĩ lồi 3D (Holographic) đầy máu thịt.

### 2.2. Xử lý Công suất & Bộ lọc Ultra Hi-End
*   **IC Khuếch đại:** TPA3255 (Chế độ BTL). Tích hợp mạch **Pseudo-GaN SiC Clamping Diode** để gọt sạch mọi gai góc (méo bậc lẻ) gây chói gắt dải High-Mid.
*   **Bộ lọc LC (Không Méo Từ Trễ - 50kHz):** Nâng cấp cực đoan lên **Cuộn cảm Lá Đồng lõi không khí (Copper Foil Air-Core, Vd: Mundorf CFC)** 7.0 µH + **Tụ màng Bạc/Đồng ngâm dầu (Silver/Gold Oil Capacitor)** 1.0 µF. Vật liệu xa xỉ này bóp chết 100% méo từ trễ (Magnetic Hysteresis) trong lõi từ công nghiệp, giải phóng sân khấu âm thanh 3D siêu thực.
*   **Z-Foil On-Board Kelvin Sense PFFB:** Điểm lấy mẫu hồi tiếp lấy tại trạm xuất âm on-board, chạy vi sai bọc mass (Differential Stripline). Sử dụng điện trở **Vishay Naked Z-Foil (0.005%)**. Sự hoàn hảo toán học này khóa cứng thông số amply, bù trừ lực dội ngược (Back-EMF) của màng 10F một cách tàn nhẫn và chính xác nhất.
*   **RF Termination Zobel:** Caddock Non-Inductive (4.7Ω) + Silver Mica (0.1µF).

---

## 3. MODULE 3 (MID-BASS): KÉP 2 x B&C 5FG44 - "AEROSPACE INTERLEAVED PBTL"
**Tính chất củ loa:** Trở kháng 8 Ohms, Le = 0.8mH. Bị nhốt trong thùng nhôm nén kín tạo áp suất phản hồi cực lớn.  
**Mục tiêu thiết kế:** Damping Factor > 2000. Tiếng Kick-bass nhanh như chớp giật, đanh gọn, không có đuôi âm. Đẳng cấp độ sạch (THD) ngang hàng dải Treble.

### 3.1. Phân rã Nguồn điện & Kiến trúc Tín hiệu
*   **Nguồn Tam lập:** Áp dụng hệ thống cách ly PVDD, GVDD và AVDD để đảm bảo sườn xung PWM không gục ngã khi Bass đánh liên hồi. 
*   **Discrete Pre-Amp Class-A:** Tối đa hóa dải động (Dynamic Range) để bắt kịp những cú "Attack" (búng dây đàn, nện trống) chớp nhoáng nhất.

### 3.2. Công nghệ Hủy nhiễu Nội tại (Ripple Cancellation Output Stage)
*   **Kiến trúc Interleaved PBTL (BTL Song song Lệch pha):** Sử dụng 2 chip TPA3255 (Mỗi chip đánh 1 củ B&C ở chế độ PBTL). Can thiệp vào xung Clock nội bộ, ép 2 nửa cầu của PBTL **đóng/cắt lệch pha nhau chính xác 180 độ**. Khi gộp lại tại ngõ ra, sóng nhiễu (Ripple Current) của nhánh A và B tự động triệt tiêu lẫn nhau. Tần số băm xung biểu kiến đập vào màng loa B&C vọt lên **1.2 MHz**, xóa sổ hoàn toàn ứng suất nhiệt trên Voice Coil.
*   **Cuộn cảm Liên kết Từ tính (Bi-filar Coupled Nanocrystalline):** Hai nhánh dòng điện trước khi gộp lại sẽ đi qua một cuộn cảm kép quấn bằng dây dẹt (Flat-wire) trên cùng một lõi **Nanocrystalline (Vật liệu Hàng không - Vd: Vacuumschmelze)** trị số 15 µH / 30A. Sự liên kết từ tính (Magnetic Coupling) ép dòng điện 2 nhánh chia sẻ hoàn hảo 50/50, chống bão hòa từ (Saturation) tuyệt đối dù Peak giật lên 30 Ampe.
*   **PBTL Z-Foil PFFB Topology:** Hồi tiếp vi sai từ trạm ngõ ra Summing Node, dùng điện trở Z-Foil để ép nội trở amply về sát 0 Ohm. Tuyệt đối KHÔNG dùng Zobel lớn (bỏ mạch 22µF) để tránh cộng hưởng RF gây cháy trở.
*   **Tụ Nguồn Bạo Chúa:** Phủ đồng nguyên khối Copper Pour sát chân PVDD. Tích hợp tổ hợp tụ Low-ESR Rubycon ZLH + Gốm MLCC cực thấp ESL.

---

## 4. MODULE 4 (SUBWOOFER): DAYTON RSS265HE-22 - "COMPOSITE GaN & PNEUMATIC OVERDRIVE"
**Tính chất củ loa:** DVC (2 Coil x 2 Ohms). RMS 800W, Peak 1600W. Hoạt động như một lò xo khí nén phi tuyến tính khổng lồ (Buồng nén 32L).  
**Mục tiêu thiết kế:** Vắt kiệt 1600W RMS. THD < 0.005% ở 100Hz. Kiểm soát độc đoán lực đẩy/hút bất đối xứng bằng AI, kết hợp cảm biến không tổn hao và hệ thống phanh động.

### 4.1. Mạch Nâng Áp (1MHz GaN MULTIPHASE BOOST)
*   **Nhiệm vụ:** Biến 48V DC thành "Khối bê tông điện áp" **±75V DC** không thể lay chuyển.
*   **Công nghệ Gallium Nitride (GaN):** Thay thế toàn bộ MOSFET Silicon bằng **GaN FETs** thế hệ mới nhất. Nhờ đặc tính Zero Qrr, tần số nâng áp đa pha (Interleaved 4-Phase) chạy biến áp phẳng (Planar Transformer) được ép lên mức **1 MHz**. Mạch phản ứng với sụt áp trong 1 micro-giây, cung cấp dòng xả peak >50A tức thời cho củ Sub. Lọc Pi (π-Filter) chặn đứng nhiễu cao tần ra ngõ ra.

### 4.2. Khoang Khuếch đại Cơ bắp & Trí tuệ Nhân tạo
*   **Kiến trúc Composite SiC (Mô phỏng NCORE):**
    *   *Trái tim sức mạnh:* IC Driver **IRS2092S** kết hợp tầng đệm BJT Totem-Pole lái dàn Sò công suất **SiC MOSFET (Wolfspeed)**. Tốc độ đóng cắt của SiC chớp nhoáng, triệt tiêu thời gian chết và méo xuyên điều chế dải cực trầm. Cấu hình Dual-Mono: 800W RMS/Coil.
    *   *Bộ não Composite:* Để phá vỡ giới hạn độ méo 0.05% của IRS2092S, khối công suất 1600W SiC này được "nhốt" vào vòng lặp hồi tiếp tổng (Global Feedback) của một **Discrete Op-Amp Class-A (Sparkos)**. Op-Amp ngoài cùng sẽ giám sát và ép khối công suất tuân thủ kỷ luật tuyến tính tuyệt đối (THD < 0.001%).
*   **Cảm Biến Dòng Điện Hàng Không (Zero-Loss Hall-Effect):** Để AI thực hiện tính năng *Asymmetric Pneumatic Overdrive* (Dẫn động khí nén bất đối xứng), DSP cần đọc chính xác dòng điện. Thay vì dùng điện trở Shunt làm tụt Damping Factor, dây loa Sub được luồn qua **Cảm biến từ trường hiệu ứng Hall (Vd: Allegro ACS37002)**. DSP nhận dữ liệu dòng điện Peak 50A tính bằng Micro-giây với điện trở chèn vào dây loa là **0.0000 Ohm**.
*   **Active Brake Chopper (Hệ thống Phanh Điện Trở Động - Chống nổ tụ):** Khi AI hãm màng loa (Electromagnetic Braking), động năng dội ngược sinh ra hiệu ứng Bus Pumping. Nếu điện áp rail dội lên vượt ngưỡng an toàn (Vd: 82V), mạch Chopper chạy bằng MOSFET độc lập lập tức mở van, xả toàn bộ động năng này vào **Khối điện trở Sứ công suất cao (Braking Resistor Bank) ngâm trong khối Tản nhiệt nước**. Tính năng AI bạo lực này giờ đây được bảo vệ an toàn tuyệt đối.

---

## 5. QUY CHUẨN THIẾT KẾ PCB BẮT BUỘC (AEROSPACE ROUTING & GROUNDING)
Để những linh kiện tiền tỷ trên không trở thành đống rác điện tử do nhiễu chéo (Crosstalk) và bức xạ RF, cấu trúc bo mạch in (PCB) phải tuân thủ kỷ luật hàng không:
1.  **Vật liệu & Kiến trúc 6 Lớp (6-Layer Rogers):** Đặt in mạch tại PCBWay với cấu trúc 6 lớp. Sử dụng vật liệu lõi **Rogers RO4350B** (cấp độ 5G/Radar) để có suy hao điện môi thấp nhất cho tần số băm xung 600kHz - 1.2MHz.
2.  **Đường truyền Vi Ba (Microwave Routing) cho PFFB:** Tại các module Treble/Mid/Bass, tín hiệu hồi tiếp PFFB đi theo chuẩn đường truyền vi sai (Differential Stripline) bọc mass. Đường mạch này chạy ngầm ở Layer 3 và Layer 4 thông qua Via mù/ngầm (Blind/Buried Vias), được kẹp giữa 2 lớp Ground Plane khổng lồ để cách ly tuyệt đối khỏi bức xạ từ khối nguồn 4000W.
3.  **Multi-Tier Star Grounding (Mass Hình Sao Đa Tầng):** Mass tín hiệu (Analog GND), Mass số (Digital GND) và Mass công suất (Power GND) phân bổ trên các Layer riêng biệt. Chúng chỉ được phép giao nhau tại MỘT ĐIỂM DUY NHẤT (Ngõ âm của cực Pin 48V) hoặc qua các hạt Ferrite Bead chịu dòng cao để bóp chết vòng lặp nhiễu (Ground Loop).
4.  **Solid Copper Busbar (Thanh cái dẫn dòng):** Trên mạch Subwoofer SiC và Boost SMPS GaN, tuyệt đối không dùng trace đồng in sẵn để gánh dòng 50A. Các đường ±75V và đường xuất âm IRS2092S phải được mở Solder Mask, hàn đính trực tiếp các thanh **Đồng nguyên khối (Solid Copper Busbar) dập máy** lên mặt PCB.

## XI. DỰ TOÁN CHI PHÍ & VẬT TƯ (BOM - BILL OF MATERIALS)
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
