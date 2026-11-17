# Akuisisi Data Hotel dan Penginapan di Bali

## Tujuan

Mengumpulkan data hotel dan penginapan di Bali menggunakan OpenStreetMap sebagai sumber data terbuka. Data ini digunakan untuk memenuhi tugas akuisisi data dan dapat dimanfaatkan sebagai bahan analisis informasi lokasi serta jenis akomodasi wisata di Bali.

## 1. Sumber Data

- **Nama:** OpenStreetMap
- **URL:** https://www.openstreetmap.org/
- **API:** Overpass API
- **URL API:** https://overpass-api.de/api/interpreter
- **Lisensi:** Open Database License (ODbL)
- **Atribusi:** Data © OpenStreetMap contributors

## 2. Tanggal dan Jam Akses

- **Tanggal akuisisi:** 17 November 2026
- **Waktu akuisisi:** 12:15
- **Informasi waktu:** Dicatat berdasarkan dokumentasi `docs/provenance.json`.

## 3. Metode Akuisisi

- **Jenis:** Akuisisi data menggunakan API Overpass.
- **Sumber:** OpenStreetMap.
- **Metode:** Mengirim permintaan data melalui API untuk memperoleh objek lokasi penginapan di wilayah Bali.
- **Format data mentah:** JSON.
- **Format data hasil pengolahan:** CSV.
- **Jumlah data yang diperoleh:** 6.122 objek.

Data JSON kemudian diolah menggunakan Python dan Pandas menjadi file CSV agar lebih mudah dibaca dan dianalisis.

## 4. Batasan Etika

- **Lisensi:** Data menggunakan Open Database License (ODbL) dari OpenStreetMap.
- **Atribusi:** Sumber OpenStreetMap dicantumkan dalam dokumentasi proyek.
- **Privasi:** Tidak mengambil data pribadi pengguna.
- **Izin akses:** Pengambilan data dilakukan melalui Overpass API.
- **Penggunaan:** Data digunakan untuk keperluan akademik.
- **Keterbatasan:** Data bergantung pada informasi yang tersedia dan diperbarui oleh kontributor OpenStreetMap. Tidak semua hotel dan penginapan di Bali pasti tercatat dalam OpenStreetMap.

## 5. Penjelasan Kolom

Nama file: `data/raw/hotel_bali.csv`

| Kolom | Tipe | Keterangan |
|---|---|---|
| osm_type | Teks | Jenis objek OpenStreetMap, seperti node, way, atau relation |
| osm_id | Bilangan bulat | Identitas unik objek di OpenStreetMap |
| name | Teks | Nama hotel atau penginapan |
| tourism | Teks | Kategori pariwisata atau akomodasi |
| latitude | Desimal | Koordinat garis lintang lokasi |
| longitude | Desimal | Koordinat garis bujur lokasi |

**Jumlah record:** 6.122 baris.

**Jumlah kolom:** 6 kolom.

## 6. Struktur Folder

```text
rtm1_2501010166/
├── README.md
├── notebooks/
│   └── akuisisi_data.ipynb
├── data/
│   └── raw/
│       ├── hotel_bali.json
│       └── hotel_bali.csv
└── docs/
    ├── provenance.json
    └── data_ethics_checklist.csv
```

## 7. Cara Menjalankan Ulang

1. Buka Google Colab.
2. Buka notebook `notebooks/akuisisi_data.ipynb`.
3. Pastikan koneksi internet tersedia.
4. Jalankan seluruh kode secara berurutan menggunakan menu **Runtime → Run all**.
5. Data hasil akuisisi akan disimpan dalam folder `data/raw/`.
6. Dokumentasi provenance dan data ethics checklist disimpan dalam folder `docs/`.

## 8. Identitas Pengambil Data

- **Nama:** I Nyoman Cahyanta Kusumadinata
- **NIM:** 2501010166
- **Institusi:** Institut Bisnis dan Teknologi Indonesia (INSTIKI)

## 9. Lisensi dan Atribusi

Dataset ini bersumber dari OpenStreetMap dan digunakan dengan memperhatikan ketentuan Open Database License (ODbL).

Atribusi sumber data:

© OpenStreetMap contributors.

https://www.openstreetmap.org/copyright
