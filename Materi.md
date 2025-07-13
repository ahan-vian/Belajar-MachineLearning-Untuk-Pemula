# 1. Pengantar Machine Learning

## Apa Itu Machine Learning?

Machine Learning (ML) adalah cabang dari kecerdasan buatan (Artificial Intelligence/AI) yang memungkinkan komputer untuk belajar dari data, mengenali pola, dan membuat prediksi atau keputusan tanpa perlu diprogram secara eksplisit untuk setiap tugas.

Alih-alih mengikuti instruksi langkah demi langkah seperti dalam pemrograman tradisional, sistem ML membangun model matematis berdasarkan data historis untuk menemukan keterkaitan antar variabel, lalu menggunakannya dalam memproses data baru.

### Tujuan Machine Learning
Tujuan utama dari ML adalah:
- Menghasilkan **prediksi yang akurat** dari data baru.
- Mengurangi **ketergantungan pada aturan buatan manusia**.
- Membantu dalam pengambilan keputusan berbasis data.

### Perbedaan dengan Pemrograman Konvensional

| Pendekatan          | Pemrograman Konvensional          | Machine Learning                        |
|---------------------|-----------------------------------|------------------------------------------|
| Metode              | Aturan ditulis oleh manusia       | Aturan dipelajari dari data              |
| Data                | Masukan yang diproses             | Sumber pembelajaran                     |
| Output              | Hasil sesuai algoritma             | Model/prediksi berdasarkan pola          |
| Contoh Aplikasi     | Kalkulator, sistem inventori      | Deteksi spam, prediksi cuaca             |

### Contoh Sederhana
Bayangkan Anda ingin membuat sistem untuk mengenali buah dari gambar. Dalam pendekatan tradisional, Anda harus menulis aturan berdasarkan bentuk, warna, dan ukuran. Dalam Machine Learning, Anda hanya perlu mengumpulkan data (gambar buah beserta labelnya), dan model akan belajar sendiri pola yang membedakan apel dari jeruk atau pisang.

### Aplikasi Machine Learning di Dunia Nyata
- **Rekomendasi Produk:** Netflix, Spotify, YouTube
- **Deteksi Penipuan:** Sistem perbankan dan kartu kredit
- **Pengolahan Bahasa Alami:** Chatbot, asisten virtual
- **Prediksi Harga:** Saham, rumah, kebutuhan logistik
- **Kesehatan:** Deteksi dini penyakit dari citra medis

### Kategori Umum Machine Learning
Machine Learning terbagi menjadi tiga pendekatan utama:
- Supervised Learning
- Unsupervised Learning
- Reinforcement Learning

Setiap pendekatan akan dijelaskan pada bagian berikutnya.

### Ringkasan
- Machine Learning adalah pendekatan berbasis data yang membangun model matematis dari contoh-contoh masa lalu.
- ML berbeda dari pemrograman tradisional karena tidak membutuhkan aturan eksplisit.
- Dengan Machine Learning, komputer belajar dari data untuk melakukan klasifikasi, regresi, deteksi, dan prediksi otomatis.

## Tiga Jenis Utama dalam Machine Learning

Machine Learning dapat diklasifikasikan ke dalam tiga pendekatan utama berdasarkan bentuk data dan cara model belajar:

1. **Supervised Learning (Pembelajaran Terawasi)**
2. **Unsupervised Learning (Pembelajaran Tak Terawasi)**
3. **Reinforcement Learning (Pembelajaran Penguatan)**

Setiap pendekatan memiliki karakteristik dan kegunaan yang berbeda. Berikut penjelasannya:


### 1. Supervised Learning

**Definisi:**
Supervised learning adalah metode pembelajaran di mana model dilatih menggunakan dataset yang sudah memiliki label (jawaban). Model belajar mengenali hubungan antara input (fitur) dan output (label), sehingga dapat membuat prediksi terhadap data baru.

**Contoh Kasus:**
- Memprediksi harga rumah berdasarkan luas dan lokasi
- Mengklasifikasikan email sebagai spam atau bukan spam
- Mendeteksi penyakit berdasarkan gejala

