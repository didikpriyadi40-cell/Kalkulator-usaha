# Kalkulator Usaha — proyek Android

Aplikasi offline sederhana untuk menghitung biaya bahan, total modal produksi, HPP per unit, omzet, laba, margin, harga impas, dan harga jual berdasarkan target laba. Data produk disimpan lokal pada perangkat melalui penyimpanan WebView.

## Status
Ini adalah proyek sumber Android, **bukan APK yang sudah dikompilasi atau diuji pada perangkat fisik**. APK debug dibuat melalui GitHub Actions.

## Isi proyek
- `app/` — kode Android dan aplikasi kalkulator offline.
- `.github/workflows/build-apk.yml` — proses otomatis membangun APK di GitHub.
- `PANDUAN_HP_ANDROID.md` — panduan mengunggah proyek dan mengunduh APK hanya dengan HP.

## Rumus
- Biaya bahan = harga kemasan × jumlah dipakai ÷ isi kemasan.
- Total modal = total biaya bahan + biaya produksi lainnya.
- HPP per unit = total modal ÷ jumlah hasil produksi.
- Laba total = (harga jual × jumlah hasil) − total modal.
- Harga jual target = HPP × (1 + target laba %).

Pastikan satuan isi kemasan dan pemakaian bahan konsisten (misalnya gram dengan gram). Biaya produksi lainnya diisi sebagai total untuk satu batch.

## Data
Produk tersimpan di penyimpanan lokal aplikasi. Menghapus data aplikasi atau mencopot pemasangan dapat menghapus data tersebut. Versi awal belum menyediakan ekspor/impor cadangan.
