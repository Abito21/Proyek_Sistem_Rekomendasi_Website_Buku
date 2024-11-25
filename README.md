# Laporan Proyek Machine Learning - Abid Juliant Indraswara

![bukuCover](https://raw.githubusercontent.com/Abito21/Proyek_Sistem_Rekomendasi_Website_Buku/main/pictures/booksCover.jpg)
_Source : https://pixabay.com/photos/books-literature-knowledge-5937716/_

## Project Overview

### Latar Belakang

Buku merupakan perantara manusia dalam menyampaikan segala hal sejak jaman dahulu hingga sekarang. Bentuknya pun seiring waktu berubah namun tidak menghilangkan esensinya dalam menyampaikan perasaan, pengetahuan dan sejenisnya. Masih diminati hingga saat ini oleh para pembaca buku dari berbagi genre baik berbentuk fisik maupun online. Buku bisa ditemui dimana saja termasuk online yang tentunya memudahkan akses para pembaca baik untuk membacanya maupun membeli nya[\[1\]](https://doi.org/10.1109/ICISC47916.2020.9171222). Teknologi berkembang pesat dengan hadirnya internet dan sekarang di dukung dengan AI baik para pembaca buku untuk menemukan buku maupun penjual buku atau juga penulis buku[\[2\]](https://doi.org/10.1109/SAPIENCE.2016.7684166).

Berbagai jenis buku tersedia dan distribusikan secara online yang jumlahnya sangat banyak serta dengan bahasa yang berbeda. Timbul beberapa masalah dari beberapa pembaca untuk dapat menemukan buku yang orisinil, kualitas fisik/ isi bagus, dengan genre yang sesuai pembaca, berdasarkan kriteria penulis yang disuka, rating yang bagus dan masih banyak lagi membuat para pembaca kebingungan menentukan pilihannya[\[1\]](https://doi.org/10.1109/ICISC47916.2020.9171222). Melalui bantuan AI pilihan-pilihan tersebut dapat dipersingkat dengan menggunakan sistem saran atau rekomendasi sehingga pembaca mudah menentukan pilihannya. Beberapa pilihan yang sulit dan banyak akan dipersingkat hanya dengan melakukan beberapa aksi kecil yang umumnya di lakukan secara online. Rekomendasi sederhana dari buku yang paling populer, buku yang laris di pasaran, buku yang memiliki review atau rating terbaik, buku yang baru saja rilis dan masih banyak lagi[\[2\]](https://doi.org/10.1109/SAPIENCE.2016.7684166). Itu baru awal ketika baru saja akses ke website khusus konten jual buku, namun ketika sudah menjadi anggota dari website tersebut melalui riwayat dari yang dibaca maupun data pengguna maka rekomendasi yang muncul akan berbeda seperti genre buku yang sering dibaca, berdasarkan penulis dan sejenisnya. Tidak dipungkiri teknologi ini memudahkan serta menguntungkan kedua belah pihak pembaca buku, penulis buku dan penjual buku[\[3\]](https://doi.org/10.1109/IAdCC.2014.6779375).

Sistem rekomendasi bukan alat yang baru di era modern ini, karena banyak digunakan untuk merekomendasikan produk yang paling sesuai kepada pengguna atau pembaca buku. Persaingan di era modern yang begitu ketat mendorong semua pihak khususnya para penjual untuk dapat menambah atau meningkatkan keuntungan dan juga mempertahankan para pengguna jasa website khusus konten jual buku[\[3\]](https://doi.org/10.1109/IAdCC.2014.6779375). Sistem rekomendasi buku harus dapat merekomendasikan buku yang sesuai dengan minat pembeli. Terdapat banyak jenis rekomendasi sistem yang digunakan. Sehingga dalam upaya peningkatan keuntungan, kemudahan penggemar atau pembaca buku dan mempertahankan para pengguna jasa penyedia jual buku maka sistem rekomendasi merupakan solusi yang tepat untuk digunakan. Oleh karena itu pada projek ini akan membuat sistem rekomendasi dengan metode Content Based Filtering menggunakan pendekatan item yang cocok bagi pengguna.

### Referensi

[1] Kommineni Madhuri. etc, "[Machine Learning based Efficient Recommendation System for Book Selection using User based Collaborative Filtering Algorithm](https://doi.org/10.1109/ICISC47916.2020.9171222)", IEEE, 2020.

[2] Mathew Praveena. etc, "[Book Recommendation System through Content Based and Collaborative Filtering Method](https://doi.org/10.1109/SAPIENCE.2016.7684166)", IEEE, 2016.

[3] Shanker Tewari Anand. etc, "[Book Recommendation System Based on Combine Features of Content Based Filtering, Collaborative Filtering and Association Rule Mining](https://doi.org/10.1109/IAdCC.2014.6779375)", IEEE, 2014.

## Business Understanding

Permasalahn yang terjadi dalam proses pengembangan bisnis, peningkatan penggunaan website konten jual buku dan mempertahankan pengguna website selain peningkatan secara promosi maka diperlukan peningkatan layanan. Peningkatan layanan dilakukan supaya dapat meningkatkan traffic kunjungan website dengan menemukan alasan kenapa pengguna sering melakukan kunjungan website konten buku. Buku dicari banyak orang biasanya sesuai dengan yang dibutuhkan atau bisa jadi ada buku baru muncul atau bisa saja buku tersebut memiliki review yang bagus dan masih banyak lagi. Melalui analisa tersebut untuk bisa memudahkan pengguna mencari buku dan untuk meningkatkan traffic kunjungan website konten buku maka perlu sebuah sistem yang memberi saran sesuai kebutuhan pengguna dan juga pengguna baru. Sistem rekomendasi sangat tepat dalam menangani kasus seperti ini, dengan memberikan rekomendasi yang sesuai dengan data dan riwayat baca buku pengguna maka dapat memberikan dampak yang luar biasa dalam peningkatan traffic serta layanan. Hal ini memungkinkan pengguna dengan mudah mencari apa yang mereka inginkan dan mampu memberikan peningkatan penjualan buku.

### Problem Statements

- Metode sistem rekomendasi apa yang digunakan untuk kasus rekomendasi buku bagi pengguna website konten buku?
- Bagaimana cara sistem rekomendasi buku dalam menentukan rekomendasi ke pengguna berdasarkan rating buku?

### Goals

- Membuat sistem rekomendasi buku dengan metode Content Based Filtering dalam upaya peningkatan pengalaman pengguna untuk dapat menemukan buku dengan efisien.
- Memberi rekomendasi buku yang disukai oleh pengguna website konten buku melalui preferensi buku dengan rating yang populer.

Tujuan utama dari projek ini adalah membuat sistem yang mampu memberikan rekomendasi kepada pengguna website konten buku sesuai dengan preferensi pengguna dengan lebih efektif dan efisien sehingga mampu memudahkan pengguna serta peningkatan traffic kunjungan website konten buku.

## Data Understanding

Dataset yang digunakan berasal dari Kaggle dengan nama [Book Recommendation Datset](https://www.kaggle.com/datasets/arashnic/book-recommendation-dataset) yang diambil oleh Cai-Nicolas Ziegler melalui proses Crawling Data. Data tersebut diambil dan memiliki acuan website konten buku [Book Crossing Community](https://www.bookcrossing.com/?) disana dapat dijumpai banyak buku untuk dicari dikembangkan oleh komunitas dan store buku untuk melakukan transaksi jual beli. Terdiri dari 278,858 pengguna (anonimus akan tetapi memiliki informasi demografi), 1,149,780 rating dan 271,379 daftar buku. Semua data tersebut terbagi ke dalam 3 file berbeda berikut daftar serta parameter yang ada :

- File Users :

  File user ini merupakan file yang bersisi data pengguna berisi 278858 data pengguna. Semua nama pengguna dan ID pengguna sudah disamarkan karena hal ini berkaitan dengan masalah privasi. Awal sudah disebutkan bawah data ini hasil crawling data website resmi dan sudah mendapatkan persetujuan dari Ron Hornbaker, CTO of Humankind Systems (disebutkan di web Kaggle). Sehingga masalah privasi sangatlah ditekankan. Oleh karena itu pada projek ini berfokus pada User ID yang sudah diolah sesuai urutan data. Terdiri 3 fitur yaitu

  1. User ID

     Informasi ID pengguna yang sudah di anonimus dan diubah ke dalam bentuk integer sesuai dengan urutan data.

  2. Location

     Data demografi pengguna berisi tiga susunan yaitu lokasi alamat, kota dan negara dengan tipe data string.

  3. Age

     Data demografi pengguna berupa usia pengguna website BookCrossing dengan tipe data integer terdapat beberapa pengguna yang tidak mencantumkan usianya.

- File Books

  File Books terdiri dari 271379 data buku yang terdiri atas 8 kolom. Identifikasi buku umumnya diketahui dari nomor ISBN nya. Namun apabila terdapat ISBN yang tidak valid pada dataset ini ISBN tersebut dihilangkan. Beberapa informasi tambahan diambil dari Amazon Web Services. Berikut terdiri dari 8 fitur yang ada pada dataset Books yaitu

  1. ISBN

     Informasi nomor ISBN buku berisikan ID unik dari buku. Ada nomor ISBN yang sengaja dihilangkan oleh pembuat dataset karena termasuk nomor ISBN yang tidak valid. Pada dataset tipe datanya merupakan tipe data string.

  2. Book-Title

     Informasi mengenai judul buku dengan memiliki tipe data string.

  3. Book-Author

     Informasi mengenai penulis buku dengan memiliki tipe data string.

  4. Year-Of-Publication

     Informasi mengenai tahun dari buku tersebut dipublikasi memiliki tipe data integer.

  5. Publisher

     Informasi mengenai penerbit buku memiliki tipe data integer.

  6. Image-URL-S

     Informasi mengenai URL link gambar sampul depan buku dengan ukuran Small data ini berasal dari Amazon Website berisikan informasi URL.

  7. Image-URL-M

     Informasi mengenai URL link gambar sampul depan buku dengan ukuran Medium data ini berasal dari Amazon Website berisikan informasi URL.

  8. Image-URL-L

     Informasi mengenai URL link gambar sampul depan buku dengan ukuran Large data ini berasal dari Amazon Website berisikan informasi URL.

- File Ratings

  File Ratings terdiri dari 1,149,780 total rating. Rating buku dapat bersifat eksplisit yang di nilai dalam rentang 1 hingga 10 atau bersifat implisit yang dinilai dengan 0. Berikut terdiri dari 8 fitur yang ada pada dataset Books yaitu

  1. User ID

     Informasi ID pengguna yang sudah di anonimus dan diubah ke dalam bentuk integer sesuai dengan urutan data. Memiliki nilai unik dan terhubung dengan dataset Users.

  2. ISBN

     Informasi nomor ISBN buku berisikan ID unik dari buku. Ada nomor ISBN yang sengaja dihilangkan oleh pembuat dataset karena termasuk nomor ISBN yang tidak valid. Pada dataset tipe datanya merupakan tipe data string. ISBN ini terhubung dengan dataset Books.

  3. Book-Rating

     Informasi mengenai rating buku dengan memiliki tipe data integer. Memiliki nilai rentang 0 hingga 10.

Data-data diatas akan diperiksa terlebih dahulu untuk mendapatkan insight dari data sebelum melakukan ke tahapan data preparation. Penentuan variabel target akan menggunakan fitur Book-Rating dalam penentuan buku yang cocok serta sesuai dilihat juga kesamaan antar penulis maupun penerbit. Beberapa tahapan yang akan dilakukan untuk pemeriksaan dan pemahaman data diantaranya

1. Membaca Informasi dan Deskripsi Kolom pada Data
2. Melakukan Visualisasi Data untuk Cek Persebaran Data

   - Visualisasi Persebaran Data Usia

     ![visualUsia](https://raw.githubusercontent.com/Abito21/Proyek_Sistem_Rekomendasi_Website_Buku/main/pictures/visualUsia.png)

   - Visualisasi Persebaran Data Rating

     ![visualRating](https://raw.githubusercontent.com/Abito21/Proyek_Sistem_Rekomendasi_Website_Buku/main/pictures/visualRating.png)

3. Melakukan Exploratory Data Analysis Metode Univariate Analysis yaitu berdasarkan per variabel yang ada.

## Data Preparation

## Data Preparation

Data preparation yaitu tahapan untuk melakukan transformasi data agar sesuai atau dapat dengan mudah digunakan ketika modeling machine learning. Bagian data preparation yang umum dilakukan ada beberapa tahapan diantaranya:

- Menghilangkan Outlier Dataset Users Kolom Usia
- Menghilangkan NaN/null Dataset Users Kolom Usia dengan interpolate() linier
- Pembulatan Nilai Integer Kolom Usia Dataset Users
- Membuat Kolom Kategori Usia pada Dataset Users
- Menghilangkan NaN/null Dataset Books dengan dropna()
- Mencari Buku yang Paling Populer
- Filter Pengguna yang Aktif dan Buku yang Terkenal
- Pembuatan Matriks Fitur Content dengan Pivot Table

Tahapan diatas dijalankan secara berurutan dari mulai penghilangan outlier, menghapus nilai NaN kemudian menggabungkan beberapa fitur. Hanya beberapa fitur penting saja yang digunakan fokusnya pada data rating, kemudian perlu menggabungkan data judul buku serta kategori usia. Karena informasinya terbatas maka hubungan rating, judul buku serta usia dapat berdampak pada keputusan yang direkomendasikan sehigga perlu dibersihkan serta dipersiapkan dengan baik.

Berikut penjelasan tahapan diatas:

1. Menghilangkan Outlier dan Pembulatan Dataset Users Kolom Usia :
   Tahapan ini dilakukan untuk menghilangkan data outlier seperti usia yang diatas rata-rata manusia normal seperti usia 200 tahun. Rasanya tidak masuk akan dengan usia 200 tahun sehingga perlu dipisahkan atau usianya dibatasi hingga 100 tahun saja. Pembulatan dilakukan agar nilai datanya stabil.
2. Menghilangkan NaN/null Dataset Users Kolom Usia dengan interpolate() Linier :
   Tahapan dilakukan untuk menghilangkan nilai NaN maupun NULL pada data usia. Metode yang digunakan adalah interpolasi linier dengan cara mengisi nilai NaN dengan cara menghitung nilai rata-rata antara dua titik data yang ada di sekitar nilai yang hilang. Metode ini digunakan karena data NaN atau NULL pada fitur usia sangat banyak sehingga sangat disayangkan apabila datanya dibuang.
3. Pembulatan Nilai Integer Kolom Usia Dataset Users :
   Pembulatan dilakukan agar nilai datanya stabil karena tipe data aslinya ada float.
4. Membuat Kolom Kategori Usia pada Dataset Users :
   Tahapan ini dilakukan dalam upaya untuk membatasi nilai usia agar hanya terdapat beberapa kategori saja sehingga mudah untuk diidentifikasi hubungan usia dengan rekomendasi yang diberikan.
5. Menghilangkan NaN/null Dataset Books dengan dropna() :
   Menghilangkan nilai NULL atau NaN pada dataset book melalui tahapan data understanding diketahui bahwa data nya kisaran 2 hingga 3. Sehingga apabila dihapus tidak akan berdampak banyak.
6. Mencari Buku yang Paling Populer :  
   Tahapan ini dilakukan untuk mereduksi jumlah yang berisi ratusan ribuan bahkan jutaan bari data pada dataset rating diperkecil matriksnya agak mudah diolah. Hal ini berkaitan dengan keterbatasan teknologi yang penulis punya sehingga perlu mereduksi matriks dengan cara yang lebih tepat yaitu mengambil judul buku yang paling populer. Mencari buku yang paling populer dimulai dari penggabungan dataset Ratings dengan dataset Books.
7. Filter Pengguna yang Aktif dan Buku yang Terkenal :  
   Tahapan filter ini dimaksudkan untuk menyaring mana pengguna yang aktif dan tidak sehingga fokusnya adalah pada buku dengan rating tinggi dengan pengguna yang aktif menilai. Sedangkan buku yang terkenal bisa menjadi acuan dengan rating yang tinggi. Tahapan ini dilakukan untuk memperkecil matriks namun mampu menghasilkan rekomendasi yang kuat.
8. Pembuatan Matriks Fitur Content dengan Pivot Table :
Tahapan ini dilakukan untuk membentuk matriks hubungan antara User-ID, Book-Title dengan Book-Rating. Acuan dari sistem rekomendasi content based filtering adalah 3 fitur ini yang nanti hasilnya adalah bentuk similarity atau kesamaan yang diolah menggunakan cosine-similarity. Walaupun menggunakan pivot bisa dibilang manual dan mungkin belum bisa maksimal menghasilkan sistem rekomendasi, namun tujuannya adalah untuk mereduksi ukuran matriks agar lebih mudah diolah pada modeling. Menggunakan TF-IDF Vectorizer dengan jumlah data sekitar 200ribuan bahkan dataset Ratings berjumlah 1juta memiliki keterbatasan device untuk mengolah. Jauh lebih mudah dan ringan menggunakan pivot menggabungkan ketiga fitur User-ID, Book-Title dan Book-Rating.

## Modeling

## Model Development

## Modeling and Result

Bagian model development akan berfokus pada pembuatan model dengan

- Content Based Filtering yang terdiri dari tahapan

  1. Cosine Similarity

     Pada tahap ini, kita mengukur kemiripan antar item (misalnya, buku atau produk) berdasarkan karakteristik mereka menggunakan Cosine Similarity. Cosine similarity adalah metode untuk mengukur seberapa mirip dua vektor berdasarkan sudut antara keduanya, bukan panjangnya. Ini sangat berguna untuk menghitung kemiripan antara dua item meskipun panjang (magnitudo) fitur item berbeda. Untuk cosine similarity tinggal dijalankan karena matrik_vector sudah dibuat berdasarkan pivot User-ID, Book-Title dan Book-Rating

  2. Rekomendasi

     Rekomendasi terdiri beberapa bagian membuat tiga fungsi yaitu similarity yang dibagi dua berdasarkan jarak terdekat dan menggunakan korelasi koefisien paerson. Terakhir membentuk fungsi rekomendasi.

     - Fungsi Jarak Terdekat : membuat fungsi kemiripan suatu item berdasarkan jarak terdekatnya.
     - Fungsi Koefisien Korelasi Paerson : membuat fungsi berdasarkan koefisien korelasi paerson.

Hasil dari fungsi similarity yang dijalankan terdapat dua yaitu

- Fungsi Similarity berdasarkan Jarak Terdekat

  Fungsi sim_distance yang diberikan bertujuan untuk mengukur kemiripan antara dua buku menggunakan konsep jarak Euclidean terbalik berdasarkan rating pengguna pada buku tersebut. Fungsi ini digunakan dalam konteks sistem rekomendasi untuk menghitung seberapa mirip dua item (misalnya dua buku) berdasarkan rating yang diberikan oleh pengguna.

- Fungsi Similarity berdasarkan Korelasi Koefisien Paerson

  Pearson Correlation Coefficient, yaitu suatu ukuran statistik yang digunakan untuk mengukur derajat hubungan linier antara dua variabel. Dalam konteks sistem rekomendasi, Pearson Correlation digunakan untuk mengukur kemiripan antara dua item (misalnya, dua buku) berdasarkan rating yang diberikan oleh pengguna. Pearson Correlation Coefficient adalah angka yang berkisar antara -1 hingga 1, yang menunjukkan sejauh mana dua variabel saling berhubungan secara linier

Hasil dari kedua fungsi diatas menghasilkan rekomendasi yang berbeda sebagai berikut

![TopRekomendasi](https://raw.githubusercontent.com/Abito21/Proyek_Sistem_Rekomendasi_Website_Buku/main/pictures/topRekomendasi.png)

## Evaluation

Evaluasi yang digunakan pada projek ini adalah precision, recall dan f1-score yang mana relevan dengan data rekomendasi menggunakan metode content based filtering. Penjelasannya sebagai berikut:

- Precision mengukur seberapa banyak rekomendasi yang relevan dibandingkan dengan total rekomendasi yang diberikan.

  ![Precision](https://raw.githubusercontent.com/Abito21/Proyek_Sistem_Rekomendasi_Website_Buku/main/pictures/precision.png)

- Recall mengukur seberapa banyak item yang relevan yang berhasil direkomendasikan oleh sistem dibandingkan dengan total item relevan yang ada.

  ![Recall](https://raw.githubusercontent.com/Abito21/Proyek_Sistem_Rekomendasi_Website_Buku/main/pictures/recall.png)

- F1-Score adalah harmonik mean dari precision dan recall, yang memberi gambaran tentang keseimbangan antara keduanya. F1-Score sangat berguna ketika Anda ingin menjaga keseimbangan antara precision dan recall, terutama ketika ada ketidakseimbangan antara keduanya.

  ![F1Score](https://raw.githubusercontent.com/Abito21/Proyek_Sistem_Rekomendasi_Website_Buku/main/pictures/f1score.png)

Berikut hasil evaluasi metric precision, recall dan f1-score:

![Eval](https://raw.githubusercontent.com/Abito21/Proyek_Sistem_Rekomendasi_Website_Buku/main/pictures/evaluasiRekomendasi.png)

Jika dilihat melalui hasil precision, recall dan f1-score rekomendasi buku dengan buku yang relevan memiliki rekomendasi yang cukup dekat sekitar 60 hingga 70%. Membuktikan bahwa sistem rekomendasi yang dibuat memiliki kedekatan terhadap penilaian yang relevan.

## Referensi

[1] K. Purnachand. etc, "Predictive Maintenance of Machines and Industrial Equipment", IEEE, 2021.

[2] Matzka Stephan, "Explainable Artificial Intelligence for Predictive Maintenance Applications", IEEE, 2020.

[3] Petr Stodola and Jiˇrí Stodola, "Model of Predictive Maintenance of Machines and Equipment", IEEE, 2019.
