# Matplotlib Archive - Evaluasi Pembelajaran

## Deskripsi

Repository ini berisi kumpulan notebook Jupyter untuk mempelajari visualisasi data menggunakan **Matplotlib** dan **NumPy** di Python.

---

## Chapter 1: Dasar-Dasar Visualisasi Data dengan Matplotlib

### Konsep yang Sudah Dipelajari

#### 1. Import Library Dasar

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
```

Semua notebook menggunakan kombinasi library ini untuk manipulasi dan visualisasi data.

---

#### 2. Membuat Line Plot (`plt.plot()`)

| File                      | Deskripsi                                 |
| ------------------------- | ----------------------------------------- |
| `bills.ipynb`             | Visualisasi tagihan gas & listrik bulanan |
| `cat_adoptions.ipynb`     | Tren adopsi kucing per bulan              |
| `home_prices.ipynb`       | Harga rumah per dekade (1980-2020)        |
| `pedometer.ipynb`         | Langkah kaki mingguan                     |
| `phone_screen_time.ipynb` | Waktu layar harian                        |
| `sport.ipynb`             | Perbandingan poin tim NBA                 |
| `test.ipynb`              | Revenue film Action vs Comedy             |

**Parameter yang dipelajari:**

- `marker` - Bentuk penanda titik data (`'o'`, `'s'`, `'^'`, `'d'`)
- `linestyle` - Gaya garis (`'-'`, `'--'`, `'-.'`, `':'`)
- `color` - Warna garis (`'blue'`, `'red'`, `'orange'`, dll.)
- `label` - Label untuk legend

---

#### 3. Membuat Bar Chart (`plt.bar()`)

| File                    | Deskripsi                                   |
| ----------------------- | ------------------------------------------- |
| `hasil_penjualan.ipynb` | Perbandingan penjualan tahunan 2023 vs 2024 |

**Parameter yang dipelajari:**

- `width` - Lebar bar
- `alpha` - Transparansi bar (0-1)
- Posisi bar menggunakan `x - width/2` dan `x + width/2` untuk grouped bar chart

---

#### 4. Kustomisasi Plot

| Fungsi                       | Kegunaan               | Contoh            |
| ---------------------------- | ---------------------- | ----------------- |
| `plt.figure(figsize=(w, h))` | Mengatur ukuran gambar | `figsize=(10, 6)` |
| `plt.title()`                | Judul grafik           |                   |
| `plt.xlabel()`               | Label sumbu X          |                   |
| `plt.ylabel()`               | Label sumbu Y          |                   |
| `plt.legend()`               | Menampilkan legend     |                   |
| `plt.grid()`                 | Menampilkan grid       | `plt.grid(True)`  |
| `plt.xticks()`               | Mengatur label sumbu X |                   |
| `plt.show()`                 | Menampilkan grafik     |                   |

---

#### 5. Operasi NumPy yang Dipelajari

| Fungsi           | Kegunaan             | File                                     |
| ---------------- | -------------------- | ---------------------------------------- |
| `np.array()`     | Membuat array        | Semua file                               |
| `np.arange()`    | Membuat range angka  | `bills.ipynb`, `phone_screen_time.ipynb` |
| `np.sum(axis=0)` | Menjumlahkan array   | `bills.ipynb`                            |
| `np.average()`   | Menghitung rata-rata | `phone_screen_time.ipynb`                |

---

#### 6. Membaca Data dari File CSV

| File                         | Deskripsi                                                                  |
| ---------------------------- | -------------------------------------------------------------------------- |
| `Fizzlewhiz Gearspark.ipynb` | Membaca `gearsparks_emporium_weekly_sales.csv` menggunakan `pd.read_csv()` |

**Dataset CSV berisi:**

- Data penjualan toko (Consumable, Weapon, Armor, Scroll, Tool, Accessory)
- Per hari dalam seminggu (Mon-Sun)

---

#### 7. Membuat DataFrame dengan Pandas

| File                  | Deskripsi                                        |
| --------------------- | ------------------------------------------------ |
| `cat_adoptions.ipynb` | Membuat DataFrame manual dengan `pd.DataFrame()` |

---

### Ringkasan Materi Chapter 1

| No  | Topik                                               | Status     |
| --- | --------------------------------------------------- | ---------- |
| 1   | Import library (numpy, pandas, matplotlib)          | ✅ Selesai |
| 2   | Membuat line plot dasar                             | ✅ Selesai |
| 3   | Membuat multiple line plots dalam satu figure       | ✅ Selesai |
| 4   | Kustomisasi marker, linestyle, dan color            | ✅ Selesai |
| 5   | Membuat bar chart                                   | ✅ Selesai |
| 6   | Membuat grouped bar chart                           | ✅ Selesai |
| 7   | Menambahkan title, labels, legend, grid             | ✅ Selesai |
| 8   | Menggunakan np.array, np.arange, np.sum, np.average | ✅ Selesai |
| 9   | Membaca data dari CSV                               | ✅ Selesai |
| 10  | Membuat DataFrame dengan Pandas                     | ✅ Selesai |

---

### Contoh Proyek yang Dibuat

1. **bills.ipynb** - Tracking tagihan utilitas (gas + listrik) selama setahun
2. **cat_adoptions.ipynb** - Analisis tren adopsi kucing
3. **Fizzlewhiz Gearspark.ipynb** - Visualisasi penjualan toko game/RPG
4. **hasil_penjualan.ipynb** - Perbandingan performa penjualan 2023 vs 2024
5. **home_prices.ipynb** - Tren harga rumah selama 4 dekade
6. **pedometer.ipynb** - Tracking aktivitas jalan kaki mingguan
7. **phone_screen_time.ipynb** - Analisis waktu layar HP + rata-rata
8. **sport.ipynb** - Perbandingan skor 4 tim NBA
9. **test.ipynb** - Perbandingan pendapatan film Action vs Comedy

---

---

## Chapter 2: Teknik Visualisasi Lanjutan dan Manipulasi Data

Chapter 2 berfokus pada teknik visualisasi yang lebih kompleks, penanganan subplot, dan integrasi data yang lebih erat dengan **Pandas**.

### Konsep yang Sudah Dipelajari

#### 1. Scatter Plot (`plt.scatter()`)

| File                   | Deskripsi                                              |
| ---------------------- | ------------------------------------------------------ |
| `rich_vs_health.ipynb` | Visualisasi korelasi Life Expectancy vs GDP per Capita |

**Fitur yang dipelajari:**

- `alpha` - Mengatur transparansi titik untuk menangani penumpukan data (_overplotting_).
- Visualisasi hubungan antar dua variabel numerik.

---

#### 2. Pie Chart (`plt.pie()`)

| File               | Deskripsi                                     |
| ------------------ | --------------------------------------------- |
| `pizza.ipynb`      | Distribusi toping pizza yang dipesan          |
| `box_office.ipynb` | (Juga menyertakan contoh distribusi kategori) |

**Parameter yang dipelajari:**

- `labels` - Nama untuk setiap potongan.
- `autopct` - Menampilkan persentase secara otomatis (`'%1.1f%%'`).
- `explode` - Menonjolkan potongan tertentu agar terpisah dari lingkaran utama.

---

#### 3. Penanganan Subplots (`plt.subplots()`)

| File               | Deskripsi                                              |
| ------------------ | ------------------------------------------------------ |
| `classes.ipynb`    | Visualisasi skor ujian siswa dalam 4 panel (4x1 & 2x2) |
| `box_office.ipynb` | Perbandingan penjualan film menggunakan panel terpisah |

**Konsep OOP (Object-Oriented) yang dipelajari:**

- `fig, axes = plt.subplots(nrows, ncols)` - Membuat grid gambar.
- Mengakses panel menggunakan indeks: `axes[0]` (1D) atau `axes[0, 1]` (2D).
- `sharex=True` - Berbagi sumbu X antar subplot untuk perbandingan yang lebih baik.

---

#### 4. Teknik Layout dan Kustomisasi Lanjutan

| Fungsi                       | Deskripsi                                                    | notebook terkait   |
| ---------------------------- | ------------------------------------------------------------ | ------------------ |
| `plt.tight_layout()`         | Menyesuaikan margin otomatis agar label tidak tumpang tindih | `classes.ipynb`    |
| `plt.xticks(rotation=angle)` | Memutar label sumbu X agar lebih mudah dibaca                | `bee.ipynb`        |
| `ax.set_title()`             | Mengatur judul pada level subplot                            | `box_office.ipynb` |

---

#### 5. Manipulasi Data dengan Pandas

| Teknik              | Kegunaan                                               | File              |
| ------------------- | ------------------------------------------------------ | ----------------- |
| `.isin(list)`       | Memfilter data berdasarkan kumpulan nilai              | `bee.ipynb`       |
| `.groupby().mean()` | Agregasi data untuk mendapatkan rata-rata per kategori | `bee.ipynb`       |
| `.unique()`         | Mengambil nilai unik dari kolom                        | `tech_guru.ipynb` |

---

### Ringkasan Materi Chapter 2

| No  | Topik                                              | Status     |
| --- | -------------------------------------------------- | ---------- |
| 1   | Membuat Scatter Plot dengan transparansi           | ✅ Selesai |
| 2   | Membuat Pie Chart dengan persentase & explosion    | ✅ Selesai |
| 3   | Implementasi Subplots (Grid 1D & 2D)               | ✅ Selesai |
| 4   | Sinkronisasi sumbu X menggunakan `sharex`          | ✅ Selesai |
| 5   | Rotasi label axis dengan `xticks(rotation)`        | ✅ Selesai |
| 6   | Penggunaan `tight_layout` untuk estetika grid      | ✅ Selesai |
| 7   | Filtering & Agregasi data tingkat lanjut di Pandas | ✅ Selesai |

---

### Contoh Proyek yang Dibuat

1. **bee.ipynb** - Analisis kehilangan koloni lebah per negara bagian (Bar Chart & Filtering).
2. **classes.ipynb** - Dasbor nilai siswa menggunakan grid Subplots.
3. **tech_guru.ipynb** - Multi-line plot penjualan produk teknologi.
4. **aquarium.ipynb** - Visualisasi populasi hiu di berbagai lokasi (Bar Chart).
5. **bill_expenses.ipynb** - Perbandingan tren biaya utilitas (Line Plot).
6. **box_office.ipynb** - Analisis pendapatan film mingguan (OOP Approach).
7. **pizza.ipynb** - Visualisasi pasar toping pizza favorit masyarakat.
8. **rich_vs_health.ipynb** - Analisis ekonomi-kesehatan global (Scatter Plot).

---

## Teknologi yang Digunakan

- Python 3.x
- NumPy
- Pandas
- Matplotlib
- Jupyter Notebook

---

_Terakhir diperbarui: Februari 2026_
