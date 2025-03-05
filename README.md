# Network Traffic Analysis Project

## 📌 Overview

This project analyzes network traffic data from five different applications by processing **PCAP** files using Python and **PyShark**. The analysis includes various traffic characteristics such as **protocol distribution, packet sizes, flow durations, and TCP flags**. Data visualization is performed using **Matplotlib** and **Seaborn**.

---

## 📂 Dataset

### **Applications Analyzed:**

- **Chrome**
- **FireFox**
- **Spotify**
- **YouTube**
- **Zoom**

### **PCAP Files** (located in the `res`/ directory):

- `chrome_record.pcapng`
- `firefox_record.pcapng`
- `spotify_record.pcapng`
- `youtube_record.pcapng`
- `zoom_record.pcapng`

---

## 🛠 Dependencies

To run this project, install the required Python libraries:

```bash
pip install pyshark pandas matplotlib numpy seaborn
```

Additionally, ensure you have **Wireshark** and **TShark** installed on your system for PyShark to function properly.

---

## 📜 How It Works

1. **Load PCAP Files** – The script loads packets from PCAP files into memory.
2. **Extract Network Features** – Key attributes such as **TTL, IP Header Length, Packet Size, and Protocols** are analyzed.
3. **Analyze and Categorize Traffic** – Differentiates between protocols, TCP flags, traffic direction (incoming vs. outgoing), and flow durations.
4. **Data Visualization** – Various graphs and histograms are generated to visualize network characteristics.

---

## 🚀 Running the Script

Run the main script to process the PCAP files and generate insights:

```bash
python src/analyze_traffic.py
```

Ensure that the `pcaps/` directory contains the required PCAP files.

---

## 📊 Key Visualizations

1. **Protocol Distribution** – Shows the percentage of different protocols (TCP, UDP, QUIC, TLS, etc.) used by each application.
2. **Packet Size Distribution** – A box plot visualizing packet sizes across different applications.
3. **Traffic Direction Analysis** – Compares the ratio of incoming and outgoing packets for each application.
4. **Flow Duration Distribution** – Histogram showing how long connections last for different applications.
5. **TCP Flags Analysis** – Displays the frequency of different TCP flags like **SYN, ACK, FIN, RST** for each application.

---

## 📌 File Structure

```
📂 network-traffic-analysis
│── 📂 res               # Directory containing PCAP files
│── 📂 src  
│────      📜 analyze_traffic.py   # Main script for analysis
│── 📜 README.md            # Project documentation (this file)
```

---

## 🔗 References

- **Wireshark & TShark Documentation**: [https://www.wireshark.org/docs/](https://www.wireshark.org/docs/)
- **PyShark Documentation**: [https://github.com/KimiNewt/pyshark](https://github.com/KimiNewt/pyshark)
- **Matplotlib & Seaborn**: [https://matplotlib.org/](https://matplotlib.org/), [https://seaborn.pydata.org/](https://seaborn.pydata.org/)

---

## 📌 Contributors

- **Adi Gam Zu Letova**
- **Shira Mursiano**
- **Yael Gil Dorani**
- **Avital Zar**

## 📩 Contact

For any inquiries, reach out via **GitHub** or university contact channels.

