[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/1niUih_B)
| Name           | NRP        | Kelas     |
| ---            | ---        | ----------|
| Wahid Badar Abiddin | 5025221025 | JarKom A |



## Put your topology config image here!

`Put your image here`

<img width="1144" height="742" alt="Screenshot 2025-10-02 193354" src="https://github.com/user-attachments/assets/29de6f09-64a2-4632-ae21-ec32f683c333" />

## Put your GNS3 Project file here!

`Put file URL here : https://github.com/Wbadara/Jarkom/tree/main/modul%202`

<br>

## Soal 1

> Dokumentasikan hasil pengelompokan subnet yang telah dibuat.

> _Document the results of the subnet grouping that has been created._

**Answer:**

- Screenshot

  `Put your screenshot in here`
  
  ![Dokumentasi Subnet](https://github.com/user-attachments/assets/55ad6388-53f7-46aa-b63d-18d15ab7c975)

- Explanation

  `Put your explanation in here : Saya membagi subnet berdasarkan switch terlebih dahulu kemudian lanjut bagian lainnya`

<br>

## Soal 2

> Lakukan konfigurasi routing agar setiap node dapat saling berkomunikasi. Pastikan setiap router dapat mengirimkan paket ke jaringan lain melalui tabel routing yang sesuai. Sertakan bukti bahwa Falcon bisa melakukan ping ke SpiderMan, DoctorStrange, dan ScarletWitch.

> _Configure routing so that each node can communicate with each other. Ensure each router can forward packets to other networks through the appropriate routing table. Include proof that Falcon can ping SpiderMan, Doctor Strange, and ScarletWitch._

**Answer:**

- Screenshot
  `Put your screenshot in here`
  
  <img width="664" height="291" alt="Screenshot 2025-10-03 185709" src="https://github.com/user-attachments/assets/8aca3c77-e377-49d0-af1b-6303fef86a37" />
  <img width="671" height="269" alt="Screenshot 2025-10-03 192653" src="https://github.com/user-attachments/assets/4f9a1470-81a8-489d-95b4-a561b038454f" />
  <img width="647" height="281" alt="Screenshot 2025-10-03 192718" src="https://github.com/user-attachments/assets/3f6b49ce-2722-4734-b74c-494add4a63e8" />

- Explanation

  `Put your explanation in here :
  Pertama saya melaakukan konfigurasi pada masing masing router dan server sesuai dengan tabel subnet yang tellah saya buat. Selanjutnya menambahkan ping pada masing masing client juga sesui tabel. Jalankan perintah "ip route add [subnet tujuan/24] via [gateway yang terhubung]" pada masing masing routeragar dapat meneruskan paket. Pada client jalankan perintah "route add default gw [gateway yang tergubung]" sehingga bisa mengirimkan paket. Selanjutnya bisa uji konektivitas dengan ping.`

<br>

## Soal 3

> Lakukan konfigurasi agar semua node dapat terhubung ke internet. Sertakan hasil uji coba dengan melakukan ping ke google.com dari node Falcon, CaptainAmerica, SpiderMan, dan Thor.

> _Configure all nodes to connect to the internet. Include test results by pinging google.com from the Falcon, CaptainAmerica, SpiderMan, and Thor nodes._

**Answer:**

- Screenshot

  `Put your screenshot in here`
  
  <img width="821" height="375" alt="Screenshot 2025-10-03 200118" src="https://github.com/user-attachments/assets/6d3e639a-1710-4829-b861-ec7cf1df8517" />
  <img width="811" height="347" alt="Screenshot 2025-10-03 200921" src="https://github.com/user-attachments/assets/67bf224f-2027-44dc-8333-161cefcf1aa2" />
  <img width="809" height="298" alt="Screenshot 2025-10-03 201329" src="https://github.com/user-attachments/assets/9b76de08-d370-4ff2-99b5-fe1b25440d72" />
  <img width="797" height="316" alt="Screenshot 2025-10-03 201543" src="https://github.com/user-attachments/assets/bb805e0d-4812-42e5-bb6d-de8b115b258c" />


- Explanation

  `Put your explanation in here:
  Pertama saya dapat alamat ip dinamis yaitu 192.168.122.184 maka saya tambahkan default gateway menuju NAT di router IronMan engan perintah "ip route add 0.0.0.0/0 via 192.168.122.1" dan "iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE" untuk melakukan NAT saat paket keluar melalui interface. Kemudian di router lainnya jalankan perintah "ip route add 0.0.0.0/0 via [gateway menuju IronMan]". Di node jalnkan perintah "nano /etc/resolv.conf" di dalam nano tambahkan tulisan 'nameserver 8.8.8.8' yang bertujuan menambahkan DNS Server. Lanjut melakukan ping ke google.com`

<br>

## Soal 4

> Berikan Falcon alamat IP dalam rentang [Prefix IP].3.20 - [Prefix IP].3.25
> <br> </br>
> Berikan Hawkeye alamat IP dalam rentang [Prefix IP].4.30 - [Prefix IP].4.35
> <br> </br>
> Berikan Hulk alamat IP dalam rentang [Prefix IP].6.50 - [Prefix IP].6.55

<br>

> _Give Falcon an IP address in the range [IP Prefix].3.20 - [IP Prefix].4.35_
> <br> </br>
> _Give Hawkeye an IP address in the range [IP Prefix].4.30 - [IP Prefix].4.35_
> <br> </br>
> _Give Hulk an IP address in the range [IP Prefix].6.50 - [IP Prefix].6.55_

**Answer:**

- Screenshot

  `Put your screenshot in here`

  <img width="811" height="319" alt="Screenshot 2025-10-03 235325" src="https://github.com/user-attachments/assets/9932a742-dedf-4934-a106-d1228378f013" />
  <img width="817" height="304" alt="Screenshot 2025-10-03 235342" src="https://github.com/user-attachments/assets/202a1611-e92a-411f-a0f8-d0bd8b4516e0" />
  <img width="808" height="280" alt="Screenshot 2025-10-03 235404" src="https://github.com/user-attachments/assets/a6038572-ceb4-4364-9a86-297ce6e19c6d" />


- Explanation

  `Put your explanation in here :
  Pertama saya melakukan routing pada routers agar dapat mengakses internet, untuk caranya sama dengan no 3 yang berbeda hanya DHCP Server dan DHCP Relay yang memiliki ip statis dan client belum dapat ip dinamis serta ip statis yang dipakai pada DHCP Server dan DHCP Relay yang berbeda.`
  
  <img width="1008" height="577" alt="Screenshot 2025-10-03 235622" src="https://github.com/user-attachments/assets/72c318d4-16fa-4171-82b1-458a2d443bdc" />

   `Setelah terhubung internet, melakukan "apt-get update" dan "apt-get install isc-dhcp-server" pada server. Dan selanjutnya ikuti cara pada modul untuk set DHCP server dan DHCP Relay.`
<br>

## Soal 5

> Berikan ScarletWitch dan Thor alamat IP dalam rentang [Prefix IP].5.40 - [Prefix IP].5.45 dan [Prefix IP].5.100 - [Prefix IP].5.105

> _Give ScarletWitch and Thor IP addresses in the range [IP Prefix].5.40 - [IP Prefix].5.45 and [IP Prefix].5.100 - [IP Prefix].5.105_

**Answer:**

- Screenshot

  `Put your screenshot in here`

- Explanation

  `Put your explanation in here`

<br>

## Soal 6

> Berikan SpiderMan dan DoctorStrange alamat IP dalam rentang [Prefix IP].7.60 - [Prefix IP].7.65  dan [Prefix IP].7.110 - [Prefix IP].7.115

> _Give SpiderMan and DoctorStrange IP addresses in the ranges [IP Prefix].7.60 - [IP Prefix].7.65 and [IP Prefix].7.110 - [IP Prefix].7.115_

**Answer:**

- Screenshot

  `Put your screenshot in here`

- Explanation

  `Put your explanation in here`

<br>

## Soal 7

> Tetapkan waktu peminjaman alamat IP pada DHCP server untuk client yang terhubung melalui Switch 2 selama 5 menit (Default), dan untuk client melalui Switch 5 selama 10 menit (Default). Tetapkan juga batas waktu peminjaman maksimal selama 2 jam.
> <br> </br>
> Tetapkan waktu peminjaman alamat IP pada DHCP server untuk client yang terhubung melalui Switch 1 dan Switch 3 selama 2 menit (Default). Tetapkan juga batas waktu peminjaman maksimal selama 100 menit.

<br>

> _Set the IP address lease period on the DHCP server for clients connected through Switch 2 to 5 minutes (default), and for clients connected through Switch 5 to 10 minutes (default). Also, set the maximum lease period to 2 hours._
> <br> </br>
> _Set the IP address lease time on the DHCP server for clients connected via Switch 1 and Switch 3 to 2 minutes (default). Also set the maximum lease time limit to 100 minutes._

**Answer:**

- Screenshot

  `Put your screenshot in here`

- Explanation

  `Put your explanation in here`

<br>

## Soal 8

> Ubah konfigurasi DHCP Server agar Hawkeye, Thor, dan SpiderMan mendapatkan IP statis dengan [Prefix IP].x.5, namun masih menggunakan DHCP.

> _Change the DHCP Server configuration so that Hawkeye, Thor, and SpiderMan get static IPs with [Prefix IP].x.5, but still use DHCP._

**Answer:**

- Screenshot

  `Put your screenshot in here`

- Explanation

  `Put your explanation in here`

<br>

## Soal 9

> Buatlah konfigurasi DHCP Failover dengan WinterSoldier sebagai DHCP server backup untuk CaptainAmerica.

> _Create a DHCP Failover configuration with WinterSoldier as the backup DHCP server for CaptainAmerica._

**Answer:**

- Screenshot

  `Put your screenshot in here`

- Explanation

  `Put your explanation in here`

<br>

## Soal 10

> Buatlah konfigurasi agar CaptainAmerica dan WinterSoldier berjalan dengan mode Load Balancing.

> _Create a configuration so that CaptainAmerica and WinterSoldier run in Load Balancing mode._

**Answer:**

- Screenshot

  `Put your screenshot in here`

- Explanation

  `Put your explanation in here`

<br>
  
## Problems

## Revisions (if any)
