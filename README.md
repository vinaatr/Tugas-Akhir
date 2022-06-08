# Laporan Tugas Akhir
### Nama          : Vina Trisnawati Rahayu
### NIM           : 205150301111004
### Mata Kuliah   : Arsitektur Jaringan Terkini
### Program Studi : Teknik Komputer
##

## Kata Pengantar
Puji syukur kehadirat Tuhan Yang Maha Esa yang telah memberikan rahmat dan hidayah-Nya sehingga saya dapat dengan lancar menyusun laporan tugas akhir ini guna melengkapi tugas dari mata kuliah Arsitektur Jaringan Terkini. Laporan tugas akhir ini berisikan 4 bagian utama kegiatan pengulangan tugas yang pernah diberikan yakni dimulai dari tugas 1 hingga tugas 4. Saya sebagai penulis berharap semoga laporan yang telah saya buat sedemikian rupa dapat diterima dengan baik. Jika di dalam laporan ini terdapat kesalahan atau kekurangan, saya meminta permohonan maaf sebesar - besarnya. Demikian yang bisa saya sampaikan, saya ucapkan terima kasih. 

## Pembahasan
Di dalam pembuatan dan melakukan pengerjaan tugas akhir ini, kita menggunakan salah satu platform cloud yakni Amazon Web Services (AWS) Academy. Sebelum masuk ke dalam pembahasan bagian utama, kita perlu memulainya dengan login akun AWS Academy terlebih dahulu seperti berikut ini :
1. Login akun AWS Academy sebagai student menggunakan gmail.
<img src="https://user-images.githubusercontent.com/89560767/171982460-a347329f-ad7c-47da-bd7a-3dfe149f4d01.png" width="700">
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp Gambar 1.1
</br>2. Setelah login berhasil, AWS menampilkan menu dashboard untuk pengguna memilih <i>learner lab</i> yang akan digunakan. Pada mata kuliah "Arsitektur Jaringan Terkini" ini, kita menggunakan <i>"Learner Lab ALLFv1-15355"</i>.
<img src="https://user-images.githubusercontent.com/89560767/171984855-0b50ca76-95d7-4fe7-8225-d4429217d35b.png" width="700">
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp Gambar 1.2
</br>3. Di dalam learner lab yang dipilih, terdapat beberapa menu yang salah satu nya adalah modul. Dan di dalam modul tersebut terdapat beberapa opsi lagi, yang mana kita akan memilih <i>"Learner Lab - Foundational Services"</i>. 
<img src="https://user-images.githubusercontent.com/89560767/171995439-f1405073-f6c7-4ea4-9c20-746261fd80c7.png" width="700">
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp Gambar 1.3
</br>4. Setelah itu, tampilan akan seperti Gambar 1.4 yang mana tampilan tersebut merupakan tempat dimana kita akan melakukan perintah - perintah untuk instalasi dan pembuatan topologi dan lain - lain. Sebelum itu, yang perlu diperhatikan adalah simbol merah yang berada disamping tulisan AWS harus berwarna hijau seperti Gambar 1.5 agar AWS dapat berjalan. Maka dari itu, kita perlu memulai nya dengan mengklik <i>Start Lab</i>.
<img src="https://user-images.githubusercontent.com/89560767/171995599-5c701e12-96ef-4fb7-b2b8-947ace03d45d.png" width="700">
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp Gambar 1.4
<img src="https://user-images.githubusercontent.com/89560767/171995612-60404fbd-d3c7-488b-8f95-920ea0078843.png" width="700">
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp Gambar 1.5
</br>5. Setelah simbol AWS sudah berwarna hijau seperti Gambar 1.5, kita klik AWS dan akan muncul seperti Gambar 1.6 lalu kita klik EC2 untuk melanjutkan pembuatan instance.
<img src="https://user-images.githubusercontent.com/89560767/172000977-50df26fa-319f-4c39-98f3-e135b4012e13.png" width="700">
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp Gambar 1.6
</br></br>
Untuk selanjutnya, kita masuk ke 4 poin utama yakni sebagai berikut :

#### A. Pembuatan EC2 Instance di AWS Academy
Setelah melakukan langkah - langkah login diatas, kita melanjutkan dengan membuat instance baru sesuai dengan ketentuan yang diberikan. Instance ini bertujuan untuk memberikan keseimbangan komputasi, memori, dan sumber daya jaringan, serta digunakan untuk berbagai beban kerja. Langkah - langkah dalam pembuatan instance sebagai berikut :
1. Kita klik <i>Launch Instance</i>
<img src="https://user-images.githubusercontent.com/89560767/172526171-d9f95843-b260-4377-ae61-fd7217472bb8.png" width="700">
2. 
<img src="https://user-images.githubusercontent.com/89560767/172526454-2fa908ad-7916-45b1-b6d0-91de0dddc0df.png" width="700">
3.  
<img src="https://user-images.githubusercontent.com/89560767/172526820-8c25a9ac-821a-4cbf-a0e0-18400af609e4.png" width="700">
4.
<img src="https://user-images.githubusercontent.com/89560767/172527254-a1ac7b45-7370-4968-a749-bc35145dd58c.png" width="700">
5.
<img src="https://user-images.githubusercontent.com/89560767/172527326-73be4fa4-31ea-4d22-9dbe-1af9ecbe8738.png" width="700">
6.
<img src="https://user-images.githubusercontent.com/89560767/172526907-32aff2e0-04a2-48f1-bf68-30a910f8d799.png" width="700">
7.
<img src="https://user-images.githubusercontent.com/89560767/172526950-7766ace7-f032-4a3b-ad73-09edc8ecf0ed.png" width="700">
8.
<img src="https://user-images.githubusercontent.com/89560767/172527422-e0218cd5-c3f6-4d81-90ef-5a9728f903c5.png" width="700">
11. Kita perlu mencari tau info mengenai ssh keys nya tersimpan dimana dengan menggunakan perintah ls. Dan key tersebut tersimpan di di .ssh/
