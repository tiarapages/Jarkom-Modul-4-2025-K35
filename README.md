# Jarkom-Modul-4-2025-K35

| Nama | NRP |
|---|---|
| Tiara Putri Prasetya | 5027241013 |
| Naufal Ardhana | 5027241118 |

# Tabel Subnetting IP
| Nama Subnet | Rute | Jumlah IP | Jumlah IP + 1 | Netmask |
| :--- | :--- | :--- | :--- | :--- |
| A1 | Valinor > Shadow (99), Anarion (67), Lindon (132) | 298 | 299 | 512 (/23) |
| A2 | Valmar > Doriath (17), Arnor (10) | 27 | 28 | 32 (/27) |
| A3 | Inter-Router (Valinor - Valmar - Formost) via Switch | 3 (Router Interfaces) | 3 (Router Interfaces) | 8 (/29) |
| A4 | Eregion > Mirkwood (23), Morgul (102) | 125 | 126 | 128 (/25) |
| A5 | Valmar > Imrahil (27), Gwaith (4), Utumno (2) | 33 | 34 | 64 (/26) |
| A6 | Gudhur > Palantir (46), Edhil (73) | 119 | 120 | 128 (/25) |
| A7 | Gudhur > IronCrown (5), Hobbiton (4), Grond (4) | 13 | 14 | 16 (/28) |
| A8 | Numenor > Arthadain (246), Mirdain (628) | 874 | 875 | 1024 (/22) |
| A9 | Melkor > PC Khazad (252), Server Melkor (250) | 502 | 503 | 512 (/23) |
| A10 | Erain > Balrog (256), Gothmog (84), Thranduil (129) | 469 | 470 | 512 (/23) |
| A11 | Anor > Beacon (279), Silmaril (381) | 660 | 661 | 1024 (/22) |
| A12 | Throne > Server Erebor (2) | 2 | 3 | 8 (/29) |
| A13 | Morgoth > Erendis (27), Elrond (34) | 61 | 62 | 64 (/26) |
| A14 | Inter-Router (Amroth - Throne - Morgoth) via Switch | 3 (Router Interfaces) | 3 (Router Interfaces) | 8 (/29) |
| A15 | WAN Minastir <--> Amroth | 2 (Point-to-Point) | 2 (Point-to-Point) | 4 (/30) |
| A16 | WAN Minastir <--> Anor | 2 (Point-to-Point) | 2 (Point-to-Point) | 4 (/30) |
| A17 | WAN Amonsul <--> Minastir | 2 (Point-to-Point) | 2 (Point-to-Point) | 4 (/30) |
| A18 | WAN Formost <--> Amonsul | 2 (Point-to-Point) | 2 (Point-to-Point) | 4 (/30) |
| A19 | WAN Amonsul <--> Eregion | 2 (Point-to-Point) | 2 (Point-to-Point) | 4 (/30) |
| A20 | WAN Eregion <--> Numenor | 2 (Point-to-Point) | 2 (Point-to-Point) | 4 (/30) |
| A21 | WAN Guldur <--> Numenor | 2 (Point-to-Point) | 2 (Point-to-Point) | 4 (/30) |
| A22 | WAN Numenor <--> Mordor | 2 (Point-to-Point) | 2 (Point-to-Point) | 4 (/30) |
| A23 | WAN Mordor <--> Erain | 2 (Point-to-Point) | 2 (Point-to-Point) | 4 (/30) |

# Hasil Topologi VLSM
<img width="1170" height="649" alt="image" src="https://github.com/user-attachments/assets/0d981e30-f66c-4a6e-8849-ee0813edac3c" />

