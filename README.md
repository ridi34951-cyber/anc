## Build APK otomatis lewat GitHub Actions

1. Buat repository GitHub baru.
2. Upload seluruh isi folder proyek ini ke root repository (pastikan folder `.github/workflows/` ikut ter-upload).
3. Buka tab **Actions** pada repository.
4. Pilih workflow **SonicShield Android Build**.
5. Tekan **Run workflow** (atau push ke branch `main`/`master`).
6. Tunggu sampai job selesai dengan tanda hijau.
7. Buka hasil run, bagian **Artifacts**, lalu unduh `SonicShield-debug-apk`.

Workflow membangun APK debug dengan JDK 17, Gradle 8.11.1, dan Android SDK 35. File APK diunggah sebagai artifact GitHub Actions selama 14 hari.

Catatan: workflow ini hanya membangun APK debug dari source yang ada. Kontrol ANC perangkat belum terimplementasi karena protokol vendor A9 Pro belum diidentifikasi.
