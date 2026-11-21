# Changelog

## 16.0-20261121

- Battery: the phone now reaches deep sleep. The kernel looked for chip
  firmware only in /lib/firmware, so every suspend attempt was aborted;
  standby drain is about half of what it was (measured ~1.3 %/h instead
  of ~2.9 %/h with the screen off)
- Web pages: images, logos and icons no longer disappear in the browser
  and other apps that show web content (WebView now rasterizes on the CPU
  on this GPU)
- Launcher: the app drawer follows Settings > Display > Style (dark with
  the Dark style, light with the Light style; the automatic styles still
  follow the wallpaper)

## 16.0-20261115 (first release)

Android 9 (LineageOS 16.0), Android security patch level 2022-01-05
(the last of LineageOS 16.0) plus later LineageOS 16.0 fixes.

Based on the exynos5420 team's device tree, kernel and Exynos 5422
hardware support, ported to Pie and fixed for daily use:

- RIL: calls, SMS, mobile data, USSD, SIM PIN, network type selection
  (3G/2G)
- Audio: earpiece, speaker, wired headset, Bluetooth (A2DP, HFP calls);
  call audio routed like the stock ROM; quiet and noisy microphone
  recordings fixed (video and voice recorder)
- Wi-Fi (2.4 and 5 GHz), hotspot, USB tethering; no more failed joins
  when the framework scanned during a connection
- Camera (photo, 1080p video), hardware video decoding and encoding;
  the camera no longer hangs on the second launch
- Fingerprint, heart rate sensor, IR blaster, hall sensor (flip cover),
  notification LED colours, GPS, off-mode charging, USB OTG
- Power profiles (power saving / balanced / performance), zram
- SELinux enforcing
- Built-in Updater (OTA) and GApps kept across updates
- Some time locations actualized, e.g. Kyiv
