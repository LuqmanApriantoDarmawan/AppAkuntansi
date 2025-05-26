# 🏪 Aplikasi Akuntansi Toko Modern

Aplikasi desktop untuk manajemen akuntansi toko modern dengan antarmuka grafis yang intuitif dan fitur lengkap.  
Dibangun menggunakan **Python**, **PyQt5**, dan **MySQL**, aplikasi ini dirancang untuk memudahkan pengelolaan produk, transaksi, dan laporan keuangan.

---

## 🌟 Fitur Unggulan

### 📦 Manajemen Produk
- ✅ Tambah, edit, dan hapus produk
- 📊 Menampilkan stok produk secara real-time
- 🔍 Pencarian produk cepat dan efisien

### 💰 Manajemen Transaksi
- 🧾 Mencatat transaksi penjualan
- 📅 Filter transaksi berdasarkan periode waktu
- 📈 Visualisasi riwayat transaksi

### 📊 Laporan Keuangan
- 📉 Grafik interaktif untuk laporan laba rugi
- 🔢 Analisis keuangan otomatis
- 🗓️ Laporan keuangan berdasarkan periode yang dapat disesuaikan

### 📤 Ekspor Data
- 📄 Ekspor laporan ke format Excel (.xlsx)
- 🖨️ Ekspor laporan ke format PDF profesional
- 🖼️ Termasuk grafik dalam hasil ekspor

---

## 🛠️ Teknologi

| Komponen       | Teknologi     |
|----------------|----------------|
| **Frontend**   | PyQt5          |
| **Backend**    | Python 3.8+    |
| **Database**   | MySQL          |
| **Visualisasi**| Matplotlib     |
| **Ekspor Excel**| OpenPyXL      |
| **Ekspor PDF** | FPDF           |

---

## 🚀 Instalasi

### 📦 Prasyarat
- Python 3.8 atau lebih baru
- MySQL Server
- Git (opsional)

### 🔧 Langkah-langkah
1. Clone repositori ini:
   ```bash
   git clone https://github.com/Jiepra/Akuntasi_App.git
   cd Akuntasi_App
2. Install dependensi Python:
   ```bash
   pip install -r requirements.txt
3. Setup database:
   ```bash
   Buat database MySQL bernama akuntansi
   Jalankan skema SQL yang disediakan
4. Konfigurasi koneksi:
   ```bash
   Edit DB_CONFIG di admin_app.py sesuai setting MySQL Anda.
6. Jalankan aplikasi:
   ```bash
   python admin_app.py

   python client_app.py

---

## 🏗️ Struktur Database

### 📑 Tabel: `produk`
| Kolom        | Tipe Data     | Keterangan              |
|--------------|---------------|--------------------------|
| `id`         | INT (PK, AI)  | ID unik produk           |
| `kode`       | VARCHAR(20)   | Kode barang              |
| `nama`       | VARCHAR(100)  | Nama produk              |
| `harga_beli` | INT           | Harga beli               |
| `harga_jual` | INT           | Harga jual               |
| `stok`       | INT           | Jumlah stok tersedia     |

### 📑 Tabel: `transaksi`
| Kolom          | Tipe Data     | Keterangan                    |
|----------------|---------------|--------------------------------|
| `id`           | INT (PK, AI)  | ID transaksi                   |
| `tanggal`      | DATE          | Tanggal transaksi              |
| `kode_produk`  | VARCHAR(20)   | Kode produk                    |
| `jumlah`       | INT           | Jumlah barang terjual          |
| `total_harga`  | INT           | Total harga dari transaksi     |

> **Catatan**: Anda dapat menambahkan tabel `pengguna` atau `akun` jika aplikasi dikembangkan lebih lanjut dengan sistem login.

---

## 📜 Lisensi
Proyek ini dilisensikan di bawah MIT License.

© 2025 Jiepra. Dibuat dengan ❤️ untuk manajemen toko modern.
