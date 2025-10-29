# Praktikum 6: Bootstrap

**Nama:** Manuel Johansen Dolok Saribu

**Nim:** 312410493

Mata Kuliah: Pemograman Web 1

Dosen Pengampu: Agung Nugroho, S.Kom., M.Kom.,

---

## Langkah-Langkah Praktikum

### Refactor Layout Praktikum 4

**Tujuan:**  
Mengubah layout sederhana dari Praktikum 4 agar menggunakan sistem grid Bootstrap dan komponen-komponen siap pakai.

**Langkah-langkah:**
1. Buat file `home.html`.
2. Tambahkan Bootstrap 5 CDN di dalam `<head>`.
3. Ganti struktur navigasi lama dengan komponen `<nav class="navbar navbar-expand-lg ...">`.
4. Gunakan **Grid System** (`.row`, `.col-md-8`, `.col-md-4`) untuk membagi main content dan sidebar.
5. Ganti elemen *box* atau *widget-box* lama menjadi komponen **Bootstrap Card**:
   ```html
   <div class="card">
     <div class="card-body">
       <h5 class="card-title">Heading</h5>
       <p class="card-text">...</p>
     </div>
   </div>
   ```
6. Hapus seluruh penggunaan CSS `float` dan `clear` karena layout kini diatur oleh grid Bootstrap.
7. Tambahkan footer di bagian bawah halaman menggunakan class `bg-dark text-white`.

---

### Refactor Form Praktikum 5

**Tujuan:**  
Menyusun ulang salah satu form dari Praktikum 5 agar tampak modern dan rapi dengan komponen form Bootstrap.

**Langkah-langkah:**
1. Buat file `kontak.html`.
2. Tambahkan Bootstrap CDN.
3. Gunakan class:
   - `.form-label` untuk label input.
   - `.form-control` untuk input, textarea, dan select.
   - `.btn btn-primary` untuk tombol submit.
4. Tambahkan validasi sederhana menggunakan JavaScript (opsional).
5. Hubungkan file ini dengan menu “Kontak” pada navbar di `home.html`:
   ```html
   <li class="nav-item"><a class="nav-link" href="kontak.html">Kontak</a></li>
   ```

---

### Membuat Halaman Portfolio Sederhana

**Tujuan:**  
Membuat halaman `portfolio.html` menggunakan Bootstrap untuk menampilkan biodata singkat dan beberapa proyek.

**Langkah-langkah:**
1. Buat file `portfolio.html`.
2. Tambahkan Navbar di bagian atas halaman.
3. Buat section **“Tentang Saya”**:
   - Gunakan `.container` dan `.row`.
   - Gunakan `.col-md-4` untuk foto dengan class `.img-fluid`.
   - Gunakan `.col-md-8` untuk nama dan deskripsi diri.
4. Buat section **“Portfolio Saya”**:
   - Gunakan `.container` dan `.row`.
   - Buat tiga `.col-md-4`, masing-masing berisi komponen `.card`:
     ```html
     <div class="card">
       <img src="..." class="card-img-top" alt="...">
       <div class="card-body">
         <h5 class="card-title">Proyek 1</h5>
         <p class="card-text">Deskripsi singkat proyek.</p>
       </div>
     </div>
     ```
5. Tambahkan footer di bagian bawah halaman.

---

## Integrasi Navigasi
Ketiga halaman (`home.html`, `kontak.html`) dihubungkan dengan **Navbar Bootstrap**.  
Contoh struktur navigasi:
```html
<ul class="navbar-nav ms-auto">
  <li class="nav-item"><a class="nav-link active" href="home.html">Home</a></li>
  <li class="nav-item"><a class="nav-link" href="kontak.html">Kontak</a></li>
</ul>
```

---

## Kesimpulan
Dalam Praktikum 6 ini:
- Layout dari praktikum sebelumnya berhasil direfaktor menggunakan **Bootstrap 5 Grid System**.
- Komponen **Card** dan **Form** Bootstrap digunakan untuk menggantikan struktur lama berbasis CSS manual.
- Halaman **Portfolio** dibuat dengan desain responsif dan navigasi terintegrasi.
- Tidak ada penggunaan `float` atau `clear`, semua layout mengandalkan sistem grid Bootstrap.

> Dengan Bootstrap, tampilan web menjadi lebih modern, rapi, dan mudah dikembangkan untuk berbagai ukuran layar (mobile-friendly).
