# Fungsi DAYS360

## Pengertian

Fungsi `DAYS360` mengembalikan jumlah hari antara dua tanggal berdasarkan tahun dengan 360 hari per tahun \(dua belas bulan dengan 30 hari per bulan\), yang digunakan dalam beberapa perhitungan akuntansi. Gunakan fungsi ini untuk membantu menghitung pembayaran jika sistem akuntansi Anda berdasarkan pada dua belas bulan dengan 30 hari per bulan.

## Sintaks

```text
DAYS360(start_date,end_date,[method])
```

Sintaks fungsi `DAYS360` memiliki argumen berikut:

* `Start_date`**,** `end_date`    Diperlukan. Dua tanggal di antaranya yang ingin Anda ketahui jumlah harinya. Jika `start_date` terjadi setelah `end_date`, fungsi `DAYS360` akan mengembalikan angka negatif. Tanggal harus dimasukkan dengan menggunakan fungsi `DATE`**,** atau berasal dari hasil rumus atau fungsi lain. Misalnya, gunakan `DATE(2008,5,23)` untuk mengembalikan tanggal 23 Mei, 2008. Masalah bisa muncul jika tanggal dimasukkan sebagai teks.
* `Method`    Opsional. Nilai logika yang menentukan apakah akan menggunakan metode A.S. atau Eropa dalam perhitungan.

| **Metode** | **Didefinisikan** |
| :--- | :--- |
| `FALSE` atau dihilangkan | AS Metode \(NASD\). Jika tanggal mulai adalah hari terakhir suatu bulan, maka menjadi sama dengan hari ke-30 bulan yang sama. Jika tanggal berakhir adalah hari terakhir suatu bulan dan tanggal mulainya lebih awal dari hari ke-30 suatu bulan, tanggal berakhir menjadi sama dengan hari ke-1 bulan berikutnya; jika tidak, tanggal berakhir menjadi sama dengan hari ke-30 bulan yang sama. |
| `TRUE` | Metode Eropa. Tanggal mulai dan tanggal berakhir yang terjadi pada hari ke-31 suatu bulan menjadi sama dengan hari ke-30 dari bulan yang sama. |

**Catatan:** Excel menyimpan tanggal sebagai nomor seri berurutan sehingga bisa digunakan dalam perhitungan. Secara default, 1 Januari 1900 adalah nomor seri 1, dan 1 Januari 2008 adalah nomor seri 39448 karena 39.447 hari setelah 1 Januari 1900.

## Contoh

| **Tanggal** |  |  |
| :--- | :--- | :--- |


| 1-Jan-11 |  |  |
| :--- | :--- | :--- |


| 30-Jan-11 |  |  |
| :--- | :--- | :--- |


| 1-Feb-11 |  |  |
| :--- | :--- | :--- |


| 31-Des-11 |  |  |
| :--- | :--- | :--- |


| **Rumus** | **Deskripsi** | **Hasil** |
| :--- | :--- | :--- |


| `=DAYS360(A3,A4)` | Jumlah hari antara 30/01/2011 dan 01/02/2011, berdasarkan pada 360 hari dalam setahun. | 1 |
| :--- | :--- | :--- |


| `=DAYS360(A2,A5)` | Jumlah hari antara 01/01/2011 dan 31/12/2011, berdasarkan pada 360 hari dalam setahun. | 360 |
| :--- | :--- | :--- |


| `=DAYS360(A2,A4)` | Jumlah hari antara 01/01/2011 dan 01/02/2011, berdasarkan pada 360 hari dalam setahun. | 0,30 |
| :--- | :--- | :--- |


{% page-ref page="fungsi-tanggal-dan-waktu.md" %}

