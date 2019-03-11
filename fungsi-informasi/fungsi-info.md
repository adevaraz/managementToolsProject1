# Fungsi INFO

## Deskripsi

Mengembalikan informasi tentang lingkungan operasi saat ini.

## Sintaks

INFO\(type\_text\)

Sintaks fungsi INFO memiliki argumen ini:

* **Type\_text**    Diperlukan. Teks yang menentukan tipe informasi apa yang Anda inginkan dikembalikan.

|  **Type\_text** |  **Mengembalikan** |
| :--- | :--- |


| "directory" | Jalur direktori atau folder saat ini. |
| :--- | :--- |


| "numfile" | Jumlah lembar kerja aktif di dalam buku kerja yang terbuka. |
| :--- | :--- |


<table>
  <thead>
    <tr>
      <th style="text-align:left">&quot;origin&quot;</th>
      <th style="text-align:left">
        <p>Mengembalikan referensi sel absolut sel paling atas dan sel paling kiri
          yang tampak di jendela, berdasarkan posisi gulir saat ini, sebagai teks
          yang diawali dengan &quot;$A:&quot;. Nilai ini ditujukan untuk kompatibel
          dengan Lotus 1-2-3 rilis 3.x. Nilai sebenarnya yang dikembalikan bergantung
          pada pengaturan gaya referensi saat ini. Menggunakan D9 sebagai contoh,
          nilai yang dikembalikan adalah sebagai berikut:</p>
        <ul>
          <li> <b>Gaya referensi A1</b> &quot;$A:$D$9&quot;.</li>
          <li> <b>Gaya referensi R1C1</b> &quot;$A:R9C4&quot;</li>
        </ul>
      </th>
    </tr>
  </thead>
  <tbody></tbody>
</table>| "osversion" | Versi sistem operasi saat ini, sebagai teks. |
| :--- | :--- |


| "recalc" | Mode rekalkulasi saat ini; mengembalikan "Automatic" atau "Manual". |
| :--- | :--- |


| "release" | Versi Microsoft Excel, sebagai teks. |
| :--- | :--- |


| "system" | Nama lingkungan operasi: Macintosh = "mac" Windows = "pcdos" |
| :--- | :--- |


{% hint style="info" %}
**Penting:** Dalam versi Microsoft Excel yang sebelumnya, nilai "memavail", "memused", dan "totmem" type\_text mengembalikan informasi memori. Jenis-jenis type\_text ini tidak lagi tersedia dan sekarang mengembalikan nilai kesalahan \#N/A.
{% endhint %}

## Contoh

Salin contoh data di dalam tabel berikut ini dan tempel ke dalam sel A lembar kerja Excel yang baru. Agar rumus menunjukkan hasil, pilih datanya, tekan F2, lalu tekan Enter. Jika perlu, Anda bisa menyesuaikan lebar kolom untuk melihat semua data.

| **Rumus** | **Deskripsi** | **Hasil** |
| :--- | :--- | :--- |
| '=INFO\("numfile"\) | Jumlah lembar kerja aktif | INFO\("numfile"\) |
| '=INFO\("recalc"\) | Mode perhitungan ulang untuk buku kerja. | =INFO\("recalc"\) |

