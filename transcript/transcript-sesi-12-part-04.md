| Abstrak                                                                                       |
| --------------------------------------------------------------------------------------------- |
| Rancangan video modul 4 mengenai "Internal Process MongoDB: Oplog, Replication, dan Sharding" |
|                                                                                               |

|            |                                                                     |           |                 |
| ---------- | ------------------------------------------------------------------- | --------- | --------------- |
| Title      | Memahami Internal Process MongoDB: Oplog, Replication, dan Sharding | Budget    |                 |
| Subject    |                                                                     | Publisher |                 |
| Status     |                                                                     | Director  | Al Muhdil Karim |
| Production |                                                                     | Release   |                 |
| Channel    |                                                                     | Platform  | youtube.com     |
| Team       | Ibnu Dzaky Solihin, Gibran zizzami, Irfansyah                       | Partner   |                 |
|            |                                                                     |           |                 |

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

| Timeline      | Concern         | Narator | Footage | prompt                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| ------------- | --------------- | ------- | ------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 00:00 – 01:00 | Pembukaan video | Host    |         | Di era digital saat ini, kebutuhan akan sistem basis data yang andal, skalabel, dan tangguh semakin meningkat. MongoDB sebagai salah satu database NoSQL terpopuler, menawarkan sejumlah mekanisme internal yang menjamin replikasi data, pemrosesan paralel, serta ketersediaan tinggi.  <br>Dalam video ini, kita akan membahas tiga komponen penting dalam internal process MongoDB, yaitu: **Oplog**, **Replication**, dan **Sharding**. |
|               |                 |         |         |                                                                                                                                                                                                                                                                                                                                                                                                                                              |

| Title |
| ----- |
|       |

| Timeline    | Concern                              | Narator | Footage                                               | prompt                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| ----------- | ------------------------------------ | ------- | ----------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 1:00 - 2:00 | indexing                             | Host    | Host inframe menjelaskan mengenai indexing            | Mari kita mulai dari Oplog, atau Operations Log.<br>Oplog merupakan sebuah log sirkular yang menyimpan catatan semua operasi penulisan yang terjadi dalam replika utama atau primary node.<br><br>Oplog digunakan dalam sistem replika untuk memastikan bahwa semua secondary node menerima dan mengeksekusi perintah yang sama seperti primary.<br><br>Setiap operasi seperti insert, update, dan delete dicatat dalam urutan waktu.<br><br>Node-node lain dalam replika set akan membaca Oplog dari primary dan mereplikasi operasinya secara asinkron, sehingga menjaga konsistensi data antar node.<br><br>Contoh sederhananya, jika sebuah dokumen ditambahkan ke database di primary node, maka informasi penambahan tersebut akan dicatat di Oplog. Secondary node kemudian mengeksekusi perintah yang sama berdasarkan Oplog tersebut.<br><br>Keunggulan Oplog adalah memungkinkan proses replikasi menjadi efisien dan tidak memerlukan re-sinkronisasi penuh setiap saat.                                                                                                                                                                                                              |
| 2:00 - 5:00 | penjelasan Memory Management MongoDB | Host    | Host inframe menjelaskan Memory Management MongoDB    | Replication dalam MongoDB dilakukan melalui apa yang disebut Replica Set.<br>Replica set adalah sekelompok server MongoDB yang menyimpan data yang sama, dengan satu node berperan sebagai primary, dan sisanya sebagai secondary.<br><br>Primary node adalah tempat utama semua operasi tulis dilakukan.<br><br>Secondary node akan mereplikasi data dari primary secara real-time menggunakan Oplog.<br><br>Manfaat dari replikasi adalah:<br><br>High Availability: Jika primary node gagal, salah satu secondary dapat secara otomatis dipilih menjadi primary baru melalui proses election.<br><br>Data Redundancy: Salinan data disimpan di beberapa server, mengurangi risiko kehilangan data.<br><br>Load Distribution: Operasi baca (read) dapat diarahkan ke secondary node untuk mengurangi beban di primary.<br><br>Proses replikasi ini memungkinkan sistem MongoDB tetap berfungsi walaupun terjadi kegagalan pada salah satu node.<br><br>MongoDB juga memungkinkan pengaturan prioritas node, delay pada replikasi, serta penggunaan read preference untuk optimasi performa.                                                                                                    |
| 5:00 - 8:00 | Buffer Pool & WiredTiger             | Host    | Host inframe dan menjelaskan Buffer Pool & WiredTiger | Sharding adalah teknik partisi data horizontal yang digunakan MongoDB untuk mengelola koleksi data yang sangat besar.<br>Dengan sharding, data dibagi ke dalam beberapa bagian yang disebut shard, dan setiap shard disimpan di server yang berbeda.<br><br>Komponen utama dalam sistem sharding MongoDB adalah:<br><br>Shard: Tempat penyimpanan data yang dibagi berdasarkan shard key.<br><br>Config Server: Menyimpan metadata mengenai distribusi data antar shard.<br><br>Query Router (mongos): Meneruskan permintaan aplikasi ke shard yang sesuai.<br><br>Keuntungan dari sharding:<br><br>Scalability: Dapat menangani volume data dan trafik yang besar dengan menambah shard baru.<br><br>Performance: Membagi beban kerja antar server, mempercepat query dan penulisan.<br><br>Fault Tolerance: Jika satu shard mengalami gangguan, shard lain tetap bisa diakses.<br><br>Sharding sangat berguna saat kita bekerja dengan big data atau aplikasi yang memiliki pertumbuhan data sangat cepat.<br><br>Namun, perlu diperhatikan bahwa pemilihan shard key yang tepat sangat penting. Shard key yang buruk bisa menyebabkan data tidak tersebar merata atau menciptakan bottleneck. |





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

| Timeline    | Concern | Narator | Footage                        | prompt                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| ----------- | ------- | ------- | ------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 8:00 - 9:00 | Penutup | Host    | Host inframe dan menutup video | kita telah membahas tiga komponen internal penting dalam MongoDB:<br><br>Oplog yang menjadi dasar untuk replikasi data,<br><br>Replication yang memastikan ketersediaan dan konsistensi data antar node,<br><br>serta Sharding sebagai solusi untuk skala besar dan performa tinggi.<br><br>Dengan memahami proses internal ini, kita dapat memanfaatkan MongoDB secara optimal, membangun sistem yang tidak hanya handal tetapi juga scalable dan efisien.<br><br>Terima kasih telah menyaksikan.<br>Jangan lupa like dan subscribe untuk konten teknologi lainnya. |
