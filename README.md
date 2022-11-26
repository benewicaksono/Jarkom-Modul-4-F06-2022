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

- Ketiga, kita dapat mengitung pembagian IP dengan membuat pohon. lalu, memilih subnet besar yaitu 192.202.0.0 dengan netmask /20. 
<br>
<p align="center">
  <img src="img/pohon.png" width="600">
</p><br>


