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

### GNS3 | CIDR |

## RUTE SUBNET

| Nama Subnet | Rute                                                                        | Jumlah IP | Netmask               |
| ----------- | --------------------------------------------------------------------------- | --------- | --------------------- |
| A1          | HoloLive - HoloEn                                                           | 2         | /30                   |
| A2          | HoloEn - Router0                                                            | 2         | /30                   |
| A3          | Router0 - Switch2 - Gura_Ayne_Ina - Switch2 - Kiara_Calli                   | 503       | /23                   |
| A4          | HoloEn - HoloAdvent                                                         | 2         | /30                   |
| A5          | HoloAdvent - Switch0 - FuwaMoco - Switch0 - ShioriNerissa - Switch- - Biboo | 27        | /27                   |
| A6          | Router0 - HoloPromise - HoloCouncil - HoloPromise - Router4                 | 3         | /29                   |
| A7          | Router4 - Tys                                                               | 4         | /29                   |
| A8          | HoloCouncil - Switch4 - KroniMumei - Switch4 - BaeFauna                     | 62        | /26                   |
| A9          | GEN 1                                                                       | 4         | /30 (255.255.255.252) |
| A10         | GEN 2                                                                       | 4         | /30 (255.255.255.252) |
| A11         | DEV_IS                                                                      | 9         | /28 (255.255.255.240) |
| A12         | Kuroe_Kurueme                                                               | 29        | /27 (255.255.255.224) |
| A13         | Sora_Beta_2                                                                 | 42        | /26 (255.255.255.192) |

## VLSM

Metode VLSM Sendiri disini digunakan pada Cisco Packet Tracer `CPT`

### TREE VLSM

Berikut Treenya :

## PEMBAGIAN IP VLSM

Berikut Pembagian IPnya :

| Subnet | Network ID  | Netmask               | Broadcast   | IP Range                  |
| ------ | ----------- | --------------------- | ----------- | ------------------------- |
| A1     | 10.77.0.0   | /27 (255.255.255.224) | 10.77.0.31  | 10.77.0.1 - 10.77.0.30    |
| A2     | 10.77.0.32  | /27 (255.255.255.224) | 10.77.0.63  | 10.77.0.33 - 10.77.0.62   |
| A3     | 10.77.0.64  | /29 (255.255.255.248) | 10.77.0.71  | 10.77.0.65 - 10.77.0.70   |
| A4     | 10.77.0.72  | /27 (255.255.255.224) | 10.77.0.103 | 10.77.0.73 - 10.77.0.102  |
| A5     | 10.77.0.104 | /27 (255.255.255.224) | 10.77.0.135 | 10.77.0.105 - 10.77.0.134 |
| A6     | 10.77.0.136 | /26 (255.255.255.192) | 10.77.0.199 | 10.77.0.137 - 10.77.0.198 |
| A7     | 10.77.0.200 | /25 (255.255.255.128) | 10.77.0.255 | 10.77.0.201 - 10.77.0.254 |
| A8     | 10.77.1.0   | /28 (255.255.255.240) | 10.77.1.15  | 10.77.1.1 - 10.77.1.14    |
| A9     | 10.77.1.16  | /30 (255.255.255.252) | 10.77.1.19  | 10.77.1.17 - 10.77.1.18   |
| A10    | 10.77.1.20  | /30 (255.255.255.252) | 10.77.1.23  | 10.77.1.21 - 10.77.1.22   |
| A11    | 10.77.1.24  | /28 (255.255.255.240) | 10.77.1.39  | 10.77.1.25 - 10.77.1.38   |
| A12    | 10.77.1.40  | /27 (255.255.255.224) | 10.77.1.71  | 10.77.1.41 - 10.77.1.70   |
| A13    | 10.77.1.72  | /26 (255.255.255.192) | 10.77.1.135 | 10.77.1.73 - 10.77.1.134  |

## KONFIGURASI
