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

### GNS3 | CIDR |

## RUTE SUBNET

| Nama Subnet | Rute                                                                        | Jumlah IP | Netmask |
| ----------- | --------------------------------------------------------------------------- | --------- | ------- |
| A1          | HoloLive - HoloEn                                                           | 2         | /30     |
| A2          | HoloEn - Router0                                                            | 2         | /30     |
| A3          | Router0 - Switch2 - Gura_Ayne_Ina - Switch2 - Kiara_Calli                   | 503       | /23     |
| A4          | HoloEn - HoloAdvent                                                         | 2         | /30     |
| A5          | HoloAdvent - Switch0 - FuwaMoco - Switch0 - ShioriNerissa - Switch- - Biboo | 27        | /27     |
| A6          | Router0 - HoloPromise - HoloCouncil - HoloPromise - Router4                 | 3         | /29     |
| A7          | Router4 - Tys                                                               | 4         | /29     |
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

![alt text](<img/VMLS Tree.png>)

## PEMBAGIAN IP VLSM

Berikut Pembagian IPnya :

| Subnet | Network ID | Netmask         | Broadcast | IP Range        |
| ------ | ---------- | --------------- | --------- | --------------- |
| A1     | 10.77.     | 255.255.255.252 | 10.77.    | 10.77. - 10.77. |
| A2     | 10.77.     | 255.255.255.252 | 10.77.    | 10.77. - 10.77. |
| A3     | 10.77.     | 255.255.254.0   | 10.77.    | 10.77. - 10.77. |
| A4     | 10.77.     | 255.255.255.252 | 10.77.    | 10.77. - 10.77. |
| A5     | 10.77.     | 255.255.255.224 | 10.77.    | 10.77. - 10.77. |
| A6     | 10.77.     | 255.255.255.248 | 10.77.    | 10.77. - 10.77. |
| A7     | 10.77.     | 255.255.255.248 | 10.77.    | 10.77. - 10.77. |
| A8     | 10.77.     | 255.255.255.192 | 10.77.    | 10.77. - 10.77. |
| A9     | 10.77.     | 255.255.255.252 | 10.77.    | 10.77. - 10.77. |
| A10    | 10.77.     | 255.255.255.252 | 10.77.    | 10.77. - 10.77. |
| A11    | 10.77.     | 255.255.252.0   | 10.77.    | 10.77. - 10.77. |
| A12    | 10.77.     | 255.255.255.252 | 10.77.    | 10.77. - 10.77. |
| A13    | 10.77.     | 255.255.255.192 | 10.77.    | 10.77. - 10.77. |
| A14    | 10.77.     | 255.255.255.252 | 10.77.    | 10.77. - 10.77. |
| A15    | 10.77.     | 255.255.254.0   | 10.77.    | 10.77. - 10.77. |
| A16    | 10.77.     | 255.255.255.252 | 10.77.    | 10.77. - 10.77. |
| A17    | 10.77.     | 255.255.255.248 | 10.77.    | 10.77. - 10.77. |
| A18    | 10.77.     | 255.255.255.240 | 10.77.    | 10.77. - 10.77. |
| A19    | 10.77.     | 255.255.248.0   | 10.77.    | 10.77. - 10.77. |
| A20    | 10.77.     | 255.255.255.252 | 10.77.    | 10.77. - 10.77. |
| A21    | 10.77.     | 255.255.255.128 | 10.77.    | 10.77. - 10.77. |
| A22    | 10.77.     | 255.255.254.0   | 10.77.    | 10.77. - 10.77. |

## KONFIGURASI
