Proyek ini merupakan simulasi pengujian konektivitas jaringan menggunakan Cisco Packet Tracer. Tujuan dari pengujian ini adalah untuk memastikan bahwa komunikasi antar perangkat (PC-A dan PC-B) melalui Switch dan Router dapat berjalan dengan baik setelah konfigurasi jaringan dilakukan.

🧩 Topologi Jaringan
![Topologi Jaringan](https://github.com/user-attachments/assets/ee6b2124-de5e-48aa-98b9-00e323ddae0d)

| Perangkat         | Interface        | IP Address                          | Subnet Mask   |
| ----------------- | -----------------| ----------------------------------- | ------------- |
| PC0 (PC-A)        | FastEthernet0    | 192.168.1.3                         | 255.255.255.0 |
| PC1 (PC-B)        | FastEthernet0    | 192.168.0.3                         | 255.255.255.0 |
| Router0 (ISR4321) | G0/0/0 & G0/0/1  | Disesuaikan dengan segment jaringan | —             |

⚙️ Langkah Pengujian
1. Konfigurasi IP address pada masing-masing PC sesuai tabel di atas.
2. Hubungkan PC-A dan PC-B melalui switch dan router sesuai topologi.
3. Lakukan pengujian konektivitas dari PC-B ke PC-A dengan perintah:
ping 192.168.1.3
4. Amati hasil yang muncul di Command Prompt.

📊 Hasil Pengujian

🟥 Sebelum Konfigurasi Berhasil
Pada awal pengujian, koneksi gagal karena konfigurasi routing pada router belum dilakukan.
Hasil ping menunjukkan Request Timed Out (RTO) seperti gambar berikut:
![before konfigurasi](https://github.com/user-attachments/assets/ca813cfc-655c-4856-96ee-ddb41bcdeb5c)

🟩 Setelah Konfigurasi Berhasil
Setelah melakukan konfigurasirouting, pengujian ulang menunjukkan hasil berhasil terkoneksi:
![after konfigurasi](https://github.com/user-attachments/assets/803019e6-5c4f-4803-8158-32611e0db283)

🔍 Kesimpulan
Pada awalnya, konektivitas antara PC-B dan PC-A gagal karena belum ada konfigurasi routing yang sesuai.
Setelah melakukan konfigurasi routing, ping berhasil menandakan komunikasi antar perangkat berjalan normal.
Hasil ini menunjukkan jaringan telah terkoneksi dengan baik melalui switch dan router yang digunakan.

Berikut adalah link video youtube pada saat melakukan konfigurasi dari awal sampai selesai: https://youtu.be/VK_lx5DXMgs
