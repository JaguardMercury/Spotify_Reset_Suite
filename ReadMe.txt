1.,PERSIAPAN AKUN DEVELOPER SPOTIFY
________________________________________
Sebelum menjalankan aplikasi, kamu perlu membuat Spotify Developer App untuk mendapatkan izin akses.
Langkah-langkah:
1.Buka situs: https://developer.spotify.com/dashboard/
2.Login menggunakan akun Spotify kamu.
3.Klik tombol "Create an App".
4.Isi nama aplikasi, misalnya: Spotify Purifier Tool.
5.Di bagian Redirect URI, tambahkan alamat berikut:
http://127.0.0.1:8888/callback
6.Klik Save.
7.Catat Client ID dan Client Secret karena akan digunakan nanti di aplikasi.
________________________________________
2.,MENJALANKAN APLIKASI
________________________________________
1.Pastikan library spotipy sudah terpasang: pip install spotipy
2.Jalankan program utama:
python main.py
3.Masukkan data berikut sesuai aplikasi developer kamu:
	Client ID
	Client Secret
	Redirect URI (gunakan: http://127.0.0.1:8888/callback)
________________________________________
3.AUTENTIKASI SPOTIFY
________________________________________
Setelah klik "Connect", browser akan terbuka menuju halaman login Spotify.
Masuk dengan akun kamu, lalu tekan tombol "Agree" untuk memberikan izin akses.
Jika berhasil, kamu akan diarahkan kembali ke aplikasi.
________________________________________
4.MEMILIH AKSI YANG INGIN DIJALANKAN
________________________________________
Setelah berhasil login, aplikasi akan menampilkan empat pilihan utama:
1.Delete All Liked Songs
Menghapus seluruh lagu yang pernah disukai.
2.Delete All Playlists
Menghapus semua playlist yang kamu buat atau ikuti.
3.Unfollow All Artists
Berhenti mengikuti seluruh artis yang kamu follow.
4.Remove All Albums, EPs & Singles
Menghapus semua rilisan yang tersimpan di perpustakaanmu.
Kamu bisa memilih salah satu sesuai kebutuhan.
________________________________________
5.PROSES PENGHAPUSAN
________________________________________
Setelah memilih aksi, program akan mulai bekerja.
Proses dilakukan bertahap (maksimal 50 item per batch) sesuai batas API Spotify.
Waktu yang dibutuhkan tergantung jumlah data di akunmu.
Ketika selesai, akan muncul pesan:
"Done. Your Spotify library has been cleaned."
________________________________________
6.SELESAI
________________________________________
Sekarang akun Spotify kamu sudah bersih dari data yang dipilih.
Tidak ada data pribadi yang disimpan secara lokal oleh aplikasi.
Kamu dapat menutup program dengan aman.
________________________________________
CATATAN PENTING
•Aplikasi hanya berfungsi pada akun yang sedang login.
•Pastikan kamu benar-benar ingin menghapus data sebelum menekan tombol konfirmasi.
•Semua perubahan bersifat permanen dan tidak dapat dikembalikan.
•Gunakan koneksi internet yang stabil untuk menghindari error API.
•Gunakan secara bertanggung jawab untuk akun milik sendiri.

