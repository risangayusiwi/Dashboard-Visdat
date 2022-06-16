# Rancangan Dashboard


## Dataset
Penelitian ini menggunakan data sekunder yang bersumber dari Badan Pusat Statistik. 
Data yang digunakan merupakan data-data indikator kemiskinan pada 34 provinsi di Indonesia yang diambil pada bulan September 2021. 
Variabel yang digunakan sebagai indikator adalah Garis Kemiskinan, Persentase Penduduk Miskin, Indeks Kedalaman Kemiskinan, dan Indeks Keparahan Kemiskinan.
Dari variabel tersebut akan dilakukan analisis cluster yang menghasilkan kelompok tingkat kemiskinan.

## Prepocessing Data
Pada prepocessing data dilakukan data cleaning, data integration, dan data transformation. 
- Data cleaning  berfungsi untuk mengganti missing value, mengatasi data noise, dan  menghilangkan data yang redundan. 
- Data integration berfungsi menggabungkan variabel-varabel menjadi satu bentuk data. 
- Data transformation berfungsi untuk menormalisasikan data, pada tahap ini data distandarisasi agar tidak terdapat perbedaan satuan yang besar. 

## Metode Analisis
1. Analisis Deskriptif
  - Pada analisis deskriptif dihitung nilai minimum, nilai maksimum, rata-rata dan standar deviasi untuk melihat persebaran dari data.
  - Selain itu, dilakukan visualisasi berupa boxplot menggunakan data yang telah distandarisasi untuk mengetahui outlier pada data.
    - ![boxplot](https://user-images.githubusercontent.com/75960081/174086895-467303a1-0b32-4016-adb0-fddecc452c5d.jpg)
2. Analisis Cluster Menggunakan K-Means
Analisis cluster dilakukan dengan beberapa tahapan. Berikut ini adalah tahapan-tahapan menggunakan algoritma K-Means.
  - Menentukan nilai K : pertimbangan memilih k optimal menggunakan metode Slihouette dan penelitian terdahulu
  - Cluster menggunakan K-Means : Berdasarkan hasil analisis cluster diperoleh 3 cluster, yaitu cluster 1 (tingkat kemiskinan sedang) terdiri dari 16 provinsi, cluster 2 (tingkat kemiskinan rendah) terdiri dari 15 provinsi, dan cluster 3 (tingkat kemiskinan tinggi) terdiri dari 3 provinsi.
  - Karakteristik Setiap cluster : 
    ![cluster](https://user-images.githubusercontent.com/75960081/174087536-dad90b9b-feac-43a9-9979-10e85b19164a.jpg)
    - Cluster 1 adalah kelompok provinsi yang memiliki tingkat kemiskinan sedang, dimana rata-rata indikator Persentase Penduduk Miskin, Indeks Kedalaman, dan Indeks Keparahan  sedang. Namun Indikator Garis Kemiskinan memiliki rata-rata yang rendah.
    - Cluster 2 adalah kelompok provinsi yang memiliki tingkat kemiskinan rendah, dimana rata-rata indikator Persentase Penduduk Miskin, Indeks Kedalaman, dan Indeks Keparahan  rendah. Namun Indikator Garis Kemiskinan memiliki rata-rata yang tinggi.
    - Cluster 3 adalah kelompok provinsi yang memiliki tingkat kemiskinan tinggi, dimana rata-rata indikator Persentase Penduduk Miskin, Indeks Kedalaman, dan Indeks Keparahan  tinggi. Namun Indikator Garis Kemiskinan memiliki rata-rata yang sedang.

## Visualisasi Data dan Dashboard
- Visualisasi data dilakukan pada setiap indikator tingkat kemiskinan dan hasil dari analisis cluster yang bersifat interaktif. Setelah itu visualisasi data ini akan disatukan ke dalam bentuk dashboard. Visualisasi yang digunakan adalah:
  - Peta tematik : digunakan untuk melihat persebaran setiap variabel di 34 provinsi di Indonesia
  - Bar chart : digunakan untuk membandingkan suatu variabel di tiap provinsi
  - Pie chart : digunakan untuk melihat persentase provinsi yang termasuk dalam tingkat kemiskinan rendah, sedang, atau tinggi
  - Tabulasi data : tabel yang berisi data yang digunakan
  - Boxplot : digunakan untuk melihat sebaran data dan mendeteksi outlier
- Pada penelitian ini, terdapat 5 halaman dashboard, yaitu:
  - Hasil Cluster
    ![hasil cluster (1)](https://user-images.githubusercontent.com/75960081/174028590-7857c509-b493-4512-8d3f-f27a06865add.png)
    ![hasil cluster(2)](https://user-images.githubusercontent.com/75960081/174028627-8a9344a8-2ffb-481b-93ba-6106779e0860.png)
  - Garis Kemiskinan
    ![garis kemiskinan](https://user-images.githubusercontent.com/75960081/174028622-593f8948-0689-41a7-a9f0-af5305c04152.png)
  - Persentase Penduduk Miskin
    ![persentase penduduk miskin](https://user-images.githubusercontent.com/75960081/174028714-0a696f5f-3c0b-479f-b435-6a3fa7f682d3.png)
  - Indeks Kedalaman Kemiskinan
    ![indeks kedalaman](https://user-images.githubusercontent.com/75960081/174028676-fd583e4d-02e2-42a1-95af-667cb278b39e.png)
  - Indeks Keparahan Kemiskinan
    ![indeks keparahan](https://user-images.githubusercontent.com/75960081/174028698-20418389-a737-491d-9d7f-3dc3dcef84af.png)
    

