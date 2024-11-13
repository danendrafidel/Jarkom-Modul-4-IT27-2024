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

### GNS3 | CIDR |

![alt text](<img/Topologi GNS.png>)

### Cisco Packet Tracer | VLSM |

![alt text](<img/Topologi CPT.png>)

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

| Subnet | Network ID  | Netmask         | Broadcast    | IP Range                  |
| ------ | ----------- | --------------- | ------------ | ------------------------- |
| A1     | 10.77.0.240 | 255.255.255.252 | 10.77.0.243  | 10.77.0.241 - 10.77.0.242 |
| A2     | 10.77.0.244 | 255.255.255.252 | 10.77.0.247  | 10.77.0.245 - 10.77.0.246 |
| A3     | 10.77.2.0   | 255.255.254.0   | 10.77.3.255  | 10.77.2.1 - 10.77.3.254   |
| A4     | 10.77.0.248 | 255.255.255.252 | 10.77.0.251  | 10.77.0.249 - 10.77.0.250 |
| A5     | 10.77.0.128 | 255.255.255.224 | 10.77.0.159  | 10.77.0.129 - 10.77.0.158 |
| A6     | 10.77.0.208 | 255.255.255.248 | 10.77.0.215  | 10.77.0.209 - 10.77.0.214 |
| A7     | 10.77.0.216 | 255.255.255.248 | 10.77.0.223  | 10.77.0.217 - 10.77.0.222 |
| A8     | 10.77.0.0   | 255.255.255.192 | 10.77.0.63   | 10.77.0.1 - 10.77.0.62    |
| A9     | 10.77.0.252 | 255.255.255.252 | 10.77.0.255  | 10.77.0.253 - 10.77.0.254 |
| A10    | 10.77.1.0   | 255.255.255.252 | 10.77.1.3    | 10.77.1.1 - 10.77.1.2     |
| A11    | 10.77.8.0   | 255.255.252.0   | 10.77.11.255 | 10.77.8.1 - 10.77.11.254  |
| A12    | 10.77.1.4   | 255.255.255.252 | 10.77.1.7    | 10.77.1.5 - 10.77.1.6     |
| A13    | 10.77.0.64  | 255.255.255.192 | 10.77.0.127  | 10.77.0.65 - 10.77.0.126  |
| A14    | 10.77.1.8   | 255.255.255.252 | 10.77.1.11   | 10.77.1.9 - 10.77.1.10    |
| A15    | 10.77.4.0   | 255.255.254.0   | 10.77.5.255  | 10.77.4.1 - 10.77.5.254   |
| A16    | 10.77.1.12  | 255.255.255.252 | 10.77.1.15   | 10.77.1.13 - 10.77.1.14   |
| A17    | 10.77.0.224 | 255.255.255.248 | 10.77.0.231  | 10.77.0.225 - 10.77.0.230 |
| A18    | 10.77.0.192 | 255.255.255.240 | 10.77.0.207  | 10.77.0.193 - 10.77.0.206 |
| A19    | 10.77.16.0  | 255.255.248.0   | 10.77.23.255 | 10.77.16.1 - 10.77.23.254 |
| A20    | 10.77.1.16  | 255.255.255.252 | 10.77.1.19   | 10.77.1.17 - 10.77.1.18   |
| A21    | 10.77.0.160 | 255.255.255.128 | 10.77.0.191  | 10.77.0.161 - 10.77.0.190 |
| A22    | 10.77.6.0   | 255.255.254.0   | 10.77.7.255  | 10.77.6.1 - 10.77.7.254   |

## KONFIGURASI
