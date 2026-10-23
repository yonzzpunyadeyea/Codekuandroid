# CodeKu — Aplikasi Belajar Coding Android

CodeKu adalah aplikasi Android berbasis WebView dengan tema dark mode navy. Fitur:
- Materi dasar Python, HTML, CSS, JavaScript, plus pengenalan Java, C++, SQL, dan Git.
- 12 pelajaran ringkas dengan contoh kode dan penjelasan.
- Editor HTML/JavaScript lokal; HTML dibuka sebagai halaman, JavaScript menampilkan console.log.
- Eksekusi Python online menggunakan Piston API (butuh internet; layanan pihak ketiga).
- Kuis, XP, dan progres yang tersimpan secara lokal.
- Tidak perlu akun.

## Cara membangun APK
1. Instal **Android Studio** di komputer/laptop.
2. Ekstrak ZIP ini.
3. Android Studio → **Open** → pilih folder `CodeKuAndroid` (folder yang berisi `settings.gradle`).
4. Tunggu Gradle Sync. Pastikan Android SDK Platform 35 tersedia; bila diminta, instal.
5. Pilih **Build → Build Bundle(s) / APK(s) → Build APK(s)**.
6. APK debug akan tersedia di `app/build/outputs/apk/debug/app-debug.apk`.
7. Untuk memasang di HP, pindahkan APK ke Android, buka file, lalu izinkan pemasangan dari sumber tersebut bila diminta.

## Cara mencoba
Jalankan aplikasi melalui tombol Run di Android Studio pada emulator atau perangkat Android yang terhubung lewat USB debugging.

## Catatan penting
- Paket ini adalah **kode sumber proyek Android**, bukan APK yang sudah dikompilasi. APK perlu dibangun melalui Android Studio.
- Python dijalankan melalui internet ke `https://emkc.org/api/v2/piston/execute`; jika layanan sedang tidak tersedia, Python tidak akan berjalan.
- Jangan mengirim kata sandi, token, atau data pribadi ke editor maupun layanan eksekusi online.
- Materi dan editor dasar tetap tersedia offline. Tidak ada backend akun/cloud.
