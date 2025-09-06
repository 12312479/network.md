# network.md
3) Wi‑Fi design (settings and values)

SSID plan

GH-STaff — secured corporate Wi‑Fi

Security: WPA3-Enterprise (if AP + RADIUS support) or WPA2-Enterprise if WPA3 unavailable

Authentication: 802.1X with RADIUS (e.g., FreeRADIUS or Microsoft NPS)

VLAN: Staff VLAN (10)

Band: 2.4 GHz + 5 GHz (dual-band) with band steering enabled

Channel plan: use automatic channel allocation with 20/40/80 MHz on 5 GHz where supported; ensure non-overlapping channels on 2.4 GHz (1,6,11)

Roaming: 802.11r/k (fast roaming) if supported by APs and clients

DTIM/Beacon interval: default 100 ms (adjust per vendor guidance)

GH-Guest — Guest Wi‑Fi

Security: WPA2-Personal or open with captive portal (HTTPS) and time-limited access

VLAN: Guest VLAN (20) with strict ACLs to block internal resource access and allow only internet

Bandwidth limit: apply per-client rate limit (e.g., 5–10 Mbps) on gateway to prevent abuse

GH-IoT — IoT devices (cameras, sensors)

Security: WPA2-PSK with strong passphrase or isolated wired VLAN for devices that cannot do EAP

VLAN: IoT VLAN (30) with firewall rules permitting only specific outbound flows

Important AP settings (example values)

Transmit power: set to auto; for high-density areas reduce to 15–20 dBm to limit co-channel interference

SSID broadcast: enabled for guest/staff; hidden SSID is not a security mechanism, so avoid relying on it

Management interface: dedicated management VLAN (e.g., VLAN 99) with access only from admin subnet

Firmware: keep AP firmware up-to-date; enable automated alerting for updates
