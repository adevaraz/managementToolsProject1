# REPLACE, REPLACEB Function

REPLACE berfungsi untuk menggantikan bagian dari string teks, berdasarkan jumlah karakter yang Anda tentukan, dengan string teks berbeda.

REPLACE berfungsi untuk menggantikan bagian dari string teks, berdasarkan jumlah byte yang Anda tentukan, dengan string teks berbeda.

{% hint style="info" %}
* REPLACE selalu menghitung setiap karakter, byte tunggal atau byte ganda, sebagai 1, tak peduli seperti apa pengaturan bahasa default-nya.
* REPLACEB menghitung setiap karakter byte ganda sebagai 2 saat Anda mengaktifkan bahasa pengeditan yang mendukung DBCS dan menetapkannya sebagai bahasa default. Jika tidak, REPLACEB menghitung setiap karakter sebagai 1.
{% endhint %}

### Sintaks

```text
REPLACE(old_text, start_num, num_chars, new_text)
```

```text
REPLACEB(old_text, start_num, num_bytes, new_text)
```

| Argumen | Fungsi |
| :--- | :--- |
| old\_text | Teks yang ingin diganti beberapa karakternya. |
| start\_num | Posisi karakter di old\_text yang ingin Anda ganti dengan new\_text. |
| num\_chars | Jumlah karakter di old\_text yang ingin Anda ganti dengan new\_text menggunakan REPLACE. |
| new\_bytes | Jumlah byte di old\_text yang ingin Anda ganti dengan new\_text menggunakan REPLACEB. |
| new\_text | Teks yang akan mengganti karakter di old\_text. |

### Contoh

![](../.gitbook/assets/image%20%2812%29.png)

