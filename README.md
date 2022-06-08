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
Setelah melakukan langkah - langkah login diatas, kita melanjutkan dengan membuat instance baru sesuai dengan ketentuan yang diberikan. Ketentuan tersebut sebagai berikut :
* Name and tags: Tugas Akhir
* OS Images: Ubuntu Server 22.04 LTS 64 bit
* Instance type: t2.medium
* Key pair: vockey
* Edit Network settings: allow SSH, allow HTTP, allow HTTPS, allow TCP port 8080, allow TCP port 8081
* Configure storage: 30 GiB, gp3
</br>
Instance ini bertujuan untuk memberikan keseimbangan komputasi, memori, dan sumber daya jaringan, serta digunakan untuk berbagai beban kerja. Langkah - langkah dalam pembuatan instance sebagai berikut :
</br>1. Kita klik <i>Launch Instance</i>
<img src="https://user-images.githubusercontent.com/89560767/172526171-d9f95843-b260-4377-ae61-fd7217472bb8.png" width="700">
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp Gambar 1.7
</br>2. Di dalam launch instance ini, kita mengisi sesuai dengan ketentuan yang diberikan. Pertama name and tags nya kita beri nama Tugas Akhir.
<img src="https://user-images.githubusercontent.com/89560767/172526454-2fa908ad-7916-45b1-b6d0-91de0dddc0df.png" width="700">
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp Gambar 1.8
</br>3. Melakukan pemilihan OS image yang digunakan yakni Ubuntu Server 22.04 LTS 64 bit
<img src="https://user-images.githubusercontent.com/89560767/172526820-8c25a9ac-821a-4cbf-a0e0-18400af609e4.png" width="700">
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp Gambar 1.9
</br>4.Melakukan pemilihan Instance type: t2.medium Key pair: vockey 
<img src="https://user-images.githubusercontent.com/89560767/172527254-a1ac7b45-7370-4968-a749-bc35145dd58c.png" width="700">
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp Gambar 2.0
</br>5. Memilih Key pair: vockey 
<img src="https://user-images.githubusercontent.com/89560767/172527326-73be4fa4-31ea-4d22-9dbe-1af9ecbe8738.png" width="700">
6.
<img src="https://user-images.githubusercontent.com/89560767/172526907-32aff2e0-04a2-48f1-bf68-30a910f8d799.png" width="700">
7.
<img src="https://user-images.githubusercontent.com/89560767/172526950-7766ace7-f032-4a3b-ad73-09edc8ecf0ed.png" width="700">
8.
<img src="https://user-images.githubusercontent.com/89560767/172527422-e0218cd5-c3f6-4d81-90ef-5a9728f903c5.png" width="700">
9.
<img src="https://user-images.githubusercontent.com/89560767/172527871-2600511a-8931-448e-b9a3-e37ef05498fd.png" width="700">
<img src="https://user-images.githubusercontent.com/89560767/172528655-30ed25f7-6d0e-41bd-9024-0a8a1de4c35c.png" width="700">
10.
<img src="https://user-images.githubusercontent.com/89560767/172527935-a0cb250a-29ea-43f0-9176-eb8e28b15e1c.png" width="700">
11.
<img src="https://user-images.githubusercontent.com/89560767/172528098-716dfc86-bca9-4215-ac8b-8a809f0a122e.png" width="700">
12. Kita perlu mencari tau info mengenai ssh keys nya tersimpan dimana dengan menggunakan perintah ls. Dan key tersebut tersimpan di di .ssh/
<img src="https://user-images.githubusercontent.com/89560767/172528165-d7c49d5f-5845-48bc-9b95-e7892e217824.png" width="700">
13.
<img src="https://user-images.githubusercontent.com/89560767/172530514-9b577280-b557-4129-8da2-7bcaab2dc4fa.png" width="700">
<img src="https://user-images.githubusercontent.com/89560767/172530523-375a25a5-09f8-4244-9ade-e8e726e6595a.png" width="700">
14.
<img src="https://user-images.githubusercontent.com/89560767/172534043-c366a38d-69fe-423c-937b-5771ecb14e27.png" width="700">
<img src="https://user-images.githubusercontent.com/89560767/172534089-7d807d65-96b7-4ac3-8e56-decbe37a30d2.png" width="700">
15.
<img src="https://user-images.githubusercontent.com/89560767/172534178-9b9b5cdb-bc0c-496e-a2a3-a82a26e80fc9.png" width="700">
16. 
<img src="https://user-images.githubusercontent.com/89560767/172534579-bde7ea0e-4f2c-489b-a594-9b80fc872a8d.png" width="700">
<img src="https://user-images.githubusercontent.com/89560767/172534597-56f9035f-3a9f-424d-a0aa-29e34f1ef595.png" width="700">
17.
<img src="https://user-images.githubusercontent.com/89560767/172535336-024236b7-6b0b-4fbe-a7cc-16742c9673ce.png" width="700">
18.
<img src="https://user-images.githubusercontent.com/89560767/172535468-a071dd8e-abde-4b93-9a4f-9e071bc5d3ef.png" width="700">
19.
<img src="https://user-images.githubusercontent.com/89560767/172535589-7d6ea150-efd0-4b7e-9559-927c79ca739e.png" width="700">
<img src="https://user-images.githubusercontent.com/89560767/172535688-5d4869db-49de-4d52-a049-2ccb94b6fed8.png" width="700">
20.
<img src="https://user-images.githubusercontent.com/89560767/172535941-4da8f770-4906-4775-b14c-b0d0e89abf9c.png" width="700">
21.
<img src="https://user-images.githubusercontent.com/89560767/172536025-823c019b-efe6-4b9e-b8a2-05476fee5b21.png" width="700">

