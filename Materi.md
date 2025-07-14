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
  {
  \text{MSE}_{\text{train}} = \frac{1}{n_{\text{train}}} \sum_{i=1}^{n_{\text{train}}} (y_i - \hat{y}_i)^2
  }
  $

- Validation Error:
  $
  {
  \text{MSE}_{\text{val}} = \frac{1}{n_{\text{val}}} \sum_{i=1}^{n_{\text{val}}} (y_i - \hat{y}_i)^2
  }
  $

- Test Error:
  $
  {
  \text{MSE}_{\text{test}} = \frac{1}{n_{\text{test}}} \sum_{i=1}^{n_{\text{test}}} (y_i - \hat{y}_i)^2
  }
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
- ${\( \mu \)}$ adalah rata-rata (mean)
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


## 2.2 Encoding: Label, One-Hot, Ordinal

Sebagian besar algoritma Machine Learning hanya dapat memproses data numerik. Oleh karena itu, data kategorikal (seperti warna, jenis, kelas, status) harus diubah menjadi angka melalui proses yang disebut **encoding**.

Encoding sangat penting untuk mencegah kesalahan interpretasi model terhadap nilai kategori.

### Analogi

Bayangkan kamu sedang mengisi formulir pendaftaran yang menanyakan pekerjaan:
- Pelajar
- Karyawan
- Wirausaha

Jika sistem tidak bisa membaca huruf, maka setiap pilihan harus dikonversi menjadi angka atau kode agar bisa diproses. Proses pengubahan ini disebut encoding.

### 1. Label Encoding

Label Encoding mengubah setiap kategori menjadi nilai bilangan bulat unik.

**Contoh:**

| Warna   | Encoded |
|---------|---------|
| Merah   | 0       |
| Hijau   | 1       |
| Biru    | 2       |

**Karakteristik:**
- Sederhana dan efisien
- Cocok untuk data ordinal
- Tidak cocok untuk data nominal karena memberi kesan adanya urutan

**Risiko:**  
Model dapat menganggap bahwa "Biru > Hijau > Merah", padahal tidak ada hubungan numerik antara kategori tersebut.

### 2. One-Hot Encoding

One-Hot Encoding mengubah setiap kategori menjadi vektor biner, di mana hanya satu elemen bernilai 1 dan sisanya 0.  
| Warna | Merah | Hijau | Biru |
| ----- | ----- | ----- | ---- |
| Merah | 1     | 0     | 0    |
| Hijau | 0     | 1     | 0    |
| Biru  | 0     | 0     | 1    |

**Karakteristik**
- Tidak memperkenalkan urutan palsu
- Cocok untuk data nominal

**Resiko**  
Bisa membuat data terlalu besar yang dapat menyebabkan overfitting

### 3. Ordinal Encoding
Ordinal Encoding digunakan untuk data kategorikal yang memang memiliki tingkatan atau urutan logis. Mirip label encoding, tapi urutan sengaja didefinisikan karena memang ada tingkatan logis.

contoh : 

| Ukuran Baju | Encoded |
| ----------- | ------- |
| Kecil       | 1       |
| Sedang      | 2       |
| Besar       | 3       |

**Karakteristik**
- Menghormati urutan logis
- Cocok untuk fitur seperti level pendidikan, rating, atau ukuran

**Perbandingan Metode Encoding**
| Metode           | Cocok Untuk  | Keunggulan                     | Kekurangan                    |
| ---------------- | ------------ | ------------------------------ | ----------------------------- |
| Label Encoding   | Data ordinal | Ringkas dan cepat              | Menimbulkan urutan semu       |
| One-Hot Encoding | Data nominal | Akurat, tidak ada urutan palsu | Dimensi tinggi (kolom banyak) |
| Ordinal Encoding | Data ordinal | Menangkap tingkatan logis      | Tidak cocok untuk data acak   |

**Kesimpulan**
- Gunakan **Label Encoding** hanya jika data memiliki sedikit kategori dan tidak akan menyebabkan makna urutan yang keliru.
- Gunakan **One-Hot Encoding** untuk kategori bebas tanpa urutan seperti warna, kota, atau jenis barang.
- Gunakan **Ordinal Encoding** jika kategori memiliki urutan seperti kecil → sedang → besar atau level pendidikan.


## 2.3 Missing Value: Drop, Imputasi, Model-based

Dalam praktik nyata, dataset sering kali tidak lengkap. Nilai yang hilang disebut sebagai **missing value**, dan dapat menyebabkan algoritma Machine Learning gagal berfungsi atau menghasilkan prediksi yang tidak akurat.

Menangani missing value secara tepat adalah langkah penting dalam preprocessing data.

### Analogi

Bayangkan kamu sedang memasak berdasarkan resep, tetapi beberapa bahan tidak disebutkan. Jika kamu tetap memasak tanpa menangani bagian yang hilang, hasil masakan bisa gagal total. Begitu juga dengan data: jika ada informasi yang hilang dan tidak ditangani, model tidak akan belajar dengan baik.

### Penyebab Missing Value

- Sensor gagal merekam data
- Pengguna tidak mengisi formulir
- Data rusak saat diambil atau disimpan
- Format input tidak sesuai saat proses penggabungan data


### 1. Drop (Menghapus Data yang Hilang)

Cara termudah adalah menghapus baris atau kolom yang memiliki nilai kosong.

**Kapan digunakan:**
- Jumlah missing value sangat kecil
- Kolom atau baris tersebut tidak penting

**Risiko:**
- Mengurangi jumlah data
- Bisa membuang informasi penting

### 2. Imputasi Sederhana (Mean/Median/Modus)

Mengisi nilai yang hilang dengan statistik sederhana seperti :
- **Mean( rata-rata )** untuk data numerik
- **Median** jika data memiliki outlier
- **Modus( nilai terbanyak )** untuk data kategorikal

**Kapan digunakan ?**
- Proporsi missing value sedang
- Distribusi data diketahui atau stabil

### 3. Imputasi Berdasarkan Model

Menggunakan Machine Learning untuk memperkirakan nilai yang hilang berdasarkan fitur lain.

**Contoh teknik:**
- Regresi Linear
- K-Nearest Neigbors (KNN)
- Decision Tree

**Kapan Digunakan:**
- Banyak data hilang pada fitur penting
- fitur lain saling berkorelasi

### 4. Imputasi Konstanta / Placeholder
Mengisi nilai kosong dengan nilai tetap, seperti:
- 0, -999, "Unknown", atau "None"
- Ditambah kolom flag misalnya is_missing

**Kapan digunakan:**
- Saat ingin memberi sinyal eksplisit ke model bahwa nilai tersebut memang hilang

**Strategi berdasarkan kondisi:**
- Jika **jumlah data hilang < 5%** → gunakan **imputasi**
- Jika **hilang > 50%** dan tidak penting,  pertimbangkan untuk **dibuang**
- Jika fitur **sangat penting dan banyak yang hilang**  pertimbangkan **imputasi model-based**

**Ringkasan Mode**
| Metode            | Cocok Saat...                       | Keunggulan                          | Kekurangan                           |
| ----------------- | ----------------------------------- | ----------------------------------- | ------------------------------------ |
| Drop              | Data hilang sedikit                 | Sederhana dan cepat                 | Kehilangan informasi                 |
| Mean/Median/Modus | Data cukup stabil                   | Efisien                             | Tidak memperhitungkan fitur lain     |
| Model-based       | Data penting dan saling berkorelasi | Akurat, mempertimbangkan fitur lain | Lebih kompleks dan berat             |
| Konstanta / Flag  | Butuh penanda eksplisit             | Bisa dilacak oleh model             | Bisa bias jika digunakan sembarangan |

**Kesimpulan**
- Missing value adalah hal umum dalam data nyata dan harus ditangani dengan hati-hati.

- Ada berbagai metode untuk menangani missing value, mulai dari menghapus, mengisi statistik, hingga prediksi berbasis model.

- Pemilihan metode tergantung pada jumlah data yang hilang, pentingnya fitur, dan hubungan antar fitur lainnya.

## 2.4 Feature Engineering & Feature Selection