# Tabel Subnet yang benar
| Subnet | Network ID     | Netmask             | Broadcast        | Range IP                            |
|--------|----------------|---------------------|------------------|-------------------------------------|
| A8     | 10.81.0.0      | 255.255.252.0 (/22) | 10.81.3.255      | 10.81.0.1 - 10.81.3.254             |
| A11    | 10.81.4.0      | 255.255.252.0 (/22) | 10.81.7.255      | 10.81.4.1 - 10.81.7.254             |
| A9     | 10.81.8.0      | 255.255.254.0 (/23) | 10.81.9.255      | 10.81.8.1 - 10.81.9.254             |
| A10    | 10.81.10.0     | 255.255.254.0 (/23) | 10.81.11.255     | 10.81.10.1 - 10.81.11.254           |
| A1     | 10.81.12.0     | 255.255.254.0 (/23) | 10.81.13.255     | 10.81.12.1 - 10.81.13.254           |
| A4     | 10.81.14.0     | 255.255.255.128 (/25)| 10.81.14.127    | 10.81.14.1 - 10.81.14.126           |
| A6     | 10.81.14.128   | 255.255.255.128 (/25)| 10.81.14.255    | 10.81.14.129 - 10.81.14.254         |
| A13    | 10.81.15.0     | 255.255.255.192 (/26)| 10.81.15.63     | 10.81.15.1 - 10.81.15.62            |
| A5     | 10.81.15.64    | 255.255.255.192 (/26)| 10.81.15.127    | 10.81.15.65 - 10.81.15.126          |
| A2     | 10.81.15.128   | 255.255.255.224 (/27)| 10.81.15.159    | 10.81.15.129 - 10.81.15.158         |
| A7     | 10.81.15.160   | 255.255.255.240 (/28)| 10.81.15.175    | 10.81.15.161 - 10.81.15.174         |
| A3     | 10.81.15.176   | 255.255.255.248 (/29)| 10.81.15.183    | 10.81.15.177 - 10.81.15.182         |
| A12    | 10.81.15.184   | 255.255.255.248 (/29)| 10.81.15.191    | 10.81.15.185 - 10.81.15.190         |
| A14    | 10.81.15.192   | 255.255.255.248 (/29)| 10.81.15.199    | 10.81.15.193 - 10.81.15.198         |
| A15    | 10.81.15.200   | 255.255.255.252 (/30)| 10.81.15.203    | 10.81.15.201 - 10.81.15.202         |
| A16    | 10.81.15.204   | 255.255.255.252 (/30)| 10.81.15.207    | 10.81.15.205 - 10.81.15.206         |
| A17    | 10.81.15.208   | 255.255.255.252 (/30)| 10.81.15.211    | 10.81.15.209 - 10.81.15.210         |
| A18    | 10.81.15.212   | 255.255.255.252 (/30)| 10.81.15.215    | 10.81.15.213 - 10.81.15.214         |
| A19    | 10.81.15.216   | 255.255.255.252 (/30)| 10.81.15.219    | 10.81.15.217 - 10.81.15.218         |
| A20    | 10.81.15.220   | 255.255.255.252 (/30)| 10.81.15.223    | 10.81.15.221 - 10.81.15.222         |
| A21    | 10.81.15.224   | 255.255.255.252 (/30)| 10.81.15.227    | 10.81.15.225 - 10.81.15.226         |
| A22    | 10.81.15.228   | 255.255.255.252 (/30)| 10.81.15.231    | 10.81.15.229 - 10.81.15.230         |
| A23    | 10.81.15.232   | 255.255.255.252 (/30)| 10.81.15.235    | 10.81.15.233 - 10.81.15.234         |


