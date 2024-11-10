**02_KELOMPOK F_1 Klasifikasi dengan Model Pembelajaran Mesin Terbimbing**
1.  Kumpulan data : SC_HW1_bank_data
2.  Perpustakaan : Pandas, Numpy, Scikit-learn
3.  Tujuan : Membangun model klasifikasi untuk memprediksi kolom target 
    “Exited”.

**Langkah-langkah :**
1.  Menghapus Kolom Tidak Relevan : Hilangkan kolom yang tidak diperlukan 
    untuk mencetak agar data lebih bersih.
2.  One-Hot Encoding : Lakukan pengkodean one-hot menggunakan 
    pd.get_dummies()untuk kategorikal data.
3.  Pisahkan Fitur (X) dan Target (Y) : Pisahkan variabel fitur (X) dan 
    target (Y), di mana Y merujuk ke kolom "Exited".
4.  Scaling atau Normalisasi : Lakukan scaling untuk memastikan data berada 
    dalam rentang yang sesuai.

**Model yang dipilih :**
1.  Model #1 : Regresi Logistik. Model ini dipilih karena sederhana dan 
    cocok untuk klasifikasi biner.
2.  Model #2 : Pohon Keputusan. Model ini menawarkan interpretasi yang 
    jelas 
    melalui pohon keputusan dan sering kali berguna untuk data dengan fitur 
    yang kompleks.
3.  Model #3 : Hutan Acak. Merupakan ansambel dari banyak pohon keputusan 
    yang meningkatkan akurasi dengan mengurangi risiko overfitting.
    
valuasi : Setiap model dievaluasi berdasarkan akurasi dan laporan klasifikasi. Model terbaik dipilih dengan mempertimbangkan metrik seperti akurasi, presisi, recall, dan f1-score.

**02_KELOMPOK F_2 Segmentasi Data dengan Clustering KMeans**
1.  Kumpulan data : cluster_s1
2.  Pustaka : Pandas, Numpy, Scikit-learn, Matplotlib, Seaborn
3.  Tujuan : Mengelompokkan data menjadi beberapa cluster menggunakan 
    KMeans.

**Langkah-langkah :**
1.  Menentukan Jumlah Cluster Terbaik : Gunakan Metode Elbow atau 
    Silhouette 
    Score untuk menemukan jumlah cluster yang optimal.
2.  Pemodelan dengan KMeans : Bangun model KMeans dengan jumlah cluster 
    yang telah ditentukan.
3.  Masukkan Label Cluster ke dalam DataFrame : Tambahkan kolom label hasil 
    clustering ke DataFrame untuk mengetahui cluster dari tiap data.
4.  Plot Hasil Clustering : Visualisasikan hasil clustering dengan Seaborn 
    untuk melihat pembagian data dalam setiap cluster.
5.  Dengan langkah-langkah ini, Anda dapat melakukan segmentasi data 
    menggunakan KMeans dan memvisualisasikan hasilnya untuk analisis lebih 
    lanjut.

**02_KELOMPOK F_3 Regresi dengan TensorFlow-Keras**
1.  Tugas : Memprediksi Harga Rumah
2.  Dataset : Harga Rumah di California
3.  Tujuan : Melakukan prediksi harga rumah dengan pengaturan input ganda 
    menggunakan Multilayer Perceptron (MLP).

**langkah-langkah :**
1.  Mengonversi Data ke DataFrame : Ubah array numpy featuresdan targetke 
    bentuk Pandas DataFrame untuk kemudahan manipulasi data.
2.  Membagi Data : Pisahkan data menjadi train, validation, dan test untuk 
    melatih dan menguji performa model.
3.  Standarisasi dan Normalisasi : Standarisasi menggunakan 
    StandardScalerdan normalisasi dengan MinMaxScalerdata train, 
    validation, dan test.
4.  Membangun Model :
   -  Buat lapisan tersembunyi pertama dengan 30 neuron dan fungsi aktivasi 
      ReLU.
   -  Buat layer tersembunyi kedua dengan 30 neuron dan fungsi aktivasi ReLU.
5.  Pengaturan Pelatihan :
    Tentukan jumlah epoch (jumlah iterasi pelatihan).
    Tentukan ukuran batch.
6.  Simpan dan Muat Ulang Model : Tentukan nama file dengan ekstensi 
    kerasuntuk menyimpan model, kemudian muat ulang model untuk prediksi 
    dengan data baru ( x_new_Adan x_new_B).

**02_KELOMPOK F_4 Klasifikasi dengan PyTorch**
1.  Tugas : Mengklasifikasikan Transaksi Penipuan Kartu Kredit
2.  Dataset : Penipuan Kartu Kredit 2023
3.  Tujuan : Klasifikasi transaksi penipuan kredit menggunakan Multilayer 
    Perceptron (MLP) dengan framework PyTorch.

**Langkah-langkah :**
1.  Mengimpor Dataset : Gunakan fungsi read_by_CPUuntuk mengimpor dataset ke 
    dalam Pandas DataFrame.
2.  Menghapus Kolom ID : Hilangkan kolom ID agar tidak mengubah klasifikasi.
3.  Menentukan Fitur dan Target : Gunakan data_gpuuntuk mendefinisikan X 
    (fitur) dan Y (target).
4.  Membagi Dataset :
   -  Gunakan splitCPUuntuk membagi dataset dengan komposisi 80% untuk train 
      set dan 20% untuk test set.
   -  Gunakan splitGPUuntuk membagi dataset yang sama pada GPU.
5.  Aktifkan GPU : Gunakan CUDA untuk mempercepat proses pelatihan.
6.  Pengaturan Batch dan Hyperparameter :
   -  Tentukan ukuran batch dan atur model hyperparameter seperti jumlah 
      epoch, learning rate, dll.
7.  Parameter dan Hyperparameter :
   -  Parameter : Nilai model yang dipelajari selama pelatihan (misalnya, 
      bobot dan bias neuron).
   -  Hyperparameters : Pengaturan yang menentukan bagaimana model dibor, 
      seperti jumlah epoch, learning rate, atau ukuran batch.
8.  Input Model dan Parameter yang Dapat Dilatih :
   -  entukan ukuran input sesuai dengan fitur pada data.
   -  Semua parameter pada MLP bersifat "trainable", sehingga total 
      parameter sama dengan parameter yang dapat dibor.
9.  ine-Tuning : Jika akurasi model masih di bawah 95%, lakukan fine-tuning 
    engan mengatur kembali hyperparameters atau menambah lapisan dan neuron 
    pada model.