Dalam Machine Learning, kualitas input (fitur) sangat menentukan kualitas output (prediksi). Model yang baik dengan fitur yang buruk tetap akan memberikan hasil yang tidak akurat. Oleh karena itu, dua proses penting dalam preprocessing adalah:

- **Feature Engineering**: membuat atau memodifikasi fitur agar lebih informatif.
- **Feature Selection**: memilih fitur yang paling relevan dan menghapus yang tidak penting.

### Apa Itu Fitur?

Fitur (feature) adalah variabel input yang diberikan kepada model untuk dipelajari. Setiap fitur membawa informasi yang (semoga) berguna dalam menentukan nilai target (label).

Contoh dalam prediksi harga rumah:
- Luas bangunan
- Jumlah kamar
- Lokasi
- Tahun dibangun

### Analogi

Bayangkan kamu sedang memasak. Bahan mentah (fitur asli) belum tentu langsung cocok untuk dimasak. Kamu perlu mencuci, mengiris, atau bahkan mencampur bahan agar hasil akhirnya lezat. Proses ini sama seperti feature engineering — mengolah data mentah menjadi input yang siap digunakan model.

---

### Feature Engineering

**Tujuan:** menciptakan fitur baru, membersihkan, atau mentransformasi fitur lama agar model dapat belajar lebih baik.

**Contoh Teknik:**
- **Transformasi Nilai:**  
  Log transform untuk meratakan sebaran nilai
- **Ekstraksi Tanggal/Waktu:**  
  Dari `tanggal` → `bulan`, `hari`, `hari_ke_dalam_minggu`
- **Interaksi Antar Fitur:**  
  Harga per meter = `harga total` / `luas tanah`
- **Pembuatan Fitur Baru:**  
  Dari `tanggal lahir` → hitung `usia`

### Feature Selection

**Tujuan** nya untuk memilih subset fitur yang paling relevan dan menghapus fitur yang tidak berguna atau mengganggu.  
**Mengapa penting?**  
- Mengurangi overfitting

- Mempercepat pelatihan

- Meningkatkan interpretabilitas model

**Contoh Teknik:**

**Filter Method**
Korelasi Pearson, Chi-Square, ANOVA

**Wrapper Method**
Recursive Feature Elimination (RFE)

**Embedded Method**
Lasso Regression (L1 Regularization) yang otomatis menekan bobot fitur tidak penting menjadi nol

Contoh L1 Regularization (Lasso):

$$
Loss=MSE+λ∑∣wi∣\text{Loss}
$$

**Perbandingan Feature Engineering vs Feature Selection**
| Proses              | Tujuan                              | Teknik Utama                      |
| ------------------- | ----------------------------------- | --------------------------------- |
| Feature Engineering | Meningkatkan kualitas fitur         | Transformasi, kombinasi, derivasi |
| Feature Selection   | Mengurangi fitur yang tidak berguna | Korelasi, RFE, regularisasi L1/L2 |

**Tips Praktis**
- Jangan terlalu banyak fitur tanpa alasan. Terlalu banyak fitur justru bisa menyebabkan noise dan overfitting.

- Pahami domain masalah untuk menciptakan fitur yang bermakna.

- Gunakan seleksi otomatis (misal: Lasso, Random Forest feature importance) untuk memfilter fitur setelah proses rekayasa.

- Uji performa model sebelum dan sesudah pemilihan fitur.

**Kesimpulan**  
- Feature Engineering membantu menciptakan fitur yang lebih kuat dan bermakna dari data mentah.

- Feature Selection membantu menyaring fitur yang benar-benar penting untuk meningkatkan efisiensi dan akurasi model.

- Kedua proses ini sangat penting untuk membangun model Machine Learning yang andal dan hemat sumber daya.

# 3. Evaluasi Model

Setelah model Machine Learning dilatih, kita perlu mengevaluasi performanya — tidak hanya pada data pelatihan, tetapi juga pada data yang belum pernah dilihat sebelumnya. Evaluasi model sangat penting untuk:

- Mengetahui apakah model bekerja dengan baik
- Menghindari overfitting atau underfitting
- Membandingkan beberapa model untuk memilih yang terbaik

Metode evaluasi tergantung pada jenis tugas: klasifikasi atau regresi.

## 3.1 Evaluasi Model Klasifikasi

Untuk tugas klasifikasi (biner atau multikelas), kita menggunakan metrik seperti:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

### Confusion Matrix

Confusion Matrix adalah tabel yang menunjukkan hasil prediksi model terhadap data sebenarnya dalam bentuk perhitungan **benar/salah** dan **positif/negatif**.

|                    | Prediksi Positif | Prediksi Negatif |
|--------------------|------------------|------------------|
| **Data Positif**   | True Positive (TP) | False Negative (FN) |
| **Data Negatif**   | False Positive (FP)| True Negative (TN)  |

### Analogi

Bayangkan model adalah dokter dan tugasnya mendeteksi penyakit serius:
- **TP**: Dokter mendeteksi pasien sakit yang memang sakit → benar
- **FP**: Dokter bilang pasien sakit, padahal sehat → false alarm
- **FN**: Dokter bilang sehat, padahal pasien sakit → ini sangat berbahaya
- **TN**: Dokter bilang sehat, dan memang sehat → benar

### Accuracy

**Akurasi** menunjukkan seberapa sering model membuat prediksi yang benar.

$$
\text{Accuracy} = \frac{TP + TN}{TP + TN + FP + FN}
$$

Cocok jika distribusi data seimbang.

### Precision

**Precision** menunjukkan dari semua prediksi positif, berapa banyak yang benar-benar positif.

$$
\text{Precision} = \frac{TP}{TP + FP}
$$

Cocok ketika **kesalahan positif (false positive)** harus diminimalkan.  
Contoh: sistem spam filter (jangan sampai email penting dikira spam).

### Recall

**Recall** menunjukkan dari semua data positif, berapa banyak yang berhasil dideteksi.

$$
\text{Recall} = \frac{TP}{TP + FN}
$$

Cocok ketika **kesalahan negatif (false negative)** harus diminimalkan.  
Contoh: deteksi penyakit (lebih baik salah mendeteksi sehat sebagai sakit, daripada melewatkan pasien yang sakit).

### F1-Score

**F1-Score** adalah rata-rata harmonis antara precision dan recall. Digunakan jika perlu keseimbangan antara keduanya, terutama saat data tidak seimbang.

$$
\text{F1} = \frac{2 \cdot \text{Precision} \cdot \text{Recall}}{\text{Precision} + \text{Recall}}
$$

Nilai F1 berkisar antara 0 dan 1. Semakin tinggi, semakin baik.

### Perbandingan Singkat

| Metrik      | Fokus Utama               | Cocok Untuk                        |
|-------------|----------------------------|------------------------------------|
| Accuracy    | Semua prediksi             | Data seimbang                      |
| Precision   | Kebenaran prediksi positif | Minimalkan false positive          |
| Recall      | Kelengkapan prediksi       | Minimalkan false negative          |
| F1-Score    | Keseimbangan presisi & recall | Data tidak seimbang             |

### Contoh Kasus

Misalkan dari 100 data:
- TP = 40
- FP = 10
- FN = 5
- TN = 45

Maka:
- Accuracy = (40 + 45) / 100 = 0.85
- Precision = 40 / (40 + 10) = 0.80
- Recall = 40 / (40 + 5) = 0.89
- F1-Score = 2 * (0.80 * 0.89) / (0.80 + 0.89) ≈ 0.84

### Kesimpulan

- Jangan hanya mengandalkan akurasi, terutama jika data tidak seimbang.
- Gunakan precision dan recall untuk memahami jenis kesalahan yang dibuat model.
- F1-Score membantu jika diperlukan keseimbangan antara false positive dan false negative.
- Confusion Matrix memberikan gambaran menyeluruh tentang performa model klasifikasi.


## 3.2 Evaluasi Model Regresi: MAE, MSE, RMSE, R²

Untuk tugas Machine Learning yang bersifat regresi — yaitu ketika target (label) berupa nilai kontinu — diperlukan metrik evaluasi yang berbeda dari klasifikasi. Tujuannya adalah mengukur seberapa dekat prediksi model terhadap nilai sebenarnya.