### nyoba
| Subnet | Prefix | Netmask | Network ID | Range IP | Broadcast |
|:---|:---|:---|:---|:---|:---|
| A8 | /22 | 255.255.252.0 | 10.81.0.0 | 10.81.0.1 - 10.81.3.254 | 10.81.3.255 |
| A11 | /22 | 255.255.252.0 | 10.81.4.0 | 10.81.4.1 - 10.81.7.254 | 10.81.7.255 |
| A1 | /23 | 255.255.254.0 | 10.81.8.0 | 10.81.8.1 - 10.81.9.254 | 10.81.9.255 |
| A9 | /23 | 255.255.254.0 | 10.81.10.0 | 10.81.10.1 - 10.81.11.254 | 10.81.11.255 |
| A10 | /23 | 255.255.254.0 | 10.81.12.0 | 10.81.12.1 - 10.81.13.254 | 10.81.13.255 |
| A4 | /25 | 255.255.255.128 | 10.81.14.0 | 10.81.14.1 - 10.81.14.126 | 10.81.14.127 |
| A6 | /25 | 255.255.255.128 | 10.81.14.128 | 10.81.14.129 - 10.81.14.254 | 10.81.14.255 |
| A5 | /26 | 255.255.255.192 | 10.81.15.0 | 10.81.15.1 - 10.81.15.62 | 10.81.15.63 |
| A13 | /26 | 255.255.255.192 | 10.81.15.64 | 10.81.15.65 - 10.81.15.126 | 10.81.15.127 |
| A2 | /27 | 255.255.255.224 | 10.81.15.128 | 10.81.15.129 - 10.81.15.158 | 10.81.15.159 |
| A7 | /28 | 255.255.255.240 | 10.81.15.160 | 10.81.15.161 - 10.81.15.174 | 10.81.15.175 |
| A3 | /29 | 255.255.255.248 | 10.81.15.176 | 10.81.15.177 - 10.81.15.182 | 10.81.15.183 |
| A12 | /29 | 255.255.255.248 | 10.81.15.184 | 10.81.15.185 - 10.81.15.190 | 10.81.15.191 |
| A14 | /29 | 255.255.255.248 | 10.81.15.192 | 10.81.15.193 - 10.81.15.198 | 10.81.15.199 |
| A15 | /30 | 255.255.255.252 | 10.81.15.200 | 10.81.15.201 - 10.81.15.202 | 10.81.15.203 |
| A16 | /30 | 255.255.255.252 | 10.81.15.204 | 10.81.15.205 - 10.81.15.206 | 10.81.15.207 |
| A17 | /30 | 255.255.255.252 | 10.81.15.208 | 10.81.15.209 - 10.81.15.210 | 10.81.15.211 |
| A18 | /30 | 255.255.255.252 | 10.81.15.212 | 10.81.15.213 - 10.81.15.214 | 10.81.15.215 |
| A19 | /30 | 255.255.255.252 | 10.81.15.216 | 10.81.15.217 - 10.81.15.218 | 10.81.15.219 |
| A20 | /30 | 255.255.255.252 | 10.81.15.220 | 10.81.15.221 - 10.81.15.222 | 10.81.15.223 |
| A21 | /30 | 255.255.255.252 | 10.81.15.224 | 10.81.15.225 - 10.81.15.226 | 10.81.15.227 |
| A22 | /30 | 255.255.255.252 | 10.81.15.228 | 10.81.15.229 - 10.81.15.230 | 10.81.15.231 |
| A23 | /30 | 255.255.255.252 | 10.81.15.232 | 10.81.15.233 - 10.81.15.234 | 10.81.15.235 |

### Tabel Alokasi IP per Unit (Diurutkan per Subnet)

