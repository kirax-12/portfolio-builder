# Portfolio Builder

Tool web untuk membuat website portofolio pribadi tanpa ngoding: isi form, lihat hasilnya langsung, lalu unduh satu file HTML yang bisa dibuka di mana saja.

**Demo live:** buka `index.html` di browser — tidak perlu server, tidak perlu build.

## Cara Pakai

1. Isi data di panel kiri: nama, peran/jabatan, tagline, tentang saya, email, dan link GitHub / LinkedIn / Instagram.
2. Tambahkan skill lewat input skill (Enter atau tombol **+ Tambah**) — skill tampil sebagai chip dan bisa dihapus dengan tombol ×.
3. Isi project: judul, deskripsi singkat, dan link. Baris project bisa ditambah dan dihapus.
4. Pilih **warna aksen** (kuning, pink, biru, hijau, oranye) dan **template** tampilan.
5. Panel kanan menampilkan preview yang berubah real-time mengikuti setiap ketikan dan pilihan.
6. Klik **Isi Contoh** untuk melihat contoh data terisi penuh, atau **Unduh HTML** untuk mengunduh `portofolio.html` — file standalone yang siap dibuka langsung atau di-upload ke hosting / GitHub Pages.

Field boleh dikosongkan: file hasil unduhan tetap rapi karena memakai teks placeholder bawaan.

## Template yang Tersedia

| Template | Karakter |
|---|---|
| **Neo-Brutalism** | Cream, border tebal 2px, bayangan keras, warna flat berani |
| **Minimal Bersih** | Putih lapang, garis tipis, aksen seperlunya, kesan tenang |
| **Gelap Modern** | Latar gelap elegan, teks terang, aksen menyala |

## Teknologi

- Satu file `index.html` mandiri — HTML, CSS, dan JavaScript inline, tanpa framework dan tanpa gambar eksternal.
- Preview memakai `<iframe srcdoc>` yang dirender dari generator yang sama persis dengan file unduhan, jadi yang dilihat = yang diunduh.
- Unduhan dibuat lewat `Blob` + `a.download` langsung di browser; tidak ada data yang dikirim ke server mana pun.
- Font: Space Grotesk, Space Mono, Caveat (tool) dan Inter (template Minimal) via Google Fonts.
- Gaya visual tool mengikuti *Remike Web Style* (neo-brutalism cream).

## Struktur

```
portfolio-builder/
├── index.html   ← seluruh aplikasi (tool + generator portofolio)
└── README.md
```

---

Dibuat oleh **Remike Dev**
