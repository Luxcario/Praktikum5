# Praktikum5
Nama : Muhamad David Ali

NIM : 312210291

Kelas : TI 22 A1

## DAFTAR ISI <br>
| No | Description | Link |
|-----|------|-----|
|1|Latihan5|[Click Here](https://github.com/Luxcario/Praktikum5#latihan)|
|2|Praktikum5 |[Click Here](https://github.com/Luxcario/Praktikum5#langkah-langkah-)|
|3|Flowchart| [Click Here](https://github.com/Luxcario/Praktikum5/blob/main/README.md#flowchart)|

## Latihan
Buat Dictionary daftar kontak
- Nama sebagai key, dan nomor sebagai value
- Tampilkan kontaknya Ari
- Tambah kontak baru dengan nama Riko, nomor 087654544
- Ubah kontak Dina dengan nomor baru 088999776
- Tampilkan semua Nama
- Tampilkan semua Nomor
- Tampilkan daftar Nama dan nomornya
- Hapus kontak Dina

### Langkah-langkah :
1. Buat program terlebih dahulu seperti gambar di bawah ini

daftarKontak = {"nama" : "nomor Telepon"}
kontak = {'Ari': '081267888', 'Dina' :'087677776'}


#print
print(30*"=")
print("   nama   |  Nomor Telepon  |")
print(30 *"-")
print("   # Ari  | ",kontak['Ari'])
print("   # Dina | ",kontak['Dina'])
print(30 * "=")


#Tampilkan kontak Ari
print("Tampilkan kontaknya Ari")
print("    Ari  | ", kontak['Ari'])
print(30 * "=")


#Tambah kontak baru dengan nama Riko, nomor 087654544
print("Tambah kontak baru dengan nama Riko, nomor 087654544")
kontak['Riko'] = '087654544'
print("    Riko    | ", kontak['Riko'])
print(30*"═")


#Ubah kontak Dina dengan nomor baru 088999776
print("Ubah kontak Dina dengan nomor baru 088999776")
kontak['Dina'] = '088999776'
print("    Dina    | ", kontak['Dina'])
print(30*"═")


#Tampilkan semua Nama
print("Tampilkan semua nama")
print(kontak.keys())
print(30*"═")


#Tampilkan semua nomor
print("Tampilkan semua nomor")
print(kontak.values())
print(30*"═")


#Tampilkan semua Nama dan Nomornya
print("Tampilkan semua nama dan nomornya")
print(kontak.items())
print(30*"═")

#Hapus kontak Dina
print("Hapus kontak Dina")
kontak.pop('Dina')
print(kontak.items())
print(30*"═")                    






### Penjelasan Program :
1. Buatlah Dictionary berupa Nama, NIM, Nilai Tugas, Nilai UTS, Nilai UAS
2. Lalu inputlah menu pilihan berupa Lihat, Tambah, Ubah, Hapus, Cari, Keluar
3. Gunakanlah perulangan for, dengan perintah for i in range(len(Nama)):. Fungsi "len" ialah untuk mengembalikan panjang (jumlah anggota) dari suatu objek.
4. Lalu inputlah Nama, NIM, Nilai Tugas, Nilai UTS, Nilai UAS
5. Lalu mencari nilai akhir dengan perhitungan nilai tugas 30%, nilai uts 35% dan uas 35% , dengan perintah float
6. Jika ingin melihat dictionary data ketik "L", jika ingin menambah data ketik "T", jika ingin mengubah data ketik "U", jika ingin menghapus ketik "H", jika ingin mencari data ketik "C" dan jika ingin keluar dari data ketik "K"
7. Lalu cetak dengan perintah print ("Pilih menu yang tersedia")
8. Selesai


print("====================================")
print("======>  Program Input Nilai  <======")
print("====================================")
data = {}
while True:
    print("")
    m = input("===>> (L)ihat, (T)ambah, (U)bah, (H)apus, (C)ari, (K)eluar : <=== ")
    print("================================================================")
    print("| NO |  Nama     |   Nim    |  Tugas  |  UTS  |  UAS  |   Akir |")
    print("================================================================")
    print(">>>>>>>>>>>>>>>>>>>>>>>> TIDAK ADA DATA <<<<<<<<<<<<<<<<<<<<<<<<")
    if m.lower() == 'k':
        break

    elif m.lower() == 'l':
        print("----- DAFTAR NILAI -----")
        print("==================================================================================")
        print("| NO |   NAMA     |   NIM        |  TUGAS   |   UTS     |   UAS      |  AKHIR    |")
        print("==================================================================================")
        i = 0
        for x in data.items():
            i += 1
            print("|  1 |{0:9}   |{1:9}     |{2:9} |{3:9}  |{4:9}   |{5:9}  |" .format(x[0], x[1][0],
                                                                                       x[1][1], x[1][2], x[1][3],
                                                                                       x[1][4], i))

        else:
            print("====================>>>>>>>>>>>>> Tidak Ada Data <<<<<<<<<<<<<====================")

    elif m.lower() == 't':
        print("--------------- Tambah Data ---------------")
        nama = input("Nama                  : ")
        nim = input("Nim                   : ")
        tugas = float(input("Masukan Nilai Tugas   : "))
        uts = float(input("Masukan Nilai UTS     : "))
        uas = float(input("Masukan Nilai UAS     : "))
        akhir = (int(tugas) * .30) + (int(uts) * .35) + (int(uas) * .35)
        data[nama] = nim, tugas, uts, uas, akhir

    elif m.lower() == 'u':
        print("----- Ubah Data Mahasiswa -----")
        nama = input("Nama  : ")
        if nama in data.keys():
            nim = input("Nim : ")
            tugas = float(input("masukan nilai tugas : "))
            uts = float(input("masukan nilai Uts : "))
            uas = float(input("masukan nilai uas : "))
            akhir = (int(tugas) * .30) + (int(uts) * .35) + (int(uas) * .35)
            data[nama] = nim, tugas, uts, uas, akhir

        else:
            print("Tidak Ada data")

    elif m.lower() == 'h':
        print("Hapus Data Mahasiswa")
        nama = input("nama : ")
        if nama in data.keys():
            print("Datanya", nama, "adalah {0}".format(data[nama]))
        else:
            print("Tidaak Ada Data")

    else:
        print("Pilih menu yang tersedia")

### Flowchart 

![Flowchart ] 
![image](https://user-images.githubusercontent.com/116184002/204699668-3ba3c465-d41b-4190-8b43-926d4ceb28d7.png)