| Subnet | Unit / Interface | IP Address |
|:---|:---|:---|
| **A8 (/22)** | Router (Gateway Numenor) | `10.81.0.1` |
| A8 | Host Block (Arthadain) | `10.81.0.2` |
| A8 | Host Block (Mirdain) | `10.81.0.3` |
| **A11 (/22)** | Router (Gateway Anor) | `10.81.4.1` |
| A11 | Host Block (Beacon) | `10.81.4.2` |
| A11 | Host Block (Silmaril) | `10.81.4.3` |
| **A1 (/23)** | Router (Gateway Valinor) | `10.81.8.1` |
| A1 | Host Block (Shadow) | `10.81.8.2` |
| A1 | Host Block (Anarion) | `10.81.8.3` |
| A1 | Host Block (Lindon) | `10.81.8.4` |
| **A9 (/23)** | Router (Gateway Melkor) | `10.81.10.1` |
| A9 | Host Block (PC Khazad) | `10.81.10.2` |
| A9 | Host Block (Server Melkor) | `10.81.10.3` |
| **A10 (/23)** | Router (Gateway Erain) | `10.81.12.1` |
| A10 | Host Block (Balrog) | `10.81.12.2` |
| A10 | Host Block (Gothmog) | `10.81.12.3` |
| A10 | Host Block (Thranduil) | `10.81.12.4` |
| **A4 (/25)** | Router (Gateway Eregion) | `10.81.14.1` |
| A4 | Host Block (Mirkwood) | `10.81.14.2` |
| A4 | Host Block (Morgul) | `10.81.14.3` |
| **A6 (/25)** | Router (Gateway Gudhur) | `10.81.14.129` |
| A6 | Host Block (Palantir) | `10.81.14.130` |
| A6 | Host Block (Edhil) | `10.81.14.131` |
| **A5 (/26)** | Router (Gateway Valmar) | `10.81.15.1` |
| A5 | Host Block (Imrahil) | `10.81.15.2` |
| A5 | Host Block (Gwaith) | `10.81.15.3` |
| A5 | Host Block (Utumno) | `10.81.15.4` |
| **A13 (/26)** | Router (Gateway Morgoth) | `10.81.15.65` |
| A13 | Host Block (Erendis) | `10.81.15.66` |
| A13 | Host Block (Elrond) | `10.81.15.67` |
| **A2 (/27)** | Router (Gateway Valmar) | `10.81.15.129` |
| A2 | Host Block (Doriath) | `10.81.15.130` |
| A2 | Host Block (Arnor) | `10.81.15.131` |
| **A7 (/28)** | Router (Gateway Gudhur) | `10.81.15.161` |
| A7 | Host Block (IronCrown) | `10.81.15.162` |
| A7 | Host Block (Hobbiton) | `10.81.15.163` |
| A7 | Host Block (Grond) | `10.81.15.164` |
| **A3 (/29)** | Router Interface (Valinor) | `10.81.15.177` |
| A3 | Router Interface (Valmar) | `10.81.15.178` |
| A3 | Router Interface (Formost) | `10.81.15.179` |
| **A12 (/29)** | Router (Gateway Throne) | `10.81.15.185` |
| A12 | Server (Erebor 1) | `10.81.15.186` |
| A12 | Server (Erebor 2) | `10.81.15.187` |
| **A14 (/29)** | Router Interface (Amroth) | `10.81.15.193` |
| A14 | Router Interface (Throne) | `10.81.15.194` |
| A14 | Router Interface (Morgoth) | `10.81.15.195` |
| **A15 (/30)** | Router Interface (Minastir) | `10.81.15.201` |
| A15 | Router Interface (Amroth) | `10.81.15.202` |
| **A16 (/30)** | Router Interface (Minastir) | `10.81.15.205` |
| A16 | Router Interface (Anor) | `10.81.15.206` |
| **A17 (/30)** | Router Interface (Amonsul) | `10.81.15.209` |
| A17 | Router Interface (Minastir) | `10.81.15.210` |
| **A18 (/30)** | Router Interface (Formost) | `10.81.15.213` |
| A18 | Router Interface (Amonsul) | `10.81.15.214` |
| **A19 (/30)** | Router Interface (Amonsul) | `10.81.15.217` |
| A19 | Router Interface (Eregion) | `10.81.15.218` |
| **A20 (/30)** | Router Interface (Eregion) | `10.81.15.221` |
| A20 | Router Interface (Numenor) | `10.81.15.222` |
| **A21 (/30)** | Router Interface (Guldur) | `10.81.15.225` |
| A21 | Router Interface (Numenor) | `10.81.15.226` |
| **A22 (/30)** | Router Interface (Numenor) | `10.81.15.229` |
| A22 | Router Interface (Mordor) | `10.81.15.230` |
| **A23 (/30)** | Router Interface (Mordor) | `10.81.15.233` |
| A23 | Router Interface (Erain) | `10.81.15.234` |


# Subnet Tree VLSM
<img width="773" height="696" alt="image" src="https://github.com/user-attachments/assets/3e031599-c290-44a0-91ed-06d31525207e" />


# Config Node
```
# A3 (Inter-Router ke Valinor & Formost)
# Ini adalah interface "WAN" Anda.
# Saya asumsikan gateway-nya adalah IP router Formost di subnet A3.
auto eth0
iface eth0 inet static
    address 10.81.15.177
    netmask 255.255.255.248
    gateway 10.81.15.178
    # IP Valmar = 10.81.15.177
    # IP Gateway (misal: Formost) = 10.81.15.178

# A5 (LAN: Imrahil, Gwaith, Utumno)
auto eth1
iface eth1 inet static
    address 10.81.15.65
    netmask 255.255.255.192
    # Network A5 = 10.81.15.64/26
    # IP Gateway (Valmar) = 10.81.15.65

# A2 (LAN: Doriath, Arnor)
auto eth2
iface eth2 inet static
    address 10.81.15.129
    netmask 255.255.255.224
    # Network A2 = 10.81.15.128/27
    # IP Gateway (Valmar) = 10.81.15.129
```

