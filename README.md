👕 Clothing Brand - Premium Fashion Store
Aplikasi e-commerce berbasis PHP (Native) sederhana yang memungkinkan pengguna untuk menjelajahi katalog produk, mengelola keranjang belanja, dan melakukan checkout transaksi menggunakan basis data berbasis file teks (.txt).

🚀 Cara Menjalankan Aplikasi
Ikuti langkah-langkah berikut untuk menjalankan aplikasi di lingkungan lokal Anda:

Persiapan Lingkungan:

Pastikan Anda telah menginstal web server lokal (seperti XAMPP, WampServer, atau Laragon).

Aplikasi ini memerlukan PHP versi 7.4 atau lebih baru.

Penempatan Folder:

Salin folder proyek ini ke dalam direktori server Anda (misalnya C:/xampp/htdocs/clothing-brand/).

Inisialisasi Sistem (Wajib):

Buka browser dan jalankan file installer untuk membuat folder data dan file yang diperlukan:

Plaintext

http://localhost/clothing-brand/init.php
Halaman ini akan otomatis membuat folder data/, receipts/, dan file-file pendukung lainnya.

Akses Aplikasi:

Halaman Utama: http://localhost/clothing-brand/index.php

Login Customer: http://localhost/clothing-brand/login.php

Setup/Reset: http://localhost/clothing-brand/init.php

📁 Struktur Program
Aplikasi ini menggunakan penyimpanan berbasis teks (Flat-file database) agar ringan dan mudah dipindahkan.

Plaintext

FINALSDATA/
├── 📁 admin/               # Panel administrasi (Manajemen stok & user)
├── 📁 assets/              # File statis (CSS, JS, dan Gambar produk)
├── 📁 data/                # Database berbasis teks (.txt)
│   ├── customers.txt       # Data akun customer
│   ├── products.txt        # Katalog & stok produk
│   ├── transactions.txt    # Rekap transaksi utama
│   └── KTP.txt             # Validasi data penduduk
├── 📁 receipts/            # Kumpulan struk belanja (format .txt)
├── index.php               # Halaman utama (Best Seller)
├── allproduct.php          # Katalog lengkap produk
├── cart.php                # Manajemen keranjang belanja
├── checkout.php            # Proses pembayaran & pembuatan struk
├── dashboard.php           # Profil & riwayat transaksi customer
├── login.php               # Halaman masuk customer
├── register.php            # Halaman pendaftaran
├── init.php                # Script setup/instalasi awal
└── logout.php              # Proses keluar sesi
📝 Contoh Penggunaan
1. Masuk Sebagai Customer
Aplikasi telah menyediakan data awal untuk pengujian. Anda dapat login menggunakan data dari data customer dan passwordnya.docx:

NIK: 3374010101950001

Password: Budi01011995

2. Berbelanja
Buka menu All Products.

Klik tombol Add to Cart pada produk yang diinginkan (contoh: MA-1 Bomber atau Jeans Slim Fit).

Klik menu Cart untuk melihat daftar belanja.

Klik Proceed to Checkout.

3. Pembayaran & Struk
Pilih metode pembayaran (Cash, Debit, E-Wallet, dll).

Klik Process Payment.

Setelah berhasil, sistem akan mengarahkan ke halaman sukses.

Anda dapat mengklik Download Receipt untuk mendapatkan struk fisik berformat teks seperti berikut:

Plaintext

================================================================================
                            CLOTHING BRAND
================================================================================
ID Transaksi   : TRX20250510...
Nama           : BUDI SANTOSO
TOTAL          : Rp 400.000
METODE BAYAR   : E-Wallet
================================================================================
4. Memantau Riwayat
Buka halaman Dashboard untuk melihat total pengeluaran Anda dan daftar seluruh transaksi yang pernah dilakukan sebelumnya.

🔐 Informasi Kredensial Admin
URL Login: admin/login_admin.php

Username: admin

Password: admin123

© 2025 Clothing Brand. Dibuat untuk tujuan pembelajaran manajemen data berbasis PHP.
