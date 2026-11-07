# SonicShield — Powered by Ridi

Prototype Android Studio untuk Samsung Galaxy A16 / Android 16 dan pengujian TWS A9 Pro.

## Status versi 0.1.0
- UI tiga mode: ANC, Transparency, Off.
- Branding Powered by Ridi.
- Pemeriksaan Bluetooth dan daftar perangkat yang terdaftar/terlihat.
- Permintaan izin mikrofon dan Bluetooth.
- Belum mengirim perintah ANC/Transparency ke A9 Pro.
- Belum melakukan pemrosesan anti-noise atau ANC akustik.

## Mengapa kontrol ANC belum aktif?
Android tidak memiliki API universal untuk mengubah mode ANC pada semua TWS. A9 Pro mungkin menggunakan protokol vendor khusus atau kontrol lokal dari charging case. Protokolnya harus diidentifikasi dan diuji sebelum tombol dapat mengubah mode perangkat secara nyata.

Mikrofon TWS juga tidak otomatis tersedia untuk aplikasi. Profil Bluetooth HFP/SCO dan routing audio bergantung pada implementasi Android serta firmware TWS. Aplikasi ini tidak membuat anti-noise untuk diputar ke telinga karena latensi Bluetooth dapat membuat hasil tidak sinkron dan tidak aman.

## Build
1. Buka folder ini melalui Android Studio versi terbaru.
2. Gunakan JDK 17.
3. Sync Gradle.
4. Build > Build APK(s).

Jika Android Studio meminta Android SDK Platform 35, instal melalui SDK Manager.