# Konfigurasi Client
```
[PC-Shadow]
Interface=FastEthernet0
IPv4 Address=10.81.12.2
Subnet Mask=255.255.255.192
Default Gateway=10.81.12.1

[Server-Anarion]
Interface=FastEthernet0
IPv4 Address=10.81.11.2
Subnet Mask=255.255.255.128
Default Gateway=10.81.11.1

[Laptop-Lindon]
Interface=FastEthernet0
IPv4 Address=10.81.10.2
Subnet Mask=255.255.255.0
Default Gateway=10.81.10.1

[Laptop-Donath]
Interface=FastEthernet0
IPv4 Address=10.81.13.34
Subnet Mask=255.255.255.224
Default Gateway=10.81.13.33

[Laptop-Arnor]
Interface=FastEthernet0
IPv4 Address=10.81.13.35
Subnet Mask=255.255.255.224
Default Gateway=10.81.13.33

[PC-Imrahil]
Interface=FastEthernet0
IPv4 Address=10.81.13.2
Subnet Mask=255.255.255.224
Default Gateway=10.81.13.1

[PC-Gwaith]
Interface=FastEthernet0
IPv4 Address=10.81.13.66
Subnet Mask=255.255.255.248
Default Gateway=10.81.13.65

[Laptop-Utumno]
Interface=FastEthernet0
IPv4 Address=10.81.13.67
Subnet Mask=255.255.255.248
Default Gateway=10.81.13.65

[PC-Mirkwood]
Interface=FastEthernet0
IPv4 Address=10.81.14.2
Subnet Mask=255.255.255.0
Default Gateway=10.81.14.1

[PC-Morgul]
Interface=FastEthernet0
IPv4 Address=10.81.14.3
Subnet Mask=255.255.255.0
Default Gateway=10.81.14.1

[PC-Erendis]
Interface=FastEthernet0
IPv4 Address=10.81.15.2
Subnet Mask=255.255.255.248
Default Gateway=10.81.15.1

[PC-Harad]
Interface=FastEthernet0
IPv4 Address=10.81.15.10
Subnet Mask=255.255.255.248
Default Gateway=10.81.15.9
```

