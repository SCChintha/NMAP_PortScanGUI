# 🔍 Network Port Scanner GUI

A lightweight, fast, and user-friendly TCP port scanner built using **Python** and **Tkinter**. This tool enables users to scan open ports on a target machine through an intuitive graphical interface—no command-line knowledge required.

---

## 🚀 Features

- 🖥️ **Simple GUI Interface**
  - Enter target host, start port, and end port with ease

- ⚡ **High-Speed Multi-threading**
  - Supports up to **500 concurrent threads** for fast scanning

- 🔎 **Service Detection**
  - Identifies common services like FTP, SSH, HTTP, HTTPS, MySQL, RDP, etc.

- 📊 **Real-Time Updates**
  - Live progress bar and elapsed time tracking

- ⛔ **Interrupt Anytime**
  - Stop scan safely without crashing the application

- 💾 **Export Results**
  - Save scan results to a `.txt` file

- 🌍 **Cross-Platform Support**
  - Works on Windows, macOS, and Linux

---

## 🛠️ Technologies Used

- **Python 3.7+**
- **Tkinter (GUI)**
- **Socket Programming**
- **Threading & Semaphore**
- **Queue (Thread-safe communication)**

---

## 📋 Requirements

- Python 3.7 or newer  
- Tkinter (pre-installed with Python)

> For Ubuntu/Debian:
```bash
sudo apt install python3-tk

## Installation

```bash
git clone https://github.com/SCChintha/NMAP_PortScanGUI.git
cd NMAP_PortScanGUI
```

## Usage

```bash
python portscanergui.py
```
1. Enter the **Target** – an IP address (e.g. `192.168.1.1`) or hostname (e.g. `scanme.nmap.org`).
2. Set the **Start Port** and **End Port** (defaults: `1` – `1024`).
3. Click **Start Scan**. Open ports appear in real time in the results pane.
4. Click **Stop** to cancel a scan early.
5. After a scan completes, click **Save Results** to write the open-port list to a text file.

## Detected Services

The following ports are automatically labelled:

| Port | Service   |
|------|-----------|
| 21   | FTP       |
| 22   | SSH       |
| 23   | Telnet    |
| 25   | SMTP      |
| 53   | DNS       |
| 80   | HTTP      |
| 110  | POP3      |
| 143  | IMAP      |
| 443  | HTTPS     |
| 3306 | MySQL     |
| 3389 | RDP       |
| 5900 | VNC       |
| 8080 | HTTP-Alt  |
Ports not in the list are reported as `Unknown`.

## Project Structure

```
NMAP_PortScanGUI/
├── portscanergui.py   # Main application (scanner + GUI)
└── README.md
```
## Disclaimer

Use this tool only on hosts and networks you own or have explicit permission to scan. Unauthorized port scanning may be illegal in your jurisdiction.

