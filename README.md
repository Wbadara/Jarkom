[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/tPVgLsdF)
| Name | NRP | Class |
| ---- | --- | ----- |
| Wahid Badar Abiddin  | 5025221025 | Jarkom A   |

## Task 1

- Flag

`JARKOM25{Ja0G_Bbbb4ng3t_S1_JLM0E1GT6AH5RTER0UYX2ZDOKNVFDU0xl0vel1hfc5u006a9d00ymc1ogwbb1_9ed732fa42b07d7b607686bcf8ee2116}`

> a. Berapa banyak packet yang terekam pada file pcapng?

> _a. How many packets are recorded in the pcapng file?_

**Answer:** `9596`

- Filter expression

  `put your filter here (if any)`

- Explanation

  `Untuk melihat banyaknya packet yang terekam pada file cukup melihat di sisi kanan bawah.`
  
  <img width="1912" height="1014" alt="Screenshot 2025-09-11 192443" src="https://github.com/user-attachments/assets/7cd9251a-d2fc-4af6-80a2-0df7af36f649" />


- Output result

  `Di sisi kanan bawah terlihat tulisan packets:9596, jadi banyaknya packet adalah 9596.`

<br>
<br>

> b. Ada berapa jenis protocol (total) yang terekam pada traffic?

> _b. How many types of protocol (totals) are recorded in the traffic?_

**Answer:** `12`

- Filter expression

  `put your filter here (if any)`

- Explanation

  `Untuk melihat banyaknya jenis protocol yang terekam pada traffic bisa melalui menu Statistics, kemudian pilih Protocol Hierarchy.`

  <img width="1525" height="677" alt="Screenshot 2025-09-11 193124" src="https://github.com/user-attachments/assets/e5669d08-e11c-4693-a4d1-554c4d3f5616" />

  `Muncul sebuah tab yang akan menampilkan informasi mengenai protocol yang ada.`

- Output result

  `Terdapat 12 protocol yang ditampilkan.`

<br>
<br>

> c. Ada berapa jenis protocol berbasis TCP yang terekam pada traffic?

> _c. How many types of TCP-based applications protocol are recorded in the traffic?_

**Answer:** `8`

- Filter expression

  `put your filter here (if any)`

- Explanation

  `Untuk menjawab ini, dapat dilihat lagi pada tab Protocol Hierarchy. Namun karena yang diminta banyaknya protocol yang berbasis TCP maka cukup lihat yang ada di bagian Transmission Control Protocol (TCP).`

- Output result

  `Terdapat 8 protocol yang ditampilkan.`

  <br>
  <br>

> d. Ada berapa banyak packet dengan protokol TCP murni yang terekam pada traffic (tanpa data)?

> _d. How many packets with pure TCP protocol are recorded in the traffic (without data)?_

**Answer:** `3223`

- Filter expression

  `put your filter here (if any)`

- Explanation

  `put your explanation here`

- Output result

  `put your output result here`

## Task 2

- Flag

  `put your flag here`

> a. Berapa banyak packet berhasil yang berbasis murni TCP dan memiliki flag [ACK]?

> _a. How many packets succeed that are pure TCP based and have [ACK] flag?_

**Answer:** `put your answer here`

- Filter expression

  `put your filter here (if any)`

- Explanation

  `put your explanation here`

- Output result

  `put your output result here`

  <br>
  <br>

> b. Berapa banyak packet berhasil yang berbasis murni TCP yang hanya memiliki flag [ACK]?

> _b. How many packets succeed that are pure TCP based and have only [ACK] flag?_

**Answer:** `put your answer here`

- Filter expression

  `put your filter here (if any)`

- Explanation

  `put your explanation here`

- Output result

  `put your output result here`

  <br>
  <br>

> c. Berapa banyak packet berhasil yang berbasis murni TCP dan memiliki flag selain hanya [ACK]?

> _c. How many packets succeed that are pure TCP based and contain flags other than just [ACK] flag?_

**Answer:** `put your answer here`

- Filter expression

  `put your filter here (if any)`

- Explanation

  `put your explanation here`

- Output result

  `put your output result here`

  <br>
  <br>

