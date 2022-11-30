# Praktikum5
Nama : Muhamad David Ali

NIM : 312210291

Kelas : TI 22 A1

## DAFTAR ISI <br>
| No | Description | Link |
|-----|------|-----|
|1|Latihan5|[Click Here](#latihan)|
|2|Praktikum5 |[Click Here](#praktikum-6)|
|3|Flowchart|

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

### Flowchart Praktikum-6

![Flowchart ]
