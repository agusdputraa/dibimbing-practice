# 🎬 Dinetflix - Netflix Clone Landing Page

![Dinetflix](https://img.shields.io/badge/Status-Active-success)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?logo=tailwind-css&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

Sebuah landing page modern yang terinspirasi dari Netflix, dibangun dengan **HTML5**, **TailwindCSS**, dan **Vanilla JavaScript**. Proyek ini menampilkan desain responsif, animasi interaktif, dan UI/UX yang menarik.

## ✨ Fitur Utama

### 🏠 Halaman Utama (index.html)
- **Hero Section** dengan background gambar Netflix asli
- **Email Validation** dengan animasi shake untuk input yang tidak valid
- **Trending Section** menampilkan 5 film/series terpopuler dengan ranking
- **Feature Cards** dengan gradient warna yang menarik (violet, pink, emerald, amber)
- **Interactive Favorites** - klik poster untuk menandai sebagai favorit dengan efek ring kuning
- **Scroll Animation** menggunakan Intersection Observer API
- **Fully Responsive** - optimal di mobile, tablet, dan desktop

### 💰 Halaman Pricing (pricing.html)
- **3 Paket Berlangganan**:
  - Basic Plan (100k/bulan) - 2 devices, HD resolution
  - Standard Plan (120k/bulan) - 4 devices, UHD resolution
  - Ultimate Plan (180k/bulan) - 6 devices, 4K resolution
- **Comparison Table** dengan fitur lengkap setiap paket
- **Icon Integration** menggunakan Feather Icons
- **Hover Effects** pada tombol dengan scale dan shadow
- **Footer** lengkap dengan social media links dan navigasi

## 🎨 Teknologi yang Digunakan

- **HTML5** - Struktur semantik
- **TailwindCSS (CDN)** - Utility-first CSS framework
- **Vanilla JavaScript** - Interaktivitas tanpa framework
- **Google Fonts (Poppins)** - Typography modern
- **Feather Icons** - Icon set yang clean dan minimalis
- **Material Symbols** - Icon untuk rating/favorit

## 🚀 Cara Menggunakan

### Metode 1: Langsung Buka di Browser
1. Clone atau download repository ini
```bash
git clone <repository-url>
cd dibimbing-practice-master
```

2. Buka file `index.html` di browser favorit Anda
```bash
# Windows
start index.html

# macOS
open index.html

# Linux
xdg-open index.html
```

### Metode 2: Menggunakan Live Server
1. Install Live Server extension di VS Code
2. Klik kanan pada `index.html`
3. Pilih "Open with Live Server"

### Metode 3: Menggunakan Python HTTP Server
```bash
# Python 3
python -m http.server 8000

# Buka browser dan akses
# http://localhost:8000
```

## 📁 Struktur Proyek

```
dibimbing-practice-master/
│
├── index.html          # Halaman utama dengan hero section dan trending
├── pricing.html        # Halaman pricing dengan tabel perbandingan
└── README.md          # Dokumentasi proyek (file ini)
```

## 🎯 Custom Tailwind Configuration

Proyek ini menggunakan custom color palette:

```javascript
colors: {
  kakaes: {
    brown: "#3b2f2f",
    cream: "#f5f0ea",
    gold: "#c4a47f",
  },
}
```

Font family custom:
```javascript
fontFamily: {
  sans: ["Poppins", "ui-sans-serif", "system-ui", "sans-serif"],
}
```

## 💡 Fitur JavaScript Interaktif

### 1. Email Validation
```javascript
// Validasi email dengan regex
// Animasi shake jika email tidak valid
// Alert konfirmasi jika berhasil
```

### 2. Favorite Toggle
```javascript
// Klik poster untuk toggle favorit
// Efek ring kuning dan icon bintang
// State management sederhana
```

### 3. Scroll Animation
```javascript
// Intersection Observer untuk lazy animation
// Fade in + translate Y effect
// Fallback untuk browser lama
```

## 🎨 Gradient Color Palette

| Feature | Gradient |
|---------|----------|
| Enjoy on TV | `from-violet-600 to-indigo-600` |
| Download Shows | `from-pink-600 to-rose-600` |
| Watch Everywhere | `from-emerald-600 to-teal-600` |
| Kids Profiles | `from-amber-600 to-orange-600` |

## 📱 Responsive Breakpoints

- **Mobile**: < 640px (max-sm)
- **Tablet**: 640px - 768px (sm)
- **Desktop**: > 768px (md)

Semua elemen telah dioptimalkan untuk setiap breakpoint dengan utility classes TailwindCSS.

## 🔧 Customization

### Mengubah Warna Tema
Edit konfigurasi Tailwind di dalam tag `<script>`:
```javascript
tailwind.config = {
  theme: {
    extend: {
      colors: {
        primary: "#your-color",
        // tambahkan warna custom lainnya
      },
    },
  },
};
```

### Mengubah Harga Paket
Edit langsung di `pricing.html`:
```html
<span class="text-3xl font-bold">100k</span>
```

### Menambah Trending Items
Tambahkan div baru di section trending dengan struktur yang sama:
```html
<div class="relative w-[calc(50%-0.5rem)] sm:w-[calc(33.333%-0.67rem)] md:w-auto">
  <span class="absolute text-white text-6xl md:text-[100px] text-shadow-lg font-bold bottom-0 -left-2 md:-left-4">6</span>
  <img class="w-full h-auto" src="your-image-url.jpg" />
</div>
```

## 🌟 Best Practices yang Diterapkan

- ✅ Semantic HTML5
- ✅ Mobile-first approach
- ✅ Accessibility considerations
- ✅ Performance optimization (CDN, lazy loading)
- ✅ Clean and maintainable code
- ✅ Consistent naming conventions
- ✅ Responsive images
- ✅ Cross-browser compatibility

## 🐛 Known Issues & Limitations

- Slider functionality di pricing.html masih dalam development
- Beberapa duplicate CSS di pricing.html yang perlu dibersihkan
- Email tidak benar-benar terkirim (hanya validasi frontend)
- Sign In button belum terhubung ke backend

## 🔮 Future Improvements

- [ ] Integrasi dengan backend API
- [ ] Implementasi authentication system
- [ ] Database untuk menyimpan user preferences
- [ ] Video player integration
- [ ] Search functionality
- [ ] Filter by genre/category
- [ ] User profile management
- [ ] Payment gateway integration
- [ ] Multi-language support
- [ ] Dark/Light mode toggle

## 📄 License

Proyek ini dibuat untuk keperluan pembelajaran dan practice. Bebas digunakan untuk tujuan edukasi.

## 👨‍💻 Author

Dibuat dengan ❤️ untuk latihan Dibimbing

## 🙏 Acknowledgments

- Design inspiration: [Netflix](https://www.netflix.com)
- Icons: [Feather Icons](https://feathericons.com/)
- Fonts: [Google Fonts - Poppins](https://fonts.google.com/specimen/Poppins)
- CSS Framework: [TailwindCSS](https://tailwindcss.com)

---

⭐ Jika proyek ini membantu, jangan lupa beri star!
