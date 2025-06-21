# Insight dari Ulasan Aplikasi dengan AI: Studi Kasus IBM Granite dan Dataset Google Play - Muhammad Daniel Ilyasa

## Project Overview

Project ini berfokus pada analisis sentimen berdasarkan ulasan pengguna di platform aplikasi Google play. Dengan bertujuan untuk menggali insight bermakna dari dataset ulasan pengguna aplikasi dengan memanfaatkan kecerdasan buatan, khususnya Large Language Model (LLM) IBM Granite.Dengan pendekatan berbasis prompt engineering dan integrasi melalui LangChain Agent Toolkit, model AI digunakan untuk melakukan klasifikasi sentimen, deteksi emosi, dan evaluasi kegunaan ulasan bagi developer. Setiap review dianalisis tidak hanya dari sisi positif atau negatif, tetapi juga dari sisi emosional dan kontribusinya terhadap perbaikan aplikasi. Seluruh proses dilakukan secara otomatis dan diperkuat dengan visualisasi data seperti  bar chart.Proyek ini menunjukkan bagaimana AI modern dapat berperan sebagai asisten analitik yang mampu menyaring ulasan yang benar-benar bermakna, mempermudah pengambilan keputusan produk, dan memperkuat strategi pengembangan aplikasi yang berbasis data.

---

## Raw Dataset link
Dataset yang digunakan dalam proyek ini diperoleh dari Kaggle: [google-playstore-user-reviews](https://www.kaggle.com/datasets/rowemorehouse/googleplaystoreuserreviews). Dataset ini menyajikan kumpulan ulasan pengguna dari berbagai aplikasi yang tersedia di platform Google Play. Setiap baris dalam dataset merepresentasikan satu ulasan yang ditinggalkan oleh pengguna terhadap suatu aplikasi.

---

## Insight & Findings
Dengan melakukan Analisis Sentimen pada review google play store dengan menggunakan IBM Granite, proyek ini berhasil mengungkap insight yang lebih dalam dari sekadar label sentimen biasa. Setiap ulasan pengguna tidak hanya diklasifikasikan, tetapi juga dianalisis berdasarkan emosi yang terkandung serta nilai kegunaannya bagi pengembangan aplikasi. Berikut temuan utama:

### 1. Klasifikasi Sentimen 
Model Granite berhasil menangkap nuansa yang sering kali terlewat oleh sistem label bawaan. Misalnya:

- Ulasan yang diberi label Netral ternyata mengandung keluhan serius yang disampaikan secara sopan.

- Ulasan yang terdengar positif di awal, namun berisi kritik tajam di bagian akhir, berhasil diklasifikasikan ulang sebagai Negatif.

 Insight: Model mampu mendeteksi ambiguitas dalam struktur ulasan, menghasilkan klasifikasi yang lebih manusiawi dan kontekstual.

 ### 2. Deteksi Emosi Dalam Analisis Sentimen
 Untuk mengeksplorasi lebih jauh dan mendalam untuk menyempurnakan analisis sentimen pada proyek ini, dilakukan prompt tambahan untuk mendeteksi emosi, diperoleh variasi ekspresi seperti:
 - Frustrated, disappointed, confused, hingga grateful.

- Emosi negatif dominan pada aplikasi dengan bug, iklan berlebihan, atau update merugikan.

- Emosi positif muncul pada aplikasi review makanan.

 Insight: Pengguna tidak hanya “tidak puas”, mereka frustrasi karena bug atau kecewa karena fitur berbayar. Ini memperkaya analisis beyond positive–negative.

 ### 3. Ulasan Bernilai Tidak Selalu Berbintang Tinggi
 Prompt untuk mengukur kegunaan ulasan bagi developer menunjukkan bahwa:

- Banyak ulasan positif yang hanya berisi pujian singkat seperti “Great app!” dinilai tidak berguna.

- Sebaliknya, ulasan negatif yang menjelaskan masalah secara detail (misal: "fitur crash saat klik tombol A") dianggap sangat berguna.

 Insight: Dengan prompt yang fokus pada kegunaan praktis, model dapat membantu menyaring ulasan prioritas tinggi untuk tim pengembang

 ### 4. Granite Mendeteksi Kritik Terselubung
Beberapa ulasan yang secara eksplisit terlihat netral, ternyata setelah dianalisis oleh Granite mengandung:

- Kritik halus (“Unfortunately it's been slow lately”)

- Saran tersembunyi (“Maybe it would be better if there was a backup feature”)

 Insight: Kemampuan membaca antara baris membuat AI cocok dijadikan asisten analitik real-time untuk pengambilan keputusan produk.

 ### 5. Visualisasi Sentimen & Emosi Mengungkap Tren Produk
Hasil akhir dari LangChain Agent menunjukkan distribusi:

- Sentimen: Positif masih dominan, tetapi emosi negatif meningkat pada update tertentu.

- Grafik batang sentimen membantu mengidentifikasi aplikasi yang perlu perhatian khusus.Bila ditambah pie chart emosi, bisa diketahui aplikasi mana yang menimbulkan frustrasi tertinggi.

 Insight: Gabungan analisis AI + visualisasi menghasilkan representasi user experience yang lebih utuh.

 ---

 ## AI Support Explanation
  Dalam proyek ini, model IBM Granite 3.3-8B Instruct digunakan sebagai asisten analitik berbasis AI untuk memahami ulasan pengguna aplikasi di Google Play Store. AI ini tidak hanya mengklasifikasikan sentimen, tetapi juga mendeteksi emosi dan menilai seberapa berguna ulasan bagi pengembang. Dengan bantuan prompt yang dirancang khusus, Granite mampu memberikan hasil yang disertai alasan logis, bukan sekadar label. Integrasi dengan LangChain Agent juga memungkinkan AI menjawab pertanyaan berbasis data secara langsung, seperti menghitung jumlah ulasan negatif atau membuat visualisasi distribusi sentimen. Peran AI ini terbukti efektif dalam menyaring ulasan penting, mempercepat proses analisis, dan membantu pengambilan keputusan produk yang lebih tepat sasaran.
