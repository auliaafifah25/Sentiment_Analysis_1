# Laporan Proyek Machine Learning - Aulia Afifah

## Domain Proyek

Dalam proyek yang diangkat yaitu aplikasi DANA. DANA adalah aplikasi keuangan yang inovatif dan berkembang pesat di Indonesia. Dikenal sebagai platform pembayaran digital, DANA telah meraih popularitas karena kemudahan dan beragam fitur yang ditawarkannya kepada penggunanya. Dengan DANA, pengguna dapat melakukan berbagai transaksi keuangan, mentransfer uang, membayar tagihan, hingga berbelanja secara online.

Satu hal yang menarik, DANA juga dapat diunduh melalui Playstore, di mana para pengguna memiliki kesempatan untuk memberikan ulasan dan penilaian terhadap aplikasi ini. Melalui ulasan-ulasan tersebut, kita dapat memperoleh wawasan yang berharga mengenai pengalaman pengguna dengan aplikasi DANA, termasuk kepuasan, keluhan, dan saran untuk perbaikan.

Pada proyek ini akan melakukan predictive analytics terhadap aplikasi DANA yang terdapt di Playstore Indonesia. Data yang digunakan adalah 50 ribu ulasan aplikasi DANA yang telah dilabeli, yang diperoleh dari hasil pengambilan data di Playstore Indonesia. Dalam proyek ini, akan menjelajahi ulasan-ulasan aplikasi DANA lebih lanjut, untuk memahami bagaimana persepsi dan sentimen pengguna terhadap aplikasi ini.

**Rubrik/Kriteria Tambahan (Opsional)**:

Predictive analitycs terhadap aplikasi DANA merupakan langkah yang penting dalam memahami pandangan pengguna terhadap layanan keuangan digital tersebut. Berikut adalah alasan mengapa penyelesaian masalah ini penting:

