# Data Science Project : Tweet Sentiment Analysis

## Background
media sosial khususnya Twitter atau X merupakan suatu sarana komuikasi dan pemasaran dimana semua orang dapat berbagi pemikiran, ide, dan pengamalan mereka. Twitter atau X juga salah satu media sosial yang banyak digunakan untuk mengekspresikan diri dan mengutarakan pendapat, baik pro maupun kontra dalam berbagai topik. Tidak jarang banyak pengguna yang menggunakan kata-kata abusive atau kasar dalam mengutarakan pendapatnya.

Analisis sentimen adalah salah satu proses komputasi yang dilakukan dengan menganalisis teks digital yang digunakan untuk menentukan apakah kata-kata atau kalimat yang disampaikan memiliki makna atau emosional tertentu. Analisis sentimen akan memahami dan dapat mengelompokkan kata-kata atau kalimat kedalam kategori positif, negatif, dan netral.

## Goals
Tujuan dari proyek ini adalah membangun model Machine Learning yang dapat mengklasifikasikan teks atau tweet menjadi beberapa kategori, seperti teks positif, teks negatif, dan teks netral.

**Metode Penelitian**

- **LSTM** merupakan jenis dari jaringan saraf tiruan yang didesain untuk memahami ketergantungan jangka panjang dalam data. Oleh karena itu, LSTM sangat sesuai digunakan untuk berbagai tugas seperti Pengenalan suara, penerjemahan bahasa, dan analisis sentimen.
- **MLP** adalah jenis jaringan saraf tiruan yang terdiri dari beberapa lapisan neuron yang saling terhubung satu sama lain. MLP digunakan untuk mempelajari pola-pola yang kompleks dan non-linear pada data input, seperti pengenalan wajah, prediksi harga saham, dan pengenalan pola pada teks.

## Data
Data yang akan digunakan merupakan dataset yang diperoleh dari Twitter atau X yang berisikan tweet mengenai topik tertentu. Dataset ini kemudian akan di cleansing terlebih dahulu sebelum digunakan untuk data latih model yang kemudian akan dibagi menjadi 3 kategori yaitu negatif, positif, dan netral.

## Langkah Kerja
Berikut merupakan langkah-langkah yang akan dilakuka untuk analisis sentimen :

- Mengubah teks menjadi lowercase
- Menghapus noise, seperti hastag, retweet, metion, emoji, link, dan special character
- Mengubah kata alay menjadi kata tidak alay
- Tokenisasi
- Remove Stopwords
- Melakukan steeming
- Tf-ldf (MLP)
- Sequences dan Padding (LSTM)

## Kesimpulan
Metrik evaluasi yang digunakan adalah Classification Report. Dalam Classification Report, terdapat beberapa matriks, seperti akurasi, precision, recall, dan F1 Score.

Dari hasil evaluasi, diperoleh nilai model LSTM memiliki performa yang lebih baik dibandingkan dengan model MLP. Rata-rata akurasi yang diperoleh setelah dilakukan cross validation adalah 0,91 untuk model LSTM, sedangkan untuk model MLP adalah 0,8245.
