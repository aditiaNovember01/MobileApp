# ProjectMobile

Proyek ini terdiri dari dua bagian utama:

- **backend/**: API backend menggunakan Laravel
- **frontend/**: Aplikasi mobile menggunakan Flutter

---

## Backend (Laravel)

### Setup

1. Masuk ke folder backend:
   ```bash
   cd backend
   ```
2. Install dependency:
   ```bash
   composer install
   ```
3. Copy file environment:
   ```bash
   cp .env.example .env
   ```
4. Generate key:
   ```bash
   php artisan key:generate
   ```
5. Atur konfigurasi database di file `.env`
6. Jalankan migrasi:
   ```bash
   php artisan migrate
   ```
7. Jalankan server:
   ```bash
   php artisan serve
   ```
   API akan berjalan di `http://localhost:8000`

---

## Frontend (Flutter)

### Setup

1. Masuk ke folder frontend:
   ```bash
   cd frontend
   ```
2. Install dependency:
   ```bash
   flutter pub get
   ```
3. Jalankan aplikasi:
   ```bash
   flutter run
   ```
   Pastikan emulator/device sudah aktif.

---

## Catatan Integrasi

- Pastikan URL API di aplikasi Flutter mengarah ke backend Laravel, misal:
  - Android emulator: `http://10.0.2.2:8000/api/...`
  - Device fisik/real: gunakan IP komputer Anda, misal `http://192.168.x.x:8000/api/...`
- Untuk deployment, backend dan frontend bisa dihosting secara terpisah.

---

## License

Silakan tambahkan lisensi sesuai kebutuhan.
