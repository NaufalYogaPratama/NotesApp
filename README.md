Notes App Back-End
Notes App Back-End adalah proyek backend yang dibangun menggunakan Node.js dan beberapa library serta framework untuk mendukung pengembangan aplikasi RESTful API. Aplikasi ini menyediakan API untuk pengelolaan catatan (notes) yang dapat diakses oleh klien.

Fitur
Membuat, membaca, mengubah, dan menghapus catatan (CRUD) melalui RESTful API.
Menggunakan UUID untuk mengidentifikasi catatan secara unik.
Pengembangan dan monitoring lebih mudah dengan hot reloading.
Tools, Libraries, dan Frameworks yang Digunakan
Tools
Nodemon: Digunakan untuk memonitor perubahan pada file dan melakukan restart server otomatis saat ada perubahan, memudahkan pengembangan.
Libraries
nodeid: Digunakan untuk menghasilkan UUID yang unik bagi setiap catatan yang dibuat.
Frameworks
Node.js: Runtime JavaScript yang memungkinkan penulisan kode backend menggunakan JavaScript.
Hapi: Framework untuk membangun server dan menangani routing, sangat mendukung pembuatan RESTful API di Node.js.
Instalasi
Clone repositori ini ke komputer Anda:

bash
Salin kode
git clone https://github.com/username/notes-app-back-end.git
cd notes-app-back-end
Install semua dependencies yang dibutuhkan:

bash
Salin kode
npm install
Menjalankan Server dalam Mode Development
Jalankan perintah berikut untuk memulai server dengan hot reloading (dengan bantuan nodemon):

bash
Salin kode
npm run dev
Jika Anda ingin menjalankan server tanpa hot reloading, gunakan perintah berikut:

bash
Salin kode
npm start
RESTful API Endpoints
HTTP Method	Endpoint	Deskripsi
GET	/notes	Mendapatkan semua catatan
GET	/notes/{id}	Mendapatkan catatan tertentu
POST	/notes	Menambahkan catatan baru
PUT	/notes/{id}	Memperbarui catatan tertentu
DELETE	/notes/{id}	Menghapus catatan tertentu
Struktur Proyek
plaintext
Salin kode
notes-app-back-end/
├── node_modules/
├── src/
│   ├── handlers/         # Handler untuk setiap route
│   ├── routes/           # Definisi route RESTful API
│   ├── models/           # Model untuk mengelola data
│   └── server.js         # File utama untuk menjalankan server
├── .gitignore
├── package.json
└── README.md
Dependencies
Node.js - Download Node.js
Hapi - Framework server untuk membangun RESTful API.
Nodemon - Tool pengembangan untuk hot reloading.
nodeid - Library untuk membuat UUID.
Lisensi
Proyek ini dilisensikan di bawah MIT License.