#### B. Membuat Custom Topologi Mininet
Setelah melewati pembuatan instance EC2 dan instalasi mininet, flowmanager, dan juga ryu. Maka, untuk bagian selanjutnya yaitu membuat custom topologi berupa topology mininet 2 host dan 2 switch serta topology mininet 3 switch (loop) dengan 6 host sebagai berikut :

<b> 1.1 Topologi Mininet 2 host dan 2 switch </b>
</br>1. 
<img src="https://user-images.githubusercontent.com/89560767/172621671-df3b1bf7-943d-4615-b210-d8990538e01c.png" width="700">
2.
<img src="https://user-images.githubusercontent.com/89560767/172621709-91f6aa1e-daa0-4f16-9866-771f98e8c71a.png" width="700">
3.
<img src="https://user-images.githubusercontent.com/89560767/172621880-c2649ad9-088a-4e5a-a5c7-4c0f24919512.png" width="700">
4.
<img src="https://user-images.githubusercontent.com/89560767/172622153-33f406a9-56be-4207-8e9d-9c30a0faf7e4.png" width="700">
5.
<img src="https://user-images.githubusercontent.com/89560767/172622199-958ea335-b61c-4c70-8751-c9cb661e8821.png" width="700">

</br><b> 1.2 Topologi Mininet 3 switch (loop) dan 6 host </b>
</br>1.
<img src="https://user-images.githubusercontent.com/89560767/172622794-b0153ff2-6ebe-40f1-ac2d-e4d6c95d4ef8.png" width="700">

2.
<img src="https://user-images.githubusercontent.com/89560767/172622833-8f41da29-d373-427c-8b27-68580dd6c3b7.png" width="700">

3.
<img src="https://user-images.githubusercontent.com/89560767/172622893-76f06195-fa96-4a96-bdcf-e1d075bc7c00.png" width="700">

4.
<img src="https://user-images.githubusercontent.com/89560767/172622952-6e28aded-f40f-4ed9-ab47-2c79c654f436.png" width="700">

5.
<img src="https://user-images.githubusercontent.com/89560767/172623015-d1bac1f3-8fdb-4d79-84d6-85ae669ba3aa.png" width="700">

#### C. Membuat aplikasi Ryu Load Balancer
<img src="https://user-images.githubusercontent.com/89560767/172624155-6a484291-77b6-42b6-8163-1a1c084dcdcb.png" width="700">