## Task 3

- Flag

  `put your flag here`

> a. Pada port berapa client telnet terbuka?

> _a. In what port is the telnet client open?_

**Answer:** `54184`

- Filter expression

  `telnet`

- Explanation

  `Saya memfilter packet dengan kata kunci telnet agar hanya menampilkan packet yang berbasis telnet.`

  <img width="1912" height="619" alt="Screenshot 2025-09-13 210926" src="https://github.com/user-attachments/assets/85b1fdff-6ec2-441c-91fa-9aab00bdc14a" />

  `Kemudian di bagian bawah kiri terdapat deskipsi dari Packet telnet. Kita bisa melihat bagian TCP, disana tertulis source port maupun destination portnya. Port yang digunakan oleh client adalah destination port.`

- Output result

  `Destination Port: 54184`

  <br>
  <br>

> b. Berapa byte file response yang dikirim dari server?

> _b. How many bytes of the response files are sent from the server?_

**Answer:** `put your answer here`

- Filter expression

  `put your filter here (if any)`

- Explanation

  `put your explanation here`

- Output result

  `put your output result here`

  <br>
  <br>

> c. Apa username yang digunakan client telnet untuk berhubungan dengan server?

> _c. What telnet client's username is used to connect with the server?_

**Answer:** `put your answer here`

- Filter expression

  `put your filter here (if any)`

- Explanation

  `put your explanation here`

- Output result

  `put your output result here`

  <br>
  <br>

> d. Apa password client telnet?

> _d. What is the telnet client's password?_

**Answer:** `put your answer here`

- Filter expression

  `put your filter here (if any)`

- Explanation

  `put your explanation here`

- Output result

  `put your output result here`

  <br>
  <br>

## Task 4

- Flag

  `JARKOM25{G04t__a4n4liz333er_RH8R4YB174XLCYX5N7H8fr0gbg1m0qcaghuinc7r3ys1723761467_f44807b5adb04d4035936e06fff6c5a0}`

> a. Apa perintah pertama yang ditulis client pada koneksi telnet?

> _a. What is the first command that client wrote on telnet connection?_

**Answer:** `echo`

- Filter expression

  `telnet`

- Explanation

  `Melakukan filter telnet agar hanya menampilkan packet yang berbasis telnet. Kemudian melakukan follow stream pada salah satu komunikukasi agar dapat melihat seluruh percakapan antara server dan client. Namun untuk melihat perintah pertama yang ditulis client kita bisa tau dengan filter client to server agar hanya menampilkan percakapan client ke server.`

  <img width="1256" height="896" alt="Screenshot 2025-09-13 223855" src="https://github.com/user-attachments/assets/d3604b8e-2a18-43d2-ab20-99532bd9c42c" />

  `Filternya ada di bagian bawah yang bertuliskan ip:port client to ip:port server.`

- Output result

  `Tertera untuk perintah pertamanya adalah 'echo'.`

  <br>
  <br>

> b. Apa nama file .txt di server (ditulis bersama ekstensinya)?

> _b. What is the name of .txt file on the server (write with the extension)?_

**Answer:** `test.txt`

- Filter expression

  `telnet`

- Explanation

  `Caranya sama dengan mencari perintah pertama client, namun karena kita mencari di server maka kita menggunakan filter server to client.`

  <img width="1374" height="893" alt="Screenshot 2025-09-13 224437" src="https://github.com/user-attachments/assets/1935c336-5be6-486c-aa3d-80a7a2eb5737" />

  `Filternya ada di bagian bawah yang bertuliskan ip:port server to ip:port client.`

- Output result

  `Nama file txt adalah test.txt`

  <br>
  <br>

> c. Apa kata pertama dari frasa yang dimasukkan client ke dalam file sebelumnya?

> _c. What is the first word that the client inserted into the previous file?_

**Answer:** `Jarkom`

- Filter expression

  `telnet`

- Explanation

  `Kembali kita melihat ke komunikasi antara client dan server untuk mencari tahu kata pertama dari frasa yang dimasukkan client.`

  <img width="1256" height="896" alt="Screenshot 2025-09-13 223855" src="https://github.com/user-attachments/assets/a3125f2d-537c-41ed-9b21-d5c7315587e1" />

