# Analisis Permasalahan dan Solusi Setiap Layanan Transjakarta
## Latar Belakang
TransJakarta adalah sebuah sistem transportasi Bus Rapid Transit (BRT) pertama di Asia Tenggara dan Selatan dengan jalur lintasan terpanjang di dunia (208 km). Sistem BRT ini didesain berdasarkan sistem TransMilenio di Bogota, Kolombia. Terhitung sejak 1 Februari 2004, TransJakarta resmi beroperasi. Transjakarta tidak luput darai permasalahan, terdapat beberapa laporan dan permasalaha terkait kinerja layanan tranportasi umum ini. Oleh karena itu dibutuhkan analisis untuk mencarikan solusi dari setiap permasalahan yang ada. T
## Permasalahan Transjakarta
Transjakarta terbagi menjadi beberapa layanan,seperti: layanan wisata,layanan angkut,layanan BRT, layanan mikrotrans dan layanan royaltrans. Analisis setiap layanan dibedakanan karena terdapat beberapa kebijakan yang berbeda antar layanan.
1. Keterbatasan [Armada](https://validnews.id/nasional/transjakarta-jelaskan-kondisi-armada-busC)
2. Pelecehan seksual,yang korbannya mayoritas adalah [perempuan](https://komnasperempuan.go.id/kabar-perempuan-detail/pastikan-keamanan-perempuan-di-transportasi-publik-komnas-perempuan-dan-transjakarta-bahas-pencegahan-hingga-penanganan-kekerasan-seksual#:~:text=Iwan%20Samariansyah%20menambahkan%20bahwa%20hingga,yang%20mayoritas%20korbannya%20penumpang%20perempuan.)
3. Antian panjang saat melakukan tapIn dan [tapOut](https://www.tempo.co/arsip/sistem-tap-in-dan-tap-out-transjakarta-sempat-bermasalah-ini-cara-mengadu-ke-ylki-274581)
4. [Aksesibilitas](https://www.geriatri.id/artikel/2212/lansia-gratis-naik-transjakarta-ini-cara-mudah-daftarnya) yang kurang ramah bagi lansia 
5. Waktu tunggu dan perjalanan menjadi lebih [lama](https://kumparan.com/kumparannews/13-tahun-balada-armada-transjakarta) ketika jam sibuk
6. Beberapa penumpang mendapatkan layanan gratis walau tidak menaiki mikrotran ataupun bis wisata
## Dataset Transjakarta
1.	transID: ID transaksi unik untuk setiap transaksi
2.	payCardID: Kartu yang digunakan pelanggan sebagai tiket masuk dan keluar.
3.	payCardBank: Nama bank penerbit kartu pelanggan
4.	payCardName: Nama pelanggan yang tercantum dalam kartu.
5.	payCardSex: Jenis kelamin pelanggan yang tercantum dalam kartu
6.	payCardBirthDate: Tahun lahir pelanggan
7.	corridorID: ID koridor / ID rute sebagai kunci untuk pengelompokan rute.
8.	corridorName: Nama koridor / Nama rute berisi awal dan akhir untuk setiap rute.
9.	arah: 0 untuk Pergi, 1 untuk Kembali. Arah rute. 
10.	tapInStops: ID perhentian Tap In (pintu masuk) untuk mengidentifikasi nama perhentian
11.	tapInStopsName: Nama perhentian Tap In (pintu masuk) tempat pelanggan melakukan tap in.
12.	tapInStopsLat: Lintang Perhentian Tap In
13.	tapInStopsLon: Bujur Perhentian Tap In
14.	stopStartSeq: Urutan perhentian, perhentian pertama, perhentian kedua, dst. Terkait dengan arah.
15.	tapInTime: Tanggal dan waktu Tap In(masuk)
16.	tapOutStops: ID Perhentian Tap Out (Keluar) untuk mengidentifikasi nama perhentian
17.	tapOutStopsName: Nama perhentian Tap out (keluar) tempat pelanggan melakukan tap out.
18.	tapOutStopsLat: Lintang perhentian Tap Out
19.	tapOutStopsLon: Bujur perhentian Tap Out
20.	stopEndSeq: Urutan perhentian, perhentian pertama, perhentian kedua, dst. Terkait dengan arah.
21.	tapOutTime: Tanggal dan waktu Tap Out
22.	payAmount: Jumlah yang dibayarkan pelanggan. Sebagian gratis dan sebagian tidak.

