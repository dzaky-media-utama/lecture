| Abstrak                                              |
| ---------------------------------------------------- |
| Rancangan video modul 4 mengenai "instalasi mariaDB" |

|            |                                               |           |                 |
| ---------- | --------------------------------------------- | --------- | --------------- |
| Title      | Tutorial instalasi mariaDb                    | Budget    |                 |
| Subject    |                                               | Publisher |                 |
| Status     |                                               | Director  | Al Muhdil Karim |
| Production |                                               | Release   |                 |
| Channel    |                                               | Platform  | youtube.com     |
| Team       | Ibnu Dzaky Solihin, Gibran zizzami, Irfansyah | Partner   |                 |
|            |                                               |           |                 |

# Source

| No  | Access Time | Publisher | Link |
| --- | ----------- | --------- | ---- |
|     |             |           |      |
|     |             |           |      |

# Concept

| No  | Description                              |
| --- | ---------------------------------------- |
| 1   | Tutorial Instalasi mariaDB<br><br>konten |
| 2   | Disajikan dalam narasi presentasi        |


# Transcript

| Intro |
| ----- |
|       |

| Timeline      | Concern         | Narator | Footage | prompt                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| ------------- | --------------- | ------- | ------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 00:00 – 01:00 | Pembukaan video | Host    |         | Dalam pengelolaan data, sering kali kita fokus pada bagaimana data ditampilkan atau dikueri. Namun, di balik semua itu, ada proses kompleks yang bekerja secara diam-diam — mulai dari bagaimana data disimpan di disk, bagaimana ia diindeks, hingga bagaimana integritasnya dijaga.  <br>Semua hal ini dikendalikan oleh komponen yang disebut _storage engine_.  <br>Setiap storage engine memiliki cara unik dalam mengelola file, tabel, dan indeks.  <br>Memahami struktur internal ini bukan hanya penting untuk efisiensi, tetapi juga untuk skalabilitas dan keandalan sistem.<br> <br>Hari ini, kita akan membahas salah satu aspek fundamental dalam sistem manajemen basis data, namun sering kali tersembunyi dari perhatian: yaitu _Storage Engine_ dan _Struktur File Internal_. |
|               |                 |         |         |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |

| Title |
| ----- |
|       |

