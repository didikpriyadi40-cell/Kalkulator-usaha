# Panduan membuat APK hanya dengan HP Android

> Perlu akun GitHub. APK belum tersedia sebelum langkah build selesai.

1. Unduh ZIP proyek ini, lalu ekstrak menggunakan aplikasi Files/File Manager.
2. Buka Chrome dan masuk ke https://github.com. Buat akun atau masuk.
3. Tekan tanda `+` → `New repository`. Beri nama `kalkulator-usaha`, pilih `Public` atau `Private`, lalu buat repository.
4. Di repository, pilih `Add file` → `Upload files`.
5. Dari folder hasil ekstrak `Kalkulator_Usaha_Android`, unggah **isi foldernya** (folder `app`, file `build.gradle`, `settings.gradle`, `gradle.properties`, `README.md`, `PANDUAN_HP_ANDROID.md`, dan folder tersembunyi `.github`). Jangan hanya mengunggah ZIP.
6. Pastikan `.github/workflows/build-apk.yml` ikut terunggah. Jika tidak terlihat, aktifkan opsi “tampilkan file tersembunyi” di File Manager, lalu unggah folder `.github` juga. GitHub versi HP kadang lebih mudah dipakai dengan Chrome → menu titik tiga → `Situs desktop`.
7. Setelah semua file dipilih, isi pesan commit bila diminta, lalu tekan `Commit changes`.
8. Buka tab `Actions` di repository. Pilih workflow `Build APK Kalkulator Usaha`. Jika belum berjalan otomatis, tekan `Run workflow` → `Run workflow`.
9. Tunggu sampai status selesai dengan tanda centang hijau. Buka proses build yang berhasil, gulir ke bagian `Artifacts`, lalu unduh `Kalkulator-Usaha-debug-APK`.
10. Ekstrak ZIP hasil unduhan. Instal file `app-debug.apk`. Jika Android meminta izin, izinkan aplikasi Files/Chrome memasang aplikasi dari sumber tersebut.

## Catatan
- GitHub Actions membangun APK debug untuk uji coba/pemasangan pribadi, bukan APK rilis Play Store.
- Bila build gagal, buka log langkah yang merah dan kirim tangkapan layar/pesan error agar bisa dibantu.
- Jangan bagikan kata sandi atau kode verifikasi GitHub kepada siapa pun.
