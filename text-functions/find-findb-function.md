# FIND, FINDB Function

Fungsi FIND dan FINDB berfungsi menemukan satu string teks dari string teks kedua, dan mengembalikan nomor posisi mulai string teks pertama dari karakter pertama string teks kedua.

{% hint style="info" %}
sensitif huruf besar/kecil
{% endhint %}

* FIND selalu menghitung setiap karakter, baik byte tunggal atau byte ganda sebagai 1, tak peduli apa pun pengaturan bahasa default-nya.
* FINDB menghitung setiap karakter dengan byte ganda sebagai 2 ketika Anda mengaktifkan pengeditan bahasa yang mendukung DBCS lalu mengaturnya sebagai bahasa default. Jika tidak, FINDB menghitung setiap karakter sebagai 1.

### Sintaks

```text
FIND(find_text, within_text, [start_num])
```

```text
FINDB(find_text, within_text, [start_num])
```

| Argumen | Fungsi |
| :--- | :--- |
| find\_text | Teks yang ingin Anda temukan. |
| within\_text | Teks yang berisi teks yang ingin Anda temukan. |
| start\_num | Opsional. Menentukan karakter yang digunakan untuk memulai pencarian. Karakter pertama dalam within\_text adalah angka karakter 1. Jika Anda menghapus start\_num, diasumsikan menjadi 1. |

### Contoh

![](../.gitbook/assets/image%20%283%29.png)

