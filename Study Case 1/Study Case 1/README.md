# TABEL PENGUJIAN

Tabel pengujian digunakan untuk menguji setiap studi kasus dengan beberapa kombinasi kondisi `True` dan `False`.

## 1. Seleksi Peserta Praktikum - AND

| Aktif | Nilai Memenuhi | Prasyarat | Hasil |
|---|---|---|---|
| True | True | True | Peserta DITERIMA praktikum |
| True | False | True | Peserta TIDAK DITERIMA praktikum |
| False | True | True | Peserta TIDAK DITERIMA praktikum |
| True | True | False | Peserta TIDAK DITERIMA praktikum |
| False | False | False | Peserta TIDAK DITERIMA praktikum |

## 2. Seleksi Penerima Beasiswa - AND

| Aktif | Nilai Memenuhi | Prasyarat | Hasil |
|---|---|---|---|
| True | True | True | Mahasiswa LOLOS seleksi beasiswa |
| True | True | False | Mahasiswa TIDAK LOLOS seleksi beasiswa |
| True | False | True | Mahasiswa TIDAK LOLOS seleksi beasiswa |
| False | True | True | Mahasiswa TIDAK LOLOS seleksi beasiswa |
| False | False | True | Mahasiswa TIDAK LOLOS seleksi beasiswa |

## 3. Persetujuan Mengikuti Ujian - AND

| Aktif | Nilai Memenuhi | Prasyarat | Hasil |
|---|---|---|---|
| True | True | True | Mahasiswa BOLEH mengikuti ujian |
| True | False | True | Mahasiswa TIDAK BOLEH mengikuti ujian |
| False | True | True | Mahasiswa TIDAK BOLEH mengikuti ujian |
| True | True | False | Mahasiswa TIDAK BOLEH mengikuti ujian |
| False | False | False | Mahasiswa TIDAK BOLEH mengikuti ujian |

## 4. Penentuan Peserta Prioritas - OR

| Pengalaman | Sertifikat | Hasil |
|---|---|---|
| True | False | Peserta MENDAPAT PRIORITAS |
| False | True | Peserta MENDAPAT PRIORITAS |
| True | True | Peserta MENDAPAT PRIORITAS |
| False | False | Peserta TIDAK MENDAPAT PRIORITAS |

## 5. Kesempatan Mengikuti Program Kampus - OR

| Aktif | Pengalaman | Sertifikat | Hasil |
|---|---|---|---|
| True | False | False | Mahasiswa DAPAT MENGIKUTI PROGRAM |
| False | True | False | Mahasiswa DAPAT MENGIKUTI PROGRAM |
| False | False | True | Mahasiswa DAPAT MENGIKUTI PROGRAM |
| True | True | False | Mahasiswa DAPAT MENGIKUTI PROGRAM |
| False | False | False | Mahasiswa TIDAK DAPAT MENGIKUTI PROGRAM |

## 6. Rekomendasi Peserta Kegiatan - OR

| Nilai Memenuhi | Pengalaman | Sertifikat | Hasil |
|---|---|---|---|
| True | False | False | Peserta DIREKOMENDASIKAN |
| False | True | False | Peserta DIREKOMENDASIKAN |
| False | False | True | Peserta DIREKOMENDASIKAN |
| True | False | True | Peserta DIREKOMENDASIKAN |
| False | False | False | Peserta TIDAK DIREKOMENDASIKAN |

## 7. Pilihan Syarat Pengalaman atau Sertifikat - XOR

| Pengalaman | Sertifikat | Hasil |
|---|---|---|
| True | False | Syarat PILIHAN VALID |
| False | True | Syarat PILIHAN VALID |
| True | True | Syarat PILIHAN TIDAK VALID |
| False | False | Syarat PILIHAN TIDAK VALID |

## 8. Seleksi Jalur Kelulusan - XOR

| Nilai Memenuhi | Prasyarat | Hasil |
|---|---|---|
| True | False | Jalur KELULUSAN VALID |
| False | True | Jalur KELULUSAN VALID |
| True | True | Jalur KELULUSAN TIDAK VALID |
| False | False | Jalur KELULUSAN TIDAK VALID |