**Ciri Khas:**
- Dataset terdiri dari fitur (X) dan label (y)
- Model belajar dari contoh berlabel
- Cocok untuk tugas klasifikasi dan regresi

**Analogi:**
Seperti siswa yang belajar dari buku latihan soal dan kunci jawaban. Ia belajar pola dari soal dan jawaban yang benar, sehingga saat diberikan soal baru, ia bisa menjawab dengan benar karena sudah mengenal polanya.

**Ilustrasi Dataset:**

| Ukuran Rumah (m²) | Lokasi     | Harga (Rp)        |
|-------------------|------------|-------------------|
| 100               | Bandung    | 850.000.000       |
| 80                | Jakarta    | 1.200.000.000     |

Model akan belajar: "Jika ukuran rumah besar dan lokasinya strategis, maka harganya cenderung tinggi."


### 2. Unsupervised Learning

**Definisi:**
Unsupervised learning digunakan saat data **tidak memiliki label**. Model bertugas mencari pola tersembunyi, struktur, atau pengelompokan di dalam data tanpa arahan eksplisit.

**Contoh Kasus:**
- Mengelompokkan pelanggan berdasarkan kebiasaan belanja
- Segmentasi pasar dalam marketing
- Visualisasi dan reduksi dimensi data

**Ciri Khas:**
- Data hanya memiliki input (fitur), tanpa label
- Tujuan utama adalah eksplorasi dan pengelompokan
- Cocok untuk clustering dan analisis eksploratif

**Analogi:**
Seperti seseorang yang baru pertama kali datang ke kota asing tanpa peta. Ia tidak tahu lokasi restoran, toko, atau taman, tapi dengan mengamati lingkungan, ia bisa mulai mengelompokkan area berdasarkan pola yang dilihat.

**Ilustrasi:**
Diberikan data tinggi dan berat dari ribuan orang, model dapat mengelompokkan individu ke dalam kategori seperti kurus, normal, atau obesitas tanpa mengetahui label aslinya.


### 3. Reinforcement Learning

**Definisi:**
Reinforcement learning adalah metode di mana agen (komputer atau robot) belajar dari pengalaman dengan berinteraksi langsung dengan lingkungan. Agen akan mencoba berbagai aksi dan menerima **umpan balik berupa reward (imbalan)** atau **penalty (hukuman)** untuk menentukan strategi terbaik dalam jangka panjang.

**Contoh Kasus:**
- Robot belajar bergerak atau berjalan
- AI bermain game (catur, Go, Dota)
- Sistem rekomendasi yang menyesuaikan dengan perilaku pengguna secara dinamis

**Ciri Khas:**
- Tidak ada label tetap
- Pembelajaran melalui feedback lingkungan
- Cocok untuk pengambilan keputusan sekuensial

**Analogi:**
Seperti melatih hewan peliharaan. Jika anjing duduk ketika diperintah, ia diberi camilan (reward). Jika tidak, ia diabaikan. Lama kelamaan, anjing belajar bahwa duduk akan memberinya camilan, dan ia mengulang perilaku tersebut.

**Ilustrasi:**
Dalam permainan video game, AI mencoba berbagai strategi. Jika berhasil menang, ia mendapatkan poin (reward). Jika kalah, poinnya berkurang. Dari sini, AI belajar strategi terbaik melalui banyak percobaan.


### Ringkasan Perbandingan

| Aspek               | Supervised Learning           | Unsupervised Learning        | Reinforcement Learning         |
|---------------------|-------------------------------|-------------------------------|---------------------------------|
| Tipe Data           | Berlabel (X, y)               | Tidak berlabel (X)           | Interaksi dan feedback         |
| Tujuan              | Prediksi / Klasifikasi        | Klasterisasi / Pola Data     | Strategi optimal jangka panjang|
| Proses Belajar      | Dari contoh & jawaban         | Dari struktur data           | Dari trial & error             |
| Evaluasi            | Akurasi, error, loss          | Visualisasi, Silhouette      | Total reward                   |
| Contoh              | Prediksi harga, spam detection| Segmentasi pelanggan         | AI bermain game, robot navigasi|


## Dataset: Fitur (X) dan Label (y)

