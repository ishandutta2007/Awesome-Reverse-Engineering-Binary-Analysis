# Awesome-Reverse-Engineering-Binary-Analysis
# Awesome-Reverse-Engineering-Binary-Analysis

# Top RF & Wireless Cybersecurity Monitoring Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Wireless Intrusion Detection (WIDS), Spectrum Analysis, Wi-Fi/BLE Auditing, SDR & RF Surveillance Detection*  
**Last updated: November 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **RF & Wireless Cybersecurity Monitoring**. These tools enable passive wireless packet sniffing, rogue access point detection, Bluetooth Low Energy (BLE) and cellular anomaly monitoring, Software-Defined Radio (SDR) spectrum analysis, and wireless vulnerability scanning.

**Examples** include Kismet Cloud, Hak5 Cloud C2, WiGLE, Tenable Nessus, Qualys Network Scanner, Rapid7 InsightVM, PRTG Wireless, Ekahau Cloud, NetSpot, Acrylic Wi-Fi, and `CIS-C0/RFSentinel` (the category leaders). 

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosted wireless intrusion detection, SDR signal intelligence, Wi-Fi/BLE auditing, and privacy-focused RF counter-surveillance — ideal for security researchers, network defenders, red teamers, and RF engineers.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saashosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Hak5 Cloud C2](https://hak5.org)**  
  Self-hosted and cloud-connected command-and-control platform for managing remote WiFi Pineapple, Packet Squirrel, and wireless auditing field sensors.

- **[WiGLE (Wireless Geographic Logging Engine)](https://wigle.net)**  
  Crowdsourced cloud database and mapping platform consolidating global Wi-Fi, Bluetooth, and cellular tower wardriving telemetry.

- **[Tenable Nessus](https://tenable.com)**  
  Commercial vulnerability assessment scanner capable of auditing wireless access points, rogue devices, and network infrastructure exposures.

- **[Qualys Network Scanner (VMDR)](https://qualys.com)**  
  Cloud-based vulnerability management and continuous asset discovery platform monitoring wireless controllers and connected endpoints.

- **[Rapid7 InsightVM](https://rapid7.com)**  
  Enterprise vulnerability risk management platform offering live dashboards and automated scanning across wired and wireless network segments.

- **[PRTG Network Monitor (Wireless Sensors)](https://paessler.com)**  
  Infrastructure monitoring platform featuring dedicated SNMP, QoS, and signal-strength sensors for enterprise wireless networks.

- **[Ekahau Cloud](https://ekahau.com)**  
  Enterprise Wi-Fi site survey, RF spectrum interference analysis, and wireless network design platform with cloud collaboration.

- **[NetSpot](https://netspotapp.com)**  
  Commercial wireless site survey, Wi-Fi heatmap visualization, and channel interference troubleshooting software for macOS and Windows.

- **[Acrylic Wi-Fi](https://acrylicwifi.com)**  
  Commercial suite of Wi-Fi analyzer, packet sniffer, and RF heatmapping utilities for Windows wireless diagnostics and security audits.


## Open-Source GitHub Projects

- **[CIS-C0/RFSentinel](https://github.com/CIS-C0/RFSentinel)**  
  Free, open-source, no-root Android RF detector that passively monitors Bluetooth LE, Wi-Fi beacons, and cellular towers to alert on trackers, drones, ALPR cameras, and IMSI catchers.

- **[Kismet](https://github.com)**  
  Industry-standard open-source passive wireless network detector, sniffer, and Wireless Intrusion Detection System (WIDS) supporting Wi-Fi, Bluetooth, Zigbee, ADS-B, and SDRs.

- **[Bettercap](https://github.com)**  
  Modular, high-speed open-source network attack and monitoring framework supporting 802.11 Wi-Fi, Bluetooth Low Energy, and 2.4GHz wireless HID auditing.

- **[Aircrack-ng](https://github.com)**  
  Complete open-source suite of tools to assess Wi-Fi network security, focusing on packet capture, monitor mode management, replay testing, and WPA/WEP auditing.

- **[Wifite2](https://github.com)**  
  Automated open-source wireless auditing tool designed to orchestrate `aircrack-ng`, `reaver`, and `hcxdumptool` workflows cleanly.

- **[hcxdumptool](https://github.com)**  
  Lightweight, high-performance open-source C utility for capturing WLAN traffic, PMKIDs, and EAPOL handshakes for authorized penetration testing.

- **[OpenVAS (Greenbone Vulnerability Management)](https://github.com)**  
  Full-featured open-source vulnerability scanner and management suite serving as a self-hosted alternative to Nessus and Qualys.

- **[Sparrow-wifi](https://github.com)**  
  Next-generation open-source graphical Wi-Fi and Bluetooth analyzer for Linux built for drone/agent-based remote RF spectrum reconnaissance.

- **[Wavemon](https://github.com)**  
  Lightweight open-source ncurses-based monitoring application for tracking real-time wireless signal levels, noise, and link statistics on Linux.

- **[Horst](https://github.com)**  
  Minimalist open-source IEEE 802.11 wireless LAN analyzer designed for troubleshooting dense Wi-Fi environments and mesh networks.

- **[ESP32 Marauder](https://github.com)**  
  Open-source suite of Wi-Fi and Bluetooth offensive/defensive monitoring firmware engineered for portable ESP32 and Flipper Zero hardware.

- **[nzyme](https://github.com)**  
  Open-source wireless intrusion defense system (WIDS) that collects 802.11 management frames and forwards structured security telemetry to SIEMs.

- **[rtl_433](https://github.com)**  
  Versatile open-source receiver and protocol decoder for ISM band (433.92 MHz, 868 MHz, 915 MHz) IoT sensors, weather stations, and wireless alarms using SDRs.

- **[URH (Universal Radio Hacker)](https://github.com)**  
  Complete open-source suite for investigating unknown wireless protocols, demodulating RF signals, and analyzing raw SDR captures.

- **[GNU Radio](https://github.com)**  
  Foundational open-source software development toolkit providing signal processing blocks to implement software-defined radios and spectrum analyzers.

- **[Inspectrum](https://github.com)**  
  Open-source radio signal analysis tool for visually inspecting captured IQ samples, spectrograms, and symbol timings from SDR hardware.

- **[Wireshark](https://github.com)**  
  The world's foremost open-source network protocol analyzer with deep dissectors for 802.11 Wi-Fi, Bluetooth, Zigbee, LoRaWAN, and LTE/5G frames.

### Additional Strong Open-Source Options

- **[GQRX](https://github.com)** and **[SDR++](https://github.com)** for real-time wide-band waterfall spectrum visualization across RTL-SDR, HackRF, and USRP devices.
- **[Airgeddon](https://github.com)** for multi-use bash-based wireless auditing and evil-twin detection workflows on Linux.
- **[BlueHydra](https://github.com)** for continuous Bluetooth Classic and BLE device discovery and tracking.
- **[Rayhunter (EFF)](https://github.com)** for open-source cellular network monitoring to detect fake base stations (IMSI catchers / Stingrays) on mobile hotspots.
- Many community **Flipper Zero Sub-GHz analyzers**, **Meshtastic RF telemetry nodes**, and **TinySA spectrum scripts** for portable field monitoring.

**Frameworks for building custom systems**: Combine **Kismet**, **nzyme**, **rtl_433**, and **OpenVAS** with **Grafana / OpenSearch** and **CIS-C0/RFSentinel** for continuous, multi-spectrum wireless security monitoring.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Active wireless auditing, deauthentication testing, and RF transmission are strictly regulated by law (e.g., FCC, WPC, ETSI); use passive monitoring tools responsibly and only audit networks or spectrum you have explicit authorization to test.

---

**Made for wireless security researchers, RF engineers, SOC analysts, and privacy advocates.**  
Let's make the wireless spectrum more transparent, resilient, and secure.
