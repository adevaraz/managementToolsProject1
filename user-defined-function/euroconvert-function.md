# EUROCONVERT Function

Fungsi EUROCONVERT berfungsi untuk mengonversi angka ke euro, mengonversi angka dari euro ke mata uang anggota euro, atau mengonversi angka dari satu mata uang anggota euro ke mata uang lain dengan menggunakan euro sebagai perantara \(triangulasi\). Mata uang yang tersedia untuk dikonversi adalah mata uang negara-negara anggota Uni Eropa \(UE\) yang telah mengadopsi euro. Fungsi ini menggunakan nilai konversi tetap yang dibuat oleh UE.

## Sintaks

```text
EUROCONVERT(number,source,target,full_precision,triangulation_precision)
```

| Argumen | Fungsi |
| :--- | :--- |
| number | Nilai mata uang yang ingin Anda konversi, atau referensi ke sebuah sel yang berisi nilai tersebut. |
| source | String tiga huruf, atau referensi ke sel yang berisi string tersebut |
| target | String tiga huruf, atau referensi sel, yang terkait dengan kode ISO mata uang hasil konversi angka. |
| full\_precision | Sebuah nilai logika \(TRUE atau FALSE\), atau ekspresi yang mengevaluasi sebuah nilai sebagai TRUE atau FALSE, yang menentukan cara menampilkan hasilnya. |
| triangulation\_precision | Sebuah bilangan bulat sama dengan atau lebih dari 3 yang menentukan jumlah digit signifikan yang akan digunakan untuk nilai euro langsung ketika mengonversi antara dua mata uang anggota euro. Jika Anda menghilangkan argumen ini, Excel tidak membulatkan nilai euro perantara tersebut. Jika Anda memasukkan argumen ini ketika mengonversi dari suatu mata uang anggota euro ke euro, Excel menghitung nilai euro perantara yang kemudian dapat dikonversi ke mata uang anggota euro. |