Beberapa metrik evaluasi regresi yang umum digunakan meliputi:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- Coefficient of Determination (R²)

### Analogi Umum

Bayangkan kamu menebak tinggi badan temanmu.  
- Jika tebakanmu selalu berbeda 5 cm dari tinggi aslinya, maka MAE = 5.  
- Jika beberapa tebakanmu sangat meleset jauh, MSE dan RMSE akan menunjukkan itu dengan nilai besar.  
- Jika tebakanmu lebih baik daripada asal menebak rata-rata, maka R² akan mendekati 1.


### Mean Absolute Error (MAE)

MAE mengukur rata-rata dari selisih absolut antara nilai prediksi dan nilai aktual.

$$
\text{MAE} = \frac{1}{n} \sum_{i=1}^{n} |y_i - \hat{y}_i|
$$

**dimana :**  
- $n$ : Jumlah data  
- $y_i$ : Nilai sebenarnya(Actual)  
- $\hat{y}_i$ : Nilai prediksi 

**Karakteristik:**
- Interpretasi mudah dan intuitif
- Tidak memperhitungkan arah kesalahan
- Tidak sensitif terhadap outlier


### Mean Squared Error (MSE)

MSE mengukur rata-rata kuadrat dari selisih antara nilai aktual dan nilai prediksi.

$$
\text{MSE} = \frac{1}{n} \sum_{i=1}^{n} (y_i - \hat{y}_i)^2
$$

**Karakteristik:**
- Memberikan penalti besar untuk kesalahan besar
- Cocok saat ingin menghindari prediksi yang jauh meleset
- Nilainya dalam satuan kuadrat (misal: cm², kg²)

### Root Mean Squared Error (RMSE)

RMSE adalah akar kuadrat dari MSE, sehingga kembali ke satuan asli dari target.

$$
\text{RMSE} = \sqrt{\text{MSE}} = \sqrt{ \frac{1}{n} \sum_{i=1}^{n} (y_i - \hat{y}_i)^2 }
$$

**Karakteristik:**
- Mudah diinterpretasikan karena satuannya sama dengan target
- Lebih sensitif terhadap outlier dibanding MAE
- Makin kecil RMSE, makin baik modelnya


### Coefficient of Determination (R² Score)

R² mengukur seberapa baik variasi dalam data target dapat dijelaskan oleh model.

$$
R^2 = 1 - \frac{ \sum (y_i - \hat{y}_i)^2 }{ \sum (y_i - \bar{y})^2 }
$$

**Keterangan:**
- $y_i$ : nilai aktual  
- $\hat{y}_i$ : nilai prediksi  
- $\bar{y}$ : rata-rata nilai aktual  

**Interpretasi:**
- R² = 1 → model sempurna
- R² = 0 → model sama buruknya dengan rata-rata
- R² < 0 → model lebih buruk daripada tebak rata-rata


### Contoh Sederhana

Misalkan kita memiliki 3 data aktual dan prediksi:

| Data | y (aktual) | 𝑦̂ (prediksi) | |y - 𝑦̂| | (y - 𝑦̂)²   |
|------|------------|----------------|------------|-------------|
| 1    | 10         | 12             | 2          | 4           |
| 2    | 15         | 14             | 1          | 1           |
| 3    | 20         | 18             | 2          | 4           |

- MAE = (2 + 1 + 2) / 3 = **1.67**
- MSE = (4 + 1 + 4) / 3 = **3.0**
- RMSE = √3.0 ≈ **1.73**
- R² dihitung dari selisih prediksi vs rata-rata


### Perbandingan Metrik

| Metrik | Fokus                         | Sensitif Outlier | Satuan      | Interpretasi Mudah |
|--------|-------------------------------|------------------|-------------|---------------------|
| MAE    | Rata-rata kesalahan absolut   | Tidak            | Sama dengan target | Ya            |
| MSE    | Penalti kesalahan besar       | Ya               | Kuadrat dari target | Tidak        |
| RMSE   | Akar dari MSE                 | Ya               | Sama dengan target | Ya            |
| R²     | Proporsi variasi yang dijelaskan | Tidak       | Skor 0–1 (bisa negatif) | Ya     |



### Kesimpulan

- Gunakan **MAE** saat ingin tahu rata-rata kesalahan secara langsung.
- Gunakan **RMSE** jika ingin memberi penalti pada prediksi yang meleset jauh.
- Gunakan **R²** untuk mengukur seberapa baik model menjelaskan variasi target.
- Tidak ada metrik yang mutlak terbaik — pilih sesuai konteks dan tujuan bisnis atau eksperimen.


## 3.3 Cross-Validation: K-Fold, Stratified, Repeated

Dalam evaluasi model Machine Learning, kita ingin mengukur seberapa baik model bekerja pada data yang belum pernah dilihat sebelumnya. Namun, membagi data hanya sekali menjadi train-test dapat menghasilkan evaluasi yang **kurang stabil** dan **bias** tergantung dari pembagian tersebut.

Untuk mengatasi hal ini, digunakan teknik yang disebut **cross-validation** — metode evaluasi yang lebih adil dan menyeluruh.

### Analogi

Bayangkan kamu seorang guru yang ingin menguji pemahaman siswa, tapi hanya punya 30 soal. Alih-alih membuat satu tes tetap, kamu membuat 5 set soal berbeda dan memberi nilai rata-ratanya. Ini membantu mengurangi bias penilaian dari soal tertentu. Begitulah prinsip kerja cross-validation.


### 1. K-Fold Cross-Validation

**Prinsip:**
- Dataset dibagi menjadi **K bagian (fold)**.
- Model dilatih pada K-1 fold dan diuji pada 1 fold.
- Proses diulang sebanyak K kali dengan fold uji yang bergantian.
- Nilai evaluasi diambil sebagai **rata-rata dari semua iterasi**.

**Contoh:**
Jika `K = 5`, maka:
- Model dilatih 5 kali
- Setiap fold digunakan sekali sebagai data uji
- Skor akhir = rata-rata dari 5 skor

### 2. Stratified K-Fold

K-Fold biasa tidak mempertahankan distribusi kelas. Pada dataset tidak seimbang, hal ini bisa menyebabkan fold tertentu didominasi oleh satu kelas saja.

nah

**Stratified K-Fold** membagi data sambil mempertahankan proporsi kelas yang sama di setiap fold. Cocok untuk tugas klasifikasi.

### Repeated K-Fold
K-Fold bisa memberikan hasil yang berbeda tergantung bagaimana data diacak. nah **Repeated K-Fold** mengulang proses K-Fold beberapa kali dengan pembagian acak yang berbeda untuk memperoleh evaluasi yang lebih **stabil dan akurat secara statistik.**

**contoh**  
K = 5, Repeat = 3 → total 15 pelatihan dan pengujian


### Perbandingan Cross-Validation

| Metode            | Cocok Untuk                        | Kelebihan                    | Kekurangan                         |
| ----------------- | ---------------------------------- | ---------------------------- | ---------------------------------- |
| K-Fold            | Semua jenis model                  | Umum dan sederhana           | Bisa tidak seimbang di klasifikasi |
| Stratified K-Fold | Klasifikasi (kelas tidak seimbang) | Menjaga proporsi kelas       | Hanya untuk klasifikasi            |
| Repeated K-Fold   | Semua model                        | Evaluasi lebih stabil & acak | Lebih lambat (banyak iterasi)      |

### Kesimpulan
- Cross-validation memberikan evaluasi yang lebih adil dan andal dibanding split biasa.

- Gunakan StratifiedKFold untuk klasifikasi, terutama jika kelas tidak seimbang.

- Gunakan Repeated K-Fold jika ingin hasil evaluasi yang lebih stabil secara statistik.

- Jangan hanya fokus pada skor rata-rata — perhatikan juga dispersi (variansi) antar fold.

# 4. Neural Network Dasar

Neural Network atau jaringan syaraf tiruan (JST) adalah model Machine Learning yang terinspirasi dari cara kerja otak manusia. Model ini terdiri dari unit-unit pemroses sederhana yang disebut neuron buatan, yang saling terhubung dan bekerja secara berlapis untuk menyelesaikan berbagai tugas kompleks seperti klasifikasi, regresi, hingga pengenalan pola.

