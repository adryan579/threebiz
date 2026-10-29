# ThreeBiz (Mthree Business Suite)

Sistem Administrasi & Keuangan Operasional Perusahaan — aplikasi desktop (Python + Tkinter)
untuk Request Form, Cash Advance, Reimbursement, Expense Accounts, Tunjangan Bahan Bakar,
dan Laporan Bulanan.

Dikembangkan oleh **Chameleon** — PT. Mahira Mitra Mandiri.

## Unduh

Ambil berkas terbaru di <https://github.com/adryan579/threebiz/releases/latest>

| Berkas | Untuk |
| --- | --- |
| `ThreeBiz-Setup-<versi>-clean.exe` | dipasang lewat installer (data di `%LOCALAPPDATA%\ThreeBiz\data`) |
| `ThreeBiz-Portable-<versi>.zip` | diekstrak ke folder mana saja (data di folder `data` di samping exe) |

Keduanya dibungkus tanpa database. Jangan menjalankan berkas setup tanpa akhiran `-clean`
dari sumber tidak resmi: varian itu berisi salinan data milik pembuatnya.

## Pembaruan otomatis

Sejak **v0.1.23** aplikasi memeriksa rilis terbaru di halaman Releases ini setiap kali dibuka.
Bila ada versi yang lebih baru, muncul popup **Update wajib**; berkas rilis diunduh ke folder
sementara, diverifikasi terhadap sidecar `.sha256`, dipasang oleh skrip bantu, lalu aplikasi
dibuka kembali. Folder data tidak pernah ditimpa. Tanpa koneksi internet pengecekan dilewatkan
dan aplikasi tetap berjalan seperti biasa.

## Rilis

Rilis diterbitkan dari folder build pengembang dengan `python _publish_release.py` (butuh
`GITHUB_TOKEN`). Nama berkas aset harus tetap `ThreeBiz-Setup-<versi>-clean.exe` dan
`ThreeBiz-Portable-<versi>.zip`, masing-masing dilengkapi `<nama>.sha256`, agar dikenali updater.

© 2026 PT. Mahira Mitra Mandiri. All rights reserved.
