# Uangku PWA — aplikasi keuangan pribadi

Aplikasi web progresif (PWA) berbahasa Indonesia untuk mencatat pemasukan, pengeluaran, transfer antar akun, saldo, laporan rentang tanggal, perbandingan periode, kategori, dan backup JSON.

## Terbitkan gratis dengan GitHub Pages (tanpa software lokal)

1. Buat repository baru di GitHub. Nama contoh: `uangku-pwa`.
2. Jika ingin memakai GitHub Pages gratis, pilih **Public**. Jangan simpan data keuangan dalam repository.
3. Unggah `index.html`, `manifest.webmanifest`, `sw.js`, dan `icon.svg` ke root repository melalui tombol **Add file → Upload files** pada situs GitHub.
4. Buka **Settings → Pages**.
5. Pada **Build and deployment**, pilih **Deploy from a branch**, branch `main`, folder `/(root)`, lalu **Save**.
6. Tunggu beberapa menit. Alamat biasanya `https://USERNAME.github.io/uangku-pwa/`.
7. Buka alamat tersebut melalui Chrome Android. Pilih menu ⋮ → **Tambahkan ke layar utama** atau **Install app**.

## Catatan privasi dan data

- Data transaksi disimpan pada `localStorage` browser di perangkat yang digunakan.
- Data tidak dikirim ke GitHub atau layanan cloud oleh kode aplikasi ini.
- Repository publik hanya berisi kode, bukan transaksi lokal.
- Ekspor backup JSON secara rutin. Menghapus data situs/browser dapat menghapus transaksi.
- Untuk memindahkan data, ekspor JSON dari perangkat lama, lalu pulihkan di perangkat baru.

## Perilaku periode

Periode gajian dihitung dari tanggal 25 sampai tanggal 24 berikutnya, berdasarkan tanggal hari ini. Laporan tanggal khusus dan perbandingan beberapa rentang tersedia.
