# Technical Test

Diketahui perusahaan XYZ membuat aplikasi yang memiliki kemampuan untuk mencatat orderan pesanan dari client dengan spesifikasi sebagai berikut:

## UI
![Sales Order UI](https://github.com/user-attachments/assets/9b0c8553-28cc-486f-856e-462c12ff3d85)

## Structure
![Structure](https://github.com/user-attachments/assets/3c734cba-0e30-4cd6-baea-2da0a2bea05a)

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