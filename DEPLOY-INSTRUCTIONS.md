# Leon Diamond — Deployment Instructions
**Target URL:** `leondiamond.danielhendra.com`

---

## Cara Deploy (5 menit)

### Option A: Vercel Dashboard (Drag & Drop) — PALING MUDAH

1. Buka https://vercel.com/dashboard
2. Klik **"Add New Project"**
3. Pilih **"Browse"** atau drag & drop folder `leon-diamond-deploy` ini
4. Project name: `leon-diamond`
5. Klik **Deploy**
6. Setelah deploy selesai → masuk ke **Settings → Domains**
7. Add domain: `leondiamond.danielhendra.com`
8. Di DNS manager Namecheap/GoDaddy (wherever danielhendra.com is registered):
   - Add CNAME record: `leondiamond` → `cname.vercel-dns.com`
9. Tunggu 2-5 menit → Live!

---

### Option B: Via GitHub (sama seperti aga-app)

1. Buat GitHub repo baru: `leon-diamond`
2. Upload isi folder `leon-diamond-deploy` ke repo
3. Di Vercel → Import Git Repository → pilih `leon-diamond`
4. Deploy
5. Tambah domain `leondiamond.danielhendra.com` di Settings → Domains
6. CNAME record sama seperti Option A

---

## Setelah Live

- Semua product links → redirect ke `leondiamond.com` Shopify store
- Live product images diambil dari Shopify API secara real-time
- Video hero diambil dari CloudFront CDN (sudah ada)

---

## Menambahkan Gambar (setelah generate di ChatGPT)

Taruh file gambar di folder yang sama dengan `index.html`, lalu beri tahu Claude nama file-nya.
Claude akan update `index.html` dengan reference ke file tersebut.

Atau upload ke Shopify CDN:
Admin Shopify → Settings → Files → Upload → copy URL → kasih ke Claude.

---

## Files dalam folder ini

| File | Keterangan |
|------|------------|
| `index.html` | Website utama Leon Diamond |
| `vercel.json` | Vercel deployment config |
| `DEPLOY-INSTRUCTIONS.md` | File ini |

---

*Prepared by Claude · Leon Diamond Project · May 2026*
