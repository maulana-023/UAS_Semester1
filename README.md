Repository ini dibuat untuk memenuhi Nilai UAS - Bahasa Pemrograman.
<hr>
Nama    : Maulana Muhamad <br>

NIM     : 312010188 <br>

Kelas   : TI.20. A.1 <br>
<hr>

## UAS
   ![Picture - New](pict/soal.png)

   <hr>

## SOAL 1
 Pada soal pertama diminta untuk membuat modul yang diantaranya adalah Tambah Data, Ubah Data, Dan Cari Data. 

 ### syntax dibawah berfungsi untuk menambahkan data :

```python
       if c.lower() == 't':
        print("=======Tambah Data=======")
        nama = input("Nama                :  ")
        nim = input("Nim                 :  ")
        tugas = int(input("Masukan Nilai Tugas :  "))
        uts = int(input("Masukan Nilai UTS   :  "))
        uas = int(input("Masukan Nilai UAS   :  "))
        akhir = (0.30 * tugas) + (0.35 * uts) + (0.35 * uas)
        data[nama] = nim, tugas, uts, uas, akhir
```

> jika syntax diatas dirun yang nantinya berfungsi sepeti dibawah ini, masukan 
"T" untuk Menambah Data.
![Picture - New](pict/T.png)

### syntax dibawah berfungsi untuk mengubah data :

```python
        elif c.lower() == 'u':
        print('=======Ubah Data Mahasiswa=======')
        nama = input('Nama                :  ')
        if nama in data.keys():
            nim = input('Nim                 :  ')
            tugas = int(input("Masukan Nilai Tugas :  "))
            uts = int(input("Masukan Nilai UTS   :  "))
            uas = int(input("Masukan Nilai UAS   :  "))
            akhir = (0.30 * tugas) + (0.35 * uts) + (0.35 * uas)
            data[nama] = nim, tugas, uts, uas, akhir
        else:
            print("Data Nilai Tidak Ada".format(nama))
```

> jika syntax diatas dirun yang nantinya berfungsi sepeti dibawah ini, masukan 
"U" untuk Mengubah Data.
![Picture - New](pict/U.png)

### syntax dibawah berfungsi untuk menghapus data :


```python
            elif c.lower() == 'h':
        print("=======Hapus Data Mahasiswa=======")
        nama = input("Nama :  ")
        if nama in data.keys():
            del data[nama]
        else:
            print("Data Nilai Tidak Ada".format(nama))
```

> jika syntax diatas dirun yang nantinya berfungsi sepeti dibawah ini, masukan 
"H" untuk Menghapus Data.
![Picture - New](pict/H.png)


<hr>

## SOAL 2
 Syntax dibahah ini untuk melihat hasil pencarian atau daftar nilai.

 ```python
        elif c.lower() == 'l':
        print("=======Daftar Nilai Mahasiswa=======")
        print("================================================================================================")
        print(" |NO   |     NAMA      |    NIM    |     TUGAS    |     UTS     |       UAS    |    AKHIR     | ")
        print("================================================================================================")
        i = 0
        for x in data.items():
            i += 1
            print(
                " | {6:2}  |  {0:12s} | {1:9s} | {2:11}  | {3:11} | {4:11}  |  {5:11} |".format(x[0], x[1][0], x[1][1],
                                                                                                x[1][2], x[1][3],
                                                                                                x[1][4], i))
            print("================================================================================================")
```

> jika syntax diatas dirun yang nantinya berfungsi sepeti dibawah ini, masukan 
"L" untuk Melihat hasil pencarian atau daftar nilai.
![Picture - New](pict/L.png)

<hr>

## SOAL 3
 pada soal nomer 3,Jika ingin menginput data kalian bisa memasukan hufuf "T". Gambar dibawah adalah hasil outputnya.
 ![Picture - New](pict/T.png)
 s