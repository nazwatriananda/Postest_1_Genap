print("Login Sederhana")

#memasukkan data berupa Nama, NIM, dan Kelas
Nama = input('Nama Mahasiswa : ') #Memasukkan Nama Mahasiswa, setelah dienter sistem akan melanjutkan pada tahap selanjutnya
NIM = input('NIM Mahasiswa : ') #Memasukkan NIM Mahasiswa, kemudian sistem akan melanjutkan pada tahap selanjutnya
Kelas = input('Kelas Mahasiswa : ') #Memasukkan Kelas disertai keterangan prodi, contohnya: "Sistem Informasi (Kelas)"

print('===================================')
if Nama and NIM and Kelas:
    print("Data Yang Anda Masukkan Valid, Login Anda Berhasil!!") #Jika data yang di inputkan benar atau valid, maka login yang dilakukan berhasil
else :
    print("Data Yang Anda Masukkan Tidak Valid, Silahkan Login Kembali") #Jika data yang diinputkan salah atau tidak Valid,
print('===================================')                             #sistem bisa di reset ulang dan mengulang kembali untuk mengisi data


#Penugasan membuat sebuah percabangan untuk memilih dan menghitung Bangun Ruang(Bola, Tabung, Limas Segitiga)
print("Membuat Sebuah Program Cara Menghitung Volume Bangun Ruang")
print('===================================')

#Memberikan keterangan Pilihan untuk ditampilkan pada output
print("Bangun Ruang")
print("1. Bangun Ruang Bola")
print("2. Bangun Ruang Tabung")
print("3. Bangun Ruang Limas Segitiga")

#Memberikan Pilihan Untuk memilih Bangun ruang yang tersedia pada bagian output diatas
Volume = input("Memilih Bangun Ruang (1/2/3): ")
print('=====================')

if Volume == '1' :                                    #Jika memilih '1' maka sistem akan otomatis mengarahkan pada Pilihan Bangun Ruang Bola
    print("Memilih Bangun Ruang Bola")                
elif Volume == '2' :
    print("Memilih Bangun Ruang Tabung")              #Jika memilih '2' maka sistem akan otomatis mengarahkan pada Pilihan Bangun Ruang Tabung
elif Volume == '3' :
    print("Memilih Bangun Ruang Limas Segitiga")      #Jika memilih '3' maka sistem akan otomatis mengarahkan pada Pilihan Bangun Ruang limas Segitiga
else:
    print("Tidak Memilih Bangun Ruang")

#Membuat input untuk memasukkan rumus yang diminta sebuah Bangun Ruang
if Volume == '1':
    Jari_Jari = float(input("Masukkan Jari-Jari Bola: "))                        #Pada Bangun ruang Bola, hanya perlu diinputkan sebuah nilai
    Phi = float(input("Masukkan Phi: "))                                         #Untuk mengisi Jari-Jari dan Phi
elif Volume == '2' :
    Phi = float(input("Masukkan Phi Pada Bangun Ruang: "))                       #Pada Bangun ruang Tabung, hanya perlu diinputkan sebuah nilai
    Jari_Jari = float(input("Masukkan Jari-Jari Pada Bangun Ruang : "))          #Untuk mengisi Phi, Jari-Jari, Tinggi
    Tinggi = float(input("Masukkan Tinggi Pada Bangun Ruang : "))                
elif Volume == '3' :
    Luas_Alas = eval(input("Luas Alas Pada Bangun Ruang :"))                     #Pada Bangun ruang Limas Segitiga, hanya perlu diinputkan sebuah nilai
    Tinggi_Segitiga = eval(input("Tinggi Segitiga pada Bangun Ruang :"))         #Untuk mengisi Luas Alas, Tinggi Segitiga
    
#memasukkan rumus pada sistem untuk memproses perhitungan matematika dan menjalankan proses perhitungan untuk mengeluarkan hasil output Hasil
if Volume == '1' :
    Hasil = Volume = (4/3) * Phi * (Jari_Jari ** 3)                 #Menambahkan keterangan Hasil pada baris program
    print(f"Volume Bangun Ruang Bola = {Hasil}  ")                  #Untuk mengeluarkan Hasil output dari Rumus
elif Volume == '2' :
    Hasil = Volume = Phi * (Jari_Jari ** 2) * Tinggi                 #Menambahkan keterangan Hasil pada baris program
    print(f"Volume Bangun Ruang Tabung = {Hasil}")                   #Untuk mengeluarkan Hasil output dari Rumus
elif Volume == '3' :
    Hasil = Volume = (1/3) * Luas_Alas * Tinggi_Segitiga             #Menambahkan keterangan Hasil pada baris program
    print(f"Volume Bangun Ruang Limas Segitiga = {Hasil} ")          #Untuk mengeluarkan Hasil output dari Rumus
else:
    print("Tidak Memilih Bangun Ruang")
