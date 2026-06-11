# 📝 To-Do List App (Provider & FCM)

**Identitas Mahasiswa:**
* **Nama:** Ahmad Titana Nanda Pramuda
* **NIM:** 23111102042
* **Mata Kuliah:** Aplikasi Berbasis Platform (Semester 6)

---

## 📖 Deskripsi Proyek
Aplikasi ini adalah platform manajemen tugas (*To-Do List*) berbasis mobile menggunakan framework **Flutter**. Proyek ini dirancang secara khusus untuk memadukan pengelolaan data lokal yang interaktif dengan sistem notifikasi berbasis *cloud*. 

Dalam pengembangannya, aplikasi ini mendemonstrasikan penggunaan **Provider** sebagai *state management* agar perubahan data lebih efisien dan responsif, serta **Firebase Cloud Messaging (FCM)** untuk menerima *push notification* secara *real-time* langsung dari *backend* Firebase.

## 🚀 Fitur Utama Aplikasi

### 1. Manajemen Tugas Lokal (Provider)
* **Tampil Daftar Tugas:** Menampilkan rincian tugas-tugas yang telah diinput pengguna secara dinamis.
* **Tambah Tugas Baru:** Menyediakan interaksi berupa *pop-up dialog* yang intuitif saat pengguna ingin menambahkan target pekerjaan baru.
* **Hapus Massal (Clear All):** Memiliki tombol praktis untuk menghapus seluruh tugas dari daftar sekaligus hanya dengan satu kali tekan.

### 2. Integrasi Notifikasi *Real-Time* (FCM)
* **Generasi Token Otomatis:** Begitu aplikasi dijalankan, sistem otomatis meregistrasikan perangkat ke server Firebase dan menghasilkan *FCM Registration Token*.
* **Notifikasi Latar Depan (*Foreground Notification*):** Menangkap pesan dari Firebase Console saat aplikasi sedang dibuka dan langsung menampilkannya melalui *SnackBar* berwarna hijau.

## 🛠️ Tech Stack & Dependensi
* **Framework:** Flutter (Dart)
* **State Management:** `provider`
* **Backend Service:** Firebase (Firebase Core & Firebase Messaging)
* **Alat Konfigurasi:** FlutterFire CLI

## 📁 Struktur Direktori Kode (`lib/`)
```text
lib/
 ├── firebase_options.dart   # File konfigurasi Firebase dari FlutterFire CLI.
 ├── main.dart               # Entry point aplikasi & inisialisasi FCM.
 ├── providers/
 │   └── todo_provider.dart  # Logika bisnis dan pengelolaan state To-Do List.
 └── screens/
     └── home_screen.dart    # UI utama daftar tugas dan tombol interaksi.
