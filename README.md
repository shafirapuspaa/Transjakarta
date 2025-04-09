# Analisis Permasalahan dan Solusi Setiap Layanan Transjakarta
## Latar Belakang
TransJakarta adalah sebuah sistem transportasi Bus Rapid Transit (BRT) pertama di Asia Tenggara dan Selatan dengan jalur lintasan terpanjang di dunia (208 km). Sistem BRT ini didesain berdasarkan sistem TransMilenio di Bogota, Kolombia. Terhitung sejak 1 Februari 2004, TransJakarta resmi beroperasi. Transjakarta tidak luput darai permasalahan, terdapat beberapa laporan dan permasalaha terkait kinerja layanan tranportasi umum ini. Oleh karena itu dibutuhkan analisis untuk mencarikan solusi dari setiap permasalahan yang ada. 
## Roleplay
Sebagai seorang data analys diminta untuk memberikan solusi permasalahan transjakarta yang dibagi per layanan dengan melihat beberapa data seperti:
- Koridor, waktu, jenis pembayaran, kategori usia,jenis kelamin, dan lokasi tapIn/tapOut terpadat setiap layanannya
- Frekuensi setiap penumpang
- Analisis korelasi waktu perjalanan dengan jam sibuk penumpang
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
## Rekomendasi
1. Permasalahan keterbatasan armada dapat diatasi dengan menambahkan armada baru. Jika diasumsikan satu layanan hanya mendapatkan 1 armada baru koridor S21 (angkut), 1T (Royaltrans), BW9(Wisata), 2(BRT) lah yang layak mendapatkan armada karena pertimbangan jumlah penumpang yang menggunakan koridor tersebut
2. Kasus pelecehan cukup sering terjadi saat menggunakan transjakarta. Oleh karena itu, dibuatlah bus pink(bus khusus wanita). Bus ini hanya melewati 4 koridor, Koridor 3,13,2 dan 9. Namun, jumlah perempuan pada koridor 9 cukup sedikit sehingga adanya bus wanita dirasa kurang diperlukan. Jika bus koridor 9 diganti mungkin bisa menambahkan unit bus wanita pada koridor lain seperti koridor 13(BRT, sudah ada dalam list),B14(Royaltrans),JAK 112(Mikrotrans), BW9(wisata) dan 9D(Angkut) yang memiliki jumlah penumpang perempuan terbanyak setiap layananya.
3. Antrian panjang saat melakukan tapin dan tapout dapat disebabkan karena kurangnya gate akses kartu. Hal ini dapat diatasi dengan menambahkan gate, bila diasumsikan dapat membuat gate baru (hanya pada BRT) halte yang dipilih adalah halte taman mini untuk lokasi tapin dan halte BKN untuk lokasi tapout. 
- Bila igin melihat tren lokasi pemberhentian teramai setiap layanan bisa liat dilokasi penjaringam (angkut), ST MRT FAtmawati (royal trans), Kampung rambutan mikrotrans(mikrotrans),Pantai maju (wisata), bKN (BRT). Bila igin melihat tren lokasi mulai perjalanan teramai setiap layanan bisa liat dilokasi penjaringam (angkut), GBK1 (royal trans), RSUD Pesanggrahan (mikrotrans), IRTI Monas (wisata), garuda taman mini (BRT). 
4. Untuk meningkatkan aksesibilitas lansia di transjakarta, rekomendasi yang dapat diberikan dapat berupa pembuatan lift atau jalan landai yang dapat dilalui kursi roda. Jika diasumsikan dapat menambahkan fasilitas tersebut pada satu halte (BRT) pada masing masing layanan maka halte yang mendapatkan tambahan fasilitas tersebut adalah masjid agung.
5. Waktu perjalanan menjadi lebih lama ketika jam sibuk dapat dibuktikan benar. Menurut uji korelasi dan grafik scater menunjukan hal demikian. Hal ini dapat disebabkan karena padatnya armada pada jam-jam tersebut atau jalanan yang ramai sehingga waktu perjalanan menjadi semakin lama. Untuk menangani masalah tersebut dapat menambahkan unit transjakarta dan menghimbau masyarakat untuk memakai transportasi umum
6. Beberapa penumpang yang tidak menaiki layanan mikrotrans dan bus wisata memiliki payamount = 0, mengapa demikian? 
Hal ini dapat terjadi karena penumpang menggunakan paycard DKI. Terdapat aturan yang menjelaskan bahwa ada beberapa kriteria penumpang yang menggunakan paycard DKI tidak dikenakan biaya layanan. Dalam data terdapat 1400 penumpang yang memakai Paycard DKI dengan payamoun 0 walaupun bukan termasuk layanan mikrotrans dan wisata. Namun terdapat penumpang menggunakan paycard lain mendapatkan payamount 0 yang tidak seharusnya. Hal ini dapat terjadi karena beberapa kondisi tertentu yang belum dianalisis lebih lanjut.


