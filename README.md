# Dashboard KUR – bank bjb syariah

Halaman web dashboard penyaluran KUR (satu file `index.html`, tanpa proses build).

## Cara tayang di GitHub Pages
1. Buat repository baru di https://github.com/new (mis. `dashboard-kur`).
2. Klik **Add file → Upload files**, unggah `index.html` dan `README.md`, lalu **Commit changes**.
3. Buka **Settings → Pages**. Pada *Build and deployment* pilih **Deploy from a branch**, branch **main**, folder **/(root)**, lalu **Save**.
4. Tunggu 1–2 menit. Alamatnya: `https://NAMA-GITHUB-ANDA.github.io/dashboard-kur/`

## Lewat Git (opsional)
```
git init && git add . && git commit -m "Dashboard KUR"
git branch -M main
git remote add origin https://github.com/NAMA-GITHUB-ANDA/dashboard-kur.git
git push -u origin main
```

## Memperbarui data
- Tombol **Perbarui data (Excel)** di halaman memuat file List Nasabah KUR terbaru ke browser (tidak tersimpan di GitHub; hilang saat halaman dimuat ulang).
- Untuk mengganti data bawaan halaman, buat ulang `index.html` dengan data baru lalu unggah ulang ke repository.

## Mengelola Status AO (Dedicated / AddHock)
- Di bagian *Pencapaian AO* klik **Kelola status AO**: ubah status lewat dropdown, **Tambah** AO baru, atau **Hapus status**.
- Perubahan tersimpan di browser Anda. Supaya berlaku untuk semua orang: klik **Unduh ao-status.json**, lalu unggah file itu ke repository (folder yang sama dengan `index.html`, nama harus `ao-status.json`) dan Commit.
- **Kembalikan awal** mengembalikan status bawaan halaman.

## Catatan keamanan
Data bawaan (cabang, AO, plafond, O/S) tertanam di `index.html`. Situs GitHub Pages dapat dibuka siapa saja yang tahu alamatnya pada akun gratis, walaupun repository-nya private. Pastikan sudah mendapat izin sebelum tayang.
