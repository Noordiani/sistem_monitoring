

# Sistem Informasi Project Monitoring Sederhana

Repositori ini berisi aplikasi berbasis Laravel yang digunakan untuk mengelola dan memantau proyek. Fitur utamanya meliputi input data proyek seperti judul, nama project leader, tanggal mulai dan berakhir, nama klien, progress, serta upload foto proyek.

## 👩‍💻 Dibuat oleh

**Noordiani**  
D3 Teknik Informatika  
Politeknik Hasnur  

## 📌 Fitur
- CRUD (Create, Read, Update, Delete) data proyek
- Upload foto proyek
- Tampilan monitoring menggunakan tabel
- Desain responsif menggunakan Tailwind CSS
- Akses langsung tanpa login (open access)

## 🛠️ Teknologi yang Digunakan
- **Laravel 12**
- **MySQL**
- **Tailwind CSS**
- **Laravel File Storage (storage:link)**

## 📷 Screenshot Tampilan

> Pastikan folder `public/screenshots/` berisi file gambar berikut:

### 📋 Daftar Project
![Daftar Project](screenshots/daftar_project.png)

### ➕ Tambah Project
![Tambah Project](screenshots/tambah_project.png)

### ✏️ Edit Project
![Edit Project](screenshots/edit_project.png)

## 🚀 Cara Menjalankan Project (Lokal)

```bash
# Clone repository
git clone https://github.com/Noordiani/sistem_monitoring.git
cd project-monitoring-noordiani

# Install dependency Laravel
composer install

# Salin file .env dan generate key
cp .env.example .env
php artisan key:generate

# Konfigurasi database (di file .env)
# DB_DATABASE=your_db
# DB_USERNAME=your_username
# DB_PASSWORD=your_password

# Migrasi tabel ke database
php artisan migrate

# Buat symbolic link untuk file upload
php artisan storage:link

# Jalankan server
php artisan serve

