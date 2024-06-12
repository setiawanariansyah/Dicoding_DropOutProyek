# Proyek Akhir: Menyelesaikan Permasalahan Perusahaan Edutech

## Business Understanding
Dropout menjadi permasalahan serius termasuk pada Jaya Jaya Institut. Tingginya jumlah dropout yang terjadi pada institusi memberikan dampak negatif yang serius terhadap perguruan tinggi terutama terkait dengan reputasi.

### Permasalahan Bisnis
Beberapa permasalahan yang ingin diselesaikan dalam masalah ini:
1. Apa saja faktor yang berpengaruh terhadap status dropout mahasiswa di Jaya Jaya Institut
2. Apa model terbaik yang didapatkan?

### Cakupan Proyek
Proyek ini akan mencakup beberapa hal diantaranya adalah:
1. Pembuatan model terbaik untuk melakukan prediksi
2. Pembuatan aplikasi dengan streamlit untuk deployment hasil
3. Pembuatan dashboard untuk visualisasi data berdasarkan faktor-faktor sosio-demografi yang berpenagruh terhadap status dropout mahasiswa

### Persiapan

Sumber data: https://github.com/dicodingacademy/dicoding_dataset/tree/main/students_performance

Setup environment:
```
Setup Environment - Shell/Terminal
mkdir proyek1_expertlevel
cd proyek1_expertlevel
pipenv install
pipenv shell
pip install -r requirements.txt
```

## Business Dashboard
Setelah dilakukan pemodelan, dibuat juga dashboard untuk visualisasi data. Beberapa hal yang saya tampilkan pada dashboard diantaranya adalah:
1. Terdapat histogram kursus yang diambil mahasiswa untuk melihat kursus apa saja yang diambil oleh mahasiswa
2. Terdapat treemaps pekerjaan ayah untuk melihat sebaran mahasiswa berdasarkan kategori pekerjaan ayah
3. Terdapat rata-rata kursus pada semester 2 yang disetujui oleh mahasiswa
4. Rata-rata usia pada saat mahasiswa melakukan pendaftaran
5. Terdapat histogram status perkawinan mahasiswa untuk melihat status mahasiswa
6. Terdapat histogram jumlah mahasiswa berdasarkan status

Link dashboard: https://public.tableau.com/views/ProyekAkhirDropout/Dashboard1?:language=en-US&:sid=&:display_count=n&:origin=viz_share_link

## Menjalankan Sistem Machine Learning
Langkah untuk menjalankan sistem machine learning:
1. Download dataset dan kode python yang akan digunakan
2. Download semua requirements yang digunakan
3. Buka file dropout_app.py 
4. Jalankan file kemudian masuk ke terminal dengan mengetikkan kode berikut:
```
streamlit run dropout_app.py
```

## Conclusion
Berdasarkan hasil proyek, terdapat beberapa kesimpulan yang bisa diambil:
1. Faktor yang berpengaruh terhadap status dropout mahasiswa diantaranya adalah unit kulikuler yang disetujui pada semester 2, nilai unit kulikuler pada semester 2, unit kulikuler yang disetujui pada semester 1, unit kulikuler yang dievaluasi pada semester 2, dan nilai unit kulikuler pada semester 1.
2. Berdasarkan kriteria akurasi, model terbaik yang didapatkan adalah gradient boosting 

### Rekomendasi Action Items
Berikan beberapa rekomendasi action items yang harus dilakukan perusahaan guna menyelesaikan permasalahan diantaranya:
- Melakukan pemantauan terhadap unit kulikuler yang disetujui pada semester 2, nilai unit kulikuler pada semester 2, unit kulikuler yang disetujui pada semester 1, unit kulikuler yang dievaluasi pada semester 2, dan nilai unit kulikuler pada semester 1 mahasiswa.
- Melihat rekam riwayat nilai yang dimiliki oleh mahasiswa pada semester sebelumnya.
- Melakukan pengecekan terutama pada kondisi sosial demografi mahasiswa terutama pada pekerjaan ibu dan ayah sekaligus kualifikasi keduanya.
