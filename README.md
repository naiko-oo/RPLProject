# ♻️ Bank Sampah Digital

> **Sistem Informasi Pengelolaan & Pencatatan Transaksi Bank Sampah Berbasis Web untuk Lingkungan RT/RW**

---

## 📌 Ringkasan Proyek

Banyak pengelola Bank Sampah di tingkat RT/RW masih mengandalkan pencatatan manual menggunakan buku besar. Hal ini sering menimbulkan risiko kesalahan manusia *(human error)*, keterbatasan transparansi bagi warga, serta lambatnya penyusunan laporan periodik.

**Bank Sampah Digital** hadir untuk mendigitalkan seluruh proses bisnis pengelolaan sampah—mulai dari pencatatan setoran, konversi berat sampah menjadi saldo tabungan, hingga rekapitulasi laporan secara otomatis.

---

## 🎯 Target Pengguna & Manfaat

| Peran | Profil Pengguna | Manfaat Utama |
| :--- | :--- | :--- |
| 🧑‍💼 **Pengurus (Admin)** | Pengurus RT/RW atau pengelola bank sampah setempat. | Mempercepat input setoran, meminimalisir kesalahan hitung, dan menyusun laporan bulanan secara otomatis. |
| 👥 **Nasabah (Warga)** | Warga lingkungan RT/RW yang memilah sampah rumah tangga. | Transparansi saldo tabungan dan riwayat setoran yang dapat diakses secara *real-time*. |

---

## ✨ Fitur Inti *(Core Features)*

- 🔐 **Autentikasi & Hak Akses:** Sistem *login* multi-role terpisah untuk Admin dan Nasabah.
- 🏷️ **Manajemen Kategori Sampah (CRUD):** Pengaturan jenis sampah (Plastik, Kertas, Logam, dll) beserta harga per kg.
- 👤 **Manajemen Data Nasabah (CRUD):** Pendaftaran dan pengelolaan data anggota/warga.
- ⚖️ **Pencatatan Setoran Sampah:** Kalkulasi otomatis nominal saldo berdasarkan berat ($kg$) dan kategori sampah.
- 💸 **Pencairan Saldo:** Fitur penarikan saldo tabungan sampah nasabah oleh pengurus.
- 📊 **Dashboard & Riwayat Transaksi:** Ringkasan saldo dan log transaksi terkini bagi nasabah.
- 📄 **Laporan & Rekapitulasi:** Generasi laporan total transaksi dan volume sampah berdasarkan rentang waktu.

---

## 🚫 Batasan Proyek *(Out of Scope)*

Untuk menjaga agar fokus pengembangan tetap realistis, fitur-fitur berikut **tidak tercakup** dalam versi ini:
- ❌ Integrasi *Payment Gateway* / E-Wallet (transaksi pencairan dilakukan secara tunai oleh pengurus).
- ❌ Sistem penjemputan sampah / pemetaan GPS.
- ❌ Fitur *Marketplace* atau jual-beli produk daur ulang.
- ❌ Aplikasi *Mobile Native* (Sistem dibangun sebagai *Responsive Web App*).

---

## ✅ Kriteria Keberhasilan

1. **Fungsionalitas Utama:**
   - Pencatatan setoran secara otomatis menambah saldo nasabah.
   - Pencairan saldo secara otomatis menguraikan saldo nasabah.
   - Nasabah dapat memantau riwayat transaksi melalui akun masing-masing.
2. **Integritas Data:**
   - Perhitungan nominal ($\text{berat} \times \text{harga}$) berjalan 100% akurat.
   - Terdapat validasi input (mencegah berat bernilai negatif atau penarikan melebihi sisa saldo).
3. **Arsitektur Database:**
   - Data tersimpan terstruktur dalam basis data relasional (*Users, Categories, Transactions, TransactionDetails*).
