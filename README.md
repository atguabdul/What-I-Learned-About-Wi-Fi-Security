# What I Learned About Wi-Fi Security

This repository summarizes everything I learned during my exploration of Wi-Fi networks, ethical hacking basics, and wireless security.

## 📡 Monitor Mode
- Allows the wireless adapter to **listen to all Wi-Fi traffic**, even if it's not connected.
- Used for capturing packets and analyzing nearby networks.

## 📦 Packet Sniffing (Airodump-ng)
- Shows all nearby wireless networks and details like:
  - **BSSID** (MAC address of the router)
  - **ESSID** (name of the network)
  - **Encryption types** (WEP, WPA, WPA2)
  - **Channel number**
  - **Connected clients**

## 🔐 Handshake Capture
- A **WPA/WPA2 handshake** is exchanged when a device connects to Wi-Fi.
- Capturing it lets you try to crack the password offline later.

## 🔥 Deauthentication Attack
- Sends fake disconnect packets to force a device off the network.
- Triggers handshake when the device reconnects.
- No password is required to do this.

## 🎭 Fake Authentication
- Pretends to be a client to the router.
- Helps with WEP cracking or sending further packets.

## ♻️ ARP Request Replay (WEP only)
- Repeats ARP packets to generate more traffic.
- Speeds up the process of cracking WEP keys.

## 📶 Wi-Fi Frequencies
- **2.4GHz**: Slower but covers more distance.
- **5GHz**: Faster but shorter range.
- Some adapters support both (dual-band).

## 🧪 Wi-Fi Adapters
- I learned about adapters and chipsets like:
  - **Atheros AR9271** (stable, good for 2.4GHz)
  - **Realtek 8812AU** (supports 2.4GHz & 5GHz)
- Adapters must support **Monitor Mode** and **Packet Injection**.

## 🛠️ Tools I Used
- `airmon-ng`: Enables monitor mode
- `airodump-ng`: Scans and shows networks
- `aireplay-ng`: For attacks like deauth or replay
- `Wireshark`: For packet analysis and inspection

## ⚠️ Note
This knowledge is for **learning and ethical purposes only**. Never perform these actions on networks you do not own or have permission to test.


