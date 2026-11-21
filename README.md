# STAR SEAFOOD Android wrapper

Project Android WebView yang memuat website STAR SEAFOOD secara lokal (asset HTML), dengan icon dan nama aplikasi.

## Cara menghasilkan APK dengan GitHub Actions (mudah, tanpa PC Android Studio)
1. Buat repository GitHub baru, misalnya `star-seafood-apk`.
2. Upload seluruh isi folder project ini ke repository (pastikan folder `.github/workflows` ikut terupload).
3. Buka tab **Actions** di repository. Jika diminta, aktifkan Actions.
4. Workflow **Build STAR SEAFOOD APK** akan berjalan setelah push. Jika tidak, pilih workflow lalu **Run workflow**.
5. Setelah selesai (status hijau), buka hasil workflow dan unduh artifact **STAR-SEAFOOD-APK**.
6. Ekstrak ZIP artifact, lalu instal `app-debug.apk` di HP Android. Jika diminta, izinkan instalasi dari sumber tersebut.

## Build dengan Android Studio
Buka folder project ini di Android Studio, lalu pilih Build > Build APK(s). APK debug berada di `app/build/outputs/apk/debug/app-debug.apk`.

Catatan: file APK belum dikompilasi di lingkungan ini karena Android SDK/Gradle tidak tersedia. Workflow GitHub disiapkan untuk membangunnya secara otomatis.
