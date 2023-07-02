# Capstone_Project_Modul_3
Machine Learning - Regression Model

Pada project ini kita akan membuat model regresi dengan dataset yang berisi informasi mengenai harga rumah di California.
Dataset memiliki 10 kolom, yaitu:
- longitude : Koordinat garis bujur
- langitude : koordinat garis lintang
- Housing median age : Median umur dari kumpulan rumah
- total rooms : Total kamar dari kumpulan rumah
- total bedrooms : Total kamar tidur dari kumpulan rumah
- population : Populasi pada daerah dimana kumpulan rumah itu berada
- households : Jumlah keluarga pada daerah tersebut
- median income : Median pendapatan pada daerah tersebut
- median house value : Median harga rumah pada daerah tersebut
- ocean_proximity : Lokasi rumah berdasarkan jaraknya dengan laut

Goals dari project ini adalah menghasilkan sebuah tools yang dapat membantu broker dalam menentukan harga rumah.

Tahapan yang akan kita lakukan untuk membuat model adalah sebagai berikut:
- Data Understanding
  Di tahap ini kita akan melihat apakah format data pada tiap kolom sesuai atau tidak, dan kita juka akan mengecek apakah ada missing value dan duplikat
- Data Cleaning
  Di tahap ini kita akan membersihkan data berdasarkan data understanding yang sudah kita lakukan
- Explanatory Data Analysis (EDA)
  Di tahap ini kita akan fokus menganalisa hubungan feature dengan target (median house value)
- Data Preprocessing
  Di tahap ini kita akan mengklasifikasikan data ke dalam 2 variabel, yaitu variabel X akan menyimpan kolom-kolom yang merupakan feature dan variabel y untuk kolom target, lalu     kita akan melakukan data splitting untuk menghindari information leakage
- Modeling
  Di tahap ini kita akan mencoba 2 skenario. Skenario 1 kita akan menggunakan data yang outliernya kita biarkan, dan skenario 2 kita akan mencoba mengurangi jumlah outlier pada     dataset. Hasil dari 2 skenario ini nanti akan kita evaluasi dan bandingkan.
  Pada tahap ini kita akan melakukan cross validation untuk menentukan benchmark model, yaitu model dengan algoritma yang menghasilkan hasil prediksi terbaik. Setelah itu           benchmark model akan kita lakukan hyperparameter tuning dengan harapan dapat meningkatkan performa dari model
- Evaluasi Model
  Kita akan melakukan evaluasi dengan melihat performa model berdasarkan metric RMSE, MAE, dan MAPE. Untuk melihat persebaran residual yang dihasilkan kita akan menggunakan         residual plot, dengan residual plot kita juga dapat membuat segmentasi yang menunjukan model kita memiliki performa paling baik di range harga berapa. Lalu untuk melihat          feature apa saja yang paling mempengaruhi harga rumah kita akan melakukan analisa feature importance yang nantinya akan kita bandingkan dengan EDA yang sudah kita lakukan
