| Abstrak                                                                 |
| ----------------------------------------------------------------------- |
| Rancangan modul 1 mengenai "Pemahaman mengenai konsep dasar dari RDBMS" |

|            |                                            |           |                    |
| ---------- | ------------------------------------------ | --------- | ------------------ |
| Title      | Pemahaman mengenai konsep dasar dari RDBMS | Budget    |                    |
| Subject    |                                            | Publisher |                    |
| Status     |                                            | Director  | Ibnu Dzaky Solihin |
| Production |                                            | Release   |                    |
| Channel    |                                            | Platform  | yuros.org          |
| Team       | Al Muhdil Karim                            | Partner   |                    |
|            |                                            |           |                    |

# Source

| No  | Access Time | Publisher | Link |
| --- | ----------- | --------- | ---- |
|     |             |           |      |
|     |             |           |      |

# Concept

| No  | Description                                              |
| --- | -------------------------------------------------------- |
| 1   | Pemahaman mengenai konsep dasar dari RDBMS<br><br>konten |
| 2   | Disajikan dalam narasi presentasi                        |


# Transcript

| Intro |
| ----- |
|       |

| Timeline    | Concern         | Narator | Footage | prompt                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| ----------- | --------------- | ------- | ------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 00:00-00:45 | Pembukaan video | Host    |         | Saat ini data telah menjadi fondasi setiap keputusan penting, kemampuan untuk mengelola, menyimpan, dan mengakses informasi secara efisien bukan lagi pilihan—melainkan kebutuhan. data telah menjadi fondasi dari hampir seluruh aktivitas manusia—dari keputusan bisnis hingga kecerdasan buatan. Pernahkah Anda merasa kewalahan mengelola puluhan, bahkan ratusan file Excel yang tersebar di berbagai folder, perangkat, dan email?<br><br>Ketika satu file mengalami perubahan, file lainnya tak lagi sinkron. Redundansi data, kesalahan entri, dan sulitnya pelacakan informasi menjadi masalah yang semakin kompleks—dan menghambat pengambilan keputusan yang cepat dan akurat.<br><br>Di sinilah peran sistem manajemen basis data relasional, atau **RDBMS**, menjadi sangat relevan.  <br>RDBMS hadir bukan hanya untuk menyimpan data, tetapi untuk menata, menghubungkan, dan menjadikan data sebagai aset yang benar-benar dapat diandalkan. |
|             |                 |         |         |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |

| Title |
| ----- |
|       |

