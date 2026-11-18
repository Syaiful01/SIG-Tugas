# SIG Web Interaktif — SDG 9 & SDG 11

Proyek ini adalah halaman pembelajaran dan demonstrasi SIG Web interaktif untuk mendukung pembahasan **SDG 9 (Industri, Inovasi, dan Infrastruktur)** serta **SDG 11 (Kota dan Permukiman Berkelanjutan)**.

## Fitur

- Peta Leaflet dengan tiga pilihan basemap: OpenStreetMap, CARTO Dark, dan Esri Satellite.
- Marker dan popup untuk beberapa lokasi penting di sekitar Medan.
- Layer control untuk mengaktifkan atau menonaktifkan layer tematik.
- Mode tambah titik pada peta.
- Pengukuran jarak menggunakan polyline.
- Pengukuran luas menggunakan poligon.
- Geolocation untuk menampilkan lokasi pengguna.
- Tampilan responsif untuk desktop dan perangkat mobile.
- Mode tema terang dan gelap.
- Essay bertema SDG dengan penyimpanan lokal di browser.
- Kanban proyek dengan status To-Do, In Progress, dan Done.
- Kuis singkat mengenai dasar SIG Web.

## Struktur proyek

```text
.
├── index.html
└── README.md
```

## Cara menjalankan

Buka `index.html` menggunakan browser. Untuk hasil yang lebih konsisten, jalankan melalui server lokal atau ekstensi Live Server pada VS Code.

Contoh server lokal menggunakan Python:

```bash
python -m http.server 5500
```

Kemudian buka `http://localhost:5500` pada browser.

Koneksi internet diperlukan karena Leaflet dan tile basemap dimuat dari layanan eksternal.

## Cara menggunakan peta

1. Pilih basemap melalui tombol **Ganti Basemap** atau kontrol layer di kanan atas peta.
2. Gunakan **Tambah Titik** lalu klik peta untuk membuat marker baru.
3. Gunakan **Ukur Jarak** lalu klik beberapa titik secara berurutan.
4. Gunakan **Ukur Luas** lalu klik minimal tiga titik untuk membentuk area.
5. Gunakan **Lokasi Saya** setelah memberikan izin geolocation pada browser.
6. Gunakan **Bersihkan** untuk menghapus marker dan hasil pengukuran buatan pengguna.

## Penyimpanan data

Jawaban essay, penilaian diri, tema tampilan, dan progres Kanban disimpan menggunakan `localStorage` browser. Data tersebut tersimpan pada browser/perangkat yang digunakan dan tidak dikirim ke server.

## Kesesuaian dengan rubrik

| Kriteria | Implementasi |
|---|---|
| Peta tampil dan stabil | Leaflet, kontrol zoom, tiga basemap, dan atribusi sumber peta |
| Data spasial terikat | Data koordinat lokasi ditampilkan sebagai marker dengan popup |
| Interaktivitas | Layer control, tambah titik, pengukuran jarak/luas, dan geolocation |
| Desain dan aksesibilitas | Layout responsif, kontras tema, tombol berlabel, dan atribusi |
| Dokumentasi dan publikasi | README ini dan kesiapan untuk GitHub Pages |

## Publikasi ke GitHub Pages

1. Buat repository baru di GitHub.
2. Upload `index.html` dan `README.md`.
3. Buka **Settings → Pages**.
4. Pada bagian **Build and deployment**, pilih **Deploy from a branch**.
5. Pilih branch `main` dan folder `/root`.
6. Simpan pengaturan, lalu tunggu sampai GitHub Pages membuat URL publik.

## Catatan pengumpulan

Sertakan repository GitHub, link GitHub Pages, dan ZIP yang berisi file proyek sesuai instruksi Google Classroom. Jawaban essay dikerjakan dan diperiksa secara mandiri sebelum dikumpulkan.
