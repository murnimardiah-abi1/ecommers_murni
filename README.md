# 🍵 Matchava — Website E-Commerce Matcha Latte

> *"Slow down, and sip matcha."*

Website e-commerce single-page untuk brand minuman matcha **Matchava**, dibangun dengan HTML5, CSS3, dan Vanilla JavaScript murni — tanpa framework, tanpa backend, tanpa proses build. Langsung buka di browser, langsung jalan.

---

## 📋 Daftar Isi

1. [Dokumentasi Bisnis](#-dokumentasi-bisnis)
   - [Profil Brand](#11-profil-brand)
   - [Daftar Produk & Harga](#12-daftar-produk--harga)
   - [Metode Pembayaran](#13-metode-pembayaran)
   - [Informasi Kontak](#14-informasi-kontak)
   - [Alur Pemesanan Pelanggan](#15-alur-pemesanan-pelanggan)
   - [Rencana Pengembangan Bisnis](#16-rencana-pengembangan-bisnis)
2. [Dokumentasi Teknis](#-dokumentasi-teknis)
   - [Stack Teknologi](#21-stack-teknologi)
   - [Struktur File & Folder](#22-struktur-file--folder)
   - [Arsitektur Halaman](#23-arsitektur-halaman)
   - [Logika JavaScript](#24-logika-javascript)
   - [Sistem CSS & Tema Warna](#25-sistem-css--tema-warna)
3. [Cara Menjalankan](#-cara-menjalankan)
4. [Cara Deploy ke GitHub Pages](#-cara-deploy-ke-github-pages)
5. [Panduan Kustomisasi](#-panduan-kustomisasi)
6. [Status & Batasan](#-status--batasan)

---

## 🏢 Dokumentasi Bisnis

### 1.1 Profil Brand

| | |
|---|---|
| **Nama Brand** | Matchava |
| **Tagline** | "Slow down, and sip matcha." |
| **Jenis Usaha** | Minuman siap saji berbasis matcha latte |
| **Target Pasar** | Pecinta matcha, anak muda urban, penggemar minuman kekinian sehat |
| **Keunggulan** | Matcha grade upacara dari Uji, Jepang — diwhisk langsung saat dipesan |
| **Jam Operasional** | Setiap hari, 09.00 – 21.00 |

---

### 1.2 Daftar Produk & Harga

| No | Nama Produk | Deskripsi | Harga |
|----|-------------|-----------|-------|
| 1 | Classic Matcha Latte | Rasa matcha murni, lembut dan creamy | Rp 25.000 |
| 2 | Strawberry Matcha Latte | Manis segar strawberry bertemu matcha | Rp 28.000 |
| 3 | Coconut Matcha Latte | Kelapa creamy berpadu pahit matcha | Rp 27.000 |
| 4 | Mango Matcha Latte | Mangga tropis manis dan menyegarkan | Rp 28.000 |
| 5 | Honey Matcha Latte | Manis alami madu pilihan | Rp 27.000 |
| 6 | Chocolate Matcha Latte | Perpaduan cokelat dan matcha yang kaya | Rp 29.000 |
| 7 | Vanilla Matcha Latte | Aroma vanilla lembut menenangkan | Rp 27.000 |
| 8 | Cream Cheese Matcha | Topping cream cheese asin manis khas | Rp 30.000 |

> 💡 Harga dapat diubah langsung di array `menuItems` pada file `index.html`.

**Biaya Pengiriman:** Rp 10.000 flat untuk semua pesanan (ditambahkan otomatis saat checkout).

---

### 1.3 Metode Pembayaran

| Metode | Keterangan |
|--------|-----------|
| 🔳 QRIS | Scan QR — semua dompet digital |
| 🏦 Transfer Bank | Transfer manual via rekening bank |
| 📱 E-Wallet | OVO / GoPay / DANA |
| 💵 COD | Bayar di tempat saat barang diterima |

> ⚠️ **Catatan:** Pembayaran saat ini adalah **simulasi front-end**. Belum terhubung ke payment gateway sungguhan. Lihat [Status & Batasan](#-status--batasan) untuk detail.

---

### 1.4 Informasi Kontak

| Kanal | Detail |
|-------|--------|
| 📞 Telepon / WhatsApp | 0896-0103-8762 |
| ✉️ Email | murnimardiah82@gmail.com |
| 📍 Jam Buka | Setiap hari, 09.00 – 21.00 |

---

### 1.5 Alur Pemesanan Pelanggan

```
┌─────────────────────────────────────────────────────────┐
│                   CUSTOMER JOURNEY                       │
├─────────────────────────────────────────────────────────┤
│                                                          │
│  1. Buka website → lihat Hero Section (Home)             │
│          ↓                                               │
│  2. Scroll / klik "Lihat Menu" → lihat 8 varian matcha  │
│          ↓                                               │
│  3. Klik tombol "+" pada produk → masuk Keranjang        │
│          ↓                                               │
│  4. Buka Keranjang → cek item, ubah qty jika perlu       │
│          ↓                                               │
│  5. Klik "Checkout" → isi Nama, No.HP, Email, Alamat     │
│          ↓                                               │
│  6. Klik "Lanjut ke Pembayaran" → pilih metode bayar     │
│          ↓                                               │
│  7. Klik "Bayar Sekarang" → muncul konfirmasi sukses     │
│     berisi: Order ID, total bayar, metode pembayaran     │
│          ↓                                               │
│  8. Keranjang otomatis kosong → siap order berikutnya    │
│                                                          │
└─────────────────────────────────────────────────────────┘
```

---

### 1.6 Rencana Pengembangan Bisnis

- [ ] Integrasi payment gateway resmi (Midtrans / Xendit)
- [ ] Notifikasi otomatis WhatsApp/email ke pemilik saat order masuk
- [ ] Sistem login & riwayat pesanan pelanggan
- [ ] Dashboard admin: kelola menu, harga, stok
- [ ] Ongkos kirim dinamis berdasarkan lokasi (Google Maps API)
- [ ] Program loyalitas / poin reward pelanggan
- [ ] Fitur ulasan & rating produk
- [ ] Integrasi marketplace (Tokopedia, Shopee)

---

## 🛠 Dokumentasi Teknis

### 2.1 Stack Teknologi

| Komponen | Teknologi | Keterangan |
|----------|-----------|-----------|
| Struktur | HTML5 | Semantik, aksesibel |
| Styling | CSS3 murni | Custom properties, Grid, Flexbox |
| Interaktivitas | Vanilla JavaScript | Tanpa library/framework |
| Font | Google Fonts | Fraunces (display) + Manrope (body) |
| Foto Produk | File lokal (`images/`) | 8 foto JPG |
| Dependensi | Google Fonts CDN | Satu-satunya dependensi eksternal |
| Build tool | ❌ Tidak ada | Tidak perlu npm, webpack, dll |
| Backend | ❌ Tidak ada | Murni front-end statis |

---

### 2.2 Struktur File & Folder

```
matchava/
│
├── index.html              ← Seluruh kode website (HTML + CSS + JS)
│
├── images/                 ← Folder foto produk
│   ├── classic.jpg         → Classic Matcha Latte
│   ├── strawberry.jpg      → Strawberry Matcha Latte
│   ├── coconut.jpg         → Coconut Matcha Latte
│   ├── mango.jpg           → Mango Matcha Latte
│   ├── honey.jpg           → Honey Matcha Latte
│   ├── chocolate.jpg       → Chocolate Matcha Latte
│   ├── vanilla.jpg         → Vanilla Matcha Latte
│   └── creamcheese.jpg     → Cream Cheese Matcha
│
└── README.md               ← Dokumentasi ini
```

> ⚠️ **Penting:** Nama file foto harus **persis** seperti di atas (huruf kecil semua, tidak ada spasi). Kalau berbeda, foto tidak akan muncul.

---

### 2.3 Arsitektur Halaman

Website terdiri dari satu file `index.html` dengan beberapa section:

```
index.html
│
├── <header>              Navigasi sticky (logo + menu link + tombol keranjang)
│
├── <section #home>       Hero: judul, deskripsi brand, tombol CTA
├── <section #menu>       Grid 8 kartu produk dengan foto, harga, tombol +
├── <section #about>      Cerita brand + statistik (8 rasa, 100% matcha, 5k+ cangkir)
├── <section #contact>    Kartu kontak: telepon, email, jam buka
│
├── <footer>              Copyright
│
├── .overlay              Layer gelap saat drawer/modal terbuka
├── .drawer #drawer       Panel keranjang belanja (slide dari kanan)
│
├── #checkoutModal        Modal: form data pengiriman
├── #paymentModal         Modal: pilih metode pembayaran
└── #successModal         Modal: konfirmasi transaksi berhasil
```

---

### 2.4 Logika JavaScript

#### Data Produk
Semua data produk disimpan dalam satu array `menuItems`:
```javascript
const menuItems = [
  {
    id: 1,
    name: "Classic Matcha Latte",
    desc: "Rasa matcha murni, lembut dan creamy.",
    price: 25000,        // angka (Rupiah)
    icon: "🍵",          // emoji badge di atas foto
    img: "images/classic.jpg"  // path foto
  },
  // ...
];
```
Array ini adalah **single source of truth** — kartu menu, isi keranjang, dan total harga semuanya dirender dari array ini.

#### State Keranjang
```javascript
let cart = {};
// Contoh isi: { 1: 2, 5: 1 }
// artinya: produk id=1 qty 2, produk id=5 qty 1
```

| Fungsi | Tugasnya |
|--------|---------|
| `addToCart(id)` | Tambah produk ke keranjang, buka drawer |
| `changeQty(id, delta)` | Tambah/kurangi qty; hapus otomatis jika qty ≤ 0 |
| `getCartTotal()` | Hitung total harga (price × qty semua item) |
| `getCartCount()` | Hitung total jumlah item (untuk badge angka) |
| `updateCartUI()` | Re-render isi drawer setiap kali state berubah |

#### Alur Modal
```
openCart()       → buka drawer keranjang
openCheckout()   → tutup drawer, buka modal "Data Pengiriman"
goToPayment()    → validasi form, buka modal "Metode Pembayaran"
processPayment() → validasi metode, generate Order ID,
                   buka modal sukses, reset cart & form
closeAll()       → tutup semua drawer & modal
```

#### Validasi
- Form checkout: Nama, No. HP, dan Alamat wajib diisi
- Pembayaran: wajib pilih salah satu metode
- Tombol Checkout otomatis `disabled` jika keranjang kosong

#### Generate Order ID
```javascript
const orderId = "MTV-" + Date.now().toString().slice(-8);
// Contoh hasil: MTV-48213907
```
ID dibuat dari 8 digit terakhir timestamp — unik setiap transaksi, namun ini **bukan ID resmi dari sistem pembayaran**.

---

### 2.5 Sistem CSS & Tema Warna

Semua warna menggunakan **CSS Custom Properties** di `:root` agar mudah diganti:

```css
:root {
  --matcha-deep: #3f5d3a;   /* Hijau matcha tua — warna utama */
  --matcha-mid:  #6b8c5f;   /* Hijau matcha sedang — aksen */
  --matcha-pale: #cfe0b8;   /* Hijau muda — latar badge/icon */
  --cream:       #f7f3e8;   /* Krem — latar halaman utama */
  --clay:        #c97b4a;   /* Coklat tanah — harga & aksen kontras */
  --ink:         #262017;   /* Coklat tua — teks utama */
  --paper:       #fffdf7;   /* Putih krem — latar kartu */
}
```

**Tipografi:**
- `Fraunces` (serif) → heading & harga: kesan elegan, hangat, artisanal
- `Manrope` (sans-serif) → body text: bersih, mudah dibaca

**Layout:**
- CSS Grid untuk menu (4 kolom → 2 kolom di mobile)
- Flexbox untuk navigasi, kartu, drawer
- Breakpoint utama: `880px` (tablet/mobile)

**Animasi:**
- Drawer keranjang: `transition: right 0.3s ease`
- Hover kartu: `transform: translateY(-5px)` + `box-shadow`
- Semua transisi murni CSS, tanpa library animasi

---

## 🚀 Cara Menjalankan

### Di Komputer Lokal

**Cara 1 — Langsung buka (paling simpel):**
```
Double-click file index.html → terbuka di browser
```

**Cara 2 — Pakai Live Server di VS Code (direkomendasikan):**
1. Install extension **Live Server** di VS Code
2. Klik kanan `index.html` → **Open with Live Server**
3. Website auto-refresh setiap kali kamu edit & save ✅

> Tidak perlu `npm install`, `node`, atau setup apapun.

---

## 🌐 Cara Deploy ke GitHub Pages

Ikuti langkah ini untuk website live gratis:

```
1. Buat akun GitHub (jika belum punya) → github.com

2. Klik "New repository"
   - Nama repo: matchava
   - Visibility: Public
   - Klik "Create repository"

3. Upload file:
   - Klik "uploading an existing file"
   - Drag & drop SELURUH ISI folder matchava/
     (index.html + folder images/ beserta 8 foto)
   - Klik "Commit changes"

4. Aktifkan GitHub Pages:
   - Settings → Pages (menu kiri)
   - Source: Deploy from a branch
   - Branch: main → / (root)
   - Klik Save

5. Tunggu 1-2 menit, lalu website live di:
   https://usernamekamu.github.io/matchava
```

> 💡 **Tips:** Pastikan upload folder `images/` beserta isinya sekaligus dengan `index.html`. Kalau hanya upload `index.html`-nya saja, foto tidak akan muncul.

---

## ✏️ Panduan Kustomisasi

### Ubah Nama / Harga Produk
Edit array `menuItems` di dalam `<script>` pada `index.html`:
```javascript
{id:1, name:"Nama Produk Baru", desc:"Deskripsi.", price:30000, icon:"🍵", img:"images/classic.jpg"}
```

### Tambah Produk Baru
1. Tambah objek baru di array `menuItems`
2. Simpan foto produknya di folder `images/` dengan nama yang sesuai
3. Ubah grid menu dari 4 kolom jika perlu: `.menu-grid { grid-template-columns: repeat(4, 1fr); }`

### Ubah Ongkos Kirim
```javascript
const SHIPPING = 10000; // ganti angka ini
```

### Ubah Kontak
Cari bagian `<section id="contact">` di HTML:
```html
<p>0896-0103-8762</p>
<p>murnimardiah82@gmail.com</p>
```

### Ubah Warna Tema
Edit nilai hex di `:root` pada bagian `<style>`:
```css
--matcha-deep: #3f5d3a; /* ganti warna utama di sini */
--clay: #c97b4a;        /* ganti warna aksen di sini */
```

### Ganti Foto Produk
Cukup ganti file foto di folder `images/` dengan nama yang **sama persis**. Tidak perlu edit kode.

---

## ⚠️ Status & Batasan

| Fitur | Status | Keterangan |
|-------|--------|-----------|
| Tampilan & navigasi | ✅ Selesai | Responsif, mobile-friendly |
| Keranjang belanja | ✅ Selesai | Tambah, kurangi, hapus item |
| Form checkout | ✅ Selesai | Validasi nama, HP, alamat |
| Pilih metode pembayaran | ✅ Selesai | 4 pilihan tersedia |
| Konfirmasi transaksi | ✅ Selesai | Order ID + ringkasan bayar |
| Foto produk asli | ✅ Selesai | 8 foto dari pemilik brand |
| Penyimpanan pesanan | ❌ Belum ada | Pesanan hilang saat refresh |
| Payment gateway resmi | ❌ Belum ada | Masih simulasi |
| Notifikasi ke pemilik | ❌ Belum ada | Perlu backend/WA API |
| Login pelanggan | ❌ Belum ada | Perlu autentikasi |
| Manajemen stok | ❌ Belum ada | Perlu admin panel + database |

### Rekomendasi Langkah Selanjutnya (Go-Live)

1. **Payment Gateway** → Daftar di [Midtrans](https://midtrans.com) atau [Xendit](https://xendit.co), integrasikan Snap.js
2. **Database pesanan** → Gunakan Google Sheets + Google Apps Script (gratis, tanpa server) atau Firebase
3. **Notifikasi WhatsApp** → Gunakan WA Business API atau Fonnte untuk kirim pesan otomatis ke pemilik
4. **Hosting lebih profesional** → Vercel atau Netlify (lebih cepat dari GitHub Pages, tetap gratis)

---

## 📄 Lisensi & Kredit

- Website dibuat khusus untuk brand **Matchava**
- Font: [Fraunces](https://fonts.google.com/specimen/Fraunces) & [Manrope](https://fonts.google.com/specimen/Manrope) via Google Fonts (OFL License)
- Foto produk: dokumentasi milik Matchava

---

*© 2026 Matchava. Slow down, and sip matcha. 🍵*
