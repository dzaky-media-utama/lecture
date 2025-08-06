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

| Timeline  | Concern         | Narator | Footage | prompt                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| --------- | --------------- | ------- | ------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 0:00–0:45 | Pembukaan video | Host    |         | MariaDB merupakan sistem manajemen basis data relasional yang handal, bersifat open-source, dan digunakan secara luas dalam berbagai platform, mulai dari sistem lokal hingga layanan cloud.  <br>Melalui video ini, Anda akan mempelajari langkah-langkah instalasi dan konfigurasi awal MariaDB dengan pendekatan yang aman dan efisien.<br><br>Pada kesempatan ini, kita akan membahas bagaimana cara menginstal **MariaDB** di sistem operasi **Linux**.  <br> |
|           |                 |         |         |                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |

| Title |
| ----- |
|       |

| Timeline  | Concern                           | Narator | Footage                                                                     | prompt                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| --------- | --------------------------------- | ------- | --------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 0:45–2:00 | Pengenalan mariaDB                | Host    | Host inframe menjelaskan apa itu mariaDB                                    | MariaDB adalah turunan langsung dari MySQL yang dikembangkan oleh komunitas open-source setelah akuisisi MySQL oleh Oracle.  <br>Dikenal dengan performanya yang tinggi, fleksibilitas, dan transparansi pengembangan, MariaDB menjadi pilihan populer di kalangan pengembang dan administrator sistem.  <br>Selain kompatibel dengan MySQL, MariaDB menawarkan fitur-fitur tambahan yang terus dikembangkan secara terbuka oleh MariaDB Foundation.  <br>Dalam praktiknya, MariaDB sering digunakan dalam kombinasi dengan sistem backend aplikasi web, perangkat lunak ERP, maupun platform data terdistribusi. |
| 2:00–3:15 | Persiapan                         | Host    | Host inframe menjelaskan yang perlu disiapkan untuk menginstal mariaDB      | Sebelum menginstal, ada beberapa persiapan yang perlu dilakukan.  <br>Pertama, pastikan Anda memiliki akses ke terminal sebagai pengguna root atau dengan hak akses `sudo`.  <br>Kedua, koneksi internet harus aktif karena proses instalasi akan menarik paket dari repositori resmi.  <br>Sebagai contoh, kita akan menggunakan distribusi **Ubuntu**. Namun, langkah-langkah ini juga dapat diterapkan pada distribusi berbasis Debian lainnya, dengan penyesuaian kecil untuk sistem seperti CentOS atau Fedora.                                                                                              |
| 3:15–4:00 | update softaware                  | Host    | Host inframe dan mendemonstrasikan proses update software                   | Langkah pertama adalah memperbarui repositori sistem untuk memastikan Anda mendapatkan versi perangkat lunak terbaru.  <br>Buka terminal dan ketik:<br><br>sudo apt update<br><br>Langkah ini penting untuk menjaga konsistensi sistem dan menghindari konflik saat instalasi perangkat lunak baru.                                                                                                                                                                                                                                                                                                               |
| 4:00–4:45 | instalasi mariaDB                 | Host    | Host inframe dan mendemonstrasikan instalasi mariaDB                        | Setelah sistem diperbarui, lanjutkan dengan menginstal MariaDB menggunakan perintah:<br><br>sudo apt install mariadb-server<br><br>Sistem akan mengunduh dan memasang seluruh paket yang dibutuhkan.  <br>Tunggu hingga proses instalasi selesai sepenuhnya sebelum melanjutkan ke tahap berikutnya.                                                                                                                                                                                                                                                                                                              |
| 4:45–5:30 | verifikasi status mariaDB         | Host    | Host inframe dan  mendemonstrasikan pengecekan status mariaDB               | Untuk memastikan MariaDB telah terinstal dengan benar dan berjalan, jalankan perintah:<br><br>sudo systemctl status mariadb<br><br>Jika status menunjukkan **active (running)**, berarti layanan telah berjalan dengan baik.  <br>Jika belum aktif, Anda bisa memulainya dengan:<br><br>sudo systemctl start mariadb<br><br>Untuk memastikan layanan selalu aktif saat sistem dinyalakan ulang:<br><br>sudo systemctl enable mariadb                                                                                                                                                                              |
| 5:30–6:30 | percobaan antarmuka shell mariaDB | Host    | host mendemonstrasikan pengaksesan antarmuka shell mariaDB                  | Untuk memastikan bahwa MariaDB siap digunakan, Anda bisa masuk ke antarmuka shell-nya.  <br>Gunakan perintah:<br><br>sudo mariadb<br><br>Jika berhasil, Anda akan melihat prompt `MariaDB [(none)]>`.  <br>Ini menunjukkan bahwa Anda telah masuk ke dalam lingkungan MariaDB dan siap untuk menjalankan perintah administrasi basis data.  <br><br><br><br><br><br><br><br><br><br>                                                                                                                                                                                                                              |
| 6:30–7:30 | pemeriksaan akhir                 | host    | host mendemonstrasikan pengecekan ulang untuk memastikan instalasi berhasil | Untuk memastikan bahwa instalasi Anda bersih dan aman, periksa kembali beberapa hal:<br><br>- Apakah layanan MariaDB aktif dan berjalan otomatis?<br>- Apakah Anda bisa mengakses shell MariaDB tanpa kesalahan?<br>    <br><br>Jika semua berjalan lancar, berarti Anda telah berhasil melakukan instalasi dan konfigurasi awal MariaDB secara tepat.                                                                                                                                                                                                                                                            |
| 7:30–8:30 | Kesimpulan                        | host    | host menjelaskan kesimpulan dari praktek                                    | Instalasi MariaDB di Linux merupakan fondasi penting dalam pembangunan sistem informasi yang efisien dan terpercaya.  <br>Dengan proses yang relatif sederhana, Anda telah membuka pintu menuju pengelolaan data yang lebih terstruktur dan profesional.  <br>Meskipun MariaDB merupakan perangkat lunak open-source, kapabilitasnya sangat kompetitif bahkan untuk penggunaan di tingkat enterprise.  <br>Penguasaan tahap awal ini akan sangat membantu dalam memahami struktur dan fungsi sistem manajemen basis data di kemudian hari.                                                                        |
|           |                                   |         |                                                                             | Semoga panduan ini membantu Anda dalam menginstal MariaDB dengan lancar.  <br>Jika Anda memiliki pertanyaan, jangan ragu untuk meninggalkan komentar.  <br>Sampai jumpa di video pembelajaran berikutnya.                                                                                                                                                                                                                                                                                                                                                                                                         |



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

| Timeline  | Concern | Narator | Footage                        | prompt                                                                                                   |
| --------- | ------- | ------- | ------------------------------ | -------------------------------------------------------------------------------------------------------- |
| 8:30–9:00 | Penutup | Host    | Host inframe dan menutup video | <br>Terima kasih telah menyimak, dan sampai jumpa di materi pembelajaran berikutnya.<br><br><br><br><br> |
