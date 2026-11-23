<div align="center">

# Portofolio — reyzdev

**Website portofolio pribadi** · Next.js (static export) + Cloudflare Workers

[![Live](https://img.shields.io/badge/live-reyzdev.my.id-1e3a8a?style=for-the-badge&logo=googlechrome&logoColor=white)](https://reyzdev.my.id)
[![Next.js](https://img.shields.io/badge/Next.js-16-000000?logo=nextdotjs&logoColor=white)](https://nextjs.org)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-06B6D4?logo=tailwindcss&logoColor=white)
![Cloudflare Workers](https://img.shields.io/badge/Cloudflare-Workers-F38020?logo=cloudflare&logoColor=white)

</div>

> Repo ini **cuma showcase** — kode sumbernya privat. Isinya tampilan, fitur, dan stack.

## Tampilan

<div align="center">

<img src="docs/hero.webp" width="760" alt="Hero" />

| Desktop (About) | Mobile |
|---|---|
| <img src="docs/about.webp" width="420" alt="About" /> | <img src="docs/mobile.webp" width="190" alt="Mobile" /> |

</div>

## Fitur

- **Hero animasi** — parallax berlapis, dipakai di desktop & mobile
- **Timeline pendidikan & pengalaman** yang interaktif
- **Kartu proyek** dengan lightbox detail + tab Sertifikat & Tech Stack
- **Folder interaktif** yang bisa dibuka (lihat detail proyek/kegiatan)
- **Kolom komentar** (nama, isi, foto profil opsional) tersimpan di browser
- **Form kontak** + tombol salin email + tombol kirim ke WhatsApp
- **`/cv/`** menampilkan CV (PDF) langsung di browser, plus tombol download
- SEO: metadata, Open Graph image, JSON-LD, `robots.txt`, `sitemap.xml`

## Stack

| Bagian | Teknologi |
|---|---|
| Framework | Next.js 16 (App Router, `output: "export"`) |
| Bahasa | TypeScript |
| Styling | Tailwind CSS |
| Animasi | CSS + canvas (tanpa library animasi besar) |
| Deploy | Cloudflare Workers static assets + custom domain |

## Cara deploy

Static export, hasilnya folder `out/` yang di-upload ke Cloudflare Workers:

```bash
npm run build
npx wrangler deploy
```

## Catatan

- Kode sumber: **privat**
- Versi lama (React 18 + Vite + Supabase): juga privat