Neural Network sangat efektif untuk menangani masalah non-linear dan data berdimensi tinggi seperti gambar, suara, dan teks.

## 4.1 Struktur Jaringan: Input, Hidden, Output

Bayangkan kamu adalah juri kompetisi masak. Kamu:
- Menerima input berupa **rasa, aroma, dan tampilan** dari hidangan
- Memproses semuanya dalam pikiranmu, membandingkan dengan pengalaman, selera, dan standar penilaian
- Mengeluarkan penilaian akhir: **lulus, tidak lulus, atau skor angka**

Begitu pula cara kerja Neural Network:
- Input layer menerima data
- Hidden layer memproses dengan bobot dan fungsi aktivasi
- Output layer memberikan hasil prediksi


### 1. Input Layer

**Input Layer** adalah lapisan pertama yang menerima data mentah dari luar dan meneruskannya ke jaringan. Setiap neuron pada layer ini mewakili satu fitur dari dataset.

**Contoh:**
Jika kita memiliki data dengan 3 fitur:
- suhu
- kelembaban
- tekanan udara

Maka input layer terdiri dari 3 neuron.

### 2. Hidden Layer

**Hidden Layer** adalah lapisan tengah yang melakukan sebagian besar perhitungan internal. Lapisan ini berisi neuron-neuron yang menggabungkan input, mengalikan dengan bobot, menambahkan bias, dan menerapkan fungsi aktivasi.

- Bisa terdiri dari satu atau lebih layer
- Semakin banyak layer dan neuron, semakin besar kapasitas model (tapi juga risiko overfitting)

**Peran:** Menyaring, menyusun ulang, dan mengekstraksi pola dari input.

**Contoh umum:**  
Arsitektur MLP (Multilayer Perceptron) standar memiliki 1 hingga 3 hidden layer.

### 3. Output Layer

**Output Layer** adalah lapisan terakhir yang menghasilkan hasil akhir dari model.

- Jika tugasnya **klasifikasi biner**, maka hanya 1 neuron dengan aktivasi sigmoid
- Jika **klasifikasi multikelas**, maka jumlah neuron = jumlah kelas, dengan aktivasi softmax
- Jika **regresi**, maka 1 neuron tanpa fungsi aktivasi atau menggunakan fungsi linear

### Ilustrasi Sederhana

Misalkan kita memiliki arsitektur jaringan sebagai berikut:

[INPUT] → [HIDDEN 1] → [HIDDEN 2] → [OUTPUT]

3 Neuron 5 Neuron 3 Neuron 1 Neuron


Ini berarti:
- 3 fitur masukan
- 2 hidden layer (masing-masing dengan 5 dan 3 neuron)
- 1 output (misal: prediksi nilai kontinu)

### Analogi

Bayangkan kamu adalah juri dalam lomba menyanyi:
- **Input Layer** = suara penyanyi, penampilan, teknik vokal
- **Hidden Layer** = kamu menimbang, memikirkan, menganalisis tiap aspek
- **Output Layer** = keputusan akhir: Lulus atau tidak

Setiap lapisan seperti proses berpikir bertingkat — dari pengamatan mentah hingga pengambilan keputusan.

### Catatan Penting

- Semua neuron di satu layer terhubung ke semua neuron di layer berikutnya (Fully Connected Layer)
- Input tidak diproses sendiri — jaringan mempelajari bobot dan pola hubungan antar fitur
- Banyaknya layer dan neuron sangat memengaruhi **kapasitas**, **akurasi**, dan **kompleksitas komputasi**

### Kesimpulan

- Neural Network tersusun atas tiga jenis lapisan utama: Input, Hidden, dan Output.
- Hidden layer adalah tempat utama terjadinya pemrosesan dan pembelajaran pola.
- Struktur jaringan (jumlah layer dan neuron) harus disesuaikan dengan kompleksitas tugas dan data.


## 4.2 Neuron, Bobot (Weight), dan Bias

Setiap jaringan syaraf tiruan terdiri dari elemen dasar yang disebut **neuron**. Neuron bekerja dengan menerima input, mengolahnya menggunakan **bobot (weight)** dan **bias**, lalu meneruskannya ke fungsi aktivasi untuk menghasilkan output.

### Apa itu Neuron?

Neuron adalah unit komputasi dasar dalam jaringan. Ia menerima sinyal dari neuron sebelumnya, lalu menghasilkan sinyal baru untuk diteruskan ke neuron berikutnya.

### Ilustrasi Perhitungan

Secara umum, sebuah neuron melakukan operasi berikut:

$$
z = (w_1 \cdot x_1 + w_2 \cdot x_2 + \dots + w_n \cdot x_n) + b
$$

Atau lebih ringkas:
$$
z = \mathbf{w}^\top \mathbf{x} + b
$$

- $\mathbf{x}$ = vektor input (fitur)
- $\mathbf{w} $ = vektor bobot
- $b$ = bias
- $z$ = input ke fungsi aktivasi

Kemudian, output dari neuron adalah:
$$
a = f(z)
$$
di mana \( f \) adalah fungsi aktivasi (misalnya ReLU, Sigmoid, Tanh).


### Bobot (Weight)

**Bobot** mengatur seberapa besar pengaruh suatu input terhadap hasil.

- Nilai bobot positif → memperkuat sinyal input
- Nilai bobot negatif → membalik atau melemahkan sinyal
- Semakin besar nilai absolut bobot → semakin besar pengaruh fitur tersebut

**Contoh:**
Jika prediksi didasarkan pada `umur`, maka:
- Bobot = 2 → umur sangat berpengaruh
- Bobot = 0 → umur tidak dianggap penting


### Bias

**Bias** adalah nilai tambahan yang menggeser output dari neuron.

- Tanpa bias, semua neuron harus melewati titik nol → membatasi fleksibilitas model
- Bias memungkinkan neuron belajar **fungsi yang lebih kompleks**

**Analogi:**  
Bayangkan bobot sebagai **kemiringan garis**, dan bias sebagai **titik potong dengan sumbu Y** pada grafik. Tanpa bias, garis hanya bisa melalui titik asal (0,0).

### Analogi Kehidupan Sehari-hari

Bayangkan kamu sedang menilai apakah kamu akan membeli sebuah produk.

- Input: harga, kualitas, merek
- Bobot: kamu sangat peduli pada kualitas (bobot tinggi), sedikit peduli pada merek (bobot rendah)
- Bias: kecenderungan pribadi membeli meskipun semua faktor lain netral (misal, kamu suka brand-nya)
- Aktivasi: keputusan akhir, beli atau tidak

Maka proses berpikirmu adalah neuron: mengalikan nilai input dengan bobot, menambahkan bias, lalu membuat keputusan.


### Contoh Numerik

Misalkan:
- Input: \( x_1 = 2 \), \( x_2 = 3 \)
- Bobot: \( w_1 = 0.4 \), \( w_2 = 0.6 \)
- Bias: \( b = 1 \)

Maka:
$$
z = (0.4 \cdot 2) + (0.6 \cdot 3) + 1 = 0.8 + 1.8 + 1 = 3.6
$$

Jika fungsi aktivasi adalah ReLU, maka output:
$$
a = \max(0, 3.6) = 3.6
$$


### Kesimpulan

- **Neuron** menerima input dan menghasilkan output setelah pemrosesan linier dan non-linier.
- **Bobot** mengatur seberapa penting sebuah fitur.
- **Bias** memungkinkan fleksibilitas dengan menggeser kurva aktivasi.
- Kombinasi bobot dan bias adalah inti dari pembelajaran dalam jaringan syaraf tiruan.


## 4.3 Forward Propagation

Forward propagation adalah proses inti dalam Neural Network di mana data mengalir **dari input menuju output**. Pada setiap lapisan, input dihitung menggunakan bobot dan bias, lalu dilewatkan ke fungsi aktivasi, dan diteruskan ke lapisan berikutnya.

Inilah cara jaringan **memprediksi output** dari input yang diberikan.


### Proses Forward Propagation

Untuk satu neuron:

1. Hitung input teragregasi:
   $$
   z = \mathbf{w}^\top \mathbf{x} + b
   $$

