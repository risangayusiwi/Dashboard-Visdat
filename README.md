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
2. Analisis Cluster Menggunakan K-Means
Analisis cluster dilakukan dengan beberapa tahapan. Berikut ini adalah tahapan-tahapan menggunakan algoritma K-Means.
- Menentukan nilai K : pertimbangan memilih k optimal menggunakan metode Slihouette dan penelitian terdahulu
- Cluster menggunakan K-Means : Berdasarkan hasil analisis cluster diperoleh 3 cluster, yaitu cluster 1 (tingkat kemiskinan sedang) terdiri dari 16 provinsi, cluster 2 (tingkat kemiskinan rendah) terdiri dari 15 provinsi, dan cluster 3 (tingkat kemiskinan tinggi) terdiri dari 3 provinsi.
- Karakteristik Setiap cluster : 
  - Cluster 1 adalah kelompok provinsi yang memiliki tingkat kemiskinan sedang, dimana rata-rata indikator Persentase Penduduk Miskin, Indeks Kedalaman, dan Indeks Keparahan  sedang. Namun Indikator Garis Kemiskinan memiliki rata-rata yang rendah.
  - Cluster 2 adalah kelompok provinsi yang memiliki tingkat kemiskinan rendah, dimana rata-rata indikator Persentase Penduduk Miskin, Indeks Kedalaman, dan Indeks Keparahan  rendah. Namun Indikator Garis Kemiskinan memiliki rata-rata yang tinggi.
  - Cluster 3 adalah kelompok provinsi yang memiliki tingkat kemiskinan tinggi, dimana rata-rata indikator Persentase Penduduk Miskin, Indeks Kedalaman, dan Indeks Keparahan  tinggi. Namun Indikator Garis Kemiskinan memiliki rata-rata yang sedang.

## Visualisasi Data dan Dashboard
Visualisasi data dilakukan pada setiap indikator tingkat kemiskinan dan hasil dari analisis cluster yang bersifat interaktif. Setelah itu visualisasi data ini akan disatukan ke dalam bentuk dashboard. Visualisasi yang digunakan adalah:
- Peta tematik : digunakan untuk melihat persebaran setiap variabel di 34 provinsi di Indonesia
- Bar chart : digunakan untuk membandingkan suatu variabel di tiap provinsi
- Pie chart : digunakan untuk melihat persentase provinsi yang termasuk dalam tingkat kemiskinan rendah, sedang, atau tinggi
- Tabulasi data
Pada penelitian ini, terdapat 5 halaman dashboard, yaitu:
- Hasil Cluster
  [![cluster1](image/hasil cluster(1))
  [![cluster2](image/hasil cluster(2))
- Garis Kemiskinan
  [![cluster1](image/garis kemiskinan)
- Persentase Penduduk Miskin
  [![cluster1](image/persentase penduduk miskin)
- Indeks Kedalaman Kemiskinan
  [![cluster1](image/indeks kedalaman)
- Indeks Keparahan Kemiskinan
  [![cluster1](image/indeks keparahan)
