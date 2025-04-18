# Technical Test

Diketahui perusahaan XYZ membuat aplikasi yang memiliki kemampuan untuk mencatat orderan pesanan dari client dengan spesifikasi sebagai berikut:

## UI
![Sales Order UI](https://github-production-user-asset-6210df.s3.amazonaws.com/73767596/435351014-4b298dac-198d-4af2-ab31-bf9a81188dd6.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAVCODYLSA53PQK4ZA%2F20250419%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20250419T024852Z&X-Amz-Expires=300&X-Amz-Signature=fbeb3da3a8d9bd944aba6b6e783ead09e65ae0749bd025e22236c8cb153fedd8&X-Amz-SignedHeaders=host)

## Structure
![Structure](https://github-production-user-asset-6210df.s3.amazonaws.com/73767596/435351053-2c512e74-749d-48f0-9992-ad98fd4cb1d5.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAVCODYLSA53PQK4ZA%2F20250419%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20250419T024924Z&X-Amz-Expires=300&X-Amz-Signature=8c08c723acb0a009c4426e06419654d374ea8e04c9f7dcae98d7ad31afc9df8e&X-Amz-SignedHeaders=host)

## Catatan
Untuk mempersingkat waktu pengerjaan, beberapa field yang ada di UI tidak perlu disimpan ke dalam database, cukup simpan referensinya saja. Berikut adalah beberapa catatan yang perlu diperhatikan:
- PPH & VAT tidak perlu masuk hitungan, cukup simpan referensinya saja
- Semua referensi yang ada di dalam aplikasi ini tidak perlu disimpan ke dalam database, cukup siapkan data statis di JS, simpan ID nya. Contoh:
  - Daftar customer (A, B, C)
  - Daftar currency (IDR, USD, SGD)
  - Daftar status type (Open, Closed, Cancelled)
  - Daftar order type (Sales, Sewa, Maintenance)
  - Daftar produk (PC Server, Laptop, Printer, dll)

- Cukup buat 2 tabel di database
  - Tabel sales order (sales_orders)
  - Tabel sales order detail (so_dts)
- Hanya simpan kolom yang tampil di UI saja
- Diskon hanya bisa salah satu, antara (%) atau (Amount) untuk mengurangi nilai per-item.

## Task
Buat UI untuk form create, edit, dan list sales order

## Tech Stack
Silahkan pilih tech stack yang nyaman untuk anda, berikut pilihan yang kami berikan:
- Frontend: Bebas
- Backend: Golang / PHP
- Database: MySQL / PostgreSQL