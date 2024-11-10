**Kasus #1: Klasifikasi dengan Model Pembelajaran Mesin Terbimbing**
1.  Kumpulan data : SC_HW1_bank_data
2.  Perpustakaan : Pandas, Numpy, Scikit-learn
3.  Tujuan : Membangun model klasifikasi untuk memprediksi kolom target “Exited”.

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
2.  Model #2 : Pohon Keputusan. Model ini menawarkan interpretasi yang jelas 
    melalui pohon keputusan dan sering kali berguna untuk data dengan fitur 
    yang kompleks.
3.  Model #3 : Hutan Acak. Merupakan ansambel dari banyak pohon keputusan 
    yang meningkatkan akurasi dengan mengurangi risiko overfitting.

**valuasi : Setiap model dievaluasi berdasarkan akurasi dan laporan klasifikasi. Model terbaik dipilih dengan mempertimbangkan metrik seperti akurasi, presisi, recall, dan f1-score.**

**02 KELOMPOK F Segmentasi Data dengan Clustering KMeans**
1.  Kumpulan data : cluster_s1
2.  Pustaka : Pandas, Numpy, Scikit-learn, Matplotlib, Seaborn
3.  Tujuan : Mengelompokkan data menjadi beberapa cluster menggunakan KMeans.
    Langkah-langkah :

Menentukan Jumlah Cluster Terbaik : Gunakan Metode Elbow atau Silhouette Score untuk menemukan jumlah cluster yang optimal.
Pemodelan dengan KMeans : Bangun model KMeans dengan jumlah cluster yang telah ditentukan.
Masukkan Label Cluster ke dalam DataFrame : Tambahkan kolom label hasil clustering ke DataFrame untuk mengetahui cluster dari tiap data.
Plot Hasil Clustering : Visualisasikan hasil clustering dengan Seaborn untuk melihat pembagian data dalam setiap cluster.
Dengan langkah-langkah ini, Anda dapat melakukan segmentasi data menggunakan KMeans dan memvisualisasikan hasilnya untuk analisis lebih lanjut.
