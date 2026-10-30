# CASE FILE - NFS-IR-2026-09-14

**Klasifikasi:** TRAINING / FICTIONAL
**Klien:** PT Nusantara Fintech Sejahtera (NFS)
**Jenis kasus:** Kebocoran dokumen internal (data leak)
**Tanggal kejadian:** 14 September 2026

---

## 1. Latar belakang

Pada 14 September 2026, sebuah laporan audit internal NFS berjudul
`NFS-Audit-2026-Q3.pdf` muncul di sebuah paste site publik. Dokumen tersebut
berklasifikasi RAHASIA dan hanya boleh diakses oleh Direksi serta Komite Audit.

Tim tanggap insiden NFS menemukan beberapa artefak di workstation seorang
kontraktor eksternal yang terlibat dalam proyek audit. Kontraktor tersebut
tidak lagi aktif, dan sebagian jejak digitalnya sudah dihapus.

## 2. Misi kamu

Kamu adalah analis forensik digital yang ditugaskan merekonstruksi jejak
kontraktor tersebut menggunakan **Open Source Intelligence (OSINT)**.
Selesaikan tujuh objective secara berurutan untuk menemukan lokasi drop
berisi flag.

## 3. Evidence locker

Semua artefak tersedia di folder `evidence/` (lihat juga `SHA256SUMS` untuk
verifikasi integritas):

| File | Keterangan |
|---|---|
| `01_NFS-Audit-2026-Q3.pdf` | Dokumen audit yang bocor |
| `02_forum_thread.html` | Snapshot halaman forum yang diarsipkan penyidik |
| `03_avatar.png` | Avatar akun forum |
| `05_post_photo.jpg` | Foto yang diunggah akun terkait |
| `07_leak_email.eml` | Email yang dipulihkan dari workstation |

Verifikasi hash:

```bash
sha256sum -c SHA256SUMS
```

## 4. Rules of engagement

- Gunakan **hanya** OSINT dan artefak yang diberikan.
- Jangan menghubungi, mengejar, atau melakukan doxing terhadap siapa pun.
- Jangan mengakses sistem internal NFS atau layanan pihak ketiga secara ilegal.
- Seluruh entitas dalam kasus ini **fiktif**. Kemiripan dengan pihak nyata
  tidak disengaja.
- Flag berbentuk `FLAG{...}`.

## 5. Struktur challenge

Terdapat 7 objective berurutan di platform CTF. Setiap objective mengajarkan
satu teknik dasar OSINT. Setelah semua selesai, kamu akan memperoleh lokasi
drop dan dapat membuka flag final.

Selamat berinvestigasi.
