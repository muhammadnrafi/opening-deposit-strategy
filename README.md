# Bank Marketing Campaign: Opening Deposit Strategy
### Preprared by Muhammad Naufal Rafi

# Problem Statement

Marketing Campaigns Bank biasa dilakukan untuk meningkatkan engagement customer / nasabah. Banyak cara yang dilakukan bank dalam marketing campaigns salah satu cara nya adalah dengan menghubungi calon nasabah via telepon seperti dataset yang kita gunakan pada projek kali ini. Permasalahan utamanya adalah bagaimana bank dapat secara efektif menetukan target customer / nasabah yang berpotensi untuk membuka akun, meminjam kredit atau menggunakan jasa keuangan lainnya namun tetap meminimalisir biaya yang dikeluarkan selama marketing campagings dan menghasilkan return on investment yang baik.

# Goals

Seperti yang sudah disampaikan pada diatas, maka tujuan dari projek ini adalah untuk menghasilkan marketing campaigns yang efektif dengan cara menganalisa calon customer / nasabah. Sehingga dengan projek ini diharapkan mampu memprediksi apakah calon pelanggan akan tertarik atau tidak dari marketing campaigns ini, selain itu projek ini juga dapat membantu bank untuk memantau atau mengukur kinerja marketing campaigns secara real-time dan memberikan saran untuk perbaikan.

# Analytical Approach

Jadi pada projek ini akan membangun sebuah model klasifikasi yang mampu membedakan pelanggan yang berpotensi tertarik pada campaign ini atau tidak.

**Metrics Evaluation:**  
Sehingga dengan demikian metriks evaluasi yang akan digunakan adalah ROC AUC untuk membedakan kelas positif dan kelas negatif dengan baik sehingga dapat meminmalisisr kerugian yang terjadi pada marketing campaigns.

# Data Description
1.  `age` (numerik)
2.  `job`: jenis pekerjaan (kategori: 'admin.','blue-collar','entrepreneur','housemaid','management','retired','self-employed','services','student','technician','unemployed','unknown')
3.  `marital`: status pernikahan (kategori: 'divorced','married','single','unknown'; catatan: 'divorced' berarti bercerai atau duda/janda)
4.  `education` (kategori: 'basic.4y','basic.6y','basic.9y','high.school','illiterate','professional.course','university.degree','unknown')
5.  default: apakah memiliki kredit yang gagal? (kategori: 'no','yes','unknown')
6.  housing: apakah memiliki pinjaman rumah? (kategori: 'no','yes','unknown')
7.  loan: apakah memiliki pinjaman pribadi? (kategori: 'no','yes','unknown')
8.  `contact`: jenis komunikasi kontak (kategori: 'cellular','telephone')
9.  `month`: bulan terakhir kontak dalam setahun (kategori: 'jan', 'feb', 'mar', ..., 'nov', 'dec')
10.  `day_of_week`: hari terakhir kontak dalam seminggu (kategori: 'mon','tue','wed','thu','fri')
11.  `duration`: durasi kontak terakhir, dalam detik (numerik). Catatan penting: atribut ini sangat memengaruhi target output (misalnya, jika durasi = 0 maka y = 'no'). Namun, durasi tidak diketahui sebelum panggilan dilakukan. Selain itu, setelah akhir panggilan, y jelas diketahui. Oleh karena itu, input ini hanya harus dimasukkan untuk tujuan benchmark dan harus dihapus jika niatnya adalah memiliki model prediksi yang realistis.
12.  `campaign`: jumlah kontak yang dilakukan selama kampanye ini dan untuk klien ini (numerik, termasuk kontak terakhir)
13.  `pdays`: jumlah hari yang berlalu setelah klien terakhir kali dihubungi dari kampanye sebelumnya (numerik; 999 berarti klien sebelumnya tidak dihubungi)
14.  `previous`: jumlah kontak yang dilakukan sebelum kampanye ini dan untuk klien ini (numerik)
15.  `poutcome`: hasil dari kampanye pemasaran sebelumnya (kategori: 'failure','nonexistent','success')
16.  `emp.var.rate`: tingkat variasi pekerjaan - indikator triwulanan (numerik)
17.  `cons.price.idx`: indeks harga konsumen - indikator bulanan (numerik)
18.  `cons.conf.idx`: indeks keyakinan konsumen - indikator bulanan (numerik)
19.  `euribor3m`: tingkat euribor 3 bulan - indikator harian (numerik)
20.  `nr.employed`: jumlah karyawan - indikator triwulanan (numerik)
21.  `y` - apakah klien berlangganan deposito jangka panjang? (biner: 'yes','no')

Source: https://www.kaggle.com/datasets/volodymyrgavrysh/bank-marketing-campaigns-dataset