| Timeline      | Concern                             | Narator | Footage                                                                              | prompt                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| ------------- | ----------------------------------- | ------- | ------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 00:46-02:00   | Perkenalan materi                   | Host    | Host inframe menjelaskan apa itu RDBMS<br><br>[[database.mp4]]                       | Konsep pengelolaan basis data telah berkembang sejak dekade 1960-an, dimulai dengan model hirarkis dan model jaringan. Sistem seperti **IBM IMS** menjadi pelopor dalam menyimpan data secara elektronik.  <br>Namun, keterbatasan model tersebut dalam hal fleksibilitas dan relasi data mendorong pencarian pendekatan yang lebih efisien.<br><br>Pada tahun 1970, terobosan besar lahir dari seorang ilmuwan komputer bernama **Edgar F. Codd** yang memperkenalkan model relasional. Melalui makalah ilmiahnya yang revolusioner, Codd menyarankan agar data dikelola dalam bentuk tabel yang saling berelasi dan diakses melalui prinsip-prinsip matematika logis.                                                                                                |
| 02:01- 03:15  | Mengapa RDBMS Penting?              | Host    | [[relational.png]]<br><br>Host inframe dan menjelaskan pentingnya RDBMS              | Model relasional yang dikembangkan Codd didasarkan pada teori himpunan dan logika predikat. Inilah yang memungkinkan RDBMS untuk menjadi sistem yang tidak hanya efisien, tetapi juga memiliki dasar ilmiah yang kuat.<br><br>Untuk berinteraksi dengan data dalam sistem ini, dikembangkanlah **SQL**—sebuah bahasa yang kini menjadi standar internasional dalam manajemen data.  <br>Dengan SQL, pengguna dapat dengan mudah menuliskan perintah untuk mencari, menambahkan, memperbarui, dan menghapus data, semua dalam format yang terstruktur dan mudah dipahami.                                                                                                                                                                                               |
| 03:16 - 04:45 | Sejarah Perkembangan Basis Data     |         | Host inframe dan menjelaskan sejarah basis data<br><br>                              | MySQL dikembangkan pada tahun 1995 oleh **Michael Widenius** dan **David Axmark**, yang memiliki visi untuk menciptakan RDBMS yang tidak hanya kuat tetapi juga dapat diakses secara bebas oleh komunitas global.<br><br>Dengan lisensi open-source, MySQL dengan cepat diadopsi oleh para pengembang, terutama karena kemudahan penggunaan, performa yang handal, dan fleksibilitas dalam integrasi.<br><br>MySQL pun menjadi tulang punggung bagi banyak aplikasi web, dan menjadi bagian dari **LAMP stack**: Linux, Apache, MySQL, dan PHP/Perl/Python.                                                                                                                                                                                                            |
| 04:46-06:00   | Model Relasional Codd dan Peran SQL | Host    | <br><br>Host inframe dan menjelaskan model<br>relasional codd dan peran SQL<br><br>  | Pada tahun 2008, MySQL diakuisisi oleh **Sun Microsystems**, dan setahun kemudian, Sun sendiri diakuisisi oleh **Oracle Corporation**.  <br>Kondisi ini menimbulkan kekhawatiran terhadap keberlangsungan MySQL sebagai proyek open-source.<br><br>Menanggapi hal ini, Michael Widenius memprakarsai proyek baru bernama **MariaDB**—sebuah _fork_ dari MySQL yang mempertahankan prinsip keterbukaan dan transparansi.  <br>Namun demikian, MySQL tetap bertahan sebagai salah satu sistem manajemen basis data paling digunakan di dunia, didukung oleh komunitas serta perusahaan teknologi besar.                                                                                                                                                                  |
| 06:01 – 07:15 | Perkembangan Perangkat Lunak RDBMS  | Host    | <br>Host inframe dan menjelaskan mengenai perkembangan perangkat lunak RDBMS<br><br> | MySQL digunakan dalam berbagai sistem, mulai dari blog pribadi hingga layanan e-commerce multinasional.  <br>Platform seperti **WordPress**, **Drupal**, hingga **Magento** menggantungkan sistem databasenya pada MySQL.<br><br>Dengan dukungan fitur seperti clustering, replikasi, dan performa tinggi dalam pengambilan data, MySQL menjadi pilihan utama tidak hanya karena gratis, tetapi juga karena terbukti stabil dan scalable dalam berbagai lingkungan produksi.<br><br><br>                                                                                                                                                                                                                                                                               |
| 07:16 – 08:30 | Sejarah Singkat MySQL               | Host    | Host inframe dan menjelaskan sejarah MySQL                                           | Di tengah meningkatnya volume dan kompleksitas data, RDBMS hadir sebagai solusi yang unggul.  <br>Sebelum kemunculannya, data disimpan secara manual dalam file datar yang tidak memiliki hubungan struktural. Hal ini menyebabkan duplikasi data, inkonsistensi, dan kesulitan dalam pemrosesan informasi.<br><br>Dengan RDBMS, pengguna dapat menjaga integritas data, melakukan transaksi secara serentak, serta mengontrol hak akses dengan lebih akurat. Sistem ini juga menerapkan prinsip **ACID**—Atomicity, Consistency, Isolation, Durability—untuk memastikan setiap transaksi berjalan dengan aman dan dapat diandalkan.<br><br>                                                                                                                           |
| 08:31 – 09:30 | Akuisisi MySQL dan Lahirnya MariaDB | Host    | Host inframe dan menjelaskan lahirnya MariaDB                                        | Relational Database Management System—disingkat RDBMS—merupakan sistem perangkat lunak yang dirancang untuk menyimpan, mengelola, dan memanipulasi data yang terstruktur dalam bentuk relasi, atau yang lebih dikenal dengan tabel.<br><br>Setiap tabel terdiri atas baris dan kolom, di mana baris merepresentasikan record, dan kolom merepresentasikan atribut. Hubungan antar tabel diatur dengan presisi melalui konsep **primary key** dan **foreign key**, menjadikan RDBMS sebagai sistem yang tidak hanya efisien, tetapi juga konsisten dan logis dalam menyimpan informasi.<br><br>Bahasa utama yang digunakan untuk berinteraksi dengan sistem ini adalah **Structured Query Language**, atau SQL—bahasa universal dalam dunia basis data.<br><br><br><br> |
| 10:46 – 12:00 | Keunggulan RDBMS secara Umum        | Host    | Host inframe dan  menjelaskan keunggulan RDBMS                                       | RDBMS memiliki keunggulan yang sulit ditandingi sistem lainnya: kemampuan untuk menjaga integritas data melalui constraint, indexing untuk efisiensi pencarian, hingga pemisahan logika akses data melalui view.<br><br>Sistem ini juga mendukung kontrol akses berbasis peran, pencatatan aktivitas pengguna, dan perlindungan data dari kerusakan atau kehilangan.  <br>Lebih jauh lagi, RDBMS juga telah terintegrasi dengan teknologi analitik dan _business intelligence_, memungkinkan organisasi untuk mengambil keputusan yang berbasis data akurat dan real-time.<br><br><br><br><br>                                                                                                                                                                         |



