Muhammad Nafis Dwi Noviansyah

#### **Analisis dan Deteksi Akun Palsu di Media Sosial**

#### **1. Project Overview**
Proyek ini bertujuan untuk membangun model machine learning yang mampu mengidentifikasikan akun palsu di mediasosial secara akurat dan efisien. sebagai respon atas maraknya masalah akun palsu dan bot. saya menggunakan dataset publik dari berbagai akun, dengan fokus pada metrik perilaku alih-alih metrik popularitas yang mudah dimanipulasi. Proyek ini sangat berguna bagi pengiklan dan pemasar digital Dengan memastikan mereka berinteraksi dan beriklan kepada audiens yang asli, mereka dapat mengoptimalkan anggaran iklan dan mendapatkan hasil yang lebih akurat dari kampanye mereka.

#### **2. Raw dataset**
- Nama File         : `user_fake_authentic_2class.csv`
- link raw dataset  :(https://github.com/Nafis811/kode-analisis-/blob/main/user_fake_authentic_2class.csv)
- Deskripsi Label:
  - `f` = akun palsu
  - `r` = akun asli

#### **3. Inisight and findings**
setelah Analisis data awal kami mengungkapkan adanya perbedaan perilaku signifikan antara akun asli dan palsu. Dengan menggunakan model machine learning berbasis pohon keputusan, kami berhasil mengidentifikasi dan mengukur faktor-faktor kunci yang membedakan kedua jenis akun ini.

#### **Kinerja Model**
Model RandomForestClassifier yang saya bangun menunjukkan kinerja yang sangat baik. saya mencapai akurasi lebih dari 90% dalam membedakan akun palsu dan asli. Yang lebih penting, tingkat false negative (akun palsu yang salah diklasifikasikan sebagai asli) sangat rendah.

#### **Fitur Pembeda Utama**
1. Pola Following (flg)
Berdasarkan analisis data, fitur flg menunjukkan bahwa akun palsu (f) memiliki pola following yang berbeda dari akun asli (r). Analisis lebih dalam sering kali menunjukkan bahwa akun palsu cenderung mengikuti sejumlah besar akun dalam waktu singkat, yang merupakan taktik untuk menarik perhatian pengguna lain agar melakukan follow back. Pola ini kontras dengan akun asli yang umumnya mengikuti akun secara lebih organik dan bertahap.

2.Pola Penggunaan Hashtag (hc)
Fitur hc menunjukkan bahwa akun palsu cenderung menggunakan hashtag dengan pola yang sangat seragam. Misalnya, mereka mungkin memposting dengan jumlah hashtag yang sama persis di setiap unggahan. Pola ini dapat menjadi indikasi bahwa akun tersebut dioperasikan oleh bot yang diprogram, bukan oleh manusia. Sebaliknya, akun asli menunjukkan variasi yang lebih besar dalam penggunaan hashtag mereka, mencerminkan perilaku manusia yang lebih spontan dan tidak teratur.

3. Penggunaan Kata Kunci Promosi (pr)
Fitur pr mengukur seberapa sering akun menggunakan kata kunci yang bersifat promosi. Akun palsu lebih sering menggunakan kata kunci promosi dibandingkan dengan akun asli. Ini karena tujuan utama akun palsu sering kali adalah untuk mengarahkan lalu lintas ke situs web tertentu atau mempromosikan produk secara instan. Pola ini menjadikan fitur pr sebagai indikator kuat untuk mendeteksi akun palsu.

### **4. Penjelasan Bantuan AI**
Model ai ini digunakan untuk membantu proses akhir analisis seperti merangkum insight insight yang sudah saya temukan dan menjadi poin poin yang dapat disimpulkan dalam presentasi sesuai objektif dari projek IBM Granite model 
