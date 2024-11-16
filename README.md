# Jarkom-Modul-4-IT27-2024

## IT 27

| No  | Nama Anggota          | NRP        |
| --- | --------------------- | ---------- |
| 1   | Danendra Fidel Khansa | 5027231063 |
| 2   | Farida Qurrotu A'yuna | 5027231015 |

## IP PREFIX

`10.77`

## DAFTAR ISI

- [Topologi](#topologi)
- [Rute Subnet](#rute-subnet)
- [VLSM](#vlsm)
- [CIDR](#cidr)

## TOPOLOGI

### Cisco Packet Tracer | VLSM |

![alt text](<img/Topologi CPT.png>)

Setelah Subnetting :

![alt text](<img/Topologi GNS Subnet.png>)

## RUTE SUBNET

| Nama Subnet | Rute                                                                        | Jumlah IP | Netmask |
| ----------- | --------------------------------------------------------------------------- | --------- | ------- |
| A1          | HoloLive - HoloEn                                                           | 2         | /30     |
| A2          | HoloEn - Router0                                                            | 2         | /30     |
| A3          | Router0 - Switch2 - Gura_Ayne_Ina - Switch2 - Kiara_Calli                   | 503       | /23     |
| A4          | HoloEn - HoloAdvent                                                         | 2         | /30     |
| A5          | HoloAdvent - Switch0 - FuwaMoco - Switch0 - ShioriNerissa - Switch- - Biboo | 28        | /27     |
| A6          | Router0 - HoloPromise - HoloCouncil - HoloPromise - Router4                 | 3         | /29     |
| A7          | Router4 - Tys                                                               | 3         | /29     |
| A8          | HoloCouncil - Switch4 - KroniMumei - Switch4 - BaeFauna                     | 62        | /26     |
| A9          | HoloLive - HoloID                                                           | 2         | /30     |
| A10         | HoloID - AREA15                                                             | 2         | /30     |
| A11         | AREA15 - Switch6 - Risu - Switch6 - Moona - Switch6 - Lofi                  | 661       | /22     |
| A12         | HoloID - Holoro                                                             | 2         | /30     |
| A13         | Holoro - Switch7 - Ollie - Switch7 - Anya - Switch7 - Reine                 | 34        | /26     |
| A14         | HoloID - Holoh3ro                                                           | 2         | /30     |
| A15         | Holoh3ro - Switch8 - Zeta - Switch8 - Kaela - Switch8 - Kobo                | 299       | /23     |
| A16         | HoloLive - HoloJP                                                           | 2         | /30     |
| A17         | HoloJP - Switch1 - DEV_IS - Switch1 - GEN:0                                 | 3         | /29     |
| A18         | DEV_IS - Re:Gloss - RirikaRaden - Re:Gloss - Ao - Re:Gloss - HajimeKanade   | 14        | /28     |
| A19         | GEN:0 - Switch3 - MiComet - Switch3 - SoraRoboAzki - Switch3 -GEN:1         | 2045      | /21     |
| A20         | GEN:1 - Gamers                                                              | 2         | /30     |
| A21         | Gamers - Switch13 - Korone - Switch13 - Okayu - Switch13 - Mio              | 120       | /25     |
| A22         | GEN:1 - Member - FBK_Matsuri - Member - Aki_Hachama                         | 470       | /23     |
| TOTAL       |                                                                             | 4263      | /19     |

## VLSM

Metode VLSM Sendiri disini digunakan pada Cisco Packet Tracer `CPT`

### TREE VLSM

Berikut Treenya :

![alt text](<img/VLSM Tree.png>)

## PEMBAGIAN IP VLSM

Berikut Pembagian IPnya :

| Subnet | Network ID      | Netmask         | Broadcast    | IP Range                    |
| ------ | --------------- | --------------- | ------------ | --------------------------- |
| A19    | 10.77.0.0/21    | 255.255.248.0   | 10.77.7.255  | 10.77.0.1 - 10.77.7.254     |
| A11    | 10.77.8.0/22    | 255.255.252.0   | 10.77.11.255 | 10.77.8.1 - 10.77.11.254    |
| A22    | 10.77.12.0/23   | 255.255.254.0   | 10.77.13.255 | 10.77.12.1 - 10.77.13.254   |
| A15    | 10.77.14.0/23   | 255.255.254.0   | 10.77.15.255 | 10.77.14.1 - 10.77.15.254   |
| A3     | 10.77.16.0/23   | 255.255.254.0   | 10.77.17.255 | 10.77.16.1 - 10.77.17.254   |
| A21    | 10.77.18.0/25   | 255.255.255.128 | 10.77.18.127 | 10.77.18.1 - 10.77.18.126   |
| A13    | 10.77.18.128/26 | 255.255.255.192 | 10.77.18.191 | 10.77.18.129 - 10.77.18.190 |
| A8     | 10.77.18.192/26 | 255.255.255.192 | 10.77.18.255 | 10.77.18.193 - 10.77.18.254 |
| A5     | 10.77.19.0/27   | 255.255.255.224 | 10.77.19.31  | 10.77.19.1 - 10.77.19.30    |
| A18    | 10.77.19.32/28  | 255.255.255.240 | 10.77.19.47  | 10.77.19.33 - 10.77.19.46   |
| A6     | 10.77.19.48/29  | 255.255.255.248 | 10.77.19.55  | 10.77.19.49 - 10.77.19.54   |
| A7     | 10.77.19.56/29  | 255.255.255.248 | 10.77.19.63  | 10.77.19.57 - 10.77.19.62   |
| A17    | 10.77.19.64/29  | 255.255.255.248 | 10.77.19.71  | 10.77.19.65 - 10.77.19.70   |
| A1     | 10.77.19.72/30  | 255.255.255.252 | 10.77.19.75  | 10.77.19.73 - 10.77.19.74   |
| A2     | 10.77.19.76/30  | 255.255.255.252 | 10.77.19.79  | 10.77.19.77 - 10.77.19.78   |
| A4     | 10.77.19.80/30  | 255.255.255.252 | 10.77.19.83  | 10.77.19.81 - 10.77.19.82   |
| A9     | 10.77.19.84/30  | 255.255.255.252 | 10.77.19.87  | 10.77.19.85 - 10.77.19.86   |
| A10    | 10.77.19.88/30  | 255.255.255.252 | 10.77.19.91  | 10.77.19.89 - 10.77.19.90   |
| A12    | 10.77.19.92/30  | 255.255.255.252 | 10.77.19.95  | 10.77.19.93 - 10.77.19.94   |
| A14    | 10.77.19.96/30  | 255.255.255.252 | 10.77.19.99  | 10.77.19.97 - 10.77.19.98   |
| A16    | 10.77.19.100/30 | 255.255.255.252 | 10.77.19.103 | 10.77.19.101 - 10.77.19.102 |
| A20    | 10.77.19.104/30 | 255.255.255.252 | 10.77.19.107 | 10.77.19.105 - 10.77.19.106 |

## KONFIGURASI

## CIDR

Metode CIDR disini menggunakan GNS3 untuk pengaplikasiannya

### Topologi CIDR |GNS3|

Gabungan 1

![alt text](<img/topo A.jpg>)

Gabungan 2

![alt text](<img/topo B.jpg>)

Gabungan 3

![alt text](<img/topo C.jpg>)

Gabungan 4

![alt text](<img/topo D.jpg>)

Gabungan 5

![alt text](<img/topo E.jpg>)

Gabungan 6

![alt text](<img/topo F.jpg>)

Gabungan 7

![alt text](<img/topo G.jpg>)

Gabungan 8

![alt text](<img/topo H.jpg>)

Gabungan 9

![alt text](<img/topo I.jpg>)

Gabungan 10

![alt text](<img/topo J.jpg>)

### Penggabungan Netmask

![alt text](<img/gabungan i-iv.png>)

![alt text](<img/gabungan v-ix.png>)

### Tree CIDR 

![alt text](<img/cidr tree.jpg>)

### Pembagian IP CIDR

![alt text](<img/pembagian IP cidr.png>)