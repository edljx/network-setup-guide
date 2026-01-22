<div align="center">
  <img src="assets/edljxtp.PNG" alt="edljx logo" width="200" />
  <h1>Home Networking Setup Guide</h1>
  <p><strong>Ditch the subscription, keep the productivity.</strong></p>
</div>

### About edljx
We are a friendly, scrappy tech hub dedicated to helping curious builders replace expensive subscriptions with practical, affordable alternatives. We believe technology should empower, not bankrupt. Whether you're a student, indie creator, or just a tinkerer, we're here to share honest guides and real-world tools that respect your wallet.

🌐 **Website:** [edljx.com](https://edljx.com)  
📧 **Community:** [more4less.edljx.com](https://more4less.edljx.com)

---

### 📖 Overview
A guide to networking for beginners: VLANs, Firewalls, and DNS blocking.

### ❓ Why This Exists?
The network is the foundation of the homelab. If your network is flat (192.168.1.1 for everything), your IoT toaster can hack your server. Better networking = better security + ad blocking.

### ⚡ How to Use
Start with DNS blocking (Pi-hole). Then graduate to a prosumer router (OPNsense/UniFi) to set up VLANs.

---


### 🚧 The Basics
| Concept | Tool/Tech | Benefit |
| :--- | :--- | :--- |
| **DNS Ad Blocking** | **[Pi-hole](https://pi-hole.net/)** / **[AdGuard Home](https://github.com/AdguardTeam/AdGuardHome)** | Blocks ads network-wide (Smart TVs, Phones, Tablets). |
| **VPN** | **[WireGuard](https://www.wireguard.com/)** / **[Tailscale](https://tailscale.com/)** | Access your home network securely from anywhere in the world. |
| **Reverse Proxy** | **[Nginx Proxy Manager](https://nginxproxymanager.com/)** | Host services at `https://plex.yourdomain.com` instead of `http://192.168.1.50:32400`. |

### 🔥 Advanced Routing
| Platform | Description |
| :--- | :--- |
| **[OPNsense](https://opnsense.org/)** | Open source firewall. Highly powerful, runs on standard hardware. The FOSS choice. |
| **[Ubiquiti UniFi](https://ui.com/)** | The 'Apple' of networking. easy to use, beautiful UI, but expensive and closed source. |
| **[Omada (TP-Link)](https://www.tp-link.com/us/business-networking/omada-sdn-router/)** | A budget-friendly alternative to UniFi with similar features. |


---
### 🤝 Contributing
Contributions are welcome! If you find a broken link or have a resource that belongs here, please open an Issue.
