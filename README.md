
### 1. Tampilan Aplikasi
![Image](https://github.com/user-attachments/assets/7adc76e4-998a-405a-b2ab-3167e25e8a37)

**Keterangan: Menampilkan daftar habit (kebiasaan) dengan checkbox dan progress bar. Antarmuka bersih dan fokus pada daftar tugas harian.**  


### 2. Uji Strikethrough
![Image](https://github.com/user-attachments/assets/e2d5adf9-39e7-4828-ab6e-802f7c2d97cb)

**Keterangan: Saat checkbox dicentang, teks habit berubah menjadi coret (strikethrough) — indikasi bahwa habit telah diselesaikan. Ini menandakan penggunaan properti TextDecoration.lineThrough.**  



### 3. Uji Tambah Habit
**Simpan tanpa mengisi nama**
![Image](https://github.com/user-attachments/assets/038e322a-bc1e-4428-8743-cf583b00b0e8)
**Keterangan: Aplikasi memunculkan validasi mencegah penyimpanan habit kosong.**

**Habit Baru setelah isi Form**
![Image](https://github.com/user-attachments/assets/79252fe5-d04e-4799-8865-2d549cc69c44)
**Keterangan:  Habit baru berhasil ditambahkan dan muncul di daftar, artinya fungsi setState() atau pengelola state lain berhasil memicu rebuild.**

### 4. Uji Edit Habit
**Dialog setelah klik Edit**
![Image](https://github.com/user-attachments/assets/fdc7329a-8970-4500-8c2b-faa87c860532)
**Keterangan: Formulir edit muncul sesuai ekspektasi.**

**Setelah Ubah nama dan deskripsi**  
![Image](https://github.com/user-attachments/assets/2d5d39c8-69bb-491b-80a5-d29a5c186506)
**Keterangan: Nama dan deskripsi habit berubah sesuai input — menunjukkan binding data dan update state bekerja dengan baik.**  


### 5. Uji Hapus Habit
**Dialog Konfirmasi untuk menghapus**
![Image](https://github.com/user-attachments/assets/15d26027-19d4-44f5-aa95-3ef1962d47c9)
**Keterangan: Proteksi terhadap penghapusan tidak disengaja.**

**Habit hilang setelah dihapus**
![Image](https://github.com/user-attachments/assets/a6cf8a78-30b0-43f6-badf-c8f4fc9a828f)
**Keterangan: Habit langsung hilang dari daftar — berhasil dihapus dari list/data model.**  


### 6. Uji Progress Bar
![Image](https://github.com/user-attachments/assets/6415e2e1-9604-4a5c-936b-fe4df54e05cb)
**Keterangan: Progress bar berubah sesuai jumlah checkbox yang dicentang.**

![Image](https://github.com/user-attachments/assets/7af8bbef-2598-4a05-a9a6-634ac473613f)
**Keterangan: Ini mencerminkan logika perhitungan proporsi habit yang selesai terhadap total habit.**  


### 7. Uji Reset
![Image](https://github.com/user-attachments/assets/7af8bbef-2598-4a05-a9a6-634ac473613f)
**Keterangan: Setelah menekan tombol Reset, seluruh checkbox ter-uncheck dan progress bar kembali ke 0%.**  


### 8. Uji Ephemeral State
![Image](https://github.com/user-attachments/assets/7af8bbef-2598-4a05-a9a6-634ac473613f)

**Keterangan: Ini menandakan bahwa semua status penyelesaian habit berhasil di-reset dan UI di-rebuild.**  


### 9. Amati Output print
![Image](https://github.com/user-attachments/assets/ce019ff3-bd00-4b7f-94dc-9f3914511deb)
**Keterangan: Pesan build ${habit.name} muncul di konsol setiap kali habit tersebut di-rebuild.
Ini muncul saat melakukan:
-Check/uncheck: karena UI habit mengalami perubahan state.
-Add/edit/delete: karena seluruh daftar habit perlu di-rebuild.
Menandakan bahwa UI menggunakan StatefulWidget atau ListView.builder yang melakukan rebuild lokal saat data berubah.**  
