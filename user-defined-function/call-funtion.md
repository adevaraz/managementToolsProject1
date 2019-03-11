# CALL Funtion

Fungsi CALL berfungsi untuk memanggil prosedur dalam pustaka link dinamis atau sumber daya kode. Terdapat dua bentuk sintaks fungsi ini. Gunakan sintaks 1 hanya dengan sumber daya kode yang terdaftar sebelumnya, yang menggunakan argumen dari fungsi REGISTER. Gunakan sintaks 2 pada daftar untuk memanggil sumber daya kode.

## Sintaks

### 1

```text
CALL(register_id,[argument1],...)
```

| Argumen | Fungsi |
| :--- | :--- |
| register\_id | nilai yang dikembalikan oleh REGISTER yang dijalankan sebelumnya atau fungsi REGISTER.ID. |
| argument1,... | Opsional. Argumen yang akan dikirim ke prosedur. |

### 2

```text
CALL(module_text,procedure,type_text,[argument1],...])
```

| Argumen | Fungsi |
| :--- | :--- |
| module\_text | Teks kutipan yang menentukan nama pustaka link dinamis \(DLL\) yang berisi prosedur di Microsoft Excel untuk Windows. |
| procedure | Teks yang menentukan nama fungsi dalam DLL di Microsoft Excel untuk Windows. Anda juga dapat menggunakan nilai ordinal fungsi dari pernyataan EXPORTS dalam file definisi modul \(.DEF\). Nilai ordinal harus dalam bentuk teks. |
| type\_text | Tipe data dari nilai yang dikembalikan dan tipe data dari semua argumen pada DLL atau sumber daya kode. Untuk DLL atau sumber daya kode \(XLL\) yang berdiri sendiri, Anda dapat menghapus argumen ini. |
| argument1,... | Opsional. Argumen yang akan dikirim ke prosedur. |

