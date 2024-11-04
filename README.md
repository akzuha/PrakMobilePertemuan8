**Cara Kerja Login**
1. API
   - Membuat Database yang berisi tabel user
   - Membuat koneksi.php untuk menyambungkan ke database
   - Membuat login.php untuk memberikan token ketika data login valid
2. Ionic
   - Mendeklarasi ProvideHttpClient agar bisa tersambung ke API
   - Pada services/authentication.service.ts berfungsi sebagai pengecekan autentikasi pengguna yang login
   - Pada guards/auth.guard.ts berfungsi untuk menjaga halaman yang hanya bisa diakses ketika pengguna sudah login
   - app/login/login.page.html untuk mengelola tampilan login
   - app/login/login.page.ts untuk mengelola pengolahan proses login
3. Alur login
   - User input
   - Dilakukan Validasi data dengan mengirim ke API
   - Menghasilkan token ketika valid
   - Token dan data user disimpan
   - Merubah status autentikasi
   - Mengarahkan ke halaman Home Page
   - Token akan dihapus ketika pengguna melakukan Logout


**Screen Record**

https://github.com/user-attachments/assets/8dc9ecfe-5412-49bb-a21d-1c47559577de