Dalam Machine Learning, dataset adalah kumpulan data yang digunakan sebagai bahan untuk melatih dan menguji model. Setiap baris dalam dataset biasanya merepresentasikan satu observasi atau contoh, yang terdiri dari fitur (X) dan, dalam kasus supervised learning, label (y).


### Apa Itu Fitur (X)?

**Fitur** adalah atribut, karakteristik, atau variabel input yang menjelaskan sebuah data atau observasi. Fitur bisa berupa nilai numerik, kategori, teks, tanggal, atau kombinasi dari semuanya.

**Contoh:**
Dalam kasus prediksi harga rumah, fitur bisa berupa:
- Luas rumah (dalam m²)
- Jumlah kamar
- Lokasi
- Tahun dibangun

**Ilustrasi Tabel Fitur:**

| Luas (m²) | Kamar | Lokasi     |
|-----------|--------|------------|
| 120       | 3      | Bandung    |
| 80        | 2      | Jakarta    |

Fitur-fitur ini akan digunakan sebagai input bagi model untuk membuat prediksi.

**Analogi:**
Bayangkan kamu menjadi detektif yang mencoba menyimpulkan siapa pelaku kejahatan. Fitur adalah semua petunjuk yang kamu kumpulkan: jejak kaki, sidik jari, waktu kejadian. Kamu belum tahu siapa pelakunya (label), tapi kamu punya semua petunjuk (fitur).


### Apa Itu Label (y)?

**Label** adalah hasil atau target yang ingin diprediksi oleh model berdasarkan fitur yang tersedia. Label hanya tersedia dalam supervised learning.

**Contoh:**
Masih dalam kasus prediksi harga rumah, labelnya adalah:
- Harga rumah (dalam rupiah)

**Ilustrasi Dataset Lengkap:**

| Luas (m²) | Kamar | Lokasi     | **Harga (Rp)**     |
|-----------|--------|------------|--------------------|
| 120       | 3      | Bandung    | 850.000.000        |
| 80        | 2      | Jakarta    | 1.200.000.000      |

Di sini, "Harga" adalah label (y), dan sisanya adalah fitur (X).

**Analogi:**
Fitur adalah soal ujian, label adalah kunci jawabannya. Saat melatih model, kita ingin model belajar cara menghubungkan soal (fitur) dengan jawaban (label), sehingga saat diberi soal baru, ia bisa menjawab dengan benar.


### Hubungan antara Fitur dan Label

Tujuan utama supervised learning adalah untuk **mempelajari fungsi atau hubungan antara X dan y**. Dengan kata lain, model belajar:  
$$y = f(X)$$  
yang berarti: _"berikan saya fitur (X), saya akan prediksi label (y).”_

**Contoh Kasus Lain:**
- **Input (X):** tinggi badan, berat badan, usia  
  **Output (y):** apakah seseorang menderita diabetes (ya/tidak)

- **Input (X):** kata-kata dalam kalimat  
  **Output (y):** apakah kalimat tersebut positif atau negatif (sentiment analysis)


### Pentingnya Memahami Fitur dan Label

- Kualitas fitur akan sangat menentukan kemampuan model dalam mempelajari pola.
- Label harus benar-benar merepresentasikan target yang ingin diprediksi.
- Jika fitur tidak relevan atau label salah, maka model yang dilatih tidak akan berguna (garbage in, garbage out).


### Ringkasan

- **Fitur (X)** adalah data input yang menjelaskan karakteristik dari suatu kasus.
- **Label (y)** adalah data output yang menjadi target prediksi.
- Dalam supervised learning, kita melatih model untuk mengenali hubungan antara fitur dan label.
- Pemahaman yang tepat tentang fitur dan label adalah dasar penting dalam semua proyek Machine Learning yang sukses.

## Overfitting vs Underfitting

Salah satu tantangan utama dalam Machine Learning adalah memastikan bahwa model tidak hanya bekerja baik pada data pelatihan, tetapi juga mampu mengeneralisasi ke data baru. Dua masalah umum yang sering muncul adalah **overfitting** dan **underfitting**.


### Apa Itu Underfitting?

