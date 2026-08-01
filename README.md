<div align="center">
  <img src="assets/edljxtp.PNG" alt="edljx logo" width="200" />
  <h1>Home Networking Setup Guide</h1>
  <p><strong>Ditch the subscription, keep the productivity.</strong></p>
</div>

### About edljx
We are a friendly, scrappy tech hub dedicated to helping curious builders replace expensive subscriptions with practical, affordable alternatives. We believe technology should empower, not bankrupt. Whether you're a student, indie creator, or just a tinkerer, we're here to share honest guides and real-world tools that respect your wallet.

🌐 **Website:** [edljx.com](https://edljx.com)  
📧 **Community:** [members.edljx.com](https://members.edljx.com)

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
| **[pfSense](https://www.pfsense.org/)** | The veteran OPNsense sibling, BSD-based. Massive community and deep documentation. |
| **[OpenWrt](https://openwrt.org/)** | Linux-based firmware you flash onto consumer routers. Turn a $60 router into enterprise-grade gear. |
| **[MikroTik RouterOS](https://mikrotik.com/software)** | Pro-grade routing on cheap hardware. Steep learning curve but unmatched price-to-power ratio. |
| **[VyOS](https://vyos.io/)** | Open source network OS built on Debian. CLI-driven, ideal for BGP/VPN at home or in the lab. |
| **[IPFire](https://www.ipfire.org/)** | Hardened Linux firewall distro with intrusion detection built in. Great for security-first setups. |

### 🌐 DNS, DHCP & IPAM
| Service | Description |
| :--- | :--- |
| **[Pi-hole](https://pi-hole.net/)** | DNS sinkhole that blocks ads for every device on your LAN via local DNS resolver. |
| **[AdGuard Home](https://github.com/AdguardTeam/AdGuardHome)** | Network-wide ad/tracker blocker with a polished web UI and DoH/DoT support. |
| **[NextDNS](https://nextdns.io/)** | Cloud-hosted DNS filter with parental controls and per-device configs. Free tier for personal use. |
| **[Unbound](https://github.com/NLnetLabs/unbound)** | Validating, recursive, caching DNS resolver. Run it locally for DNSSEC without upstream trust. |
| **[Technitium DNS](https://technitium.com/dns/)** | All-in-one DNS server with DoH, DoT, ad-blocking, and a friendly web UI. |
| **[BIND9](https://www.isc.org/bind/)** | The reference DNS server. Heavier than Unbound but ubiquitous in enterprise. |
| **[dnsmasq](https://thekelleys.org.uk/dnsmasq/doc.html)** | Lightweight DNS forwarder + DHCP server. Pairs perfectly with Pi-hole. |
| **[sismics/docs](https://github.com/sismics/docs)** | Document Management | Lightweight document management system. |
| **[ONLYOFFICE Docs](https://github.com/ONLYOFFICE/DocumentServer)** | Self-hosted Office | Self-hosted online office suite for home-server use. |
| **[FlareTunnel](https://github.com/MorDavid/FlareTunnel)** | Cloudflare Tunnel Proxy | Proxy that routes traffic through Cloudflare Workers for IP rotation and anonymity. |

### 🔐 VPN & Remote Access
| Service | Description |
| :--- | :--- |
| **[WireGuard](https://www.wireguard.com/)** | Modern kernel-mode VPN. Faster than OpenVPN, with a tiny audited codebase. |
| **[Tailscale](https://tailscale.com/)** | Zero-config WireGuard mesh built on coordinated DERP relays. |
| **[Headscale](https://github.com/juanfont/headscale)** | Self-hosted, open source implementation of the Tailscale control server. |
| **[OpenVPN](https://openvpn.net/)** | The veteran SSL/TLS VPN. Universal client compatibility, slightly slower than WireGuard. |
| **[Nebula](https://github.com/slackhq/nebula)** | Slack's overlay networking tool. Lighthouses + certificates for peer-to-peer mesh. |
| **[ZeroTier](https://www.zerotier.com/)** | Software-defined Ethernet. Creates a virtual L2 network across the internet. |
| **[Netbird](https://netbird.io/)** | Open source WireGuard overlay with SSO and ACLs. The FOSS answer to Tailscale. |

### 🧅 Reverse Proxy & Tunnels
| Service | Description |
| :--- | :--- |
| **[Nginx Proxy Manager](https://nginxproxymanager.com/)** | Web UI for issuing Let's Encrypt certs and proxying hostnames. Beginner friendly. |
| **[Caddy](https://caddyserver.com/)** | Automatic HTTPS web server written in Go. Zero-config Let's Encrypt. |
| **[Traefik](https://traefik.io/)** | Cloud-native reverse proxy with auto-discovery from Docker labels. |
| **[HAProxy](https://www.haproxy.org/)** | The fastest production-grade load balancer. Steep but powerful config. |
| **[Cloudflare Tunnel](https://www.cloudflare.com/products/tunnel/)** | Expose home services without opening firewall ports via the Cloudflare edge. |
| **[FRP (Fast Reverse Proxy)](https://github.com/fatedier/frp)** | Self-hosted NAT-traversal tunnel with TCP/UDP/HTTP support. |
| **[Bore](https://github.com/ekzhang/bore)** | Minimal CLI that exposes localhost to the internet via a public relay. |

### 📡 Wi-Fi Planning & Monitoring
| Service | Description |
| :--- | :--- |
| **[WiFi Analyzer (NetSpot-style)](https://www.netspotapp.com/)** | Survey and visualize your wireless coverage and channel usage. |
| **[Ekahau](https://www.ekahau.com/)** | Professional-grade Wi-Fi planning and troubleshooting suite. |
| **[Ubiquiti Wifiman](https://wifiman.ui.com/)** | Free mobile scanner for signal strength, channels, and AP discovery. |
| **[InSSIDer](https://www.metageek.com/products/inssider/)** | Windows/macOS tool to visualize Wi-Fi interference and roaming behavior. |

### 🛠 Diagnostics & Learning
| Service | Description |
| :--- | :--- |
| **[Wireshark](https://www.wireshark.org/)** | The canonical packet analyzer. Capture and inspect traffic at any layer. |
| **[Grafana](https://grafana.com/)** | Time-series dashboards for visualizing router, switch, and DNS metrics. |
| **[Zabbix](https://www.zabbix.com/)** | Open source network and infrastructure monitoring with alerting. |
| **[Uptime Kuma](https://github.com/louislam/uptime-kuma)** | Self-hosted monitoring with HTTP/TCP/ping probes and a clean dashboard. |
| **[Pingdom](https://www.pingdom.com/)** | SaaS uptime and page-speed monitor. Free tier for basic checks. |
| **[Mozilla SSL Configuration Generator](https://ssl-config.mozilla.org/)** | Generates hardened TLS configs for Nginx, Apache, HAProxy, and more. |
| **[SmokePing](https://oss.oetiker.ch/smokeping/)** | Latency visualization over time. Catch jitter before your VoIP users do. |


---
### 🤝 Contributing
Contributions are welcome! If you find a broken link or have a resource that belongs here, please open an Issue.