2. Masukkan ke fungsi aktivasi:
   $$
   a = f(z)
   $$

Untuk satu jaringan dengan beberapa lapisan:

- Input layer: menerima data fitur $\mathbf{x} $
- Hidden layer: menerapkan perhitungan linear + aktivasi
- Output layer: menghasilkan prediksi akhir $\hat{y}$


### Ilustrasi Alur Forward Propagation

Misalnya jaringan sederhana:

Input (x1, x2)  
↓  
Hidden Layer (3 neuron)  
↓  
Output (1 neuron)  

Setiap neuron:
- Mengalikan input dengan bobot masing-masing
- Menambahkan bias
- Memasukkan ke fungsi aktivasi
- Meneruskan output ke layer berikutnya


### Contoh Numerik Sederhana

Misalkan:
- Input: \( x_1 = 1 \), \( x_2 = 2 \)
- Bobot: \( w_1 = 0.5 \), \( w_2 = -1.0 \)
- Bias: \( b = 0.5 \)

1. Hitung \( z \):
   $$
   z = (0.5 \cdot 1) + (-1.0 \cdot 2) + 0.5 = 0.5 - 2 + 0.5 = -1.0
   $$

2. Aktivasi (gunakan ReLU):
   $$
   a = \max(0, -1.0) = 0
   $$

Output dari neuron tersebut adalah 0, yang kemudian dikirim ke layer berikutnya.


### Analogi Sederhana

Bayangkan kamu menyaring air kotor melalui beberapa filter (layer):

- Setiap filter hanya meloloskan air sesuai kriteria (fungsi aktivasi)
- Semakin banyak filter → semakin jernih hasil akhirnya
- Proses mengalir dari satu filter ke filter berikutnya tanpa kembali ke belakang

Forward propagation seperti aliran satu arah — dari input ke output, melewati proses di setiap lapisan.


### Catatan Penting

- Proses ini terjadi **setiap kali** model melakukan prediksi
- Tidak ada pembaruan parameter saat forward pass (hanya propagasi sinyal)
- Saat training, setelah forward pass akan dilakukan **backpropagation**


### Kesimpulan

- Forward propagation adalah proses inti yang membawa data dari input ke output melalui bobot, bias, dan fungsi aktivasi.
- Di setiap lapisan, nilai dihitung, diaktifkan, lalu diteruskan.
- Proses ini **tidak mengubah bobot**, tapi digunakan untuk menghitung output dan loss sebelum proses pelatihan dimulai.

## 4.4 Fungsi Aktivasi: Sigmoid, ReLU, Tanh, Softmax

Fungsi aktivasi (activation function) adalah komponen penting dalam Neural Network. Tanpanya, jaringan hanya akan menghasilkan kombinasi linier — seperti regresi biasa. Fungsi aktivasi memberikan kemampuan untuk **menangani non-linearitas** sehingga jaringan bisa mempelajari pola yang kompleks.

---

### Mengapa Fungsi Aktivasi Dibutuhkan?

Tanpa fungsi aktivasi:
- Setiap layer hanya melakukan operasi linear
- Tidak ada manfaat menambahkan banyak layer
- Jaringan tidak bisa menangani data kompleks seperti gambar atau bahasa

Dengan fungsi aktivasi:
- Jaringan bisa **belok, melengkung, dan membagi** ruang data dengan lebih fleksibel
- Dapat memetakan input ke output yang non-linier

---

### 1. Sigmoid

**Rumus:**
$$
f(x) = \frac{1}{1 + e^{-x}}
$$

**Ciri-ciri:**
- Output berada di antara 0 dan 1
- Cocok untuk klasifikasi biner
- Sering digunakan di layer output

**Kelemahan:**
- Gradient sangat kecil jika nilai input besar/kecil → **vanishing gradient**
- Tidak simetris terhadap nol

**Analogi:**
Seperti tombol volume yang menyaring sinyal keras menjadi sinyal halus (dibatasi antara 0 dan 1)

---

### 2. ReLU (Rectified Linear Unit)

**Rumus:**
$$
f(x) = \max(0, x)
$$

**Ciri-ciri:**
- Output positif tetap sama, nilai negatif jadi nol
- Sederhana dan cepat dihitung
- Sangat populer di hidden layer

**Kelemahan:**
- Jika input selalu negatif → output selalu 0 (dead neuron)

**Analogi:**
Seperti **kran air otomatis**: jika tekanan rendah (negatif), air tidak keluar; jika tekanan cukup, air mengalir proporsional

---

### 3. Tanh (Hyperbolic Tangent)

**Rumus:**
$$
f(x) = \tanh(x) = \frac{e^x - e^{-x}}{e^x + e^{-x}}
$$

**Ciri-ciri:**
- Output berada di antara -1 dan 1
- Simetris terhadap nol
- Gradient lebih besar dibanding sigmoid → pelatihan lebih stabil

**Kelemahan:**
- Tetap mengalami vanishing gradient jika input terlalu besar

**Analogi:**
Seperti pedal rem mobil: bisa mengatur arah (positif/negatif), dan juga seberapa kuat tekanan (non-linear)

---

### 4. Softmax

**Rumus (untuk neuron ke-i dari total n):**
$$
f(z_i) = \frac{e^{z_i}}{\sum_{j=1}^{n} e^{z_j}}
$$

**Ciri-ciri:**
- Output adalah distribusi probabilitas (jumlah = 1)
- Sering digunakan di **layer output klasifikasi multikelas**

**Kelemahan:**
- Tidak cocok untuk hidden layer
- Sensitif terhadap nilai ekstrem

**Analogi:**
Seperti mesin voting yang mengubah nilai skor mentah menjadi peluang proporsional untuk tiap kelas.

---

### Perbandingan Fungsi Aktivasi

| Fungsi   | Rentang Output | Kelebihan                   | Kekurangan                     | Cocok Untuk                |
|----------|----------------|-----------------------------|--------------------------------|----------------------------|
| Sigmoid  | (0, 1)         | Probabilitas, smooth        | Vanishing gradient, tidak simetris | Output biner            |
| Tanh     | (-1, 1)        | Simetris, smooth            | Masih bisa mengalami vanishing gradient | Hidden layer klasik |
| ReLU     | [0, ∞)         | Cepat, sederhana, tidak vanish | Dead neuron                   | Hidden layer modern       |
| Softmax  | (0, 1), total = 1 | Probabilitas multi-kelas | Hanya untuk output, sensitif | Output klasifikasi multikelas |

---

### Kesimpulan

- Fungsi aktivasi memberikan kemampuan non-linear pada jaringan.
- Pilihan fungsi tergantung pada posisi layer dan jenis tugas:
  - **Hidden layer** → ReLU atau Tanh
  - **Output biner** → Sigmoid
  - **Output multikelas** → Softmax
- Pemilihan fungsi yang tepat dapat mempercepat konvergensi dan meningkatkan akurasi model.

## 4.5 Output Layer (Klasifikasi dan Regresi)

Output layer adalah bagian akhir dari jaringan Neural Network yang bertugas menghasilkan **prediksi akhir** dari seluruh proses forward propagation.

Jenis dan konfigurasi output layer **sangat tergantung** pada jenis tugas Machine Learning yang sedang diselesaikan: apakah itu **klasifikasi biner**, **klasifikasi multikelas**, atau **regresi**.

---

### 1. Output untuk Klasifikasi Biner

**Tujuan:** Mengklasifikasikan input ke dalam dua kelas (positif atau negatif).

- Jumlah neuron: **1**
- Fungsi aktivasi: **Sigmoid**
- Output: Nilai antara 0 dan 1, yang bisa dianggap sebagai **probabilitas** kelas positif

**Contoh:**
- Deteksi email spam
- Prediksi apakah seseorang akan membeli produk

### 2. Output untuk Klasifikasi Multikelas
**Tujuan**: Memilih salah satu dari beberapa kelas.

- Jumlah neuron: **sama dengan jumlah kelas**

- Fungsi aktivasi: **Softmax**

- Output: Vektor probabilitas yang menjumlahkan hingga 1

**Contoh:**

- Klasifikasi jenis bunga (setosa, versicolor, virginica)