| Timeline      | Concern                                   | Narator | Footage                                                               | prompt                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| ------------- | ----------------------------------------- | ------- | --------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 01:00 – 02:30 | Pengenalan storage engiine                | Host    | Host inframe menjelaskan apa itu storage engine                       | **Storage Engine** adalah komponen inti dalam sistem basis data yang bertanggung jawab untuk menyimpan data ke dalam disk dan mengatur bagaimana data tersebut diambil kembali.<br><br>Dalam MongoDB, Storage Engine bekerja sebagai fondasi yang menentukan **performa, efisiensi penyimpanan, dan manajemen transaksi**. MongoDB sendiri mendukung lebih dari satu jenis storage engine, namun yang paling umum digunakan adalah **WiredTiger**.<br><br>Storage Engine berperan seperti jantung dalam tubuh manusia—mungkin tidak terlihat oleh pengguna, tetapi vital dalam menjaga sistem tetap hidup dan efisien.                                                                                                                                                                                                                                                                                                                                          |
| 02:30 – 04:30 | penjelasan wired tiger                    | Host    | Host inframe menjelaskan WiredTiger: Storage Engine Utama MongoDB     | **WiredTiger** merupakan storage engine default sejak MongoDB versi 3.2. Engine ini membawa banyak keunggulan dibandingkan pendahulunya, seperti:<br><br>- **Kompresi data** untuk efisiensi ruang penyimpanan.<br>    <br>- **Concurrency control** menggunakan Multi-Version Concurrency Control (MVCC), yang memungkinkan banyak operasi berjalan secara bersamaan tanpa konflik.<br>    <br>- **Journaling** untuk memastikan konsistensi data jika terjadi crash sistem.<br>    <br><br>Secara internal, WiredTiger menyimpan data dalam bentuk **B-Tree** dan **checkpoint-based snapshot**, yang membuat operasi baca dan tulis menjadi sangat efisien.  <br>Selain itu, dukungan untuk **document-level locking** memberikan fleksibilitas yang luar biasa dalam menangani transaksi berskala besar.                                                                                                                                                    |
| 04:30 – 06:30 | pengenalan Struktur File Internal MongoDB | Host    | Host inframe dan menjelaskan Struktur File Internal MongoDB           | Ketika MongoDB dijalankan, berbagai jenis file akan muncul di direktori data-nya. Masing-masing memiliki fungsi spesifik:<br><br>1. **.wt Files**  <br>    File ini menyimpan koleksi dan indeks. Ekstensi `.wt` menunjukkan bahwa data dikelola oleh WiredTiger. Misalnya, `collection-0--123456789.wt` adalah file untuk sebuah koleksi.<br>    <br>2. **WiredTiger.wt**  <br>    Merupakan file metadata yang menyimpan konfigurasi global dari WiredTiger.<br>    <br>3. **Journal Files**  <br>    Folder `journal/` menyimpan log transaksi yang membantu pemulihan data saat terjadi kegagalan sistem.<br>    <br>4. **Diagnostic Data**  <br>    Folder `diagnostic.data` berisi statistik dan informasi performa yang diambil secara berkala oleh MongoDB. Ini sangat membantu dalam proses **tuning dan monitoring** sistem.<br>    <br><br>Melalui struktur ini, MongoDB memastikan data tetap aman, cepat diakses, dan terorganisir secara efisien. |
| 06:30 – 08:00 | Perbandingan dengan MMAPv1                | Host    | Host inframe dan menjelaskan Perbandingan wiredtiger dengan MMAPv1    | Sebelum WiredTiger, MongoDB menggunakan storage engine bernama **MMAPv1**. Namun, MMAPv1 memiliki keterbatasan seperti **collection-level locking** dan **tidak mendukung kompresi**.<br><br>WiredTiger hadir sebagai solusi yang lebih modern, mengurangi konflik akses dan meningkatkan efisiensi penyimpanan.<br><br>Dengan pemilihan engine yang tepat, arsitektur database bisa disesuaikan untuk mencapai performa maksimal.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| 08:00 – 09:30 | Implikasi Arsitektural & Best Practice    | Host    | Host inframe dan  menjelaskan  Implikasi Arsitektural & Best Practice | Pemahaman terhadap storage engine dan struktur file internal sangat penting, terutama bagi:<br><br>- **Administrator sistem**, untuk optimasi penyimpanan dan pemulihan data.<br>    <br>- **Developer backend**, agar query dan desain koleksi selaras dengan performa disk.<br>    <br>- **DevOps**, dalam konteks tuning cache, pemantauan file journal, serta backup.<br>    <br><br>Beberapa **best practice** yang perlu diperhatikan:<br><br>- Gunakan **kompresi** yang sesuai jika menangani data besar.<br>    <br>- Monitor penggunaan disk secara berkala.<br>    <br>- Jangan abaikan file journal—itulah pelindung utama data saat sistem gagal.                                                                                                                                                                                                                                                                                                  |




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

| Timeline  | Concern | Narator | Footage                        | prompt                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| --------- | ------- | ------- | ------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 8:30–9:00 | Penutup | Host    | Host inframe dan menutup video | MongoDB tidak hanya unggul dalam fleksibilitas data, tetapi juga dalam arsitektur penyimpanan yang canggih.  <br>Dengan mengenal lebih dalam tentang **Storage Engine dan Struktur File Internal**, kita tidak hanya memahami bagaimana data tersimpan, tapi juga bagaimana membangun sistem yang **stabil, efisien, dan dapat diskalakan**.<br><br>Terima kasih telah menyimak.  <br>Mari terus menjelajah ke dalam dunia database yang penuh kemungkinan.  <br>Sampai jumpa di video berikutnya. |