**Underfitting** terjadi ketika model terlalu sederhana untuk menangkap pola dalam data. Model gagal mempelajari hubungan yang bermakna antara fitur dan label.

**Ciri-ciri:**
- Akurasi rendah pada data pelatihan maupun data pengujian
- Error tinggi secara konsisten
- Model tidak menangkap pola penting dari data

**Penyebab umum:**
- Model terlalu sederhana (misalnya regresi linier untuk pola non-linier)
- Terlalu sedikit fitur atau informasi
- Waktu pelatihan terlalu singkat

**Analogi:**
Seperti siswa yang belajar hanya satu halaman sebelum ujian. Ia tidak cukup paham, sehingga menjawab banyak soal dengan salah, bahkan soal latihan yang sudah dilihat sebelumnya.


### Apa Itu Overfitting?

**Overfitting** terjadi ketika model terlalu kompleks sehingga tidak hanya belajar pola utama, tetapi juga “menghafal” noise atau detail spesifik dalam data pelatihan. Akibatnya, performa pada data pelatihan sangat baik, tetapi buruk pada data pengujian.

**Ciri-ciri:**
- Akurasi sangat tinggi pada data pelatihan
- Akurasi rendah pada data pengujian
- Gap besar antara training loss dan testing loss

**Penyebab umum:**
- Model terlalu kompleks untuk ukuran data
- Terlalu lama melatih model (training terlalu banyak epoch)
- Tidak ada regularisasi

**Analogi:**
Seperti siswa yang hafal soal latihan dengan sangat detail, tetapi bingung saat soal ujian sedikit berubah. Ia tahu jawaban lama, tapi tidak paham konsepnya.


### Visualisasi Sederhana (dalam Kata)

Bayangkan kamu memetakan titik data ke dalam grafik:

- **Underfitting:** Garis lurus yang tidak mengikuti pola titik — model terlalu sederhana.
- **Overfitting:** Garis berliku-liku mengikuti semua titik secara sempurna — model terlalu rumit.
- **Model ideal:** Kurva yang mengikuti tren umum titik-titik, tanpa terlalu kaku atau terlalu fleksibel.


### Evaluasi dengan Error

Untuk mengidentifikasi overfitting dan underfitting, bandingkan error/loss pada data pelatihan dan pengujian:

$$
\text{Underfitting:} \quad \text{Training Error tinggi}, \quad \text{Testing Error tinggi}
$$

$$
\text{Overfitting:} \quad \text{Training Error rendah}, \quad \text{Testing Error tinggi}
$$

$$
\text{Good Fit:} \quad \text{Training Error rendah}, \quad \text{Testing Error rendah}
$$


### Cara Mengatasi
**Underfitting:**

- Gunakan model yang lebih kompleks

- Tambahkan lebih banyak fitur relevan

- Latih model lebih lama

- Gunakan transformasi non-linier (misalnya polinomial)

**Overfitting:**

- Kurangi kompleksitas model (jumlah parameter, layer, dll.)

- Gunakan teknik regularisasi (L1, L2, Dropout)

- Tambahkan data pelatihan (data augmentation)

- Gunakan early stopping selama pelatihan

### Ringkasan
| Aspek           | Underfitting               | Overfitting                                |
| --------------- | -------------------------- | ------------------------------------------ |
| Tingkat Belajar | Terlalu rendah             | Terlalu tinggi                             |
| Training Error  | Tinggi                     | Rendah                                     |
| Testing Error   | Tinggi                     | Tinggi                                     |
| Penyebab        | Model terlalu sederhana    | Model terlalu kompleks                     |
| Solusi          | Tambah kompleksitas, fitur | Kurangi kompleksitas, gunakan regularisasi |


Memahami dan mengendalikan overfitting serta underfitting adalah langkah penting untuk menghasilkan model Machine Learning yang stabil, efisien, dan mampu mengeneralisasi dengan baik pada data baru.


## Pembagian Data: Train, Validation, dan Test Set

Dalam Machine Learning, tujuan utama adalah membangun model yang mampu mengeneralisasi, yaitu bekerja baik tidak hanya pada data pelatihan, tetapi juga pada data baru. Oleh karena itu, dataset harus dibagi ke dalam tiga bagian utama:

1. **Training Set**
2. **Validation Set**
3. **Test Set**


### 1. Training Set

**Training set** adalah bagian dari data yang digunakan untuk melatih model. Model akan mempelajari hubungan antara fitur (X) dan label (y) dari data ini, dengan menyesuaikan bobot/parameter untuk meminimalkan error.

**Peran:**
- Digunakan untuk menghitung loss selama training
- Tempat model belajar mengenali pola

**Analogi:**
Bayangkan training set sebagai buku pelajaran yang kamu baca sebelum ujian. Di sinilah kamu belajar konsep, pola, dan latihan soal.

**Contoh Pembagian:**
Jika dataset memiliki 1000 data, dan 70% digunakan untuk training:

$$
\text{Training Size} = 0.7 \times 1000 = 700 \text{ data}
$$


### 2. Validation Set

**Validation set** digunakan untuk mengevaluasi performa model selama pelatihan, **tanpa digunakan dalam proses pelatihan langsung**. Validation set penting untuk melakukan:
- Hyperparameter tuning (misal: learning rate, jumlah neuron, jumlah tree)
- Pemantauan overfitting (performa meningkat di training tapi menurun di validation)
- Early stopping

**Analogi:**
Validation set seperti **try out** sebelum ujian sebenarnya. Ia membantu kita mengecek apakah model benar-benar belajar, atau hanya menghafal.

### 3. Test Set

**Test set** adalah bagian data yang **tidak pernah disentuh** selama pelatihan. Data ini digunakan untuk mengukur performa akhir model dan **menilai kemampuannya menghadapi data baru**.

**Peran:**
- Digunakan satu kali di akhir pelatihan
- Memberi gambaran realistis tentang kemampuan generalisasi model

**Analogi:**
Test set adalah seperti **ujian nasional**: hanya digunakan sekali, dan menentukan seberapa baik model benar-benar belajar.


### Skema Pembagian Umum

| Set         | Tujuan                                | Proporsi Umum |
|-------------|----------------------------------------|----------------|
| Training    | Melatih model                          | 60–80%         |
| Validation  | Evaluasi selama pelatihan              | 10–20%         |
| Test        | Evaluasi akhir (generalisasi)          | 10–20%         |

**Contoh Pembagian 70/15/15:**

- 70% untuk training
- 15% untuk validation
- 15% untuk test


### Ilustrasi Fungsi Evaluasi

Misalkan model kita dievaluasi dengan Mean Squared Error (MSE), maka kita hitung:

Misalkan model kita dievaluasi dengan Mean Squared Error (MSE), maka kita hitung:

- Training Error:
  $
  \text{MSE}_{\text{train}} = \frac{1}{n_{\text{train}}} \sum_{i=1}^{n_{\text{train}}} (y_i - \hat{y}_i)^2
  $

- Validation Error:
  $
  \text{MSE}_{\text{val}} = \frac{1}{n_{\text{val}}} \sum_{i=1}^{n_{\text{val}}} (y_i - \hat{y}_i)^2
  $

- Test Error:
  $
  \text{MSE}_{\text{test}} = \frac{1}{n_{\text{test}}} \sum_{i=1}^{n_{\text{test}}} (y_i - \hat{y}_i)^2
  $


### Alternatif: Cross-Validation

Jika data terlalu sedikit, pembagian train/validation/test bisa mengurangi data yang tersedia. Solusinya adalah **cross-validation**, terutama **K-Fold Cross Validation**, yang akan dibahas di bagian evaluasi model.


### Ringkasan

- **Training set** digunakan untuk melatih model.
- **Validation set** digunakan untuk mengevaluasi performa selama pelatihan dan tuning hyperparameter.
- **Test set** digunakan satu kali untuk mengevaluasi performa akhir model.
- Pembagian data yang tepat membantu mencegah overfitting dan meningkatkan generalisasi model.

# 2. Preprocessing Data

Pra-pemrosesan data (data preprocessing) adalah tahap penting sebelum data digunakan dalam pelatihan model Machine Learning. Tujuan utama preprocessing adalah memastikan bahwa data berada dalam format yang bersih, konsisten, dan dapat diproses oleh algoritma dengan efektif.