- Deteksi objek dalam gambar (kucing, anjing, burung)

**Ilustrasi:**  
Jika output = [0.1, 0.7, 0.2], maka kelas ke-2 (probabilitas 0.7) dipilih.

### 3. Output untuk Regresi
**Tujuan**: Memprediksi nilai kontinu (bukan kategori).

- Jumlah neuron: 1 (umumnya)

- Fungsi aktivasi: **None** (linear) atau bisa juga ReLU, tergantung konteks

**Contoh:**

- Prediksi harga rumah

- Perkiraan suhu

- Estimasi permintaan pasar

**Output**: Angka real, misalnya 152.3

#### Perbandingan Konfigurasi Output Layer

| Tugas                  | Jumlah Neuron | Aktivasi      | Output                     |
| ---------------------- | ------------- | ------------- | -------------------------- |
| Klasifikasi Biner      | 1             | Sigmoid       | Probabilitas (0–1)         |
| Klasifikasi Multikelas | Jumlah kelas  | Softmax       | Vektor probabilitas        |
| Regresi                | 1             | Linear / None | Nilai kontinu (angka real) |

#### Tips Praktis
- **Selalu sesuaikan output layer dengan jenis tugas dan fungsi loss yang digunakan.**

  - Sigmoid → digunakan dengan binary_crossentropy

  - Softmax → digunakan dengan categorical_crossentropy

  - Linear → digunakan dengan mean_squared_error, mae, dll

- **Untuk klasifikasi multikelas**, pastikan label sudah diubah ke format one-hot atau integer class sesuai dengan kebutuhan fungsi loss.

#### Kesimpulan
- Output layer menentukan bentuk akhir dari prediksi model.

- Arsitekturnya bergantung langsung pada apakah model digunakan untuk klasifikasi biner, multikelas, atau regresi.

- Pemilihan fungsi aktivasi dan jumlah neuron di layer ini sangat penting untuk memastikan model belajar dan dievaluasi dengan benar.



# 5. Pembelajaran dalam Neural Network

Setelah jaringan syaraf tiruan (Neural Network) dibentuk dengan lapisan-lapisan dan fungsi aktivasi, langkah selanjutnya adalah **melatih jaringan tersebut agar mampu membuat prediksi yang akurat**.

Pelatihan Neural Network melibatkan proses iteratif yang disebut **pembelajaran (learning)**, di mana model:
- Mengamati data input,
- Membuat prediksi,
- Menghitung kesalahan (loss),
- Lalu **memperbaiki dirinya sendiri** melalui optimisasi.

Proses ini dilakukan berkali-kali hingga model mampu mengenali pola dan menghasilkan prediksi yang sesuai.


### Komponen Utama dalam Pembelajaran

1. **Loss Function**  
   Mengukur seberapa besar kesalahan antara prediksi dan label sebenarnya.

2. **Backpropagation**  
   Algoritma yang menghitung bagaimana kesalahan memengaruhi setiap bobot dalam jaringan menggunakan **turunan parsial**.

3. **Optimizer**  
   Metode yang digunakan untuk memperbarui bobot dan bias berdasarkan hasil backpropagation agar loss menjadi lebih kecil.

4. **Epoch, Batch, dan Mini-batch**  
   Strategi dalam menentukan berapa banyak data yang digunakan untuk memperbarui bobot setiap kali.

5. **Regularisasi dan Early Stopping**  
   Teknik untuk mencegah overfitting dan menghentikan pelatihan saat performa sudah optimal.

### Analogi

Bayangkan Neural Network seperti seorang murid yang sedang belajar matematika:
- Ia mencoba mengerjakan soal (forward propagation),
- Mengecek jawaban yang salah (loss),
- Menelusuri kembali proses berpikirnya untuk mencari kesalahan (backpropagation),
- Lalu belajar dari kesalahan tersebut agar tidak mengulanginya (optimisasi).

Semakin sering ia belajar (epoch), semakin baik kemampuannya… asalkan tidak **terlalu banyak belajar soal yang sama** hingga ia hanya menghafal (overfitting).


Di bagian ini, kita akan membahas **cara kerja pembelajaran** di dalam Neural Network, dimulai dari fungsi loss hingga proses pelatihan yang sebenarnya.


## 5.1 Loss Function: Binary/Categorical Crossentropy, MSE, MAE

Dalam proses pelatihan Neural Network, kita perlu mengukur **seberapa jauh prediksi model dari nilai sebenarnya**. Ukuran kesalahan inilah yang disebut sebagai **loss**, dan rumus matematis untuk menghitungnya disebut **loss function**.

Loss function adalah **kompas** yang menunjukkan arah pembelajaran bagi model. Nilainya akan diminimalkan melalui proses optimisasi (misalnya dengan backpropagation dan gradient descent).


### Analogi Kehidupan Sehari-hari

Bayangkan kamu belajar melempar bola ke keranjang.  
- Setiap kali meleset, kamu mendapat nilai "seberapa jauh bola dari target".
- Semakin jauh, semakin besar "loss"-nya.
- Tujuanmu adalah **meminimalkan jarak** dari target.

Demikian pula, model dilatih untuk meminimalkan loss agar prediksinya semakin mendekati data sebenarnya.


### Jenis Loss Function Berdasarkan Tugas

| Tugas             | Fungsi Loss Umum                  |
|------------------|------------------------------------|
| Klasifikasi Biner | Binary Crossentropy               |
| Klasifikasi Multikelas | Categorical Crossentropy    |
| Regresi           | Mean Squared Error (MSE), MAE     |


### 1. Binary Crossentropy

Digunakan untuk **klasifikasi biner** (label 0 atau 1).

**Rumus:**
$$
L = -[y \cdot \log(\hat{y}) + (1 - y) \cdot \log(1 - \hat{y})]
$$

- \( y \): nilai sebenarnya (0 atau 1)
- \( \hat{y} \): prediksi probabilitas dari model

**Ciri:**
- Loss kecil jika prediksi mendekati nilai sebenarnya
- Sering digunakan dengan **sigmoid** di output layer

**Contoh:**
Jika label = 1 dan prediksi = 0.9 → loss kecil  
Jika label = 1 dan prediksi = 0.1 → loss besar


### 2. Categorical Crossentropy

Digunakan untuk **klasifikasi multikelas** dengan label dalam format **one-hot** (misalnya `[0, 0, 1, 0]`).

**Rumus:**
$$
L = -\sum_{i=1}^{C} y_i \cdot \log(\hat{y}_i)
$$

- \( C \): jumlah kelas
- \( y_i \): label sebenarnya untuk kelas ke-i
- \( \hat{y}_i \): probabilitas prediksi untuk kelas ke-i

**Ciri:**
- Loss tinggi jika probabilitas untuk kelas benar rendah
- Digunakan bersama **softmax** di output layer


### 3. Mean Squared Error (MSE)

Digunakan untuk **regresi**, menghitung rata-rata kuadrat selisih antara prediksi dan nilai aktual.

**Rumus:**
$$
L = \frac{1}{n} \sum_{i=1}^{n} (y_i - \hat{y}_i)^2
$$

- Penalti besar jika kesalahan besar
- Satuan hasilnya adalah kuadrat dari satuan target

**Contoh:**
Prediksi harga rumah: nilai prediksi yang jauh dari sebenarnya akan dihukum lebih berat.


### 4. Mean Absolute Error (MAE)

Menghitung rata-rata **selisih absolut** antara prediksi dan nilai aktual.

**Rumus:**
$$
L = \frac{1}{n} \sum_{i=1}^{n} |y_i - \hat{y}_i|
$$

- Interpretasi lebih intuitif daripada MSE
- Tidak terlalu terpengaruh oleh outlier


### Perbandingan Singkat

| Fungsi Loss         | Cocok Untuk              | Keunggulan                        | Kekurangan                     |
|---------------------|--------------------------|-----------------------------------|--------------------------------|
| Binary Crossentropy | Klasifikasi biner        | Probabilistik, cocok dengan sigmoid | Tidak cocok untuk multikelas  |
| Categorical Crossentropy | Klasifikasi multikelas | Akurat dengan softmax             | Perlu one-hot encoding         |
| MSE                 | Regresi                  | Penalti besar untuk error besar   | Sensitif terhadap outlier      |
| MAE                 | Regresi                  | Lebih tahan outlier               | Gradient tidak halus           |


