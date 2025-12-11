# Praktikum Teori Graf C06

| Name           | NRP        | Kelas     |
| ---            | ---        | ---       |
| Azil Alriansyah Hidayat | 5025241070 | C |
| Dyah Utami Kesuma Dewi | 5025241186 | C |
| Najma Lail Arazy | 5025241243 | C |

## 1. **Program Knight’s Tour (8×8 Chessboard)**

Program ini menyelesaikan persoalan *Knight’s Tour*, yaitu perjalanan bidak kuda pada papan 8×8 hingga mengunjungi seluruh kotak sekali saja.

### **Cara Menjalankan Program**

1. Jalankan program Python.
2. Masukkan **posisi awal kuda (X dan Y)** dalam rentang **1–8**.

   * Program otomatis mengonversi ke indeks array (0–7).
3. Masukkan **mode perjalanan**:

   * `open`  → perjalanan tidak harus kembali ke kotak awal.
   * `closed` → langkah terakhir harus dapat menyerang kotak awal.

### **Format Input**

```
Masukkan posisi awal X (1–8): <angka>
Masukkan posisi awal Y (1–8): <angka>
Pilih mode (open / closed): <teks>
```

### **Output Program**

1. Jika solusi ada → program menampilkan:

   * Matriks 8×8 berisi urutan langkah kuda.
   * Plot visual berisi garis rute perjalanan kuda dalam urutan yang benar.
2. Jika tidak ada solusi → program menampilkan pesan error:

```
Gagal menemukan solusi untuk posisi awal tersebut!
```

### **Contoh Output**

```
Solusi ditemukan!

[54, 41, 14, 11, 56, 31, 16, 9]
[13, 0, 55, 42, 15, 10, 33, 30]
...
```

## 2. **Program Largest Monotonically Increasing Subsequence (LIS) — Tree Search**

Program ini mencari *subsequence* (bukan substring) terpanjang yang setiap elemennya meningkat secara monoton.
Pencarian dilakukan dengan model *tree search* (rekursif).

### **Cara Menjalankan Program**

1. Jalankan program Python.
2. Data input sudah terisi otomatis dalam sebuah list, namun dapat diganti:

   ```
   data_input = [4, 1, 13, 7, 0, 2, 8, 11, 3]
   ```
3. Program langsung memproses dan mencari LIS.

### **Output Program**

Program menghasilkan:

* Data input yang dipakai
* Largest Monotonically Increasing Subsequence
* Panjang subsequence tersebut

### **Contoh Output**

```
Data Input: [4, 1, 13, 7, 0, 2, 8, 11, 3]
Longest Monotonically Increasing Subsequence: [1, 7, 8, 11]
Panjang: 4
```

## Catatan

* Kedua program tidak membutuhkan library eksternal selain **matplotlib** (khusus Knight’s Tour).
* Semua parameter dapat dimodifikasi pada bagian atas kode.
* Visualisasi rute Knight’s Tour hanya tampil jika program dijalankan pada lingkungan yang mendukung GUI.
