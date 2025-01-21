# Prostore - E-commerce Website

Prostore adalah platform e-commerce yang dibangun menggunakan Next.js, Prisma, dan Neon untuk pengelolaan database serverless. Platform ini menyediakan antarmuka yang responsif dan modern bagi pengguna untuk menjelajahi dan membeli produk.

![Prostore Screenshot](https://github.com/user-attachments/assets/1fa676e1-6d53-48a9-a787-cfabe738d3ea)

---

## Features

- **Product Listing**: Menampilkan produk dengan detail, termasuk nama, harga, dan status ketersediaan.
- **Newest Arrivals Section**: Menyoroti produk-produk terbaru yang tersedia.
- **Responsive Design**: Optimasi untuk berbagai perangkat.
- **Dynamic Pricing and Ratings**: Harga dan rating produk diperbarui secara dinamis.

---

## Tech Stack

Proyek ini dibangun dengan teknologi berikut:

- **Next.js**: 15.1.5 - Untuk server-side rendering dan front-end berbasis React.
- **React**: 19.0.0 - Untuk membangun antarmuka pengguna.
- **Prisma**: 6.2.1 - Untuk ORM database dan pengelolaan PostgreSQL serverless dengan Neon.
- **Neon Database**: Untuk hosting database PostgreSQL serverless.
- **TailwindCSS**: 3.4.1 - Untuk styling dan desain responsif.
- **Shadcn UI**: Untuk komponen UI yang dapat disesuaikan dan mudah diakses.
- **TypeScript**: 5.x - Untuk keamanan tipe selama pengembangan.
- **WebSocket (ws)**: Digunakan untuk menghubungkan Neon melalui WebSocket.

---

## Installation

Untuk mengatur proyek ini secara lokal, ikuti langkah-langkah berikut:

### 1. Clone Repository

```bash
git clone https://github.com/fachrinfl/nextjs-prostore.git
nextjs-prostore
```

### 2. Install Dependencies

```bash
npm install --legacy-peer-deps
```

### 3. Konfigurasikan Environment Variables

Buat file `.env` di direktori root dan tambahkan variabel berikut:

```bash
# .env Configuration

Berikut adalah konfigurasi environment untuk aplikasi **Prostore**:

```dotenv
# Application Information
NEXT_PUBLIC_APP_NAME = "Prostore" 
# Nama aplikasi yang akan digunakan secara publik, seperti di metadata atau tampilan front-end.

NEXT_PUBLIC_APP_DESCRIPTION = "A modern ecommerce store built with Next.js" 
# Deskripsi singkat aplikasi yang dapat digunakan untuk SEO atau metadata.

# Server URL
NEXT_PUBLIC_SERVER_URL = "http://localhost:3000" 
# URL server untuk lingkungan pengembangan (localhost).

# Database Connection
DATABASE_URL = "your-neon-database-connection-string" 
# URL koneksi ke database Neon (serverless PostgreSQL). Pastikan untuk mengganti kredensial ini di lingkungan produksi.

# Configuration
LATEST_PRODUCTS_LIMIT = "4" 
# Konfigurasi untuk menentukan jumlah produk terbaru yang ditampilkan pada halaman utama.
```

### 4. Jalankan Perintah Prisma

Generate Prisma client dan inisialisasi database:

```bash
npx prisma generate
npx prisma migrate dev --name init
```

### 5. Mulai Server Pengembangan

```bash
npm run dev
```

Akses aplikasi di `http://localhost:3000`.