- Output result

  `Kata pertama dari frasa yang dikirim client adalah 'Jarkom'.`

  <br>
  <br>

## Task 5

- Flag

  `put your flag here`

> a. Berapa banyak packet berbasis HTTP yang terekam pada file pcapng?

> _a. How many HTTP packets are recorded in the pcapng file?_

**Answer:** `298`

- Filter expression

  `http`

- Explanation

  `Saya memfilter packet dengan kata kunci http agar hanya menampilkan packet yang berbasis http.`

  <img width="1916" height="1010" alt="Screenshot 2025-09-11 202148" src="https://github.com/user-attachments/assets/947543d9-befb-43f4-92b6-eff115525fc3" />

  `Untuk melihat banyaknya packet http cukup melihat di sisi kanan bawah.`

- Output result

  `Di sisi kanan bawah terlihat tulisan packets:298, jadi banyaknya packet http adalah 298.`

  <br>
  <br>

> b. Ada berapa HTTP packet yang berupa response?

> _b. How many response HTTP packets are recorded in the traffic?_

**Answer:** `149`

- Filter expression

  `http.response`

- Explanation

  `Saya memfilter packet dengan kata kunci http.response agar hanya menampilkan packet http yang berupa response.`

  <img width="1914" height="1009" alt="Screenshot 2025-09-11 202214" src="https://github.com/user-attachments/assets/ae8fac73-5a59-4f35-bb47-044a491112e5" />

   `Untuk melihat banyaknya packet http yang berupa response cukup melihat di sisi kanan bawah.`

- Output result

  `Di sisi kanan bawah terlihat tulisan packets:149, jadi banyaknya packet http yang berupa response adalah 149`

  <br>
  <br>

> c. Ada berapa paket berbasis HTTP yang berhasil?

> _c. How many HTTP packets that succeed?_

**Answer:** `put your answer here`

- Filter expression

  `put your filter here (if any)`

- Explanation

  `put your explanation here`

- Output result

  `put your output result here`

  <br>
  <br>

> d. Apa alamat IP dari client HTTP yang tersambung lokal dengan mesin lain?

> _d. What is the client HTTP IP Address in connection with other local machine?_

**Answer:** `put your answer here`

- Filter expression

  `put your filter here (if any)`

- Explanation

  `put your explanation here`

- Output result

  `put your output result here`

  <br>
  <br>

## Task 6

- Flag

`JARKOM25{br0mb44rdin0u_Cr0ccc0c0c0cdi1l10l_6568748739awaesa8cjr61izyfsh1n0bu0VKSEUMY9HV6QZR_38834497141fb9b4b26519a9578f4251}`

> a. Apakah kamu menemukan fake flag? Tuliskan seluruhnya!

> _a. Did you find the fake flag? Write it whole!_

**Answer:** `FakeFlag{JarkomGampang}`

- Filter expression

  `http.request`

- Explanation

  `Saya memfilter packet dengan kata kunci http.request agar hanya menampilkan packet http yang berupa request karena fake flag berada di file yang direquest oleh client. Kemudian saya cari file flag.txt yang berisikan fake flag.`

  <img width="1848" height="491" alt="Screenshot 2025-09-13 195513" src="https://github.com/user-attachments/assets/100d79b0-a279-46c6-a19b-e7221469c000" />

  `Setelah menemukan file flag.txt, saya melakukan follow stream agar dapat melihat seluruh percakapan file tersebut.`

  <img width="496" height="395" alt="Screenshot 2025-09-11 215232" src="https://github.com/user-attachments/assets/0341741f-74c6-4d43-bc9a-ac23bca42fbd" />

- Output result

  `Tertulis FakeFlag{JarkomGampang} di file tersebut.`

  <br>
  <br>

> b. Tuliskan username dan password yang tertulis! (format username:password)

> _b. Write the written username and password! (format username:password)_

**Answer:** `Rey:123`

- Filter expression

  `http.request`

