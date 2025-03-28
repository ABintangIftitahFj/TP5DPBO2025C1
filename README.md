## JANJI
Saya A Bintang Iftitah FJ dengan NIM 2305995 mengerjakan Tugas Praktikum 5 dalam mata kuliah Desain dan Pemrograman Berorientasi Objek untuk keberkahanNya maka saya tidak melakukan kecurangan seperti yang telah dispesifikasikan. Aamiin.

## Desain Program 
Program di buat dalam bentuk oop pada java swing untuk interface pengguna. Program memiliki tujuan CRUD (create,read,update,delete) dengan menggunakan koneksi localhost mysql menggunakan JDBC.

## Desain class 

### 1. Class Mahasiswa 
class ini berguna dalam menyimpan atribut untuk data mahasiswa yaitu NIM,Nama,JenisKelamin,dan JalurMasuk mahasiswa. 

### 2. Class menu Extends JFrame 
class ini berguna dalam Graphical user interface (GUI) dan memiliki methode insert update delete.

### 3. Class Database
kelas ini berfungsi untuk menymabungkan database local dengan program swing ui. Terdapat methode untuk menjalankan query sql 'select' , dan `insertUpdateDeletequery`.

## Alur Program 

## 1. Tampilan Awal  
Saat program dijalankan, objek `Menu` akan dibuat, yang kemudian menampilkan jendela utama.  
Pada konstruktor `Menu`, dilakukan inisialisasi koneksi ke database MySQL serta pengaturan fungsi untuk tombol, tabel, dan elemen tampilan lainnya.  

## 2. Menambahkan Data  
Pengguna mengisi formulir dengan data berikut:  
- `nim`  
- `nama`  
- `jenisKelamin`  
- `jalurMasuk`  

Setelah itu, pengguna menekan tombol **Add**, yang akan memanggil method `insertData()` untuk:  
- Mengambil nilai dari form input.  
- Menyimpan data ke dalam database.  
- Memperbarui tampilan tabel dengan `setTable()`.  
- Mengosongkan form melalui `clearForm()`.  
- Menampilkan pop-up sebagai konfirmasi keberhasilan.
- jika ada data yang kosong pop up pesan eror akan muncul.  

## 3. Memperbarui Data  
Pengguna memilih salah satu data dalam tabel untuk diedit, mengubah isi form sesuai kebutuhan, lalu menekan tombol **Update**.  
Tombol ini akan memanggil `updateData()`, yang akan:  
- Mengambil data dari form input.  
- Memperbarui entri yang sesuai di database.  
- Memperbarui tampilan tabel menggunakan `setTable()`.  
- Mengosongkan form dengan `clearForm()`.  
- Menampilkan notifikasi keberhasilan.
- Jika ada data yang kosong pesan eror akan muncul.

## 4. Menghapus Data  
Pengguna memilih data dari tabel lalu menekan tombol **Delete**. Sebelum penghapusan, program akan menampilkan pop-up konfirmasi.  
Jika pengguna menyetujui, maka `deleteData()` akan dijalankan untuk:  
- Mengambil nilai `nim` dari form input.  
- Menghapus data yang sesuai dari database.  
- Memperbarui tampilan tabel dengan `setTable()`.  
- Mengosongkan form menggunakan `clearForm()`.  
- Menampilkan notifikasi keberhasilan.  

## 5. Memilih dan Membatalkan Perubahan Data  
Ketika pengguna mengklik salah satu baris pada tabel, event `mouseListener` akan dijalankan untuk:  
- Mengambil data dari baris yang dipilih.  
- Memasukkan data tersebut ke dalam form input.  
- Mengubah tombol **Add** menjadi **Update**.  
- Menampilkan tombol **Delete** dan **Cancel**.  
- Jika tombol **Cancel** ditekan, maka form akan dikosongkan menggunakan `clearForm()`.

## Dokumentasi 


 ![Screenshot 2025-03-27 233348](https://github.com/user-attachments/assets/f3a0a5e0-a7b6-4ffd-95b8-b6c75a2ad503)

![Screenshot 2025-03-27 233520](https://github.com/user-attachments/assets/5948ebdc-c072-4492-9388-89587a364322)

![Screenshot 2025-03-27 233812](https://github.com/user-attachments/assets/6343034f-9c7d-46a0-b06f-fe930f0608af)


![Screenshot 2025-03-27 233532](https://github.com/user-attachments/assets/9373d5f5-21b5-4a6c-be41-ac24678e1ef3)
![Screenshot 2025-03-27 233555](https://github.com/user-attachments/assets/800c2ce9-a387-41be-ae5d-1c130d96e880)
