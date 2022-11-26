# Jarkom-Modul-4-F06-2022

## Kelompok F06

|               Nama               |      NRP      |
| -------------------------------- | ------------- |
| Benedictus Bimo Cahyo Wicaksono  |  5025201097   |  
| Andhika Ditya Bagaskara D.       |  5025201096   |
| Theresia Nawangsih               |  5025201144   |

# Topologi Soal
<p align="center">
  <img src="img/topologi_soal.png" width="600">
</p><br>

## Catatan Soal
- Soal shift dikerjakan pada Cisco Packet Tracer dan GNS3 menggunakan metode perhitungan CLASSLESS yang berbeda.
`Keterangan: Bila di CPT menggunakan VLSM, maka di GNS3 menggunakan CIDR atau Sebaliknya`
- Pembagian IP menggunakan Prefix IP yang telah ditentukan pada modul pengenalan
` F06 = 192.202`

# Cisco Packet Tracer menggunakan VLSM
- Pertama membuat topologi pada CPT, sesuai dengan yang diminta soal
<br>
<p align="center">
  <img src="img/topologi_cpt.png" width="600">
</p><br>

- Kedua dapat mebuat label pada topologi 
<br>
<p align="center">
  <img src="img/labeling.png" width="600">
</p><br>
Pada pembagian ini, terdapat 18 subnet dimulai dari A1-A18. Selanjutnya, kita dapat melakukan pembagian seperti tabel dibawah ini
<br>

<p>

| Simbol   |  Jumlah IP |  Length |  Subnet Mask  | 
| -----------| -----------| --------|---------------|
|     A1     |    1001    |   /22   | 255.255.252.0 |   
|     A2     |     2      |   /30   | 255.255.255.252 | 
|     A3     |     251    |   /24   | 255.255.252.0 | 
|     A4     |     2      |   /30   | 255.255.255.252 | 
|     A5     |     51     |   /26   | 255.255.255.192 | 
|     A6     |     2      |   /30   | 255.255.255.252 | 
|     A7     |     2      |   /30   | 255.255.255.252 | 
|     A8     |     121    |   /25   | 255.255.255.128 | 
|     A9     |     2      |   /30   | 255.255.255.252 | 
|    A10     |     211    |   /24   | 255.255.252.0 | 
|    A11     |     2      |   /30   | 255.255.255.252 | 
|    A12     |     501    |   /23   | 255.255.254.0 | 
|    A13     |     2      |   /30   | 255.255.255.252 | 
|    A14     |     71     |   /25   | 255.255.255.128 | 
|    A15     |     421    |   /25   | 255.255.255.128 | 
|    A16     |     2      |   /30   | 255.255.255.252 | 
|    A17     |     2      |   /30   | 255.255.255.252 | 
|    A18     |     271    |   /23   | 255.255.254.0  |  
</p>
Berdasarkan total IP dan netmask yang dibutuhkan, maka kita dapat menggunakan netmask /20 untuk memberikan pengalamatan IP pada subnet.

</p>

- Ketiga, kita dapat mengitung pembagian IP dengan membuat tree. lalu, memilih subnet besar yaitu 192.202.0.0 dengan netmask /20. 
<br>
<p align="center">
  <img src="img/pohon.png" width="600">
</p><br>
Untuk pembagian nya dimulai dari 192.202.0.0/20 hingga 192.202.11.224/30

- Keempat, setelah membuat tree, kita dapat melanjutkan dengan pembagian IP untuk Network ID dan Broadcast Address
<p>

|    Simbol   |  Network ID  | Broadcast Address | 
| ------------| -------------|-------------------|
|     A1      |    1001      |   192.202.3.255   |
|     A2      |     2        |   192.202.11.195  | 
|     A3      |     251      |   192.202.8.255   |
|     A4      |     2        |   192.202.11.199  | 
|     A5      |     51       |   192.202.11.191  |  
|     A6      |     2        |   192.202.11.203  |
|     A7      |     2        |   192.202.11.207  | 
|     A8      |     121      |   192.202.10.124  | 
|     A9      |     2        |   192.202.11.211  |  
|    A10      |     211      |   192.202.9.255   |  
|    A11      |     2        |   192.202.11.215  |   
|    A12      |     501      |   192.202.5.255   |   
|    A13      |     2        |   192.202.11.219  |  
|    A14      |     71       |   192.202.10.255  |   
|    A15      |     421      |   192.202.11.127  |   
|    A16      |     2        |   192..202.11.223 |   
|    A17      |     2        |   192.202.11.227  |   
|    A18      |     271      |   192.202.7.255   |   
</p>

