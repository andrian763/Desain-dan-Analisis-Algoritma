# Desain dan Analisis Algoritma – Integer Knapsack

Proyek ini merupakan implementasi dan perbandingan dua algoritma pemecahan masalah **Integer Knapsack**: **Dynamic Programming** dan **Branch and Bound**, dengan menggunakan data produk dari `GroceryDataset.csv`. Proyek ini disusun sebagai tugas akhir mata kuliah **Desain dan Analisis Algoritma**, dengan fokus pada efisiensi pemrosesan, pengambilan keputusan berbasis nilai (rating), dan pemanfaatan struktur data serta pendekatan algoritmik dalam konteks dunia nyata.

---

## 🗂 Dataset

Dataset berisi informasi produk kebutuhan sehari-hari seperti nama produk, harga, rating, fitur, dan deskripsi. Dataset ini telah melalui tahap _cleaning_ dan preprocessing, di antaranya:
- Penghapusan kolom yang tidak relevan (`Currency`, `Discount`)
- Penanganan missing values dan data non-numerik pada kolom `Price` dan `Rating`
- Ekstraksi nilai numerik dari string teks (misalnya "4.3 out of 5 stars")

Hasil akhir disimpan sebagai `cleaned_dataset.csv`.

---

## 🧠 Tujuan Masalah

Menyelesaikan masalah **pemilihan produk terbaik** yang memberikan **nilai (rating) tertinggi** tanpa melebihi **anggaran tertentu**, menggunakan dua algoritma:
- **Dynamic Programming**
- **Branch and Bound**

---

## ⚙️ Tools & Bahasa Pemrograman
- Python 3.x
- Pandas
- Time module
- Jupyter Notebook

---

## 📈 Langkah dan Tahapan
1. **Import dan pembersihan data**
2. **Perhitungan total dan rata-rata rating**
3. **Implementasi algoritma Integer Knapsack:**
   - **Dynamic Programming**
   - **Branch and Bound**
4. **Evaluasi hasil:** waktu eksekusi, total profit, rata-rata rating, total harga, dan item yang dipilih
5. **Analisis kompleksitas waktu dan ruang**

---

## 🧮 Hasil Eksekusi

### ✅ Dynamic Programming
- **Total Rating (Profit):** 38
- **Rata-rata Rating:** 4.75
- **Total Harga:** $147.72
- **Waktu Eksekusi:** 0.0433 detik
- **Kompleksitas:** O(n × W) = O(600 × 150)

### ✅ Branch and Bound
- **Total Rating (Profit):** 13.3
- **Rata-rata Rating:** 4.43
- **Total Harga:** $144.97
- **Waktu Eksekusi:** 0.0020 detik
- **Kompleksitas:** O(n × W) = O(600 × 150)

---

## 🧩 Produk Terpilih (Contoh)
- Cokelat Premium
- Ekstrak Vanila
- Lint Roller
- Campuran Pancake Bebas Gluten
- Suplemen Vitamin
- Rempah Organik

> Produk dipilih berdasarkan rasio rating terhadap harga untuk memaksimalkan kualitas dalam batasan anggaran.

---

## 📌 Cara Menjalankan

1. Buka file notebook: `ProjekDAA.ipynb`
2. Pastikan dataset `cleaned_dataset.csv` tersedia di direktori kerja
3. Jalankan seluruh cell dari atas hingga bawah di Jupyter Notebook

---

## 📚 Referensi

- [GeeksforGeeks – 0-1 Knapsack Problem (DP)](https://www.geeksforgeeks.org/0-1-knapsack-problem-dp-10/)
- [GeeksforGeeks – 0-1 Knapsack using Branch and Bound](https://www.geeksforgeeks.org/0-1-knapsack-using-least-count-branch-and-bound/)

---