- Explanation

  `Saya memfilter packet dengan kata kunci http.request agar hanya menampilkan packet http yang berupa request karena file yang berisikan username dan password pasti direquest oleh client. Kemudian saya cari file lain yang kemungkinan berisikan username dan password.`

  <img width="1852" height="397" alt="Screenshot 2025-09-13 200701" src="https://github.com/user-attachments/assets/e7871c3a-123c-4e23-b357-dac025ec9df8" />

  `Setelah menemukan file tersebut, saya melakukan follow stream agar dapat melihat seluruh percakapan filenya.`

  <img width="575" height="410" alt="Screenshot 2025-09-11 215245" src="https://github.com/user-attachments/assets/b5096307-37f5-421a-a6ce-663eb3efc8f8" />

- Output result

  `Tertuis username: Rey dan password: 123.`

  <br>
  <br>

## Task 7

- Flag

  `JARKOM25{tr4l4lel0_tr1lil1_4qb3bekajjk3b0s0sQXB7DFJ2W5127HJ_22df90cc1d9cc2780b2cb77930418245}`

> Apa nama gambar yang direquest oleh client? (tulis dengan ekstensinya)

> _What is the image that is being requested by the client? (write with its extension)_

**Answer:** `donalbebek.jpg`

- Filter expression

  `http.request`

- Explanation

  `Gambar yang direquest oleh client dapat kita lihat dari menerapkan filter http.request kemudian cari file dengan ekstensi jpg.`

  <img width="1846" height="406" alt="Screenshot 2025-09-13 201405" src="https://github.com/user-attachments/assets/b30ac018-2d50-46f2-bcb7-c22f34d3ad00" />

- Output result

  `Terdapat file donalbebek.jpg`

  <br>
  <br>

## Task 8

- Flag

  `put your flag here`

> a. Berapa banyak packet berbasis FTP yang terekam pada file pcapng? (with the data)

> _a. How many FTP packets are recorded in the pcapng file? (with the data)_

**Answer:** `put your answer here`

- Filter expression

  `put your filter here (if any)`

- Explanation

  `put your explanation here`

- Output result

  `put your output result here`

  <br>
  <br>

> b. Apa username dan password client di koneksi FTP? (tulis dalam format username:password)

> _b. What is the client's username and password in FTP connection? (write in following format username:password)_

**Answer:** `put your answer here`

- Filter expression

  `put your filter here (if any)`

- Explanation

  `put your explanation here`

- Output result

  `put your output result here`

  <br>
  <br>

> c. What is the client's command for showing server directory that was sent on request packet?

> _c. Apa command client untuk melihat direktori server yang dikirimkan dalam request packet?_

**Answer:** `put your answer here`

- Filter expression

  `put your filter here (if any)`

- Explanation

  `put your explanation here`

- Output result

  `put your output result here`

  <br>
  <br>

## Task 9

- Flag

  `put your flag here`

> a. Apa alamat IP dari FTP server?

> _a. What is the FTP server IP Address?_

**Answer:** `172.16.16.101`

- Filter expression

  `ftp`

- Explanation

  `Melakukan filter ftp agar hanya menampilkan packet yang berbasis ftp. Kemudian untuk melihat alamat IP dari ftp server kita dapat melihat di deskripsi Internet Protocol pada bagian kiri bawah.`

  <img width="1896" height="656" alt="Screenshot 2025-09-13 210600" src="https://github.com/user-attachments/assets/52e242ae-ed58-4f36-b638-d07af98308bb" />


- Output result

  `IP ftp server adalah IP source yaitu 172.16.16.101`

  <br>
  <br>

> b. Berapa banyak file yang ada dalam direktori FTP server?

> _b. How many files are there inside the FTP server directory?_

**Answer:** `put your answer here`

- Filter expression

  `put your filter here (if any)`

- Explanation

  `put your explanation here`

- Output result

  `put your output result here`

  <br>
  <br>

> c. Apa nama dari file yang digunakan dalam page.html? (tulis lengkap namanya beserta ekstensinya dan dipisahkan dengan koma ',')

> _c. What are the filenames used in the page.html? (write the filebames with their extensions and separate them with comma ',')_

