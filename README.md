# # UAV Intrusion Detection Dataset (UAV-NIDD)
UAV-NIDD is a real-world, dynamic intrusion detection dataset collected from a physical UAV network testbed. It includes benign traffic and ten cyber-attack types targeting UAVs, access points, and ground control stations, designed to support research in UAV cybersecurity, IDS, and machine learning.

## 🔍 Motivation

UAV networks are increasingly used in surveillance, delivery, disaster response, and critical infrastructure monitoring. Their reliance on wireless communication and UAV-specific protocols makes them vulnerable to cyber and cyber-physical attacks.

Existing intrusion detection datasets do not adequately capture:
- UAV-specific communication protocols
- Multi-node UAV network interactions
- Real-world attack behavior

UAV-NIDD addresses these gaps by providing real network traffic collected from physical UAVs operating in realistic scenarios.

---

## 🧪 Testbed Overview

The dataset was generated using a real UAV network composed of:

- **UAVs**
  - PX4 Vision Dev Kit v1.5 (main access point UAV)
  - DJI Mavic Air
  - DJI Mini 3 Pro

- **Network Components**
  - Ground Control Stations (GCS)
  - UAV-to-UAV communication
  - UAV-to-GCS communication
  - UAV-to-Access Point communication
Traffic was captured during real flight operations under both benign and attack conditions.

---

## ⚔️ Attack Scenarios

UAV-NIDD includes traffic from three high-level compromise scenarios:

1. **Compromised UAV initiates a network-wide attack**
2. **Compromised Access Point leads to network-wide attack**
3. **Compromised Ground Control Station (GCS) initiates network-wide attack**

---

## 🚨 Attack Types Included

The dataset contains the following cyber and cyber-physical attacks:

- Scanning (SYN, TCP, UDP)
- Reconnaissance
- DoS
- DDoS (ICMP, UDP, SYN Flood)
- De-authentication
- Man-in-the-Middle (MITM)
- Replay Attack
- Evil Twin
- GPS Jamming & GPS Spoofing
- Brute-Force Attack
- Fake Landing Packet Attack

Each attack is executed multiple times with controlled duration and targets.

---

## 📊 Features

UAV-NIDD provides rich, multi-layer network features extracted from captured traffic:

- **UAV Case**: 45 features
- **Access Point Case**: 51 features
- **GCS Case**: 85 features

Feature categories include:
- Frame-level wireless features
- Network flow statistics
- Transport-layer attributes
- Protocol-specific fields (e.g., MAVLink, DJI SDK)

These features support both binary and multi-class intrusion detection.
### 📦 Download Options

#### 🟢 Full Dataset (PCAP Files)

If you want **raw network traffic**, download the PCAP files:
🔗 **https://doi.org/10.6084/m9.figshare.25486462**

* 📡 Packet-level data
* Suitable for:

  * Network analysis
  * Packet inspection
  * Feature extraction

---




## 📌 Citation

If you use **UAV-NIDD** in your research, experiments, or publications, please cite the following paper:

```bibtex
@article{Hadi2025UAVNIDD,
  author    = {Hassan Jalil Hadi and Yue Cao and Muhammad Khurram Khan and Naveed Ahmad and Yulin Hu and Chao Fu},
  title     = {UAV-NIDD: A Dynamic Dataset for Cybersecurity and Intrusion Detection in UAV Networks},
  journal   = {IEEE Transactions on Network Science and Engineering},
  volume    = {12},
  number    = {4},
  pages     = {2739--2758},
  year      = {2025},
  doi       = {10.1109/TNSE.2025.3553442}
}

```

---

## 👨‍💻 Maintainer

**CyberSar Lab**
🔗 https://cybersar.kaust.edu.sa/