### Kesimpulan

- Loss function adalah ukuran kesalahan model yang ingin diminimalkan.
- Pilihlah loss function sesuai dengan jenis tugas dan format output model.
- Kombinasi loss, aktivasi output, dan data label harus **selaras** agar pelatihan berjalan dengan baik.

## 5.2 Backpropagation dan Turunan Parsial

Setelah model membuat prediksi dan menghitung **loss**, langkah berikutnya adalah **mengoreksi kesalahan tersebut**. Caranya adalah dengan menghitung bagaimana **setiap bobot dalam jaringan** berkontribusi terhadap kesalahan, lalu memperbaruinya agar performa meningkat.

Proses ini disebut **Backpropagation**.


### Apa Itu Backpropagation?

Backpropagation (Propagation Backward) adalah algoritma yang digunakan untuk:
- **Menghitung turunan (gradien)** dari loss terhadap setiap parameter (bobot dan bias),
- Menyebarkan informasi kesalahan **dari output ke input** melalui rantai turunan.

Metode ini sangat efisien karena menggunakan prinsip **turunan berantai (chain rule)** dari kalkulus.


### Rumus Dasar: Chain Rule

Jika:
- \( L \): Loss akhir
- \( z \): input ke neuron
- \( w \): bobot
- \( x \): input dari neuron sebelumnya

Maka:
$$
\frac{\partial L}{\partial w} = \frac{\partial L}{\partial z} \cdot \frac{\partial z}{\partial w}
$$

Karena $z = w \cdot x + b $, maka:
$$
\frac{\partial z}{\partial w} = x
$$


### Alur Backpropagation

1. **Forward pass**: hitung prediksi dan loss
2. **Backward pass**:
   - Hitung turunan loss terhadap output layer
   - Hitung gradien terhadap bobot & bias di layer output
   - Teruskan ke layer sebelumnya (hidden) menggunakan chain rule
3. **Update bobot**: gunakan hasil gradien dan optimasi (misal SGD, Adam)


### Contoh Sederhana

Misal:
- \( x = 2 \), \( w = 0.5 \), \( b = 0.1 \)
- Fungsi aktivasi: ReLU
- Target \( y = 1 \)

Forward:
$$
z = w \cdot x + b = 0.5 \cdot 2 + 0.1 = 1.1 \\
a = \text{ReLU}(1.1) = 1.1 \\
L = \frac{1}{2}(y - a)^2 = \frac{1}{2}(1 - 1.1)^2 = 0.005
$$

