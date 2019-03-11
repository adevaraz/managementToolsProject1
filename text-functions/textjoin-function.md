# TEXTJOIN Function

Fungsi `TEXTJOIN` menggabungkan teks dari beberapa rentang dan/atau string, serta menyertakan pemisah yang Anda tentukan antara tiap nilai teks yang akan digabungkan. Jika pemisah adalah string teks kosong, fungsi ini akan secara efektif menggabungkan rentang.

{% hint style="info" %}
Fungsi ini hanya tersedia di Excel untuk Office 365, Excel untuk Office 365 untuk Mac, Excel 2019, Excel 2019 untuk Mac, Excel Online, Excel untuk iPad, Excel untuk iPhone, Excel untuk tablet Android, Excel untuk ponsel Android, dan Excel Mobile
{% endhint %}

### Sintaks

```text
TEXTJOIN (delimiter, ignore_empty, text1, [text2], …)
```

| **Argumen** | **Deskripsi** |
| :--- | :--- |
| **pembatas** | String teks, kosongkan salah satu, atau satu atau beberapa karakter yang dimasukkan oleh tanda kutip ganda, atau referensi ke string teks yang valid. Jika angka disediakan, akan diperlakukan sebagai teks. |
| **ignore\_empty** | Jika TRUE, mengabaikan sel kosong. |
| **teks1** | Item teks untuk bergabung. String teks, atau array string, seperti rentang sel. |
| **\[teks2, ...\]** | Teks tambahan item untuk bergabung. Bisa maksimal 252 argumen teks untuk item teks, termasuk **text1**. Masing-masing bisa berupa teks string, atau array string, seperti rentang sel. |