Router Valinor
```
enable
configure terminal
hostname Valinor-Atas

! Konfigurasi Sub-Interface (Router-on-a-Stick)
interface FastEthernet0/0
 no shutdown
exit

interface FastEthernet0/0.10
 encapsulation dot1Q 10
 ip address 10.81.10.1 255.255.255.0
exit

interface FastEthernet0/0.20
 encapsulation dot1Q 20
 ip address 10.81.11.1 255.255.255.128
exit

interface FastEthernet0/0.30
 encapsulation dot1Q 30
 ip address 10.81.12.1 255.255.255.192
exit

! Interface WAN ke Switch2
interface FastEthernet0/1
 ip address 10.81.15.225 255.255.255.248
 no shutdown
exit

! Konfigurasi EIGRP
router eigrp 100
 no auto-summary
 network 10.81.10.0 0.0.0.255
 network 10.81.11.0 0.0.0.127
 network 10.81.12.0 0.0.0.63
 network 10.81.15.224 0.0.0.7
exit

end
write memory
```
Router Valmar
```
enable
configure terminal
hostname Valinor-Bawah

! Interface WAN ke Switch2
interface FastEthernet0/0
 ip address 10.81.15.227 255.255.255.248
 no shutdown
exit

! Interface LAN ke Donath/Arnor
interface FastEthernet1/0
 ip address 10.81.13.33 255.255.255.224
 no shutdown
exit

! Interface LAN ke Gwaith/Utumno
interface FastEthernet2/1
 ip address 10.81.13.65 255.255.255.248
 no shutdown
exit

! Interface LAN ke Imrahil
interface FastEthernet3/1
 ip address 10.81.13.1 255.255.255.224
 no shutdown
exit

! Konfigurasi EIGRP
router eigrp 100
 no auto-summary
 network 10.81.13.0 0.0.0.31
 network 10.81.13.32 0.0.0.31
 network 10.81.13.64 0.0.0.7
 network 10.81.15.224 0.0.0.7
exit

end
write memory
```
Router Fornost
```
enable
configure terminal
hostname Fornost

! Interface WAN ke Switch2
interface FastEthernet0/0
 ip address 10.81.15.226 255.255.255.248
 no shutdown
exit

! Interface WAN ke Amansul
interface FastEthernet0/1
 ip address 10.81.200.1 255.255.255.252
 no shutdown
exit

! Konfigurasi EIGRP
router eigrp 100
 no auto-summary
 network 10.81.15.224 0.0.0.7
 network 10.81.200.0 0.0.0.3
exit

end
write memory
```
Router Amansul
```
enable
configure terminal
hostname Amansul

! Interface WAN ke ISP/Cloud
interface FastEthernet0/0
 ip address 10.81.200.5 255.255.255.252
 no shutdown
exit

! Interface WAN ke Fornost
interface FastEthernet0/1
 ip address 10.81.200.2 255.255.255.252
 no shutdown
exit

! Interface WAN ke Eregion
interface FastEthernet1/0
 ip address 10.81.200.13 255.255.255.252
 no shutdown
exit

! Interface WAN ke Minastir
interface FastEthernet1/1
 ip address 10.81.200.9 255.255.255.252
 no shutdown
exit

! Rute Default ke Internet
ip route 0.0.0.0 0.0.0.0 10.81.200.6

! Konfigurasi EIGRP dan redistribusi rute default
router eigrp 100
 no auto-summary
 network 10.81.200.0 0.0.0.3
 network 10.81.200.4 0.0.0.3
 network 10.81.200.8 0.0.0.3
 network 10.81.200.12 0.0.0.3
 redistribute static
exit

end
write memory
```
ROuter Eregion
```
enable
configure terminal
hostname Eregion

! Interface WAN ke Amansul
interface FastEthernet0/0
 ip address 10.81.200.14 255.255.255.252
 no shutdown
exit

! Interface WAN ke Numenor
interface FastEthernet0/1
 ip address 10.81.200.17 255.255.255.252
 no shutdown
exit

! Interface LAN ke Morgul/Mirkwood
interface FastEthernet1/0
 ip address 10.81.14.1 255.255.255.0
 no shutdown
exit

! Konfigurasi EIGRP
router eigrp 100
 no auto-summary
 network 10.81.14.0 0.0.0.255
 network 10.81.200.12 0.0.0.3
 network 10.81.200.16 0.0.0.3
exit

end
write memory
```
Router Minastir
```
enable
configure terminal
hostname Minastir

! Interface WAN ke Amansul
interface FastEthernet0/0
 ip address 10.81.200.10 255.255.255.252
 no shutdown
exit

! Konfigurasi EIGRP
router eigrp 100
 no auto-summary
 network 10.81.200.8 0.0.0.3
exit

end
write memory
```
Router Numenor
```
enable
configure terminal
hostname Numenor

! Interface WAN ke Eregion
interface FastEthernet0/0
 ip address 10.81.200.18 255.255.255.252
 no shutdown
exit

! Interface WAN ke Gudur
interface FastEthernet0/1
 ip address 10.81.200.21 255.255.255.252
 no shutdown
exit

! Interface LAN ke Erendis
interface FastEthernet1/0
 ip address 10.81.15.1 255.255.255.248
 no shutdown
exit

! Konfigurasi EIGRP
router eigrp 100
 no auto-summary
 network 10.81.15.0 0.0.0.7
 network 10.81.200.16 0.0.0.3
 network 10.81.200.20 0.0.0.3
exit

end
write memory
```
Router Gudur
```
enable
configure terminal
hostname Gudur

! Interface LAN ke Harad
interface FastEthernet0/0
 ip address 10.81.15.9 255.255.255.248
 no shutdown
exit

! Interface WAN ke Numenor
interface FastEthernet0/1
 ip address 10.81.200.22 255.255.255.252
 no shutdown
exit

! Konfigurasi EIGRP
router eigrp 100
 no auto-summary
 network 10.81.15.8 0.0.0.7
 network 10.81.200.20 0.0.0.3
exit

end
write memory
```



# Penggabungan CIDR

<img width="1680" height="938" alt="Frame A" src="https://github.com/user-attachments/assets/bae785cf-5a8d-4c5a-8f5f-fd9abf6ce244" />

# Tree CIDR

<img width="1090" height="788" alt="Frame 5 (1)" src="https://github.com/user-attachments/assets/b9ee2ede-cac7-4a26-9cd1-6c7befdee321" />



### PERTAMA

<img width="1680" height="938" alt="Frame B" src="https://github.com/user-attachments/assets/b1081360-cc44-4abe-ad6e-346e62533a7a" />

| Subnet | Subnet 1 | Netmask 1 | Subnet 2 | Netmask 2 | Netmask Akhir |
| :--- | :--- | :--- | :--- | :--- | :--- |
| B1 | A1 | /23 | A3 | /29 | /22 |
| B2 | A2 | /27 | A5 | /26 | /25 |
| B3 | A6 | /25 | A7 | /27 | /24 |
| B4 | A10 | /23 | A9 | /23 | /22 |
| B5 | A14 | /29 | A13 | /26 | /25 |
| B6 | A16 | /30 | A11 | /22 | /21 |

