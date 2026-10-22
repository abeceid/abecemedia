# abece.my.id

Situs profil **abece**, rumah cerita. Dibangun dengan [Astro](https://astro.build) dan menghasilkan HTML statis.

## Menjalankan

```bash
npm install
npm run dev      # http://localhost:4321
npm run build    # hasil di dist/
```

## Mengubah isi tanpa menyentuh tampilan

| File | Isi |
|---|---|
| `src/data/site.json` | Nama, tagline, kota, tahun berdiri, kontak |
| `src/data/units.json` | Unit di bawah naungan abece. Tambahkan satu objek untuk unit baru (Postfive, Anekdot Pustaka, dll.) **setelah unitnya benar-benar berjalan** |
| `src/data/timeline.json` | Tonggak perjalanan, format `{ "when": "Okt 2026", "title": "...", "text": "..." }`. Bagian timeline baru tampil otomatis kalau isinya minimal 4 |

## Deploy

Cloudflare Pages:
- **Build command:** `npm run build`
- **Build output directory:** `dist`

Atau unggah manual isi folder `dist/` lewat dashboard Cloudflare Pages.
