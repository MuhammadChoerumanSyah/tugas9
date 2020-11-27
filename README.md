# lab-5
# latihan 1

<img src="D:\tugasheru9\tugas9\foto\latihan1.png">
code :
<img src="D:\tugasheru9\tugas9\foto\latihan2.png">
 Penjelasan :
•	a = [1, 3, 5, 7, 9] list A dengan 5 elemen
 Akses list
•	print(a[2]) menampilkan elemen ke -3
•	print(a[1:3) mengambil elemen ke 2 sampai elemen ke 4
•	print(a[4) mengambil elemen terakhir
 Ubah elemen list
•	a[3] =4 mengubah elemen ke 4 dengan nilai lainnya
•	a[3:5] =8, 10 mengubah elemen ke 4 sampai dengan terakhir
 Tambah elemen list
•	b = a [0:2] mengambil 2 bagian dari list pertama (A) dan jadikan list kedua (B)
•	b.append(‘halo) menambah list dengan nilai string
•	b.extend([10, 20, 30]) menambah list B dengan 3 nilai
•	x = a + b menggabungkan list B dengan list A
 Output :
[output](Output1)

# Tugas praktikum
<img src="D:\tugasheru9\tugas9\foto\tugaspraktikum4.png">
Code :
<img src="D:\tugasheru9\tugas9\foto\code.png">
<img src="D:\tugasheru9\tugas9\foto\code1.png">

 Penjelasan :
•	data = [] ,membuat list kosong yang nanti akan di isi
•	while ulangi data = [] Membuat list kosong yang nanti akan di isi
•	while ulangi =='y': Membuat perulangan dengan variabel ulangi, dimana ketika memilih 'y' maka akan otomatis mengulang pengisian data
•	nilai_akhir = (nilai_tugas)*30/100 + (nilai_uts)*35/100 + (nilai_uas)*35/100 Nilai Akhir diambil dari perhitungan 3 komponen nilai (tugas: 30%, uts: 35%, uas: 35%)
•	data.append ([nama, nim, nilai_tugas, nilai_uts, nilai_uas, int(nilai_akhir)]) Memasukkan variable input kedalam list data 
•	ulangi = (input(‘tambah data(y/t?)’)) ketika memilih ‘t’ if ulangi ==’t’: maka mencetak hasil.
 


 Flowchart:
[flowchart](flowchart1)

# Lab 5
# Tugas Praktikum 5
<img src="D:\tugasheru9\tugas9\foto\tugaspraktikum5.png">

Penjelasan:
• data={} untuk menampung list dengan format dictionary
• Gunakanlah perulangan while untuk menampilkan data sebanyak-banyaknya
• menu = input("(T)ambah), (U)bah, (H)apus, L(ihat), (C)ari, (K)eluar: ") kita tambahkan input tambah, ubah, hapus, lihat, cari, keluar dalam variabel menu
• else: print("oh tidak, ada yang salah, silahkan cek kembali.") jika ada kesalahan dalam input maka akan tercetak oh tidak, ada yang salah, silahkan cek kembali.'
• masukkan nama, nim, nilai_tugas, nilai_uts, nilai_uas, dan nilai_akhir yang nanti akan dimasukkan kedalam data={}
• Nilai akhir didapat dari = (nilai_tugas)*30/100 + (nilai_uts)*35/100 + (nilai_uas)*35/100

Keluar
• if menu.lower() == 'k': ambil data 'K' dari menu
• lalu break untuk menghentikan seluruh proses

Lihat data
• elif menu.lower() == 'l': Kita menggunakan kondisi percabangan if, ambil data dari menu lalu kita akan mengubah perintah 'l' yang kita input menjadi huruf kecil dengan fungsi lower()
• lalu cetak print()

Tambah data
• elif menu.lower() == 't': Ambil data 't' dari menu
• nama = input("Masukkan nama: ") lalu tambahkan input nama, nim, nilai tugas, nilai uts, nilai uas
• nilai_akhir = (nilai_tugas)*30/100 + (nilai_uts)*35/100 + (nilai_uas)*35/100 untuk nilai akhir diambil dari perhitungan 3 komponen nilai(nilai_tugas:30%, nilai_uts:35%, nilai_uas:35%)
• data[nama] = [nama, nim, nilai_tugas, nilai_uts, nilai_uas, nilai_akhir] kita akan masukkan data yang tadi kita input ke dalam 'data[nama]'
• lalu cetak print()

Ubah data
• elif menu.lower() == 'u': Ambil data 'u' dari menu
• nama = input("Masukkan nama untuk mengubah data: ") kita akan menginput data yang nanti akan diubah
• if nama in data.keys(): print("Mau mengubah apa?") jika 'nama' dari didalam 'data' maka akan mengembalikan daftar menggunakan daftar menggunakan fungsi 'keys()'
• sub_data = input("(semua), (Nama), (NIM),(Tugas), (UTS), (UAS) : ") membuat menu diubah didalam sub_data
• if sub_data.lower() =="semua": ambil kata kunci 'semua di dalam sub_data jika 'semua' maka input data[nama][1] = input("Ubah NIM: ")data[nama][2] = int(input("Ubah Nilai Tugas: ")) data[nama][3] = int(input("Ubah Nilai UTS: ")) data[nama][4] = int(input("Ubah Nilai UAS: ")) data[nama][5] = data[nama][2] *30/100 + data[nama][3] + data[nama][4] = int (input("ubah Nilai UAS:"))
• data[nama][5] = data[nama][2] *30/100 + data[nama][3]*35/100 + data[nama][4]*35/100 kita dapatkan nilai akhir dengan diambil dari perhitungan 3 komponen nilai(tugas: 30%, uts: 35%, uas: 35%),
ket: [5] = nilai_akhir, dimana[0] = nama
• lalu cetak print("\Berhasil ubah data!")
• Jika kita ingin mengubah data tertentu maka elif sub_data.lower() == "nim":data[nama][1] = input("NIM:") dan berlaku juga untuk nilai tugas, UTS, dan UAS
• lalu cetak print("\Berhasil ubah data!")
• else:print("'{}' tidak ditemukan.".format(nama)) jika kita salah dalam memasukkan nama untuk mengubah data maka akan muncul 'nama tidak ditemukan'

Cari data
• elif menu.lower() == 'c': Ambil data 'c' dari menu
• nama = input("Masukkan nama untuk mencari data:") kita akan menginput data yang nanti akan dicari
• if nama in data.keys(): kita mengambil list 'nama' didalam 'data' menggunakan pengkondisian
• maka cetak print("Nama: {0}\nNIM : {1}\nNilai Tugas: {2}\nUTS: {3}\nUAS: {4}\nNilai akhir: {5}" untuk menampilkan data yang tersedia
• else:print("'{} tidak ditemukan.".format(nama)) jika data yang kita akan input salah/tidak ditemukan maka akan tercetak 'nama tidak ditemukan'

Hapus data
• elif menu.lower() 'h': Ambil data 'c' dari menu
• nama = input("Masukkan nama untuk menghapus sub_data : ") kita akan menginput data yang nanti akan dihapus
• if nama in data.keys(): kita mengambil list 'nama' didalam 'data' menggunakan pengkondisian
• del data[nama] hapus semua nam yang ada didalam 'data'
• jika sudah maka cetak print("sub_data '{}' berhasil dihapus.".format(nama))
• else:print("'{} tidak ditemukan.".format(nama)) jika data yang kita akan input salah/tidak ditemukan maka akan tercetak 'nama tidak ditemukan'

Output:
Tambah data
<img src="D:\tugasheru9\tugas9\foto\output2.png">
Ubah data
<img src="D:\tugasheru9\tugas9\foto\output3.png">
Lihat data
<img src="D:\tugasheru9\tugas9\foto\output4.png">
Mencari data
<img src="D:\tugasheru9\tugas9\foto\output5.png">
Hapus data
<img src="D:\tugasheru9\tugas9\foto\output6.png">

Flowchart:
[flowchart](flowchart2)













