Feedforward Neural Network (FNN)

Penjelasan
Feedforward Neural Network (FNN) adalah jenis jaringan saraf tiruan (Artificial Neural Network, ANN) yang dirancang untuk memproses data secara maju (feedforward). Data bergerak dari input layer ke output layer melalui satu atau lebih hidden layers, tanpa loop atau backtracking.

Komponen Utama
1. Input Layer: Menerima data fitur untuk diproses.
2. Hidden Layers: Melakukan operasi matematis seperti aktivasi non-linear untuk belajar dari pola data.
3. Output Layer: Memberikan hasil akhir berupa prediksi atau klasifikasi.
4. Activation Function: Fungsi seperti ReLU, Sigmoid, atau Softmax digunakan untuk menambah non-linearitas pada model.
5. Optimizer: Algoritma seperti Adam atau SGD digunakan untuk memperbarui bobot selama pelatihan.
6. Loss Function: Fungsi seperti cross-entropy digunakan untuk mengukur perbedaan antara prediksi dan target.

Kelebihan
1. Kemampuan Representasi yang Tinggi: FNN mampu menangkap pola kompleks dalam data, khususnya data non-linear.
2. Fleksibilitas: Dapat digunakan untuk klasifikasi, regresi, dan prediksi time series.
3. Skalabilitas: Dapat diperbesar dengan menambahkan layer dan neuron untuk menangani data besar.

Kekurangan
1. Data yang Tidak Seimbang: Cenderung bias terhadap kelas mayoritas tanpa teknik penanganan khusus.
2. Overfitting: Model yang terlalu kompleks dapat belajar pola yang tidak relevan jika data tidak mencukupi.
3. Waktu Pelatihan Lama: Memerlukan sumber daya komputasi yang lebih besar dibandingkan model tradisional.



Random Forest

Penjelasan
Random Forest adalah algoritma pembelajaran ensemble berbasis pohon keputusan. Algoritma ini menggabungkan beberapa pohon keputusan independen (decision trees) untuk membuat prediksi yang lebih akurat dan stabil.

Cara Kerja

Bootstrap Aggregating (Bagging):
1. Data dilatih menggunakan beberapa subset acak (dengan pengembalian).
2. Setiap subset digunakan untuk melatih satu pohon keputusan.

Random Feature Selection:
1. Saat membangun setiap pohon, hanya sebagian fitur yang dipilih secara acak untuk pembelahan pada setiap node.

Voting (Klasifikasi) atau Rata-rata (Regresi):
1. Untuk klasifikasi, prediksi akhir adalah hasil voting mayoritas dari semua pohon.
2. Untuk regresi, prediksi akhir adalah rata-rata prediksi semua pohon.

Kelebihan
1. Robust terhadap Overfitting: Dengan menggabungkan banyak pohon, Random Forest mengurangi risiko overfitting dibandingkan dengan pohon keputusan tunggal.
2. Skalabilitas: Dapat menangani data besar dan banyak fitur.
3. Menangani Data Tidak Seimbang: Dapat bekerja dengan baik pada data tidak seimbang dengan menyesuaikan parameter seperti class weight.

Kekurangan
1. Kurang Efisien untuk Data Sangat Besar: Jika dataset memiliki jutaan sampel, pelatihan dan prediksi dapat menjadi lambat.
2. Kurang Transparan: Model sulit diinterpretasikan dibandingkan pohon keputusan tunggal.
3. Memory Intensive: Memerlukan lebih banyak memori karena menyimpan banyak pohon.
