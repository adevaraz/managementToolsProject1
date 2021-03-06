# Fungsi YEAR

## Pengertian

Mengembalikan tahun yang terkait dengan satu tanggal. Tahun dikembalikan sebagai bilangan bulat dalam rentang 1900-9999.

## Sintaks

`YEAR(serial_number)`

Sintaks fungsi `YEAR` memiliki argumen berikut:

* `Serial_number`    Diperlukan. Tanggal dari tahun yang akan dicari. Tanggal harus dimasukkan dengan menggunakan fungsi `DATE`, atau sebagai hasil dari rumus atau fungsi lain. Contoh, gunakan `DATE(2008,5,23)` untuk tanggal 23 Mei 2008. Masalah bisa muncul jika tanggal dimasukkan sebagai teks.

{% hint style="info" %}
## Keterangan

Microsoft Excel menyimpan tanggal sebagai nomor seri berurutan sehingga bisa digunakan di dalam perhitungan. Secara default, 1 Januari 1900 adalah nomor seri 1, dan 1 Januari 2008 adalah nomor seri 39448 karena 39.448 hari setelah 1 Januari 1900.

Nilai yang dihasilkan melalui fungsi `YEAR`, `MONTH`, dan `DAY` akan menjadi nilai Masehi, tanpa memperhitungkan format tampilan untuk nilai tanggal yang diberikan. Misalnya, jika format tampilan nilai tanggal yang diberikan menggunakan kalender Hijriah, maka nilai yang dihasilkan untuk fungsi `YEAR`, `MONTH`, dan `DAY` adalah nilai yang terkait dengan tanggal Masehi yang setara.
{% endhint %}

## Contoh

| **Data** |  |  |
| :--- | :--- | :--- |
| **Tanggal** |  |  |
| 05/07/2008 |  |  |
| 05/07/2010 |  |  |
| **Rumus** | **Deskripsi \(Hasil\)** | **Hasil** |
| `=YEAR(A3)` | Tahun dari tanggal dalam sel A3 \(2008\) | 2008 |
| `=YEAR(A4)` | Tahun dari tanggal dalam sel A4 \(2010\) | 2010 |

