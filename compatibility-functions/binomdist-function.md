# BINOMDIST Function

Fungsi `BINOMDIST` mengembalikan nilai individu probabilitas distribusi binomial. Fungsi ini digunakan untuk suatu data uji atau percobaan tetap, ketika hasil suatu percobaan hanya berhasil atau gagal, hasilnya bersifat independen, dan ketika probabilitas keberhasilan bernilai konstan selama eksperimen.

{% hint style="info" %}
Fungsi `BINOMDIST` ini telah digantikan dengan fungsi yang lebih baik dan akurat yaitu fungsi `BINOM.DIST`.
{% endhint %}

Syntax fungsi `BINOMDIST` :

```text
BINOMDIST(number_s, trials, probability_s, cumulative)
```

<table>
  <thead>
    <tr>
      <th style="text-align:left">Argumen</th>
      <th style="text-align:left">Fungsi</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Number_s</td>
      <td style="text-align:left">Jumlah keberhasilan dalam percobaan.</td>
    </tr>
    <tr>
      <td style="text-align:left">Trials</td>
      <td style="text-align:left">Jumlah dari percobaan independen.</td>
    </tr>
    <tr>
      <td style="text-align:left">Probability_s</td>
      <td style="text-align:left">Probabilitas kesuksesan dalam setiap percobaan.</td>
    </tr>
    <tr>
      <td style="text-align:left">Cumulative</td>
      <td style="text-align:left">
        <p>Nilai logika yang menentukan bentuk fungsi. Jika cumulative bernilai <code>TRUE</code>,
          maka <code>BINOMDIST</code> mengembalikan fungsi distribusi kumulatif, yakni
          probabilitas bahwa paling banyak terdapat number_s keberhasilan</p>
        <p>Jika cumulative bernilai <code>FALSE</code>, maka akan dikembalikan fungsi
          massa probabilitas, yakni probabilitas bahwa terdapat number_s keberhasilan.</p>
      </td>
    </tr>
  </tbody>
</table>