---

### KEDUA

<img width="1680" height="938" alt="Frame C" src="https://github.com/user-attachments/assets/912cc11c-5bd1-40f7-8838-74f6012090a6" />

| Subnet | Subnet 1 | Netmask 1 | Subnet 2 | Netmask 2 | Netmask Akhir |
| :--- | :--- | :--- | :--- | :--- | :--- |
| C1 | B1 | /22 | B2 | /25 | /21 |
| C2 | B3 | /24 | A21 | /30 | /23 |
| C3 | B4 | /22 | A23 | /30 | /21 |
| C4 | B5 | /25 | A12 | /29 | /24 |

---

### KETIGA

<img width="1680" height="938" alt="Frame D" src="https://github.com/user-attachments/assets/12d470a6-5a77-4070-8527-e127053002bf" />

| Subnet | Subnet 1 | Netmask 1 | Subnet 2 | Netmask 2 | Netmask Akhir |
| :--- | :--- | :--- | :--- | :--- | :--- |
| D1 | C1 | /21 | A18 | /30 | /20 |
| D2 | C2 | /23 | A8 | /22 | /21 |
| D3 | C3 | /21 | A22 | /30 | /20 |
| D4 | C4 | /24 | A15 | /30 | /23 |

---

### KEEMPAT

<img width="1680" height="938" alt="Frame E (1)" src="https://github.com/user-attachments/assets/4ed941d3-124d-47f4-9763-b9db1f0c9de6" />

| Subnet | Subnet 1 | Netmask 1 | Subnet 2 | Netmask 2 | Netmask Akhir |
| :--- | :--- | :--- | :--- | :--- | :--- |
| E1 | D2 | /21 | D3 | /20 | /19 |
| E2 | D4 | /23 | B6 | /21 | /20 |

---

### KELIMA

<img width="1680" height="938" alt="Frame F (1)" src="https://github.com/user-attachments/assets/7f5bea6a-8b94-4973-81e6-414f4c8225cc" />

| Subnet | Subnet 1 | Netmask 1 | Subnet 2 | Netmask 2 | Netmask Akhir |
| :--- | :--- | :--- | :--- | :--- | :--- |
| F1 | E1 | /19 | A20 | /30 | /18 |
| F2 | E2 | /20 | A17 | /30 | /19 |

---

### KEENAM

<img width="1680" height="938" alt="Frame G (1)" src="https://github.com/user-attachments/assets/9fb00a30-b20d-4b98-a888-eea0c03b5f00" />

| Subnet | Subnet 1 | Netmask 1 | Subnet 2 | Netmask 2 | Netmask Akhir |
| :--- | :--- | :--- | :--- | :--- | :--- |
| G1 | F1 | /18 | A4 | /24 | /17 |

---

### KETUJUH

<img width="1680" height="938" alt="Frame H (1)" src="https://github.com/user-attachments/assets/d4bf6c3f-780c-47e5-a7b8-fe28f605b244" />

| Subnet | Subnet 1 | Netmask 1 | Subnet 2 | Netmask 2 | Netmask Akhir |
| :--- | :--- | :--- | :--- | :--- | :--- |
| H1 | G1 | /17 | A19 | /30 | /16 |

---

### KEDELAPAN

<img width="1680" height="938" alt="Frame I (1)" src="https://github.com/user-attachments/assets/f6dc85da-bc57-4c8a-aecf-1822b8404a40" />

| Subnet | Subnet 1 | Netmask 1 | Subnet 2 | Netmask 2 | Netmask Akhir |
| :--- | :--- | :--- | :--- | :--- | :--- |
| I1 | H1 | /16 | F2 | /19 | /15 |

---

### KESEMBILAN

<img width="1680" height="938" alt="Frame J (1)" src="https://github.com/user-attachments/assets/ea788d94-4099-4b89-b404-e1bbbaf99059" />

| Subnet | Subnet 1 | Netmask 1 | Subnet 2 | Netmask 2 | Netmask Akhir |
| :--- | :--- | :--- | :--- | :--- | :--- |
| J1 | I1 | /15 | D1 | /20 | /14 |

