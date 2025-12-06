# project4_so.Galuh-System-Health-Check

gambar : https://drive.google.com/file/d/1mugzYoA4-PVmaPxFbe-yHhyrYyCm7amm/view?usp=sharing

Perintah,Fungsi
systeminfo > documents_laporan.txt,"Perintah ini digunakan untuk menampilkan informasi detail mengenai konfigurasi sistem operasi dan perangkat keras komputer, seperti versi OS, model PC, RAM terpasang, zona waktu, dan konfigurasi kartu jaringan."

,">: Operator pengalihan yang digunakan untuk menulis output perintah ke file baru (documents_laporan.txt). Jika file sudah ada, isinya akan ditimpa (overwrite)."

chkdsk > documents_laporan.txt,Perintah ini digunakan untuk memeriksa file system dan metadata file system pada volume drive untuk mencari error logis dan fisik. Output-nya mencakup status volume dan statistik ruang disk.

,>: Operator ini menimpa file documents_laporan.txt yang sudah dibuat oleh perintah systeminfo. Perintah chkdsk ini akan menggantikan isi sebelumnya dengan hasil pemeriksaan disk.

tasklist >> documents_laporan.txt,"Perintah ini digunakan untuk menampilkan daftar semua proses (tugas) yang sedang berjalan di komputer, termasuk nama gambar, ID proses (PID), nama sesi, dan penggunaan memori."

,">>: Operator pengalihan yang digunakan untuk menambahkan (append) output perintah ke akhir file yang sudah ada (documents_laporan.txt). Jadi, hasil tasklist akan ditambahkan setelah hasil chkdsk."

type documents_laporan.txt,"Perintah ini digunakan untuk menampilkan seluruh isi dari file teks (documents_laporan.txt) langsung ke layar Command Prompt, memungkinkan pengguna untuk melihat hasil laporan yang telah dibuat."
