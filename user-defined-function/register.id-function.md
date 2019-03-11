# REGISTER.ID Function



Fungsi REGISTER.ID berfungsi untuk mengembalikan ID pendaftaran dari pustaka link dinamis \(DLL, Dynamic Link Library\) yang ditentukan atau sumber daya kode yang telah didaftarkan sebelumnya. Jika DLL atau sumber daya kode belum didaftarkan, fungsi ini mendaftarkan DLL atau sumber daya kode lalu mengembalikan ID pendaftaran. 

### Sintaks

```text
REGISTER.ID(module_text,procedure,[type_text])
```

| Argumen | Fungsi |
| :--- | :--- |
| module\_text | Teks yang menyatakan nama DLL yang memuat fungsi dalam Microsoft Excel untuk Windows. |
| procedure | Teks yang menentukan nama fungsi dalam DLL di Microsoft Excel untuk Windows. |
| type\_text | Opsional. Teks yang menyatakan tipe data nilai yang dikembalikan dan tipe data semua argumen ke DLL. Jika fungsi atau sumber daya kode sudah didaftarkan, Anda dapat menghilangkan argumen ini. |

