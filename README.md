# Post Test 3 PBO - Sistem Jadwal Kegiatan (To-Do List)

# Deskripsi Program
Program Manajemen Jadwal Kegiatan (To-do-list) dibuat untuk membantu pengguna dalam mengatur daftar kegiatan sehari-hari.\
Terdapat beberapa pilihan menu dalam program ini sebagai berikut:\
· Dapat menampilkan jadwal yang sudah dibuat.\
· Dapat menambahkan jadwal baru (Sesuai kategori atau subclass, yaitu tambah untuk jadwal mata kuliah/jadwal praktikum).\
· Dapat mengedit jadwal berdasarkan ID.\
· Dapat mencari jadwal (fitur searching).\
· Dapat menghapus jadwal berdasarkan ID.\
Dengan program ini, diharapkan pengguna dapat lebih mudah mengorganisir aktivitas harian secara terstruktur.

-----------------------------------------------------------------------------------------------------------

**1. Fitur**\
· Program mampu melakukan operasi lihat jadwal, tambah jadwal berdasarkan pilihan (tambah jadwal mata kuliah/tambah jadwal praktikum), edit jadwal, hapus jadwal, dan cari jadwal.\
· Program dapat mengelola dan menyimpan informasi seperti, kegiatan, hari, tanggal, dan skala prioritas.

**2. MVC (Model, View, Control)**\
· Model: Class storage yang akan merepresentasikan struktur data dengan properti dan constructor.\
· View: Class main sebagai tampilan awal antarmuka pengguna beserta input & output.\
· Controller: Class CRUD sebagai logika dan operasi CRUD.\
<img width="386" height="325" alt="image" src="https://github.com/user-attachments/assets/16dba0c3-9168-41a0-ae05-32ca5d35a68d" />

**3. Struktur Package**\
· package main: Berisi class main sebagai menu/antarmuka dengan pengguna.\
· package service: Berisi class CRUD sebagai logika dan operasi CRUD.\
· package model: Berisi class jadwal yang didalam nya terdapat **super class dan subsclass** sebagai tempat menyimpan dan representasi struktur data dengan properti dan constructor.

**4. Access Modifier & Properties**\
· Menggunakan access modifier private untuk properti class beserta getter dan setter.\
· Terdapat properties yaitu: ID, kegiatan, hari, tanggal, dan skala prioritas, serta tambahan dari atribut subclass.

**5. Overriding**\
Overriding adalah kemampuan subclass untuk menimpa (override) method yang sudah ada. Overriding pada program ini digunakan agar setiap jenis jadwal seperti (kuliah & praktikum) dapat menimpa setiap detail dan menampilkan atribut yang dimilikinya.

a. Penggunaan Overriding pada Subclass JadwalKuliah\
<img width="803" height="165" alt="image" src="https://github.com/user-attachments/assets/9dea8da4-4f55-49f7-95a8-b15c2791ae58" />

b. Penggunaan Overriding pada Subclass JadwalPraktikum\
<img width="800" height="172" alt="image" src="https://github.com/user-attachments/assets/e9e6ac7d-8b54-4b49-947a-a497d626322e" />

**6. Validasi input**\
Pada program ini terdapat validasi input (Error Handling) seperti akan muncul keterangan, jika tidak sesuai.\
<img width="1229" height="742" alt="Screenshot 2025-09-16 201350" src="https://github.com/user-attachments/assets/c0a556ae-a0bd-47d8-b496-fcacecd715f1" />\
<img width="1209" height="402" alt="Screenshot 2025-09-16 201506" src="https://github.com/user-attachments/assets/0b060685-86ba-48cd-99bb-2b4714280504" />

-----------------------------------------------------------------------------------------------------------

# Alur Program
Terdapat 6 pilihan menu, yaitu:
1. Lihat Jadwal
2. Tambah Jadwal
3. Edit Jadwal
4. Hapus Jadwal
5. Cari Jadwal
6. Keluar
<img width="1299" height="372" alt="image" src="https://github.com/user-attachments/assets/e10823f8-10e6-4f53-89c7-b142f8e79ae7" />

# Penjelasan Menu
**1. Lihat Jadwal**

<img width="1125" height="517" alt="image" src="https://github.com/user-attachments/assets/7cd28619-61d9-482b-912a-34630c5a54df" />


Pada menu "Lihat Jadwal", pengguna dapat melihat jadwal kegiatan yang telah pengguna tambahkan.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**2. Tambah Jadwal**\
terdapat 2 pilihan jika ingin menambahkan jadwal, yaitu ingin menambahkan jadwal untuk mata kuliah atau jadwal untuk praktikum.\
<img width="1109" height="145" alt="image" src="https://github.com/user-attachments/assets/da700f43-765a-4eb5-87d4-2fcd28a19f6a" />


a. Jadwal Kuliah

<img width="1175" height="551" alt="image" src="https://github.com/user-attachments/assets/fa6250f8-8e4d-43a7-badc-bdf839afe85c" />\
Pada menu menambahkan "Jadwal Kuliah", pengguna dapat menambahkan kegiatan mata kuliah kedalam program. Pengguna diminta untuk memasukkan kegiatan, hari, tanggal, skala prioritas, mata kuliah, dan dosen

b. Jadwal Praktikum

<img width="1153" height="550" alt="image" src="https://github.com/user-attachments/assets/85379e8a-2ddc-4223-a1fe-e53ce2d847b9" />\
Pada menu menambahkan "Jadwal Praktikum", pengguna dapat menambahkan kegiatan praktikum kedalam program. Pengguna diminta untuk memasukkan kegiatan, hari, tanggal, skala prioritas, praktikum, dan deadline.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**3. Edit Jadwal**

<img width="1205" height="228" alt="Screenshot 2025-09-16 201021" src="https://github.com/user-attachments/assets/1939993b-4bc4-43df-b905-e422ae897847" />

Pada menu "Edit Jadwal", pengguna dapat mengedit jadwal kegiatan yang sudah ada dengan cara: menginput ID jadwal yang ingin diedit, dengan memasukkan kembali nama kegiatan, hari, tanggal, dan skala prioritas kegiatan tersebut.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**4. Hapus Jadwal**

<img width="1201" height="148" alt="Screenshot 2025-09-16 201048" src="https://github.com/user-attachments/assets/329ccf2e-99b7-4e5d-ad47-d3b397012dcc" />

Pada menu "Hapus Jadwal", pengguna dapat menghapus jadwal kegiatan yang sudah ada dengan cara menginput ID jadwal yang ingin dihapus.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**5. Cari Jadwal (Searching)**

<img width="1187" height="258" alt="Screenshot 2025-09-16 201117" src="https://github.com/user-attachments/assets/286653a6-06fe-4ecc-97e0-233d8f35a087" />

Pada menu "Cari Jadwal" atau biasa disebut dengan searching. Pengguna dapat mencari jadwal kegiatan yang telah ada dengan cara cukup memasukkan keyword yang ingin dicari. Sebagai contoh saya memasukkan keyword "Post Test" lalu muncul kegiatan yang memiliki keyword atau kalimat tersebut.

**6. Keluar**

<img width="1183" height="286" alt="Screenshot 2025-09-16 201135" src="https://github.com/user-attachments/assets/6ab991e2-d053-4dd7-97f5-022768ec7303" />

Pada menu "keluar", pengguna akan keluar dari program.