| Problem |
| ------- |
|         |

| Timeline | Concern | Narator | Footage | prompt |
| -------- | ------- | ------- | ------- | ------ |
|          |         |         |         |        |
|          |         |         |         |        |

| Solution |
| -------- |
|          |

| Timeline | Concern | Narator | Footage | prompt |
| -------- | ------- | ------- | ------- | ------ |
|          |         |         |         |        |
|          |         |         |         |        |

| CTA |
| --- |
|     |

| Timeline      | Concern | Narator | Footage                                                        | prompt                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| ------------- | ------- | ------- | -------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 12:01 – 13:00 | Penutup | Host    | Host inframe dan memberikan kesimpulan sekaligus menutup video | Sebagai kesimpulan, Di balik kompleksitas dunia digital saat ini, keberadaan sistem manajemen basis data relasional menjadi fondasi yang tak tergantikan.  <br>Memahami bagaimana RDBMS bekerja bukan hanya soal teknis, tetapi juga tentang memahami bagaimana informasi dibentuk, dijaga, dan digunakan.<br> <br>Dari sejarahnya yang filosofis hingga implementasinya yang praktis, RDBMS—terutama MySQL—telah mengubah cara kita berinteraksi dengan data.  <br>Semoga pembahasan ini membuka cakrawala baru dalam memahami peran penting sistem basis data dalam membentuk peradaban digital.  <br>Terima kasih telah menyimak, dan sampai jumpa di materi pembelajaran berikutnya.<br><br><br><br><br> |



# Reference

### Intro

Ini adalah Babak 1 Anda yang membentuk beberapa detik pertama video Anda di mana Anda langsung membahas alasan mengapa seseorang ingin menonton video ini.

Tujuan dari intro Anda adalah untuk memenuhi janji dari judul video Anda sehingga pemirsa Anda merasa bahwa mereka membuat keputusan yang tepat untuk menonton video Anda. Anda ingin segera membuat mereka merasa nyaman sehingga mereka rileks dan ingin menonton sisa video Anda.

Contoh intro video:

Apakah Anda lelah karena tidak bisa menurunkan berat badan beberapa kilogram terakhir? Saya ingin menunjukkan kepada Anda metode tanpa olahraga untuk menurunkan berat badan 1-5 kilogram terakhir.
Anda ingin membuat lebih banyak video, tetapi Anda merasa kaku dan tidak alami saat berbicara di depan kamera. Saya mendengar Anda! Dalam video ini, kita akan membahas beberapa strategi sederhana untuk membantu Anda menjadi lebih santai dan menjadi diri Anda sendiri dalam video.
Dalam Intro Anda, Anda biasanya tidak ingin membahas tentang siapa Anda atau apa yang Anda lakukan. Sebaliknya, Anda ingin membuat semuanya tentang audiens Anda dan memberikan nilai di awal.

### Title

Untuk video YouTube, ini adalah titik di mana Anda menambahkan judul. Di sinilah biasanya branding Anda berjalan.

