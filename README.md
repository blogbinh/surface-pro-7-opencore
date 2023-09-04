# Surface Pro 7 - macOS - OpenCore
---
OpenCore configuration for support macOS on Surface Pro 7

> :warning: **Limited support**: I switched from Surface Pro 7 to Surface Pro X so I cannot test anymore. Feel free to send me PR so i can update the repo and the releases

### Thông số của Surface Pro 7:*
### Surface Pro 7 Specs:*
|                               |  Cấu hình thấp hơn (Lower Specs)     |   Cấu hình cao hơn (Higer Specs)             | Cấu hình cao nhất |
|-------------------------------|--------------------------------------|----------------------------------------------|-------------------|
|         **CPU**               |   Intel® Core™ i3-1005G1 Dual-core   |   Intel® Core™ i5-1035G4 Quad-core           | Intel® Core™ i5-1055G7 Quad-core 
|         **iGPU**              |     Intel® UHD Graphics 615          |                  <<                          |
|         **RAM**               |           4/8GB LPDDR3               |               8GB LPDDR3                     |
|  **Ổ lưu trữ / Storage**      |      64GB eMMC**, 128GB SSD          |               128GB SSD                      |
|         **Audio**             |              ALC(298)???             |                  <<                          |
| **Wifi + Bluetooth**          |   Intel® Wifi6 AX2??, Bluetooth 5.0  |                  <<                          |
|**Khe đọc thẻ nhớ/Card Reader**| Realtek PCI-E Card Reader, 152D:1237 |                  <<                          |
|**Cam Trước&Sau / Front&Rear Cam**|Intel(R) AVStream Camera 2500, ISP Interface, 8086:591c, 8 MPix/5 MPix|     <<    | 
| **Type Cover & Trackpad**     |Microsoft Type Cover, 045E:096F|                                      <<             |
|**Màn hình / Display**      |10.50 inch 3:2, 1920 x 1280 pixel 220 PPI, Hỗ trợ cảm ứng 10 điểm / 10-Point Capative|<<|
|      **Pin/Battery**          |26.81Wh 7.66v 3500mAh|            <<                                                 |


### Status
|  Status             |         Feature                 |            Note                      |
|---------------------|---------------------------------|--------------------------------------|
|  :white_check_mark: |  Graphic Acceleration          |  QE/CI works |
|  :white_check_mark: |  Wifi & Bluetooth              |  With [OpenIntelWireless](https://github.com/OpenIntelWireless/itlwm) |
|  :white_check_mark: |  Type Cover  (keyboard/mouse)  |  With RHUB and [BigSurface](https://github.com/Xiashangning/BigSurface)|                             
|  :white_check_mark: |  Audio                         |  With AppleALC   |
|  :white_check_mark: |  Battery Status          |  With [BigSurface](https://github.com/Xiashangning/BigSurface)                 | 
|  :white_check_mark: |  Touch & Stylus          |  With [BigSurface](https://github.com/Xiashangning/BigSurface). You need to manualy insall [IPTSDaemon](https://github.com/Xiashangning/IPTSDaemon)                | 
|                     |                                |                   |
|  :heavy_exclamation_mark: |  Camera Front and Rear        |                   | 


### Install Notes
- For a better Wifi experience, use **itlwm** instead of **AirportItlwm** with [HeliPort](https://github.com/OpenIntelWireless/HeliPort) (Simple enable/disable them in `config.plist`)
- For better trackpad support go to `System Preferences -> Trackpad` and disable `Force click and haptic feedback`

### Secure Boot
If you want to boot without the anoing red bar with the lock icon you can try [this workaround](https://github.com/badstorm/surface-pro-7-opencore/blob/master/SecureBoot.With.Grub.md). *Thanks to @Xiashangning* 
