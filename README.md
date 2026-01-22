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

### 📖 360° Overview
**Why is this helpful?**  
This repository serves as a centralized knowledge base for this topic. Instead of scattered bookmarks, we provide a curated, maintained directory.

**Who is this for?**  
Learners and professionals seeking verified, high-quality resources.

### 🌍 Impact on the Everyday Person & Tech Enthusiast
**For the Everyday Person:**  
This isn't just "computer code"; it's about autonomy. By understanding and using these tools, you stop being a passive consumer who pays monthly rent for digital life. You become an owner. It means keeping your family photos safe without paying Apple/Google, working from anywhere without restriction, or learning a skill that can double your income.

**For the Tech Enthusiast:**  
This is your playground. These resources remove the guardrails found in commercial software. You get to see "how the sausage is made," tweak every config file, and build systems that are faster, more private, and uniquely yours. It's the difference between driving an automatic sedan and tuning a manual racecar.

**How to use this safely:**  
We verify links, but the internet changes. Always check the credibility of 3rd party resources before downloading files.

### ✨ Specific Benefits to Your Life
Saves you dozens of hours of research. We cut through the noise to find the signal.

### 📚 Additional Reading
- *No specific reading linked yet. Check the main list above.*

---


A guide to networking for beginners: VLANs, Firewalls, and DNS blocking.


The network is the foundation of the homelab. If your network is flat (192.168.1.1 for everything), your IoT toaster can hack your server. Better networking = better security + ad blocking.


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
