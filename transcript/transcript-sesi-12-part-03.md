| Abstrak                                                                         |
| ------------------------------------------------------------------------------- |
| Rancangan video modul 4 mengenai "Indexing, Memory Management, dan Buffer Pool" |
|                                                                                 |

|            |                                               |           |                 |
| ---------- | --------------------------------------------- | --------- | --------------- |
| Title      | Indexing, Memory Management, dan Buffer Pool  | Budget    |                 |
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

| No  | Description                                                |
| --- | ---------------------------------------------------------- |
| 1   | Indexing, Memory Management, dan Buffer Pool<br><br>konten |
| 2   | Disajikan dalam narasi presentasi                          |


# Transcript

| Intro |
| ----- |
|       |

| Timeline      | Concern         | Narator | Footage | prompt                                                                                                                                                                                                                                                                                                                                                                                       |
| ------------- | --------------- | ------- | ------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 00:00 – 01:00 | Pembukaan video | Host    |         | Pernahkah kalian bertanya-tanya bagaimana MongoDB bisa menangani jutaan dokumen dengan kecepatan tinggi?  <br>Jawabannya ada pada tiga komponen penting: **Indexing, Memory Management, dan Buffer Pool**.<br><br>Di video ini, kita akan kupas tuntas bagaimana ketiganya bekerja di balik layar untuk memberikan performa yang optimal pada sistem basis data MongoDB.<br><br><br><br><br> |
|               |                 |         |         |                                                                                                                                                                                                                                                                                                                                                                                              |

| Title |
| ----- |
|       |

| Timeline    | Concern                              | Narator | Footage                                               | prompt                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| ----------- | ------------------------------------ | ------- | ----------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 1:00 - 4:00 | indexing                             | Host    | Host inframe menjelaskan mengenai indexing            | Index adalah struktur data khusus yang meningkatkan kecepatan operasi pencarian pada MongoDB.<br>Tanpa index, MongoDB harus melakukan collection scan, yaitu membaca seluruh dokumen satu per satu. Ini sangat tidak efisien.<br><br>MongoDB menyediakan berbagai jenis index, di antaranya:<br><br>- Single Field Index<br>- Compound Index<br>- Multikey Index untuk array<br>- Text Index untuk pencarian full-text<br>- Dan Geospatial Index untuk data lokasi.<br><br>Misalnya, jika kita memiliki koleksi produk dan sering mencari berdasarkan kategori, maka membuat index di field kategori akan sangat meningkatkan performa.<br><br>Index di MongoDB disimpan dalam struktur B-Tree, yang membuat pencarian, penyisipan, dan penghapusan data menjadi lebih cepat dan efisien.<br><br>Namun, perlu diingat: semakin banyak index, semakin besar juga penggunaan memori dan overhead saat insert atau update.<br>Oleh karena itu, gunakan index secara bijak sesuai kebutuhan query.                           |
| 4:00 - 7:00 | penjelasan Memory Management MongoDB | Host    | Host inframe menjelaskan Memory Management MongoDB    | MongoDB memanfaatkan Virtual Memory dan Memory-Mapped Files melalui sistem operasi.<br>Ini artinya, MongoDB menyerahkan sebagian besar manajemen memori ke OS, namun tetap memiliki logika internal untuk caching data dan index secara efisien.<br><br>MongoDB menggunakan RAM sebagai Working Set—yaitu kumpulan data dan index yang sering diakses.<br>Jika data tersebut ada di memori, query akan sangat cepat. Tapi jika tidak, MongoDB harus mengambilnya dari disk, yang jauh lebih lambat.<br><br>Untuk memaksimalkan performa, kita perlu memperhatikan hal-hal berikut:<br><br>Pastikan ukuran RAM cukup besar untuk menampung working set.<br><br>Optimalkan index agar query tidak membaca data berlebihan.<br><br>Gunakan profiling dan monitoring tools seperti mongostat dan mongotop untuk memantau penggunaan memori.<br><br>MongoDB juga mendukung konfigurasi wiredTigerCacheSizeGB untuk mengatur berapa banyak RAM yang digunakan oleh engine WiredTiger, storage engine default MongoDB saat ini. |
| 7:00 - 9:00 | Buffer Pool & WiredTiger             | Host    | Host inframe dan menjelaskan Buffer Pool & WiredTiger | Di balik manajemen memori MongoDB, ada Buffer Pool dari storage engine WiredTiger.<br>Buffer pool adalah area di RAM yang digunakan untuk menyimpan halaman data dari disk yang sedang atau akan digunakan.<br><br>Ketika query dijalankan, WiredTiger akan mencoba mengambil data dari buffer pool terlebih dahulu. Jika tidak ada, maka akan terjadi page fault, dan data harus diambil dari disk.<br><br>WiredTiger menggunakan algoritma Least Recently Used (LRU) untuk mengelola buffer pool.<br>Hal ini memastikan data yang paling sering digunakan tetap ada di memori, sementara data yang jarang diakses akan digantikan.<br><br>Beberapa fitur penting buffer pool:<br><br>Menyediakan caching untuk mempercepat query.<br><br>Menyimpan data yang dimodifikasi (dirty pages) sebelum ditulis ke disk.<br><br>Mengurangi jumlah I/O langsung ke disk.<br><br>Dengan pengelolaan buffer pool yang efisien, MongoDB mampu meminimalkan latensi dan meningkatkan throughput.                                    |





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

| Timeline     | Concern | Narator | Footage                        | prompt                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| ------------ | ------- | ------- | ------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 9:00 - 10:00 | Penutup | Host    | Host inframe dan menutup video | Jadi, dapat kita simpulkan bahwa:<br><br>Indexing mempercepat query dan harus disesuaikan dengan pola pencarian.<br><br>Memory Management memungkinkan MongoDB bekerja cepat dengan data yang sering digunakan.<br><br>Buffer Pool dari WiredTiger bertugas menjaga performa agar tetap tinggi dan stabil.<br><br>Ketiganya bekerja bersama untuk menciptakan sistem database yang efisien dan scalable.<br>Jika kalian ingin MongoDB kalian bekerja maksimal, pahami dan optimalkan ketiga komponen ini.<br><br>Terima kasih sudah menonton.<br>Jangan lupa untuk like, subscribe, dan aktifkan lonceng notifikasi agar tidak ketinggalan video menarik lainnya seputar teknologi dan basis data.<br>Sampai jumpa di video berikutnya! |