Urutan judul memberi tahu audiens Anda jenis acara yang mereka tonton dan tagline acara Anda. Untuk jenis video lainnya (Facebook Lives, Video Instagram, dll), Anda biasanya dapat melewati bagian ini.

### Frame the Problem

Ini adalah Babak 2 dan bagian dalam video Anda di mana Anda meningkatkan masalah dengan menambahkan konteksnya.

Bicarakan masalah yang akan Anda selesaikan dari berbagai sudut pandang untuk membantu pemirsa mendapatkan pemahaman yang lebih dalam tentang masalah tersebut. Diskusikan bagaimana masalah tersebut memengaruhi bisnis atau kehidupan mereka dan mengapa mereka menghadapi masalah ini. Dengan cara ini, Anda membangun antisipasi menuju klimaks sehingga mereka sangat menantikan solusi Anda.
Beberapa contoh teks pada titik ini:

"Mengapa begitu sulit untuk tampil alami di depan kamera?

Nah, Anda mungkin merasa sadar kamera karena beberapa alasan. Mungkin Anda menganggap kamera sebagai sebuah perangkat dan tidak melihat bahwa ada seseorang di ujung sana yang menonton video Anda.

Atau, mungkin Anda mencoba menjadi perfeksionis di depan kamera dan tersandung saat mencoba memenuhi apa yang Anda yakini sebagai ekspektasi masyarakat terhadap Anda. Atau, mungkin Anda memilih konten yang salah untuk ditampilkan di depan kamera, sehingga terkesan dipaksakan dan tidak wajar."

Membingkai masalah dengan cara ini memungkinkan Anda untuk membangun hubungan dan kepercayaan dengan audiens Anda.

### Solutions

Akhirnya tiba saatnya untuk memberikan jawaban dan resolusi Anda terhadap masalah pemirsa. Jika Anda dapat membuat resolusi Anda sesuai dengan langkah-langkah yang berurutan, biasanya lebih mudah untuk diikuti dalam video.

Jenis-jenis CTA Video:
10 Contoh Brilian
Selain itu, jika Anda dapat menunjukkan contoh praktis yang sesuai dengan setiap poin solusi, maka hal tersebut akan membantu audiens mengingat langkah-langkah Anda.

Sebagai contoh:

"Dengan beberapa penyesuaian sederhana, Anda bisa mulai tampil mengagumkan di depan kamera. Mari kita tingkatkan penampilan Anda di depan kamera dengan rutinitas 3 bagian yang sederhana ini:

Langkah 1: Bayangkan Anda sedang berbicara dengan seorang teman yang benar-benar perlu mendengar informasi yang Anda berikan.

Langkah 2: Ingatlah bahwa mencoba menjadi sempurna di depan kamera, justru akan membuat Anda terlihat kurang otentik. Jadi, akui saja kesalahan dan kebiasaan Anda dan bicaralah seperti yang Anda lakukan secara alami, tanpa ada kesalahan.

Langkah 3: Pastikan konten yang Anda sajikan di depan kamera adalah sesuatu yang sangat Anda minati dan dapat Anda bicarakan pada saat itu juga. Semangat selalu menghubungkan!"

### CTA

Untuk video, selalu merupakan ide yang bagus untuk menunjukkan kepada audiens Anda apa yang Anda ingin mereka lakukan selanjutnya. Di sinilah CTA Anda berperan. Rencanakan ajakan bertindak yang jelas, menarik, dan sesuai untuk setiap video.

Jika Anda mencari opini dan keterlibatan, mintalah orang untuk berkomentar dan berbagi. Jika Anda mencari prospek, minta orang untuk mengunduh dan berlangganan. Jika Anda mencari bukti sosial, mintalah orang untuk menyukai dan mengikuti.

Contoh CTA:

"Jika Anda ingin melatih kehadiran Anda di depan kamera, ikuti tantangan video saya selama 10 hari untuk membantu Anda menjadi seorang profesional dalam bidang video. Klik tautan dalam deskripsi untuk mendaftar!"

Setelah Anda menyampaikan nilai, ini adalah waktu Anda untuk "bertanya", jadi pastikan Anda menjelaskan dengan jelas apa yang Anda ingin audiens Anda lakukan selanjutnya!
