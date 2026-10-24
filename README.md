# Katalog Game App (Free-To-Play)

## Deskripsi Singkat
Katalog Game App adalah aplikasi mobile berbasis Flutter yang menyajikan informasi daftar game gratis (Free-To-Play). Aplikasi ini dirancang untuk mengambil data dinamis dari REST API secara *real-time* dan menampilkannya dalam antarmuka pengguna (GUI) yang interaktif, bersih, dan mudah digunakan.

## Fitur Utama
*   **Daftar Game (Home Page):** Menampilkan daftar game populer lengkap dengan *thumbnail*, judul, dan genre game.
*   **Detail Game:** Menampilkan informasi mendalam mengenai game yang dipilih, termasuk deskripsi lengkap, *screenshot* antarmuka game, dan spesifikasi sistem minimum (Minimum System Requirements).
*   **Asynchronous State Handling:** Dilengkapi dengan penanganan *state* asinkron menggunakan `FutureBuilder` untuk menampilkan animasi *Loading* saat mengambil data, status *Success* saat data tampil, dan pesan *Error* jika koneksi gagal.
*   **Navigasi Dinamis:** Menerapkan sistem *named routes* untuk perpindahan antarlayar yang mulus.

## Teknologi & Package yang Digunakan
Aplikasi ini dikembangkan menggunakan **Flutter** dan bahasa pemrograman **Dart**. Beberapa *package* tambahan yang digunakan meliputi:
*   `http`: Untuk melakukan pengiriman permintaan jaringan (HTTP request) ke API penyedia data.
*   `json_annotation` & `json_serializable`: Untuk proses konversi data JSON menjadi objek Dart (JSON Serialization) secara otomatis.
*   `build_runner`: Untuk men-*generate* file serialisasi Dart.
*   `readmore`: Untuk membuat fitur ekspansi teks (Read more/Show less) pada deskripsi detail game.

## Langkah Menjalankan Aplikasi
1. Pastikan Anda telah menginstal Flutter SDK dan Dart di perangkat Anda.
2. *Clone* repositori ini ke komputer Anda:
   `git clone https://github.com/Abdulhamiddehana/uts_mobile_game`
3. Masuk ke direktori aplikasi:
   `cd uts_mobile_game`
4. Unduh semua *package* dependensi yang dibutuhkan dengan menjalankan:
   `flutter pub get`
5. (Opsional) Jika file serialisasi belum terbentuk, jalankan perintah:
   `dart run build_runner build`
6. Hubungkan emulator atau *smartphone* Anda (dengan USB Debugging aktif).
7. Jalankan aplikasi menggunakan perintah:
   `flutter run`
