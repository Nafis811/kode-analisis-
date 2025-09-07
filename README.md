Muhammad Nafis Dwi Noviansyah

Analisis dan Deteksi Akun Palsu di Media Sosial

1. Project Overview
Proyek ini bertujuan untuk membangun model machine learning yang mampu mengidentifikasikan akun palsu di mediasosial secara akurat dan efisien. sebagai respon atas maraknya masalah akun palsu dan bot. saya menggunakan dataset publik dari berbagai akun, dengan fokus pada metrik perilaku alih-alih metrik popularitas yang mudah dimanipulasi. Proyek ini sangat berguna bagi pengiklan dan pemasar digital Dengan memastikan mereka berinteraksi dan beriklan kepada audiens yang asli, mereka dapat mengoptimalkan anggaran iklan dan mendapatkan hasil yang lebih akurat dari kampanye mereka.

Raw dataset
- Nama File         : `user_fake_authentic_2class.csv`
- link raw dataset  :(https://github.com/Nafis811/kode-analisis-/blob/main/user_fake_authentic_2class.csv)
- Deskripsi Label:
  - `f` = akun palsu
  - `r` = akun asli

Inisight and findings
setelah Analisis data awal kami mengungkapkan adanya perbedaan perilaku signifikan antara akun asli dan palsu. Dengan menggunakan model machine learning berbasis pohon keputusan, kami berhasil mengidentifikasi dan mengukur faktor-faktor kunci yang membedakan kedua jenis akun ini.

#### **Kinerja Model**
- **Akurasi**: Model `RandomForestClassifier` mencapai akurasi lebih dari 90%.
- **Efisiensi**: Model ini sangat efektif dalam mendeteksi akun palsu, dengan **tingkat *false negative* yang rendah**, yang berarti sangat sedikit akun palsu yang lolos dari deteksi.

#### **Fitur Pembeda Utama**
Model mengidentifikasi fitur-fitur berikut sebagai yang paling krusial:
- **Jumlah *Following*** (`flg`): Akun palsu cenderung memiliki pola *following* yang tidak wajar.
- **Ketersediaan *Link*** (`lin`): Fitur ini adalah pembeda kuat, di mana akun palsu hampir selalu menyertakan tautan di bio mereka.
- **Tingkat *Engagement* Komentar** (`erc`): Akun palsu memiliki interaksi yang sangat rendah, mengindikasikan kurangnya aktivitas manusia.

### **4. Penjelasan Bantuan AI**
Proyek ini dikerjakan dengan bantuan AI untuk mempercepat proses, mulai dari penulisan kode untuk analisis data, pembuatan visualisasi, hingga penyusunan kesimpulan dan rekomendasi. Bantuan ini memungkinkan fokus lebih pada interpretasi hasil daripada pada proses teknis.
