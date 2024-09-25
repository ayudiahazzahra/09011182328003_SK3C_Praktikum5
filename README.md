# 1. Eksekusi seluruh profile yang ada : 
## a. Edit file profile /etc/profile dan tampilkan pesan sebagai berikut :

![5 1](https://github.com/user-attachments/assets/2cfb939a-dd06-4347-b179-157356d1e8bc)

### Perintah sudo nano /home/ayudiah/.bash_profile digunakan untuk membuka file .bash_profile milik pengguna ayudiah dengan editor teks nano, sambil menggunakan sudo untuk mendapatkan hak akses superuser (administrator).

# b. Asumsi nama anda stD02001, maka edit semua profile yang ada yaitu : 
## /home/stD02001/.bash_profile 
## /home/. stD02001/.bash_login 
## /home/mahasiswa/.profile 
## /home/mahasiswa/.bashrc

## Ganti nama /home/mahasiswa dengan nama anda sendiri. Pada setiap file tersebut, cantumkan instruksi echo, misalnya pada /home/ mahasiswa/.bash_profile : echo “Profile dari .bash_profile” Lakukan hal yang sama untuk file lainnya, sesuaikan tampilan dengan nama file yang bersangkutan.



![5 2](https://github.com/user-attachments/assets/62ac02bf-8dd2-4d6c-b941-c6b712305a1a)

![5 3](https://github.com/user-attachments/assets/ba99107d-4227-478d-bb44-0d760f7ad1b4)

![5 4](https://github.com/user-attachments/assets/5925735d-0241-4855-a947-455a4d170883)

![5 5](https://github.com/user-attachments/assets/de1b9d9d-ff1d-417a-b5ee-9b8615634297)

![5 6](https://github.com/user-attachments/assets/69e61fb7-3a2a-42fd-b137-d12ccc686e17)

![5 7](https://github.com/user-attachments/assets/0800f0e4-8cba-4a76-88ce-8bef1a36ac5e)

![5 8](https://github.com/user-attachments/assets/d6942e51-843d-4d81-b663-0046ae8aac9a)

### bash_profile: Dijalankan saat login ke login shell. Tempat yang baik untuk mengatur variabel lingkungan yang harus diinisialisasi sekali per login.
### bash_login: Dijalankan jika .bash_profile tidak ada. Memiliki fungsi serupa dengan .bash_profile.
### profile: File umum yang digunakan oleh beberapa shell, digunakan untuk inisialisasi lingkungan di berbagai shell.
### bashrc: Dijalankan pada setiap instansi non-login shell. Umumnya digunakan untuk mengatur alias dan fungsi.

# c. Jalankan instruksi subtitute user, kemudian keluar dengan perintah exit sebagai berikut: 
## $ su mahasiswa 
## $ exit 
## kemudian gunakan opsi – sebagai berikut : 
## $su – mahasiswa 
## Jelaskan perbedaan kedua utilitas tersebut.

![5 9](https://github.com/user-attachments/assets/369536b8-f70a-4e6f-ba03-5928adbef339)
![5 10](https://github.com/user-attachments/assets/cc10b623-f7cf-44f0-8de3-d5141c9e4edd)
![5 11](https://github.com/user-attachments/assets/565c297d-68c7-40f1-9f89-6ae72c33796b)
![5 12](https://github.com/user-attachments/assets/d7dc3bda-a85f-44c6-a61c-c2520afb2676)

### su mahasiswa digunakan saat kamu hanya perlu berganti otorisasi ke pengguna lain tanpa mengubah lingkungan shell.
### su – mahasiswa digunakan saat kamu ingin sepenuhnya berpindah ke pengguna lain dan memuat seluruh konfigurasi lingkungan shell mereka, seperti variabel PATH, alias, dan pengaturan lainnya.

# 2. Prompt String (PS) 
## a. Edit file .bash_profile, ganti prompt PS1 dengan ‘>’. Instruksi export diperlukan dengan parameter nama variable tersebut, agar perubahan variable PS1 dikenal oleh semua shell 
## PS1=‟>
## export PS1

![5 13](https://github.com/user-attachments/assets/fff41851-ed8f-4348-9917-5609b591e709)

![5 14](https://github.com/user-attachments/assets/b789fc1a-1db1-4f57-a190-e8c4854d2534)

### PS1="> ": Mengubah tampilan prompt menjadi > .
### export PS1: Menyebarkan perubahan variabel PS1 agar dikenal oleh semua shell, termasuk sub-shell.

## b. Eksperimen hasil PS1 :
## $ PS1=“\! > “ 
## 69 > PS1=”\d > “ 
## Mon Sep 23 > PS1=”\t > “ 
## 10:10:20 > PS1=”Saya=\u > “ 
## Saya=mahasiswa > PS1=”\w >” 
## ~ > PS1=\h >”

![5 15](https://github.com/user-attachments/assets/f132dc59-4979-499f-b873-a8043e2588f6)
![5 16](https://github.com/user-attachments/assets/be15dc93-70bd-4a94-a26e-ef8a35c9e829)
![5 17](https://github.com/user-attachments/assets/1998172d-d0de-4e56-915f-0992adf8fb36)
![5 18](https://github.com/user-attachments/assets/567d1f79-30e6-4139-b1a1-7436ba87aab3)
![5 19](https://github.com/user-attachments/assets/ff11ef8b-56c8-4ab9-bbe5-1ac3b4a88191)
![5 20](https://github.com/user-attachments/assets/b6a78583-dc4e-469b-aa62-06c14a3ce7c7)
![5 21](https://github.com/user-attachments/assets/69c7e1a5-cabc-4794-90bf-713665e6350c)

### \! → Menampilkan nomor perintah di history.
### \d → Menampilkan tanggal saat ini.
### \t → Menampilkan waktu saat ini.
### \u → Menampilkan nama pengguna saat ini.
### \w → Menampilkan direktori kerja saat ini.
### \h → Menampilkan hostname (nama mesin).

# 3. Logout 
## Edit file .bash_logout, tampilkan pesan dan tahan selama 5 detik, sebelum eksekusi logout 
## Echo “Terima kasih atas sesi yang diberikan”
## Sleep 5 
## clear

![5 22](https://github.com/user-attachments/assets/aab28581-543d-40bf-b62b-78d886046b81)
![5 23](https://github.com/user-attachments/assets/d4cafedb-015e-4bec-a7e8-3bc347e4af07)
### cho "Terima kasih atas sesi yang diberikan":
### Menampilkan pesan perpisahan saat logout.
### Sleep 5:
### Menunda proses logout selama 5 detik, memberikan waktu untuk melihat pesan yang ditampilkan.
### clear:
### Membersihkan layar terminal setelah pesan dan penundaan selesai, sehingga sesi logout berakhir dengan layar yang bersih.

# 4. Bash script 
#a. Buat 3 buah script p1.sh, p2.sh, p3.sh dengan isi masing-masing : 
## p1.sh 
## #! /bin/bash 
## echo “Program p1” 
## ls –l 
## p2.sh 
## ! /bin/bash 
##  echo “Program p2” 
## who 
## p3.sh 
## #! /bin/bash 
##  echo “Program p3” 
## ps x

![5 24](https://github.com/user-attachments/assets/a33b6dfd-4238-4da2-a23e-bddf3082f924)

![5 25](https://github.com/user-attachments/assets/f155c0db-36a9-4eba-ae65-6ac9ff1d1446)

![5 26](https://github.com/user-attachments/assets/9bd26266-2101-43f5-8542-f69f9e3b4d47)

![5 27](https://github.com/user-attachments/assets/8bb260dc-3045-4cbb-97aa-462828b28e41)

![5 28](https://github.com/user-attachments/assets/35343978-129a-44bf-95b2-46eaf6889ea6)

![5 29](https://github.com/user-attachments/assets/f0996196-2da4-4453-b6bf-0bea840af334)

![5 30](https://github.com/user-attachments/assets/931acf5f-b6cd-431c-a04e-cf71560236d6)

![5 31](https://github.com/user-attachments/assets/0110c66d-2668-4f87-aeb9-6baf03c6cb87)

![5 32](https://github.com/user-attachments/assets/79bbb4e8-8cf4-4349-900f-b1d52c48a0e9)

![5 33](https://github.com/user-attachments/assets/22518f71-75c9-4d1c-9fa2-78460dbcb62a)

![5 34](https://github.com/user-attachments/assets/b3bbaa67-2d4d-4984-ad6e-ca27e62b33b3)

![5 35](https://github.com/user-attachments/assets/93469be8-f386-4177-936d-2d1cf8dde1b2)

![5 36](https://github.com/user-attachments/assets/453aadd8-1303-4fcc-a6e9-43f43446d300)


### p1.sh: Menampilkan daftar file/direktori saat ini secara rinci.
### p2.sh: Menampilkan daftar pengguna yang sedang login ke sistem.
### p3.sh: Menampilkan daftar proses yang sedang berjalan di sistem.

# b. Jalankan sebagai background; kemudian jalankan satu program (utilitas find) di background sebagai berikut : 
## $ jobs 
## $ find / -print > files 2>/dev/null & 
## $ jobs

![5 37](https://github.com/user-attachments/assets/c4ffa0c1-b04d-452e-a109-bf88e6dc9a8c)

![5 38](https://github.com/user-attachments/assets/a91459c3-15fd-4cdd-9c3a-075058feea8b) 


### 1. jobs
### Untuk memantau proses atau skrip yang sedang berjalan di background atau ditangguhkan (suspended).
### 2. find / -print > files 2>/dev/null &
### find / -print: Menjalankan utilitas find untuk mencari dan mencetak daftar semua file dari root (/).
### > files: Mengalihkan output dari perintah find ke dalam file bernama files.
### 2>/dev/null: Mengarahkan pesan error ke /dev/null (membuangnya), agar tidak memenuhi terminal dengan pesan kesalahan, seperti "permission denied".
### &: Menjalankan perintah di background sehingga shell tetap tersedia untuk digunakan sementara perintah tersebut masih berjalan.
### 3. jobs (Setelah find dijalankan di background)
### Fungsi: Menampilkan daftar pekerjaan yang berjalan di background, termasuk find yang baru saja dijalankan. Ini akan menunjukkan status proses, seperti running (sedang berjalan) atau stopped (ditangguhkan).

# c. Jadikan program ke 1 sebagai foreground, tekan ^Z dan kembalikan program tersebut ke background 
## $ fg %1 
## $ bg