Beberapa langkah umum dalam preprocessing antara lain:
- Normalisasi
- Encoding data kategorikal
- Penanganan missing value
- Feature engineering dan feature selection

## 2.1 Normalisasi: MinMaxScaler vs StandardScaler

### Mengapa Normalisasi Penting?

Banyak algoritma Machine Learning, seperti K-Nearest Neighbors (KNN), Support Vector Machine (SVM), dan Neural Network, sangat sensitif terhadap skala fitur. Tanpa normalisasi, fitur dengan skala besar dapat mendominasi perhitungan dan menyebabkan model bias.

### Analogi

Bayangkan kamu adalah pelatih sepak bola yang menilai pemain berdasarkan:
- Kecepatan lari (dalam detik)
- Tinggi badan (dalam cm)
- Gaji bulanan (dalam juta rupiah)

Tanpa normalisasi, model mungkin menganggap gaji lebih penting hanya karena angkanya jauh lebih besar, padahal kecepatan jauh lebih relevan. Normalisasi menyetarakan skala semua fitur agar model memperlakukan semuanya secara adil.

### MinMaxScaler

**Tujuan:** Mengubah skala nilai fitur agar berada dalam rentang [0, 1].

**Rumus:**

$$
x_{\text{scaled}} = \frac{x - x_{\text{min}}}{x_{\text{max}} - x_{\text{min}}}
$$

**Karakteristik:**
- Rentang output selalu antara 0 dan 1
- Sangat sensitif terhadap outlier
- Cocok jika data memiliki rentang nilai tetap dan stabil

**Contoh:**
Jika data suhu berkisar antara 20°C hingga 40°C dan nilai saat ini adalah 30°C:

$$
x_{\text{scaled}} = \frac{30 - 20}{40 - 20} = 0.5
$$

**Analogi:**  
Seperti mengubah semua tinggi pemain ke dalam skala 0–1, di mana 0 adalah pemain terpendek dan 1 adalah tertinggi. Ini memungkinkan perbandingan yang adil antar pemain.

### StandardScaler (Z-Score Normalization)

**Tujuan:** Mengubah fitur agar memiliki nilai rata-rata 0 dan standar deviasi 1.

**Rumus:**

$$
x_{\text{scaled}} = \frac{x - \mu}{\sigma}
$$

dengan:
- $\( \mu \)$ adalah rata-rata (mean)
- $\( \sigma \)$ adalah standar deviasi dari fitur

**Karakteristik:**
- Output tidak dibatasi ke rentang tertentu
- Lebih tahan terhadap outlier dibanding MinMax
- Cocok jika data mengikuti distribusi normal (gaussian)

**Contoh:**
Jika rata-rata berat badan adalah 60 kg dan standar deviasinya 10 kg, maka berat 70 kg akan menjadi:

$$
x_{\text{scaled}} = \frac{70 - 60}{10} = 1.0
$$

**Analogi:**  
Seperti mengukur seberapa jauh nilai seseorang dari rata-rata. Nilai 0 berarti standar, positif berarti di atas rata-rata, dan negatif berarti di bawah.

### Perbandingan MinMax vs StandardScaler

| Aspek                  | MinMaxScaler               | StandardScaler                |
|------------------------|----------------------------|-------------------------------|
| Rentang hasil          | 0 hingga 1                 | Tidak terbatas                |
| Sensitif terhadap outlier | Ya                     | Tidak terlalu                 |
| Cocok untuk            | Data stabil, range tetap   | Data normal atau bervariasi   |
| Distribusi data        | Tidak diperhitungkan       | Menyesuaikan distribusi       |

### Kesimpulan

- Normalisasi membantu model memperlakukan semua fitur secara setara.
- Gunakan MinMaxScaler jika data tidak memiliki outlier dan berada dalam rentang yang tetap.
- Gunakan StandardScaler jika data memiliki distribusi normal atau outlier yang signifikan.
- Pilih metode normalisasi sesuai dengan jenis data dan algoritma yang digunakan.
