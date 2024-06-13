# Surface Pro 7 - macOS - OpenCore
---
OpenCore configuration for support macOS on Surface Pro 7

Cấu hình OpenCore hỗ trợ macOS cho Surface Pro 7


### Surface Specs
- Intel® Core™ i5-1035G4 Quad-Core
- 8 GB LPDDR4x RAM
- Intel® Iris™ Plus
- SSD **128 GB** (!??)


### Status
### Tình trạng
|  Status             |         Feature                 |            Note                      |
|---------------------|---------------------------------|--------------------------------------|
|  :white_check_mark: |  Graphic Acceleration          |  QE/CI works |
|  :white_check_mark: |  Wifi & Bluetooth              |  With [OpenIntelWireless](https://github.com/OpenIntelWireless/itlwm) |
|  :white_check_mark: |  Type Cover  (keyboard/mouse)  |  With RHUB and [BigSurface](https://github.com/Xiashangning/BigSurface)|                             
|  :white_check_mark: |  Audio                         |  With AppleALC   |
|  :white_check_mark: |  Battery Status          |  With [BigSurface](https://github.com/Xiashangning/BigSurface)                 | 
|  :white_check_mark: |  Touch & Stylus          |  With [BigSurface](https://github.com/Xiashangning/BigSurface). You need to manualy insall [IPTSDaemon](https://github.com/Xiashangning/IPTSDaemon)                | 
|                     |                                |                   |
|  :heavy_exclamation_mark: |  Camera Front and Rear        |  **Lack of driver**           | 


### Install Notes
- For a better Wifi experience, use **itlwm** instead of **AirportItlwm** if you don't mind about continuity features (quite useless) (edit the info.plist inside kext or using with [HeliPort](https://github.com/OpenIntelWireless/HeliPort)) (Simple enable/disable them in `config.plist`)
- Để có trải nghiệm Wifi tốt hơn, dùng **itlwm** thay vì **AirportItlwm** nếu bạn không quan tâm về tính năng thông suốt (vô dụng vc) (sửa info.plist bên trong kext hoặc dùng với [HeliPort](https://github.com/OpenIntelWireless/HeliPort)) (Chỉ cần enable/disable trong `config.plist`)

* `(as now there's a bug prevent iServices work on Sonoma/Sequoia, no AirportItlwm.kext version has been compiled for Sequoia yet)`
* `(đang có bug nên iService không dùng được trên Sonoma/Sequoia, chưa có phiên bản AirportItlwm.kext biên dịch cho Sequoia)`


- For better trackpad support go to `System Settings -> Trackpad` and disable `Force click and haptic feedback`
- Để trackpad tốt hơn thì vào `Cài đặt hệ thống -> Bàn di chuột ` và tắt `Bấm mạnh và phản hồi cảm ứng`

### Secure Boot
If you want to boot without the anoing red bar with the lock icon you can try [this workaround](https://github.com/badstorm/surface-pro-7-opencore/blob/master/SecureBoot.With.Grub.md). *Thanks to @Xiashangning* 
Nếu bạn muốn boot mà không có cái ổ khoá với cái thanh đỏ (khó chịu) thì có thể thử [cách này](https://github.com/badstorm/surface-pro-7-opencore/blob/master/SecureBoot.With.Grub.md). *Xin cảm ơn @Xiashangning* 