1. 
<img src="https://user-images.githubusercontent.com/89560767/172624512-612132ac-9baf-4d6e-b1ee-8f1fc83ec761.png" width="700">
2.
<img src="https://user-images.githubusercontent.com/89560767/172624656-b2ce1d80-b424-47c0-a94b-cb4fcc04a7ac.png" width="700">
3.
<img src="https://user-images.githubusercontent.com/89560767/172624739-2cf6850e-be21-494c-bee0-620be22234c9.png" width="700">
4.
![image](https://user-images.githubusercontent.com/89560767/172633168-9cdc14de-0267-477a-80cc-8aedc3497183.png)
![image](https://user-images.githubusercontent.com/89560767/172634466-cd944299-c9cf-48e5-902f-26b447d4554f.png)
5.
![image](https://user-images.githubusercontent.com/89560767/172634541-183d37cd-d1bc-467b-b8b9-11e52d823ff7.png)
6.
![image](https://user-images.githubusercontent.com/89560767/172634597-e30ae68b-6b1d-44dd-8e8e-510e96be3e6b.png)
![image](https://user-images.githubusercontent.com/89560767/172633344-927d42b8-9379-4ba1-80b9-b7c376c5fca3.png)
7.
![image](https://user-images.githubusercontent.com/89560767/172634718-b8099b6a-8a02-40bb-8ef2-3de76ec79714.png)
![image](https://user-images.githubusercontent.com/89560767/172633427-267ac801-9ef8-4df4-b122-08d9621fa8d4.png)

#### D. Membuat aplikasi Ryu Shortest Path Routing
![topologi tugas 4](https://user-images.githubusercontent.com/89560767/172633920-4c9a00f4-2ffd-4064-b1cf-d41126df4044.png)

1.
![git clone](https://user-images.githubusercontent.com/89560767/172637346-0cb961ca-a354-43e7-bf24-3f0f2f21e088.png)
2.
![masuk cd SPF](https://user-images.githubusercontent.com/89560767/172637379-710ab213-5ab0-42c2-8bb5-93a4f8908024.png)
3.
![image](https://user-images.githubusercontent.com/89560767/172637418-3094a745-b691-4276-a956-a4d324beda47.png)
4.
![image](https://user-images.githubusercontent.com/89560767/172637484-9c838511-f093-45a3-aee9-670f28110f82.png)
5.
![image](https://user-images.githubusercontent.com/89560767/172637565-25388300-467e-43f1-a5f3-b6f4f43cdda2.png)
6.
![image](https://user-images.githubusercontent.com/89560767/172637612-5c8f0c24-a8b4-47e3-a9c0-d80f85220494.png)
7.
![image](https://user-images.githubusercontent.com/89560767/172637790-c3f9641e-7804-41f5-a87a-93035472b2ab.png)
8.
![image](https://user-images.githubusercontent.com/89560767/172637807-00600c94-6bdc-4ae7-b04f-acc30147e8dc.png)
9.
![image](https://user-images.githubusercontent.com/89560767/172637846-5b9fb0f4-c2e6-4bd0-90a6-12de254aae55.png)
![image](https://user-images.githubusercontent.com/89560767/172637923-31ab0cb7-aea0-4fae-a19f-024c532929f2.png)
![image](https://user-images.githubusercontent.com/89560767/172637967-029fee3c-e2bf-4308-9f0b-8b24d4657cac.png)
![image](https://user-images.githubusercontent.com/89560767/172638002-6b32adb6-4275-414e-ae59-0626d1025ffe.png)
![image](https://user-images.githubusercontent.com/89560767/172638035-ca733360-475f-4c14-a35c-4753620c4b0d.png)
![image](https://user-images.githubusercontent.com/89560767/172638090-18634647-70a3-486f-9b68-3ad437267f3d.png)
10.
![image](https://user-images.githubusercontent.com/89560767/172638134-ebba1ee1-dad4-4f89-8ad2-9337867e3d4e.png)
11.

