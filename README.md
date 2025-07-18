# Walking Story Photography Website

Website fotografi dengan slider otomatis, navigasi kategori, dan tooltip foto.

## Struktur File

```
d:/ak kontol/
├── index.html          # File HTML utama
├── style.css           # File CSS untuk styling
├── script.js           # File JavaScript terpisah (sederhana)
├── README.md           # Dokumentasi ini
└── images/             # Folder untuk menyimpan foto
    ├── slider/         # Foto untuk header slider
    └── categories/     # Foto untuk setiap kategori
        ├── human-interest/
        ├── culinary/
        ├── social-activity/
        ├── cityscape/
        ├── public-space/
        └── environment/
```

## Fitur Website

### 1. Header Image Slider
- Auto-slide setiap 5 detik
- Navigation arrows (prev/next)
- Dots indicator untuk navigasi langsung
- Pause on hover
- Responsive design

### 2. Category Navigation
- 6 kategori foto: Human Interest, Culinary, Social Activity, Cityscape, Public Space, Environment
- Klik kategori untuk melihat galeri foto
- Back button untuk kembali ke halaman utama
- Smooth transitions

### 3. Photo Galleries dengan Tooltip
- Hover pada foto untuk melihat tooltip dengan judul dan deskripsi
- Grid layout responsive
- Hover effects yang smooth
- Loading dari Picsum Photos API (sementara)

### 4. Responsive Design
- Mobile-friendly
- Tablet dan desktop optimized
- Smooth scrolling

## Cara Menggunakan

1. **Buka website**: Double-click `index.html` atau buka di browser
2. **Navigasi slider**: Gunakan arrows atau dots untuk navigasi manual
3. **Pilih kategori**: Klik salah satu kategori untuk melihat foto-foto
4. **Lihat tooltip**: Hover cursor pada foto untuk melihat deskripsi
5. **Kembali**: Klik "Back to Categories" untuk kembali ke halaman utama

## Mengganti Foto

### Untuk Slider:
Ganti URL di `index.html` pada bagian slider atau simpan foto di folder `images/slider/`

### Untuk Kategori:
1. Simpan foto di folder kategori yang sesuai (misal: `images/categories/culinary/`)
2. Update src di `index.html` dari Picsum URL ke path lokal
3. Contoh: `src="images/categories/culinary/foto1.jpg"`

## Teknologi yang Digunakan

- **HTML5**: Struktur website
- **CSS3**: Styling dan animasi
- **JavaScript**: Interaktivitas (slider, navigasi, tooltip)
- **Tailwind CSS**: Framework CSS untuk styling cepat
- **Picsum Photos**: API foto placeholder (sementara)

## Browser Support

- Chrome (recommended)
- Firefox
- Safari
- Edge

## Customization

### Mengubah Warna:
Edit file `style.css` pada bagian gradient dan color variables

### Menambah Kategori:
1. Tambah card kategori di `index.html`
2. Buat section view untuk kategori baru
3. Tambah folder di `images/categories/`
4. Update JavaScript jika diperlukan

### Mengubah Timing Slider:
Edit nilai `5000` (5 detik) di `script.js` pada fungsi `setInterval`

## Tips

- Gunakan foto dengan resolusi yang sama untuk hasil terbaik
- Foto slider: 1200x500px
- Foto kategori: 400x300px
- Compress foto untuk loading yang lebih cepat
- Test di berbagai device untuk memastikan responsive

## Troubleshooting

**Slider tidak berjalan**: Pastikan `script.js` ter-load dengan benar
**Foto tidak muncul**: Check path file foto dan pastikan format didukung (jpg, png, webp)
**Tooltip tidak muncul**: Pastikan CSS hover effects tidak ter-override
