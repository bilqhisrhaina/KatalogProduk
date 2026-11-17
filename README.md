# 🛍️ Aplikasi Katalog Produk

Aplikasi **Katalog Produk** berbasis JavaFX untuk mengelola data produk secara interaktif dengan penyimpanan permanen menggunakan database **SQLite** (`katalog.db`).

Project ini dikembangkan untuk memenuhi tugas **Pengantar JavaFX GUI - Level 3** dengan menerapkan arsitektur pemisahan *Model*, *Controller*, *Repository*, dan koneksi *Database* (CRUD lengkap).

## ✨ Fitur Aplikasi

- **Tambah Produk (Create):** Form input untuk menambahkan produk baru meliputi **Nama produk**, **Harga (Rp)**, dan pemilihan gambar melalui dropdown **Foto contoh** (`roti.png`, `kopi.png`, dll.) dengan tombol **Simpan**.
- **Tampilan Katalog Kartu (Read):** Menampilkan daftar produk tersimpan secara dinamis dalam bentuk kartu (*card*) visual lengkap dengan gambar produk, nama, harga, **ID** produk, serta penghitung **Jumlah produk** otomatis.
- **Edit Produk (Update):** Tombol **Edit** pada setiap kartu produk untuk memuat kembali data produk ke form dan memperbarui informasi di database.
- **Hapus Produk (Delete):** Tombol **Hapus** pada setiap kartu produk untuk menghapus data produk dari tampilan katalog sekaligus dari database SQLite.
- **Validasi Input:** Memastikan nama produk tidak kosong dan harga yang dimasukkan berupa angka yang valid sebelum disimpan ke database.
## Tampilan
<img width="751" height="497" alt="image" src="https://github.com/user-attachments/assets/839d89a8-853d-4b9f-a9c0-67cc936ebb99" />


## 🚀 Tata Cara Menjalankan Aplikasi (Run)

Aplikasi ini menggunakan Maven dan SQLite. Untuk membuka dan menjalankannya melalui **Apache NetBeans**:
1. Buka aplikasi **Apache NetBeans**, lalu buka *project* `KatalogProduk` ini (*File > Open Project*).
2. Tunggu hingga NetBeans selesai memuat seluruh *dependency* Maven (JavaFX dan SQLite JDBC).
3. Klik kanan pada nama *project* `KatalogProduk` di panel kiri, lalu pilih **Run Maven** -> **Goals...**
4. Pada kolom *Goals* yang muncul, ketikkan perintah berikut lalu klik **OK**:
   ```text
   clean javafx:run
   
