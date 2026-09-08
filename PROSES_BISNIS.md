# PROSES BISNIS ALUR PELAYANAN PASIEN
## RSUD SOSODORO DJATIKOESOEMO KAB. BOJONEGORO

---

## 📋 Daftar Isi
1. [Overview Proses](#overview-proses)
2. [Alur Masuk Pasien (Entry Point)](#alur-masuk-pasien)
3. [Alur Pemeriksaan](#alur-pemeriksaan)
4. [Alur Tindakan Medis](#alur-tindakan-medis)
5. [Alur Pembayaran](#alur-pembayaran)
6. [Alur Keluar Pasien](#alur-keluar-pasien)

---

## Overview Proses

Diagram ini menunjukkan alur lengkap pelayanan pasien di RSUD SOSODORO DJATIKOESOEMO dari masuk hingga keluar, mencakup:
- **Pendaftaran & Admission**
- **Pemeriksaan Medis**
- **Penunjang Medis (Laboratorium, Radiologi)**
- **Pemeriksaan Khusus (Fisioterapi, IRD)**
- **Proses Tindakan & Resep**
- **Pembayaran**
- **Pulang/Keluar**

---

## Alur Masuk Pasien (Entry Point)

### 1. **ANTRIAN**
**Deskripsi:** Pasien datang dan masuk antrian melalui tiga jalur masuk:
- WASIAT
- M-JKN (Aplikasi Jaminan Kesehatan Nasional)
- ONSITE (Langsung datang ke rumah sakit)

**Output:** Tiket antrian atau nomor urut

**Waktu Proses:** ~5-10 menit

---

### 2. **ADM-C (Administrasi Poli)**
**Deskripsi:** Petugas administrasi melakukan:
- Verifikasi identitas pasien
- Cek riwayat pasien (jika ada)
- Pencatatan data awal
- Pengecekan status pembayaran/asuransi

**Requirement:** Data valid, dokumen lengkap

**Output:** Berkas pasien siap untuk pemeriksaan

**Waktu Proses:** ~5-15 menit

---

## Alur Pemeriksaan

### 3. **POLI (Poliklinik - Pemeriksaan Awal)**
**Deskripsi:** Dokter spesialis melakukan:
- Anamnesis (tanya jawab)
- Pemeriksaan fisik
- Diagnosis awal
- Penentuan tindak lanjut

**Keputusan Checkpoint:**
- ✅ **YA** → Lanjut ke penentuan tindakan
- ❌ **TIDAK** → Rujuk ke Poli lain atau rawat jalan

**Output:** Catatan medis, rekomendasi pemeriksaan

**Waktu Proses:** ~15-30 menit

---

### 4. **ADM-E (Administrasi Eksekutif)**
**Deskripsi:** Petugas administrasi melakukan:
- Update data kepesertaan
- Verifikasi asuransi/pembayaran
- Pencatatan tindakan yang akan dilakukan

**Output:** Dokumen siap untuk prosedur

**Waktu Proses:** ~5-10 menit

---

### 5. **FISIOTERAPI**
**Deskripsi:** Terapis fisik melakukan:
- Evaluasi kondisi pasien
- Fisioterapi sesuai diagnosa
- Pencatatan progress

**Output:** Laporan fisioterapi, rekomendasi follow-up

**Waktu Proses:** ~30-45 menit

---

### 6. **PENUNJANG MEDIS**
Mencakup:
- **LABORATORIUM** → Pemeriksaan darah, urin, dll
- **RADIOLOGI** → Rontgen, CT Scan, USG, dll

**Output:** Hasil pemeriksaan laboratorium/radiologi

**Waktu Proses:** ~1-24 jam (tergantung jenis pemeriksaan)

---

## Alur Tindakan Medis

### 7. **TINDAKAN?** (Decision Point)
**Deskripsi:** Dokter menentukan apakah pasien memerlukan tindakan medis:
- **YA** → Lanjut ke MRS? (Perawatan Inap/UGD)
- **TIDAK** → Lanjut ke Resep

**Keputusan berdasarkan:**
- Severity kondisi pasien
- Kebutuhan observasi
- Rencana treatment

---

### 8. **MRS? (Masuk Rawat Sehari/UGD)**
**Deskripsi:** Jika diperlukan perawatan intensif:
- Penerimaan ke ruang perawatan
- Monitoring berkelanjutan
- Tindakan medis lanjutan

**Output:** Catatan observasi, rekam medis terupdate

**Waktu Proses:** Sesuai kebutuhan medis

---

### 9. **ADM-A (Administrasi Admission)**
**Deskripsi:** Petugas administrasi melakukan:
- Pendaftaran pasien rawat inap/UGD
- Penentuan ruangan
- Pencatatan biaya
- Pengecekan asuransi

**Output:** Dokumen admisi, biaya estimasi

**Waktu Proses:** ~10-20 menit

---

### 10. **IRD (Inpatient Record Discharge)**
**Deskripsi:** Dokter membuat:
- Catatan perkembangan harian
- Order medis
- Rencana perawatan
- Persiapan pulang

**Output:** Rekam medis lengkap, instruksi discharge

**Waktu Proses:** Sesuai durasi perawatan

---

## Alur Pembayaran

### 11. **PEMBAYARAN POLI** (Jika rawat jalan)
**Proses:**
- Hitung total biaya layanan
- Verifikasi asuransi
- Proses pembayaran
- Cetak kwitansi

**Output:** Bukti pembayaran

---

### 12. **PEMBAYARAN IRD** (Jika rawat inap)
**Proses:**
- Kalkulasi biaya perawatan (kamar, obat, tindakan, pemeriksaan)
- Klaim ke asuransi jika ada
- Verifikasi R. IRNA (Ruang IRNA - Instalasi Rawat Inap)
- Proses pembayaran dengan sistem KRS (Kartu Rekam Medis)

**Output:** Bukti pembayaran, rincian biaya

---

### 13. **R. IRNA (Ruang/Instalasi Rawat Inap)**
**Deskripsi:** Verifikasi dan proses pembayaran untuk:
- Biaya kamar
- Biaya perawatan
- Biaya pemeriksaan penunjang (Laboratorium, Radiologi, Farmasi, HD, Fisioterapi, IBS)

**Output:** Data pembayaran terverifikasi

---

### 14. **ADM-E (Administrasi Eksekutif - Follow up)**
**Deskripsi:** Final administrative clearance sebelum pulang:
- Verifikasi semua pembayaran
- Update sistem
- Cetak dokumen akhir

**Output:** Dokumen kelengkapan administratif

---

### 15. **BANK JATIM**
**Deskripsi:** Proses transfer pembayaran (jika ada klaim asuransi):
- Verifikasi klaim
- Transfer dana ke rumah sakit
- Pencatatan cash flow

**Output:** Konfirmasi pembayaran

---

## Alur Keluar Pasien

### 16. **RESEP?** (Decision Point)
**Deskripsi:** Dokter menentukan:
- **YA** → Ke Apotek
- **TIDAK** → Langsung pulang

---

### 17. **APOTEK**
**Deskripsi:** Apoteker melakukan:
- Verifikasi resep dokter
- Penyiapan obat
- Penjelasan cara minum obat
- Dokumentasi pemberian obat

**Output:** Obat resmi, nota apotek

**Waktu Proses:** ~10-30 menit

---

### 18. **PULANG**
**Deskripsi:** Pasien diberangkatkan dengan:
- Surat keterangan/resume medis
- Resep obat (jika ada)
- Instruksi follow-up
- Jadwal kontrol berikutnya

**Output:** Pasien keluar, catatan medis tersimpan

**Waktu Proses:** ~5-10 menit

---

## 📊 Ringkasan Proses Utama

| **Tahap** | **Departemen** | **Durasi** | **Output** |
|-----------|---|---|---|
| Antrian & Pendaftaran | ADM-C | 5-15 min | Berkas pasien |
| Pemeriksaan Awal | POLI | 15-30 min | Diagnosa awal |
| Pemeriksaan Khusus | Fisioterapi/Penunjang | 30-45 min/1-24 jam | Hasil evaluasi |
| Tindakan Medis | IRD/ADM-A | Sesuai kebutuhan | Rekam medis |
| Pembayaran | R. IRNA/ADM-E | 10-30 min | Bukti pembayaran |
| Obat & Keluar | Apotek | 10-30 min | Resep & catatan medis |

---

## ⚠️ Checkpoint Kritis

1. **TINDAKAN?** - Menentukan rawat inap vs rawat jalan
2. **MRS?** - Penentuan tingkat perawatan
3. **RESEP?** - Kebutuhan obat lanjutan
4. **Pembayaran** - Verifikasi finansial sebelum pulang

---

## 🔄 Feedback Loop

- **Penunjang Medis → POLI** - Jika hasil pemeriksaan memerlukan revisi diagnosa
- **ADM-A → R. IRNA** - Koordinasi billing untuk pasien rawat inap
- **Apotek → PULANG** - Instruksi obat sebelum pasien pergi

---

**Dokumen ini memudahkan:**
- ✅ Training staff baru
- ✅ Optimalisasi proses
- ✅ Identifikasi bottleneck
- ✅ Peningkatan kualitas layanan
- ✅ Compliance terhadap standar

---

*Terakhir diupdate: 2026-09-08*
