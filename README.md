# Surface Pro 7 - macOS - OpenCore
---
OpenCore configuration for support macOS on Surface Pro 7


### Surface Specs
- Intel® Core™ i5-1035G4 Quad-Core
- 8 GB LPDDR4x RAM
- Intel® Iris™ Plus
- SSD **128 GB** (!??)


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
|  :heavy_exclamation_mark: |  Camera Front and Rear        |  **i heard that even by now there's no sign of camera working on linux, maybe already working on ubuntu, if's that correct please take the pr for me**           | 


### Install Notes
- For a better Wifi experience, use **itlwm** instead of **AirportItlwm** with [HeliPort](https://github.com/OpenIntelWireless/HeliPort) (as now there's a bug that prevent iServices work on Sonoma) (Simple enable/disable them in `config.plist`)
- For better trackpad support go to `System Settings -> Trackpad` and disable `Force click and haptic feedback`

### Secure Boot
If you want to boot without the anoing red bar with the lock icon you can try [this workaround](https://github.com/badstorm/surface-pro-7-opencore/blob/master/SecureBoot.With.Grub.md). *Thanks to @Xiashangning* 
