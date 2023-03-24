# **MONTHLY PURCHASE PREDICTION FOR E-COMMERCE**
# Olist Brazilian E-Commerce

**Created by :**<br>
Nathania Frieska Zamris (JCDS 0106 002)<br>
Mary Amalia Wauran (JCDS 0106 006)<br>
Idam Ahmadi (JCDS 0106 007)<br>

Kami melakukan prediksi jumlah pembelian pada 4 bulan ke depan (akhir tahun 2018) berdasarkan data historis perusahaan tahun 2016-2018.
Prediksi dilakukan agar tim marketing mendapatkan gambaran berapa TIV yang bisa didapatkan sampai akhir tahun dan diharapkan membantu tim marketing menentukan **budget** yang diperlukan untuk mencapai TIV tersebut.

Disini kami juga memberi beberapa rekomendasi baik dari sisi marketing maupun bukan, berdasarkan insight data yang kami temukan, diantaranya:

1. Berapa Average Basket Size dan bagaimana kita bisa meningkatkannya?
2. Performa kota terbaik, berapa user terakuisisi, kota mana yang mempunyai potensi growth.
3. Kategori apa yang paling laku, potensi dan kendala apa yang mungkin dialami kategori tersebut.
4. Berapa jumlah transaksi kita, bagaimana caranya menjaga pengelamanan berbelanja tetap baik?
5. Adakah potensi lain yang bisa dijadikan diversifikasi produk?

**Note : Walaupun begitu analisa yang kami lakukan baru permukaan dan perlu dikaji lebih mendalam**

Kami menggunakan **Brazilian E-Commerce Public Dataset**
- Sumber : [kaggle.com](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce?select=olist_products_dataset.csv)
- Pembuat : Olist and André Sionek
- Tahun : 2018

**Olist E-Commerce** adalah pasar online Brazil yang menghubungkan pedagang (usaha kecil dan menengah) dengan pelanggan di seluruh Brazil. Pedagang dapat menggunakan Olist untuk menjual produk mereka secara online dan mengakses pangsa pasar yang lebih luas, layanan logistik, dan solusi pemrosesan pembayaran.

Kami akan membangun suatu model yang akan membantu perusahaan untuk dapat menyediakan 'tool' prediksi pembelian yang mana akan berguna untuk menentukan budget marketing. Forecasting untuk 4 bulan ke depan dilakukan dengan mencoba modeling menggunakan Fbprophet, ARIMA dan ElasticNet. Metric yang digunakan adalah MAPE dan perbandingan grafik antar modelnya sebagai penilaian.
Kami putuskan menjadikan MAPE sebagai metric penilaian karena beberapa alasan berikut:
- Grafik kita memiliki trend yang berbeda signifikan, jika menggunakan penilaian nominal error 10000 pada 2017 mungkin besar tapi di 2018 bisa jadi kecil, sedangkan dengan MAPE perbedaan persepsi seperti itu bisa dihindari
- MAPE lebih mudah dipahami oleh tim marketing