1. Meningkatkan kualitas layanan: Aplikasi DANA memberikan kemudahan dalam bertransaksi secara digital di Indonesia, sesuai dengan gaya hidup masyarakat yang semakin mengutamakan kecepatan, kemudahan, dan praktisitas. Meskipun masih tergolong baru dalam ranah pembayaran e-wallet, DANA terus mengalami pengembangan untuk menarik perhatian kaum milenial. Referensi: [Kualitas Pelayanan Aplikasi DANA Terhadap Kepuasan Konsumen](http://114.7.153.31/index.php/jis/article/view/3861)

2. Mendukung pengambilan keputusan: Menurut penelitian ini, salah satu faktor yang mempengaruhi minat pengguna terhadap aplikasi e-wallet, seperti DANA, adalah tingkat kemudahan penggunaan dan fitur-fitur layanan yang disediakan. Referensi: [Pengaruh Persepsi Kemudahan Dan Fitur Layanan Terhadap Minat Menggunakan E-Wallet Pada Aplikasi Dana Di Surabaya](https://ejournal.unesa.ac.id/index.php/jptn/article/view/45517)

3. Membangun reputasi: Menurut hasil penelitian dan analisis yang dilakukan, membangun reputasi perusahaan melalui kualitas pelayanan dan kontribusi yang diberikan dapat menjadi faktor penting dalam memperoleh kepercayaan pelanggan. Referensi: [Peran Reputasi Perusahaan dalam Membangun Kepercayaan Pelanggan Maskapai Penerbangan](https://journal.jis-institute.org/index.php/jismab/article/view/51/68)

4. Meningkatkan evaluasi kepuasan pengguna: Menurut penelitian ini, Hasil kuisioner menunjukkan bahwa sebagian besar responden percaya bahwa DANA memiliki potensi untuk menjadi bagian integral dari kehidupan sehari-hari, sementara kepuasan pengguna terhadap kinerja aplikasi DANA mencapai 100%. Oleh karena itu, dapat disimpulkan bahwa aplikasi DANA telah menunjukkan kesiapan untuk diterima secara luas dalam masyarakat. Referensi: [Analisis kepuasan masyarakat terhadap penggunaan aplikasi DANA menggunakan metode SWOT](https://jim.teknokrat.ac.id/index.php/sisteminformasi/article/view/1593)

Daftar Referensi:
Gunawan, A., Wahyuni, N., & Nursekha, V. (2021). Kualitas Pelayanan Aplikasi Dana Terhadap Kepuasan Konsumen. Journal of Integrated System, 4(2), 181-198.
Abrilia, N. D. (2020). Pengaruh Persepsi Kemudahan Dan Fitur Layanan Terhadap Minat Menggunakan E-Wallet Pada Aplikasi Dana Di Surabaya. Jurnal Pendidikan Tata Niaga (JPTN), 8(3), 1006-1012.
Majid, N. (2020). Peran Reputasi Perusahaan dalam Membangun Kepercayaan Pelanggan Maskapai Penerbangan. Jurnal Ilmu Sosial, Manajemen, Akuntansi Dan Bisnis, 1(2), 66-72.
Lathifah, L. (2022). Analisis kepuasan masyarakat terhadap penggunaan aplikasi DANA menggunakan metode SWOT. Jurnal Teknologi dan Sistem Informasi, 3(1), 20-26.

## Business Understanding

Pada bagian ini, menjelaskan proses klarifikasi masalah.
Bagian laporan ini mencakup:

### Problem Statements

- Masalah sentimen positif: Pengguna sering kali memberikan ulasan positif terkait dengan fitur atau layanan yang sangat membantu dalam aplikasi DANA. Namun, kita perlu memahami lebih lanjut mengenai fitur atau layanan apa yang paling seirng disoroti dan mengapa hal tersebut dianggap sangat membantu.
- Masalah sentimen negatif: Di sisi lain, ada beberapa keluhan yang muncul dalam ulasan pengguna terkait dengan aplikasi DANA. Dari analisis bigram, kita menemukan pola-pola yang menunjukkan masalah-masalah yang sering dialami pengguna. Namun, kita perlu menentukan prioritas masalah yang paling penting untuk diselesaikan.
- Masalah sentimen netral: Selain ulasan positif dan negatif, ada juga sebagian besar ulasan yang diberikan dengan sentimen netral terhadap aplikasi DANA. Meskipun ulasan tersebut tidak mengandung keluhan atau pujian yang signifikan, namun mereka tetap memberikan wawasan yang berharga mengenai pengalaman pengguna.

### Goals

- Tujuan pemahaman sentimen positif: Mengidentifikasi fitur atau layanan dalam aplikasi DANA yang paling sering disoroti dalam ulasan positif dan menganalisis alasan mengapa fitur-fitur tersebut dianggap sangat membantu oleh pengguna.
- Tujuan pemahaman sentimen negatif: Menentukan prioritas masalah-masalah yang paling sering muncul dalam ulasan negatif pengguna dan mengembangkan rekomendasi atau strategi untuk meningkatkan pengalaman pengguna dengan memperbaiki masalah-masalah tersebut.
- Tujuan pemahaman sentimen netral: Mengidentifikasi aspek-aspek tertentu yang paling sering disoroti dalam ulasan netral dan menentukan apakah ada peluang untuk meningkatkan atau mengoptimalkan fitur-fitur tertentu untuk mengubah sentimen netral menjadi positif.

**Rubrik/Kriteria Tambahan (Opsional)**:

- Menambahkan bagian “Solution Statement” yang menguraikan cara untuk meraih goals. Bagian ini dibuat dengan ketentuan sebagai berikut:

  ### Solution statements

  - Solusi dengan Support Vector Machine (SVM): Mengimplementasikan algoritma SVM untuk klasifikasi sentimen terhadap ulasan aplikasi DANA, melakukan proses training dan evaluasi model menggunakan data yang telah dilabeli, dan mengukur kinerja model menggunakan metrik evaluasi seperti precision, recall, dan f1-score untuk masing-masing kelas sentimen (positif, negatif, netral).
  - Solusi dengan Random Forest: Mengimplementasikan algoritma Random Forest untuk klasifikasi sentimen terhadap ulasan aplikasi DANA, melakukan proses training dan evaluasi model menggunakan data yang telah dilabeli, dan Mengukur kinerja model menggunakan metrik evaluasi seperti precision, recall, dan f1-score untuk masing-masing kelas sentimen (positif, negatif, netral).

## Data Understanding

Sumber dataset yang digunakan dalam proyek ini adalah dari Kaggle, yang dapat diakses melalui tautan berikut: DANA App Sentiment Review on Playstore Indonesia (https://www.kaggle.com/datasets/alexmariosimanjuntak/dana-app-sentiment-review-on-playstore-indonesia). Dataset ini berisi 50 ribu ulasan aplikasi DANA yang telah dilabeli, yang diperoleh dari pengambilan data di Google Playstore Indonesia.

### Variabel-variabel pada ulasan aplikasi DANA dataset adalah sebagai berikut:

Dataset ini terdiri dari 5 kolom, yaitu:

- UserName: Kolom ini berisi nama pengguna yang memberikan ulasan terhadap aplikasi DANA di Google Playstore.
- Score: olom ini menyimpan nilai atau rating yang diberikan oleh pengguna terhadap aplikasi DANA. Nilai ini berkisar dari 1 hingga 5, di mana 1 menunjukkan rating terendah dan 5 menunjukkan rating tertinggi.
- At: Kolom ini berisi informasi tanggal dan waktu ketika ulasan diberikan oleh pengguna.
- Content: Kolom ini menyimpan teks ulasan yang ditulis oleh pengguna terkait pengalaman mereka dengan aplikasi DANA.
- Sentimen: Kolom ini berisi label sentimen yang menunjukkan apakah ulasan yang diberikan oleh pengguna bersifat positif, negatif, atau netral terhadap aplikasi DANA.

**Rubrik/Kriteria Tambahan (Opsional)**:

- Melakukan beberapa tahapan yang diperlukan untuk memahami data, contohnya teknik visualisasi data atau exploratory data analysis.
- Untuk keperluan proyek ini, proyek ini hanya menggunakan 2 kolom, yaitu content dan sentimen. Kolom content berisi teks ulasan dari pengguna, sedangkan kolom sentimen berisi label sentimen dari ulasan tersebut (positif, negatif, atau netral). Dengan fokus pada kedua kolom ini, kita akan melakukan analisis sentimen terhadap aplikasi DANA berdasarkan ulasan pengguna.
- Untuk memahami data dengan lebih baik, melakukan beberapa tahapan, seperti statistik deskriptif, visualisasi data, analisis distribusi sentimen, dan analisis frekuensi data.

## Data Preparation

Pada bagian ini, teknik data preparation dilakukan seperti membaca data, analisis data, dan feature engineering dengan TF-IDF.

**Rubrik/Kriteria Tambahan (Opsional)**:

- Membaca data: Ini adalah langkah awal dari data preparation di mana data dimuat ke dalam lingkungan analisis.
- Analisis data: Analisis data awal untuk memahami struktur data, distribusi, dan menemukan masalah potensial seperti nilai yang hilang, dan lainnya.
- Feature engineering dengan TF-IDF: Transformasi teks menjadi representasi numerik menggunakan teknik TF-IDF, yang merupakan bagian penting dari data preparation untuk teks.

## Modeling

Pada bagian ini, model machine learning yang digunakan untuk menyelesaikan masalah analisis sentimen pada ulasan aplikasi DANA yaitu dua algoritma. Dua algoritma yang digunakan adalah Support Vector Machine (SVM) yaitu Support Vector Machine adalah algoritma klasifikasi yang sangat efektif untuk masalah dengan dimensi tinggi. SVM bekerja dengan mencari hyperplane yang memisahkan kelas-kelas data secara optimal dan Random Forest yaitu ensemble learning method yang menggunakan banyak pohon keputusan (decision trees) untuk meningkatkan performa dan mengurangi risiko overfitting.

**Rubrik/Kriteria Tambahan (Opsional)**:

- Support Vector Machine (SVM): Kelebihan; Efektif dalam ruang fitur berdimensi tinggi, masih efektif jika jumlah fitur lebih besar dari jumlah sampel, dan menggunakan subset dari poin pelatihan dalam fungsi keputusan, sehingga sangat hemat memori. Kekurangan; Tidak bekerja dengan baik jika dataset sangat besar, kurang efektif jika jumlah fitur lebih besar dari jumlah sampel, dan memerlukan tuning parameter seperti kernel, C, dan gamma.
- Random Forest: Kelebihan; Sangat baik dalam mengatasi data yang hilang (missing data), mampu menangani dataset dengan jumlah fitur yang sangat besar, dan mengurangi overfitting dengan cara menggabungkan banyak pohon keputusan. Kekurangan; Memerlukan lebih banyak computational resources dan hasil prediksi kurang interpretatif dibandingkan model linear.
- Memilih model terbaik: Model SVM akan digunakan untuk prediksi sentimen ulasan aplikasi DANA karena menunjukkan hasil yang lebih baik dalam evaluasi. Berdasarkan hasil evaluasi, SVM sedikit lebih unggul dengan akurasi 84% dibandingkan dengan Random Forest yang memiliki akurasi 83%. Selain itu, SVM menunjukkan performa yang lebih konsisten pada metrik precision, recall, dan f1-score untuk kelas positif dan netral.

## Evaluation

Pada bagian ini, akan menyebutkan dan menjelaskan metrik evaluasi yang digunakan dalam proyek predictive analitycs pada ulasan aplikasi DANA. Metrik yang digunakan adalah akurasi, precision, recall, dan F1 score.

- Akurasi: rasio jumlah prediksi yang benar (baik positif maupun negatif) terhadap total jumlah prediksi.
- Precision: rasio jumlah prediksi positif yang benar terhadap total jumlah prediksi positif.
- Recall: rasio jumlah prediksi positif yang benar terhadap total jumlah kasus positif aktual.
- F1 Score: metrik yang memberikan keseimbangan antara precision dan recall.
- Menjelaskan hasil proyek berdasarkan metrik evaluasi

Hasil evaluasi

1. Support Vector Machine (SVM)

- Akurasi: 0.84
- Precision: 0.79 (Positive), 0.71 (Negative), 0.90 (Neutral)
- Recall: 0.86 (Positive), 0.47 (Negative), 0.92 (Neutral)
- F1 Score: 0.82 (Positive), 0.57 (Negative), 0.91 (Neutral)

2. Random Forest

- Akurasi: 0.83
- Precision: 0.75 (Positive), 0.72 (Negative), 0.90 (Neutral)
- Recall: 0.89 (Positive), 0.33 (Negative), 0.91 (Neutral)
- F1 Score: 0.81 (Positive), 0.45 (Negative), 0.91 (Neutral)

**Rubrik/Kriteria Tambahan (Opsional)**:

- Support Vector Machine (SVM): SVM menunjukkan performa yang lebih baik secara keseluruhan dengan akurasi 84%, metrik F1 Score untuk sentimen positif dan netral cukup tinggi, masing-masing 0.82 dan 0.91, menunjukkan bahwa model ini mampu menangkap banyak ulasan yang benar-benar positif dan netral, dan precision untuk kelas negatif (0.71) menunjukkan bahwa model cukup baik dalam mengidentifikasi ulasan negatif yang sebenarnya negatif, meskipun recall untuk kelas ini lebih rendah (0.47), menunjukkan beberapa ulasan negatif yang terlewat.
- Random Forest: Random Forest memiliki akurasi sedikit lebih rendah yaitu 83%, metrik F1 Score untuk sentimen positif dan netral juga cukup tinggi, masing-masing 0.81 dan 0.91, dan precision untuk kelas negatif (0.72) hampir sama dengan SVM, tetapi recall (0.33) lebih rendah, menunjukkan lebih banyak ulasan negatif yang terlewat dibandingkan dengan SVM.

**---Ini adalah bagian akhir laporan---**
