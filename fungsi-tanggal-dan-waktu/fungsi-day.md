# Fungsi DAY

## Pengertian

Mengembalikan tanggal, yang dinyatakan dengan nomor seri. Hari diberikan sebagai bilangan bulat dengan rentang dari 1 sampai 31.

## Sintaks

```text
DAY(serial_number)
```

Sintaks fungsi DAY memiliki argumen berikut:

* `Serial_number`    Diperlukan. Tanggal yang Anda coba temukan. Tanggal harus dimasukkan menggunakan fungsi `DATE`, atau sebagai hasil dari rumus atau fungsi lain. Misalnya, gunakan `DATE(2008,5,23)` untuk tanggal 23 Mei 2008. Masalah dapat terjadi jika tanggal dimasukkan sebagai teks.

### Keterangan

Microsoft Excel menyimpan tanggal sebagai nomor seri berurutan sehingga bisa digunakan di dalam perhitungan. Secara default, 1 Januari 1900 adalah nomor seri 1, dan 1 Januari 2008 adalah nomor seri 39448 karena 39.448 hari setelah 1 Januari 1900.

Nilai yang dihasilkan melalui fungsi `YEAR`, `MONTH`, dan `DAY` akan menjadi nilai Masehi, tanpa memperhitungkan format tampilan untuk nilai tanggal yang diberikan. Misalnya, jika format tampilan nilai tanggal yang diberikan menggunakan kalender Hijriah, maka nilai yang dihasilkan untuk fungsi `YEAR`, `MONTH`, dan `DAY` adalah nilai yang terkait dengan tanggal Masehi yang setara.

## Contoh

| **Tanggal** |  |  |
| :--- | :--- | :--- |
| 15-Apr-11 |  |  |
| **Rumus** | **Deskripsi \(Hasil\)** | **Hasil** |
| `=DAY(A2)` | Hari dari tanggal dalam sel A2 \(15\) | 15 |

{% page-ref page="fungsi-tanggal-dan-waktu.md" %}