## Testing
Daunless ke Profound
<br>
![image](https://user-images.githubusercontent.com/87473932/204089542-a40f678a-af2c-4b93-afac-522c350596da.png)
<br>

Guideau ke Firefist
<br>
![image](https://user-images.githubusercontent.com/87473932/204089611-6ba2403f-6d24-4f87-8d95-f4c1d24f23cc.png)
<br>

The Witch ke the Order
<br>
![image](https://user-images.githubusercontent.com/87473932/204089671-0f52112e-16e0-42dd-b500-499124287f93.png)
<br>

Helga ke Phanora
<br>
![image](https://user-images.githubusercontent.com/87473932/204089689-3a4de703-af2c-41bd-9068-f3ef6ffc335a.png)
<br>

The Beast ke The Instrument
<br>
![image](https://user-images.githubusercontent.com/87473932/204089709-b29deb16-eb09-4e33-81b2-198166696711.png)
<br>

The Witch ke The Beast
<br>
![image](https://user-images.githubusercontent.com/87473932/204089748-5347530a-4376-4b43-ab7d-f9ac664a9a02.png)
<br>

Matt Ougat ke Corvekt
<br>
![image](https://user-images.githubusercontent.com/87473932/204089769-567690c5-e124-4595-8d39-83c541f68b8d.png)
<br>

The Beast ke Spendrow
<br>
![image](https://user-images.githubusercontent.com/87473932/204089792-455f4f11-2861-43f6-bbe3-15a295d64b73.png)
<br>

Haines ke Keith
<br>
![image](https://user-images.githubusercontent.com/87473932/204089854-dda2d614-3c60-43ba-aa9c-9221920e54ab.png)
<br>

Johan ke The Queen
<br>
![image](https://user-images.githubusercontent.com/87473932/204089873-4e7627fc-544c-4db7-b5f1-d6a22efc9032.png)
<br>

Oakleave ke The Witch
<br>
![image](https://user-images.githubusercontent.com/87473932/204089887-f8b52c8d-c3a2-402e-9195-54231117af8b.png)
<br>

Ashaf ke the Resonance
<br>
![image](https://user-images.githubusercontent.com/87473932/204089907-3971a4d2-333b-442f-b208-e6c2ff63ecc5.png)
<br>

Corvekt ke The Minister
<br>
![image](https://user-images.githubusercontent.com/87473932/204089935-6fb3f02d-648e-43d1-9dcf-f7b7becbaead.png)
<br>

Guideau ke Helga
<br>
![image](https://user-images.githubusercontent.com/87473932/204089959-bab2b1f8-7daa-4591-9769-22d73a98a019.png)
<br>

Ashaf ke The Queen
<br>
![image](https://user-images.githubusercontent.com/87473932/204089965-7a69d5a2-26e0-4d23-9896-8ea02490026b.png)
<br>

# GNS3 Menggunakan CIDR
## Step 1 (A)
![image](https://user-images.githubusercontent.com/87473932/204092627-1a4bf7c2-b5ae-4a84-824d-cad10b0f90ca.png)
## Step 2 (B)
![image](https://user-images.githubusercontent.com/87473932/204094721-bf0317f8-3bda-4687-9678-a611fc27913b.png)
## Step 3 (C)
![image](https://user-images.githubusercontent.com/87473932/204094729-84e6b71c-a773-4b89-b27a-7342734a9175.png)
## Step 4 (D)
![image](https://user-images.githubusercontent.com/87473932/204094736-b0917e76-c133-41a6-855b-7751503b2095.png)
## Step 5 (E)
![image](https://user-images.githubusercontent.com/87473932/204094745-2aac36b4-91fc-4edf-95b1-58d423b28b26.png)
## Step 6 (F)
![image](https://user-images.githubusercontent.com/87473932/204094753-4d80e79c-fdf1-4f36-973f-96fece80386b.png)
## Step 7 (G)
![image](https://user-images.githubusercontent.com/87473932/204094798-1c301b12-3deb-435a-9894-31baba915fcb.png)
## Step 8 (H)
![image](https://user-images.githubusercontent.com/87473932/204094808-5273d8e6-4b4b-4fca-b287-290f07c61d0b.png)
## Step 9 (I)
![image](https://user-images.githubusercontent.com/87473932/204094843-3637a30f-019b-4e0c-8c75-5519a493de88.png)
## Step 10 (J)
![image](https://user-images.githubusercontent.com/87473932/204094884-95f34282-4599-4c1c-9f66-9f2f450d45fe.png)
