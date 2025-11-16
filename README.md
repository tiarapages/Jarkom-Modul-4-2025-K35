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
| A3 | Inter-Router (Valinor - Valmar - Formost) via Switch2 | 3 (Router Interfaces) | 3 (Router Interfaces) | 8 (/29) |
| A4 | Eregion > Mirkwood (23), Morgul (102) | 125 | 126 | 128 (/25) |
| A5 | Valmar > Imrahil (27), Gwaith (4), Utumno (2) | 33 | 34 | 64 (/26) |
| A6 | Gudhur > Palantir (46), Edhil (73) | 119 | 120 | 128 (/25) |
| A7 | Gudhur > IronCrown (5), Hobbiton (4), Grond (4) | 13 | 14 | 16 (/28) |
| A8 | Numenor > Arthadain (246), Mirdain (628) | 874 | 875 | 1024 (/22) |
| A9 | Melkor > PC Harad? (252), Server Melkor (250) | 502 | 503 | 512 (/23) |
| A10 | Erain > Balrog (256), Gothmog (84), Thranduil (129) | 469 | 470 | 512 (/23) |
| A11 | Anor > Beacon (279), Silmaril (381) | 660 | 661 | 1024 (/22) |
| A12 | Throne > Server Erebor (2) | 2 | 3 | 8 (/29) |
| A13 | Morgoth > Erendis (27), Elrond (34) | 61 | 62 | 64 (/26) |
| A14 | WAN Amroth <--> Morgoth | 2 (Point-to-Point) | 2 (Point-to-Point) | 4 (/30) |
| A15 | WAN Minastir <--> Amroth | 2 (Point-to-Point) | 2 (Point-to-Point) | 4 (/30) |
| A16 | WAN Minastir <--> Anor | 2 (Point-to-Point) | 2 (Point-to-Point) | 4 (/30) |
| A17 | WAN Amonsul <--> Minastir | 2 (Point-to-Point) | 2 (Point-to-Point) | 4 (/30) |
| A18 | WAN Formost <--> Amonsul | 2 (Point-to-Point) | 2 (Point-to-Point) | 4 (/30) |
| A19 | WAN Amonsul <--> Eregion | 2 (Point-to-Point) | 2 (Point-to-Point) | 4 (/30) |
| A20 | WAN Eregion <--> Gudhur | 2 (Point-to-Point) | 2 (Point-to-Point) | 4 (/30) |
| A21 | WAN Gudhur <--> Numenor | 2 (Point-to-Point) | 2 (Point-to-Point) | 4 (/30) |
| A22 | WAN Numenor <--> Melkor | 2 (Point-to-Point) | 2 (Point-to-Point) | 4 (/30) |
| A23 | WAN Melkor <--> Erain | 2 (Point-to-Point) | 2 (Point-to-Point) | 4 (/30) |

# Hasil Topologi VLSM
<img width="1170" height="649" alt="image" src="https://github.com/user-attachments/assets/0d981e30-f66c-4a6e-8849-ee0813edac3c" />

# Hasil Tabel Subnet VLSM
| Subnet | Network ID | Netmask | Broadcast | Range IP |
| :--- | :--- | :--- | :--- | :--- |
| A8 | 10.81.0.0 | 255.255.252.0 | 10.81.3.255 | 10.81.0.1 - 10.81.3.254 |
| A11 | 10.81.4.0 | 255.255.252.0 | 10.81.7.255 | 10.81.4.1 - 10.81.7.254 |
| A9 | 10.81.8.0 | 255.255.254.0 | 10.81.9.255 | 10.81.8.1 - 10.81.9.254 |
| A10 | 10.81.10.0 | 255.255.254.0 | 10.81.11.255 | 10.81.10.1 - 10.81.11.254 |
| A1 | 10.81.12.0 | 255.255.254.0 | 10.81.13.255 | 10.81.12.1 - 10.81.13.254 |
| A4 | 10.81.14.0 | 255.255.255.128 | 10.81.14.127 | 10.81.14.1 - 10.81.14.126 |
| A6 | 10.81.14.128 | 255.255.255.128 | 10.81.14.255 | 10.81.14.129 - 10.81.14.254 |
| A13 | 10.81.15.0 | 255.255.255.192 | 10.81.15.63 | 10.81.15.1 - 10.81.15.62 |
| A5 | 10.81.15.64 | 255.255.255.192 | 10.81.15.127 | 10.81.15.65 - 10.81.15.126 |
| A2 | 10.81.15.128 | 255.255.255.224 | 10.81.15.159 | 10.81.15.129 - 10.81.15.158 |
| A7 | 10.81.15.160 | 255.255.255.240 | 10.81.15.175 | 10.81.15.161 - 10.81.15.174 |
| A3 | 10.81.15.176 | 255.255.255.248 | 10.81.15.183 | 10.81.15.177 - 10.81.15.182 |
| A12 | 10.81.15.184 | 255.255.255.248 | 10.81.15.191 | 10.81.15.185 - 10.81.15.190 |
| A14 | 10.81.15.192 | 255.255.255.252 | 10.81.15.195 | 10.81.15.193 - 10.81.15.194 |
| A15 | 10.81.15.196 | 255.255.255.252 | 10.81.15.199 | 10.81.15.197 - 10.81.15.198 |
| A16 | 10.81.15.200 | 255.255.255.252 | 10.81.15.203 | 10.81.15.201 - 10.81.15.202 |
| A17 | 10.81.15.204 | 255.255.255.252 | 10.81.15.207 | 10.81.15.205 - 10.81.15.206 |
| A18 | 10.81.15.208 | 255.255.255.252 | 10.81.15.211 | 10.81.15.209 - 10.81.15.210 |
| A19 | 10.81.15.212 | 255.255.255.252 | 10.81.15.215 | 10.81.15.213 - 10.81.15.214 |
| A20 | 10.81.15.216 | 255.255.255.252 | 10.81.15.219 | 10.81.15.217 - 10.81.15.218 |
| A21 | 10.81.15.220 | 255.255.255.252 | 10.81.15.223 | 10.81.15.221 - 10.81.15.222 |
| A22 | 10.81.15.224 | 255.255.255.252 | 10.81.15.227 | 10.81.15.225 - 10.81.15.226 |
| A23 | 10.81.15.228 | 255.255.255.252 | 10.81.15.231 | 10.81.15.229 - 10.81.15.230 |

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


# Penggabungan CIDR

<img width="1680" height="938" alt="Frame A" src="https://github.com/user-attachments/assets/bae785cf-5a8d-4c5a-8f5f-fd9abf6ce244" />

# Tree CIDR

<img width="1090" height="788" alt="Frame 5" src="https://github.com/user-attachments/assets/ce21ce64-bfbb-4529-b57c-df67cbe95ea5" />


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

