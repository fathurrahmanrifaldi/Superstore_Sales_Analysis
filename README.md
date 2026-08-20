#  Superstore Sales Analysis

Analisis data penjualan Superstore (2015–2018) menggunakan Excel — mulai dari data cleaning, pivot summary, visualisasi, hingga dashboard interaktif dan rekomendasi bisnis.

##  Dataset

Dataset berisi **9.800 baris transaksi** dengan informasi order, pelanggan, produk, dan penjualan, mencakup periode Januari 2015 – Desember 2018.

| Kolom | Deskripsi |
|---|---|
| Order ID, Order Date, Ship Date, Ship Mode | Detail order & pengiriman |
| Customer ID, Customer Name, Segment | Informasi pelanggan |
| City, State, Region, Postal Code | Lokasi geografis |
| Category, Sub-Category, Product Name | Detail produk |
| Sales | Nilai penjualan (USD) |

##  Proses Analisis

1. **Data Cleaning & Preparation** — pengecekan duplikat & missing value, konversi format tanggal, penambahan kolom turunan (Order Year, Month, YearMonth, Ship Duration).
2. **Pivot Table Analysis** — ringkasan penjualan per Category, Region, Segment, Ship Mode, dan Sub-Category menggunakan formula dinamis (SUMIF, COUNTIF, AVERAGEIF).
3. **Visualization** — bar chart, line chart, dan pie chart untuk melihat tren dan komposisi penjualan.
4. **Dashboard** — ringkasan interaktif dengan KPI cards dan kumpulan chart dalam satu tampilan.
5. **Insights & Recommendations** — temuan bisnis dan rekomendasi strategis berdasarkan hasil analisis.

##  Isi Workbook (`Superstore_Sales_Analysis.xlsx`)

| Sheet | Isi |
|---|---|
| `Dashboard` | KPI utama (Total Sales, Orders, Customers, Avg Sales/Transaksi) + 5 chart ringkasan |
| `Insights_Recommendations` | Insight & rekomendasi bisnis per kategori, region, segment, shipping, dan tren waktu |
| `Data` | Data bersih dalam bentuk Excel Table dengan kolom tambahan hasil cleaning |
| `Summary_Category` | Ringkasan penjualan per kategori produk |
| `Summary_Region` | Ringkasan penjualan per region |
| `Summary_Segment` | Ringkasan penjualan per segmen pelanggan |
| `Summary_ShipMode` | Ringkasan penjualan & rata-rata durasi pengiriman per ship mode |
| `Summary_SubCategory` | Ringkasan penjualan per sub-kategori produk |
| `Summary_MonthlyTrend` | Tren penjualan bulanan 2015–2018 |
| `Top10_Products` | 10 produk dengan penjualan tertinggi |
| `Top10_Customers` | 10 pelanggan dengan penjualan tertinggi |
| `Top10_State` | 10 state dengan penjualan tertinggi |

##  Temuan Utama

- **Technology** adalah kategori dengan penjualan tertinggi meskipun jumlah transaksinya paling sedikit — menandakan nilai per transaksi yang besar.
- **Region West** memimpin penjualan, sementara **Region South** paling rendah dan berpotensi jadi target ekspansi.
- Penjualan menunjukkan **pola musiman yang konsisten**, dengan puncak setiap tahun terjadi di bulan **November–Desember**.
- **Standard Class** adalah moda pengiriman paling banyak digunakan namun paling lambat, membuka peluang untuk mendorong pelanggan ke opsi pengiriman yang lebih cepat.
- Segmen **Consumer** mendominasi kontribusi penjualan dibanding Corporate dan Home Office.

##  Tools

- Microsoft Excel (formula: `SUMIF`, `COUNTIF`, `AVERAGEIF`, Excel Table, PivotChart)

##  Struktur Repository

```
├── Superstore_Sales_Analysis.xlsx   # Workbook lengkap (Data, Summary, Dashboard, Insights)
├── superstore_sales.csv                        # Dataset mentah
└── README.md
```

##  Cara Menggunakan

1. Unduh dan buka `Superstore_Sales_Analysis.xlsx` di Microsoft Excel.
2. Mulai dari sheet `Dashboard` untuk melihat ringkasan visual.
3. Lihat sheet `Insights_Recommendations` untuk insight & rekomendasi bisnis.
4. Data mentah dan hasil cleaning tersedia di sheet `Data`, dalam format Excel Table — semua summary akan otomatis ter-update jika data berubah.