**Answer:** `put your answer here`

- Filter expression

  `put your filter here (if any)`

- Explanation

  `put your explanation here`

- Output result

  `put your output result here`

  <br>
  <br>

## Task 10

- Flag

`JARKOM25{f1nisssshs55s5s533s_l1n333ee333E3_465605331129104vpsinsavm3452151231230ULGVQ16LZ0MMLE_a575ab2e1937a900e97a9f4d8cbd7424}`

> a. Apa nama file yang mengandung string terencode?

> _a. What is the filename that contains encoded string?_

**Answer:** `secret.txt`

- Filter expression

  `ftp.request`

- Explanation

  `Dengan menerapkan filter ftp.request maka hanya akan memunculkan packet ftp yang direquest oleh client. Kemudian cari file txt yang berisikan string terencode.`

  <img width="1851" height="402" alt="Screenshot 2025-09-13 202711" src="https://github.com/user-attachments/assets/3cdf462c-5e6e-4c5e-afb6-cccb7a9c83d0" />

- Output result

  `Tertulis nama filenya yaitu secret.txt`

  <br>
  <br>

> b. Apa nama file hasil copy file sebelumnya?

> _b. What is the filename of the previous file copy?_

**Answer:** `secret1.txt`

- Filter expression

  `ftp.request`

- Explanation

  `Masih sama seperti mencari file yang berisikan string terencode. Namun dalam mencari file hasil copy kita dapat mencari dengan melihat file apa yang diupload lagi.`

  <img width="1850" height="404" alt="Screenshot 2025-09-13 203410" src="https://github.com/user-attachments/assets/72783738-3715-4ed2-99a0-9b7f3b4295ed" />

  `RETR adalah "Retrieve" atau mengunduh file. MDTM adalah "Modification Date/Time" atau kapan terakhir modifikasi file. STOR adalah "Store" atau mengunggah file.`

- Output result

  `Tertera nama filenya yaitu secret1.txt`

  <br>
  <br>

> c. What is the decoded string from the previous file?

> _c. Apa decoded string dari file tersebut?_

**Answer:** `Pada suatu hari Rey bertemu dengan Nailong the Milk Dragon. Ketika bertemu, Rey mengajarkan Nailong apa itu Jaringan Komputer. Nailong pun senang karena ternyata Jaringan Komputer itu gampang.`

- Filter expression

  `ftp.request`

- Explanation

  `Setelah menemukan file yang berisikan string terencode yaitu secret.txt. Sekarang kita akan melihat isi dari file tersebut agar dapat melakukan decode. Untuk dapat melihatnya kita perlu mengekspor file dengan fitur Export Object lalu kita buka dengan notepad karena file txt.`

  <img width="1423" height="122" alt="Screenshot 2025-09-13 205643" src="https://github.com/user-attachments/assets/fefdf220-ba21-42df-89e9-39425bf349e7" />

  `Setelah mengetahui isinya, saatnya melakukan decode,`

- Output result

  `Decode dari stringnya adalah Pada suatu hari Rey bertemu dengan Nailong the Milk Dragon. Ketika bertemu, Rey mengajarkan Nailong apa itu Jaringan Komputer. Nailong pun senang karena ternyata Jaringan Komputer itu gampang.`

  <br>
  <br>

## Summary
  `Di praktikum modul 1 ini saya belajar mengidentifikasi dan menganalisa packet di wireshark. Saya melakukan koneksi ke suatu server menggunakan netcat untuk menjawab soal soal praktikum. Seperti halnya CTF (Capture The Flag), saya harus mendapatkan flagnya dengan menjawab semua pertanyaan dengan benar.`

## Problems
  `Untuk kesulitannya mungkin adalah wawasan terhadap ekspresi filter yang masih sedikit. Untuk penyelesaian dari tasknya sendiri, ketika praktikum saya hanya berhasil mendapat 5 flags, namun di hari sabtu saya mencoba mengerjakan lagi yang belum berhasil dan akhirnya saya bisa mendapatkan 4 flags lagi. Tersisa 1 flag yakni task 2 yang belum terpecahkan oleh saya.`