Backward:
$$
\frac{\partial L}{\partial a} = -(y - a) = 0.1 \\
\frac{\partial a}{\partial z} = 1 \quad (\text{karena ReLU}'(1.1) = 1) \\
\frac{\partial z}{\partial w} = x = 2 \\
\Rightarrow \frac{\partial L}{\partial w} = 0.1 \cdot 1 \cdot 2 = 0.2
$$

Hasilnya: gradien untuk \( w \) adalah 0.2


### Analogi

Bayangkan kamu membuat kesalahan dalam memasak dan ingin memperbaikinya.

- Kamu mencicipi hasilnya (loss),
- Menelusuri kembali langkah demi langkah (backpropagation),
- Menentukan bahan mana yang salah takaran (turunan),
- Lalu memperbaiki resep (update bobot).


### Mengapa Turunan?

Turunan (derivatif) menunjukkan:
- Seberapa **sensitif** loss terhadap perubahan kecil pada suatu parameter
- Arah dan besarnya perubahan yang diperlukan untuk **memperbaiki kesalahan**


### Kesimpulan

- Backpropagation adalah metode untuk menghitung gradien loss terhadap semua parameter jaringan.
- Proses ini menggunakan turunan parsial dan prinsip chain rule.
- Dengan informasi gradien ini, kita dapat **mengupdate bobot dan bias** agar model belajar dari kesalahan.


## 5.3 Optimizer: SGD, Adam, Momentum

Setelah gradien dihitung melalui backpropagation, kita perlu menggunakan informasi tersebut untuk **memperbarui bobot dan bias** dalam jaringan. Proses pembaruan inilah yang disebut **optimisasi**, dan algoritma yang digunakan disebut **optimizer**.

Optimizer menentukan:
- Seberapa besar perubahan parameter (learning rate),
- Arah pergerakan parameter berdasarkan gradien,
- Dan bagaimana mempercepat atau menstabilkan proses belajar.

---

### Rumus Dasar: Pembaruan Parameter

Secara umum, bobot diperbarui dengan:
$$
w := w - \eta \cdot \frac{\partial L}{\partial w}
$$

- $w$: bobot
- $\eta$: learning rate
- $\frac{\partial L}{\partial w} $: gradien loss terhadap bobot

---

### 1. SGD (Stochastic Gradient Descent)

SGD memperbarui parameter berdasarkan **satu data acak (batch kecil)** pada setiap iterasi.

**Karakteristik:**
- Sederhana dan efisien
- Cepat konvergen pada dataset besar
- Bisa "loncat keluar" dari local minima

**Kelemahan:**
- Cenderung **berisik** dan tidak stabil
- Mudah terjebak di lembah dangkal (plateau)

**Analogi:**
Seperti **mendaki gunung dalam kabut** — kamu melihat sebagian jalan, tapi terus bergerak meski arah sedikit bergoyang.

---

### 2. Momentum

Momentum adalah pengembangan dari SGD yang menyimpan arah gradien sebelumnya untuk mempercepat pergerakan.

**Rumus:**
$$
v_t = \gamma \cdot v_{t-1} + \eta \cdot \nabla L \\
w := w - v_t
$$

- $v_t$: kecepatan pergerakan
- $\gamma $: koefisien momentum (biasanya 0.9)

**Manfaat:**
- Mengurangi osilasi
- Mempercepat pelatihan di arah yang konsisten

**Analogi:**
Seperti **bola menggelinding di lereng** — semakin lama menggelinding, semakin cepat.

---

### 3. Adam (Adaptive Moment Estimation)

Adam adalah optimizer paling populer karena menggabungkan **Momentum** dan **RMSprop (penyesuaian adaptif learning rate)**.

**Karakteristik:**
- Menyesuaikan learning rate untuk setiap parameter
- Menggabungkan momentum + koreksi skala
- Stabil, cepat konvergen, cocok untuk data dan model besar

**Rumus inti:**
$$
m_t = β₁ · m_{t-1} + (1 - β₁) · ∇L
$$
$$
v_t = β₂ · v_{t-1} + (1 - β₂) · (∇L)²
$$
$$
m̂_t = m_t / (1 - β₁ᵗ)
$$
$$
v̂_t = v_t / (1 - β₂ᵗ)
$$
$$
w := w - η · m̂_t / (√v̂_t + ε)
$$

- $m_t$ : rata-rata gradien
- $v_t$ : rata-rata kuadrat gradien
- $β_1 , β_2$ : koefisien (biasanya 0.9 dan 0.999)

**Kelebihan**:

- Cocok untuk deep learning

- Tidak memerlukan banyak tuning manual

- Cepat dan stabil di banyak kondisi

**Kekurangan**:

- Bisa overfit pada dataset kecil

- Hasil akhir kadang tidak optimal jika learning rate tidak diturunkan perlahan

#### Perbandingan Optimizer

| Optimizer | Stabilitas    | Kecepatan   | Adaptif | Cocok Untuk                |
| --------- | ------------- | ----------- | ------- | -------------------------- |
| SGD       | Rendah        | Sedang      | Tidak   | Dataset besar              |
| Momentum  | Lebih stabil  | Lebih cepat | Tidak   | Masalah dengan osilasi     |
| Adam      | Sangat stabil | Cepat       | Ya      | Deep learning & data noise |

#### Kesimpulan
- Optimizer membantu mengarahkan pembaruan bobot agar loss menurun secara efektif.

- SGD adalah dasar yang sederhana dan efisien.

- Momentum membantu mempercepat pelatihan dengan arah yang lebih stabil.

- Adam menjadi pilihan default di banyak kasus karena adaptif dan konvergen cepat.

- Pemilihan optimizer yang tepat dapat secara signifikan memengaruhi hasil pelatihan.

## 5.4 Konsep Epoch, Batch, Mini-batch

Saat melatih model Machine Learning, kita tidak hanya memasukkan seluruh data ke model satu kali saja. Sebaliknya, data dilatih secara **berulang dan bertahap** agar model benar-benar memahami pola dari dataset.

Tiga konsep penting dalam proses pelatihan adalah:

- **Epoch**
- **Batch**
- **Mini-batch**


### 1. Epoch

**Epoch** adalah **satu kali siklus penuh** pelatihan di mana seluruh data training digunakan untuk memperbarui bobot model.

- Jika dataset memiliki 1.000 data, maka 1 epoch berarti model melihat semua 1.000 data tersebut **sekali**.
- Model biasanya dilatih selama puluhan hingga ratusan epoch.

**Analogi:**  
Seperti membaca seluruh buku sekali dari awal hingga akhir. Semakin sering dibaca, semakin paham isi bukunya.


### 2. Batch

**Batch** adalah jumlah data yang diproses **dalam satu langkah pembaruan** bobot.

- Jika seluruh data dimasukkan sekaligus → disebut **Batch Gradient Descent**
- Jika per baris (satu data) → disebut **Stochastic Gradient Descent (SGD)**

**Ciri:**
- Batch size besar = lebih stabil, tapi butuh memori besar
- Batch size kecil = lebih cepat, tapi bisa tidak stabil


### 3. Mini-batch

**Mini-batch** adalah pendekatan paling umum, yaitu membagi dataset ke dalam **kelompok kecil** (misal 32 atau 64 data), lalu memperbarui bobot setiap kali batch selesai diproses.

- Kombinasi kecepatan dari SGD + stabilitas dari full-batch
- Membantu dalam paralelisasi (GPU)

**Contoh:**
- Dataset = 1.000 data
- Batch size = 100
- Maka 1 epoch terdiri dari **10 langkah mini-batch**


### Ilustrasi Perbandingan

| Metode                 | Jumlah Data per Update | Stabilitas | Kecepatan | Cocok Untuk           |
|------------------------|------------------------|------------|-----------|------------------------|
| Batch Gradient Descent | Semua data             | Sangat stabil | Lambat     | Dataset kecil          |
| Stochastic GD (SGD)    | 1 data                 | Tidak stabil | Sangat cepat | Dataset besar          |
| Mini-batch GD          | 32 – 512 data          | Seimbang   | Cepat      | Dataset umum/deep learning |


### Analogi Sehari-hari

- **Epoch** = berapa kali kamu membaca seluruh buku
- **Batch** = berapa halaman kamu baca sebelum istirahat
- **Mini-batch** = kamu baca 5 halaman → berpikir → belajar → lanjut


### Catatan Tambahan

- Pemilihan batch size memengaruhi **kecepatan, akurasi, dan konvergensi**.
- Jumlah epoch yang terlalu banyak bisa menyebabkan **overfitting** jika tidak dibatasi (misal: dengan early stopping).


### Kesimpulan

- **Epoch** menentukan berapa kali seluruh dataset digunakan untuk melatih model.
- **Batch** adalah jumlah data dalam satu kali perhitungan update bobot.
- **Mini-batch** adalah metode umum yang menyeimbangkan kecepatan dan stabilitas pelatihan.
- Memahami dan mengatur ketiga konsep ini penting untuk pelatihan model yang efisien dan akurat.

## 5.5 Regularisasi dan Early Stopping

Ketika model dilatih terlalu lama atau terlalu kompleks, ia bisa jadi **terlalu menyesuaikan dengan data pelatihan** dan kehilangan kemampuan generalisasi. Fenomena ini disebut **overfitting**.

Untuk mengatasinya, dua strategi umum digunakan:

- **Regularisasi**
- **Early Stopping**


### 1. Regularisasi

Regularisasi adalah teknik untuk **membatasi kompleksitas model** agar tidak terlalu bergantung pada data pelatihan secara berlebihan. Ini dilakukan dengan **menambahkan penalti** terhadap nilai bobot dalam fungsi loss.


#### a. L1 Regularization (Lasso)

Menambahkan penalti berupa jumlah nilai absolut bobot.

**Rumus Loss dengan L1:**
$$
L' = L + \lambda \sum |w_i|
$$

- Dapat menyebabkan beberapa bobot menjadi **nol** → seleksi fitur otomatis
- Cocok jika ingin **mengurangi jumlah fitur penting**


#### b. L2 Regularization (Ridge)

Menambahkan penalti berupa jumlah kuadrat bobot.

**Rumus Loss dengan L2:**
$$
L' = L + \lambda \sum w_i^2
$$

- Mendorong bobot menjadi kecil tapi tidak nol
- Lebih stabil untuk pelatihan deep learning


#### c. Dropout (untuk Neural Network)

Dropout adalah teknik regularisasi unik di jaringan saraf:

- Selama pelatihan, sebagian neuron **dimatikan secara acak** pada setiap batch
- Mencegah jaringan bergantung terlalu kuat pada neuron tertentu

**Contoh:**
- Dropout rate = 0.5 → 50% neuron dinonaktifkan sementara saat pelatihan


### Analogi Regularisasi

Bayangkan kamu belajar menghadapi soal ujian:
- Tanpa regularisasi: kamu **menghafal soal latihan** tanpa memahami konsep
- Dengan regularisasi: kamu **belajar konsep secara umum** meskipun soal latihan berbeda-beda


### 2. Early Stopping

Early stopping adalah teknik untuk **menghentikan pelatihan sebelum overfitting terjadi**.

**Cara kerja:**
- Selama pelatihan, loss pada data **validasi** terus dipantau.
- Jika loss validasi mulai naik (sementara training loss turun), maka pelatihan dihentikan.

**Parameter penting:**
- **Patience**: berapa banyak epoch kita bersabar sebelum menghentikan
- **Monitor**: metrik yang diamati (biasanya `val_loss` atau `val_accuracy`)


### Kesimpulan

- **Regularisasi** membatasi bobot atau struktur model agar tidak terlalu kompleks:
  - **L1**: membuat bobot nol
  - **L2**: mengecilkan bobot
  - **Dropout**: mematikan neuron acak saat pelatihan

- **Early Stopping** mencegah overfitting dengan **menghentikan pelatihan saat performa validasi memburuk**.

Keduanya merupakan strategi penting untuk membuat model **lebih general dan tidak hanya hafal data latih**.

## 5.6 Learning Rate

**Learning rate (α atau η)** adalah parameter yang mengatur **seberapa besar langkah perubahan bobot** dilakukan saat model belajar dari kesalahan (gradien).

### Rumus Perbaruan dengan Learning Rate

Setiap kali bobot diperbarui:
$$
w := w - \eta \cdot \frac{\partial L}{\partial w}
$$

- \( w \): bobot
- \( \eta \): learning rate
- \( \frac{\partial L}{\partial w} \): gradien loss terhadap bobot


### Dampak Learning Rate

| Learning Rate | Dampak                                      |
|---------------|----------------------------------------------|
| Terlalu kecil | Pelatihan sangat lambat, bisa stagnan       |
| Terlalu besar | Model tidak stabil, bisa gagal konvergen     |
| Ideal         | Konvergen cepat dan stabil menuju minimum    |


### Ilustrasi Visual (Deskriptif)

Bayangkan mendaki bukit menuju puncak (minimum loss):

- **Langkah terlalu kecil (η kecil)** → kamu berjalan sangat pelan, mungkin menyerah sebelum sampai.
- **Langkah terlalu besar (η besar)** → kamu melompat-lompat dan melewati puncak tanpa sadar.
- **Langkah pas (η ideal)** → kamu menapaki jalur stabil dan sampai puncak dengan efisien.

### Kesimpulan
- Learning rate mengontrol seberapa besar langkah koreksi model saat belajar.

- Nilai learning rate yang tidak tepat bisa menyebabkan pelatihan gagal.

- Gunakan scheduler atau optimizer adaptif untuk hasil optimal.