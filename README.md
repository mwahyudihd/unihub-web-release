# UniHub Web (Frontend)

**UniHub** adalah aplikasi manajemen Unit Kegiatan Mahasiswa (UKM) berbasis web.  
Repositori ini berisi **frontend web** yang dibangun menggunakan **Flutter Web** dan sudah di-*build* untuk siap dipublikasikan.  

Untuk layanan backend yang berjalan dengan **Fastify**, silakan kunjungi:  
👉 [UniHub Backend Repository](https://github.com/mwahyudihd/unihub-api)

---

## 🌐 Demo (#demo)
Kunjungi aplikasi UniHub versi web di sini:  
[**Demo UniHub Web**](https://unihub-web-two.vercel.app/)

---

## 📚 Daftar Isi
- [Pendahuluan](#pendahuluan)
- [Fitur](#fitur)
- [Demo](#demo)
- [Struktur Proyek](#struktur-proyek)
- [Instalasi & Deploy](#instalasi--deploy)
- [Integrasi Backend](#integrasi-backend)
- [Kontributor](#kontributor)
- [Lisensi](#lisensi)

---

## 📖 Pendahuluan
Frontend UniHub dibangun dengan **Flutter Web** untuk memberikan antarmuka yang modern, cepat, dan responsif.  
Frontend ini mengonsumsi API dari backend (Fastify) untuk menjalankan fitur manajemen UKM.

---

## ✨ Fitur
1. **Dashboard Pengumuman UKM**  
   Menampilkan dan mengelola informasi pengumuman.
2. **Keanggotaan**  
   Menyediakan UI untuk registrasi dan daftar anggota.
3. **Keuangan**  
   Menampilkan laporan pemasukan dan pengeluaran.
4. **Manajemen Dokumen (Link)**  
   Menampilkan koleksi dokumen berbasis link.
5. **Integrasi AI (via GEMINI)**  
   - Generator pengumuman otomatis.  
   - Deskripsi UKM.  
   - Bio pengguna.  
   - Ringkasan teks.  

---

## 📂 Struktur Proyek
```

unihub-web/
│
├── build/          # File hasil build Flutter Web (siap deploy)
├── index.html
├── favicon.png
├── manifest.json
└── README.md

````

---

## ⚙️ Instalasi & Deploy

### 1. Jalankan secara lokal
Karena repo ini hanya berisi hasil build Flutter Web, cukup gunakan server statis:

```bash
# Contoh dengan Python
python3 -m http.server 8080

# atau dengan Node.js
npx serve build/web
````

Lalu buka [http://localhost:8080](http://localhost:8080).

### 2. Deploy ke Hosting

Anda bisa mengunggah isi folder `build/web` ke berbagai layanan hosting, misalnya:

* **Vercel**
* **Netlify**
* **Firebase Hosting**
* **Nginx/Apache server**

---

## 🔗 Integrasi Backend

Frontend ini terhubung ke backend UniHub (Fastify) melalui **REST API**.
Pastikan backend sudah berjalan, lalu atur base URL API di konfigurasi (misalnya file `env.js` atau konfigurasi runtime hosting).

👉 [Repo UniHub Backend](https://github.com/mwahyudihd/unihub-api)

---

## 👥 Kontributor

* **Nama Anda** – Frontend Developer

---

## 📜 Lisensi

Proyek ini dilisensikan di bawah [MIT License](LICENSE).