```bash
cd ~/IPGeo-Tracker

cat > README.md << 'EOF'
# 🌐 IPGeo-Tracker

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.6+-blue.svg)](https://python.org)
[![Termux](https://img.shields.io/badge/Termux-Compatible-black.svg)](https://termux.com)

**Advanced IP geolocation tracker for Termux and Linux systems.**

Track any IP address or domain with detailed information including country, city, ISP, coordinates, and Google Maps integration.

## 📸 Screenshots

```

╔════════════════════════════════════════╗
║        IP TRACKER PRO v3.0             ║
║      Advanced IP Intelligence          ║
╚════════════════════════════════════════╝

┌─[IP Tracker]
└──╼ $ 8.8.8.8

[] Tracking IP: 8.8.8.8
[] Time: 2026-05-22 21:44:30

╔════════════════════════════════════════╗
║           IP INFORMATION              ║
╚════════════════════════════════════════╝

IP Address    : 8.8.8.8
Country       : United States
Country Code  : US
Region        : California
City          : Mountain View
ISP           : Google LLC
Latitude      : 37.4229
Longitude     : -122.0850

📍 Google Maps: https://www.google.com/maps?q=37.4229,-122.0850

```

## ✨ Features

- 🎯 **Track any IP or domain** (e.g., `8.8.8.8`, `google.com`)
- 📍 **Get location data** (country, city, coordinates)
- 🗺️ **Google Maps integration** (direct link to location)
- 🔌 **ISP information** (internet service provider)
- 📱 **Termux optimized** (works perfectly on Android)
- 🎨 **Color-coded output** (easy to read)
- 💻 **Command-line mode** (scriptable with JSON output)
- 🚫 **No dependencies** (uses only Python standard library)

## 🚀 Installation

### Termux (Android)
```bash
pkg update && pkg upgrade
pkg install python git
git clone https://github.com/fredomae730/IPGeo-Tracker.git
cd IPGeo-Tracker
chmod +x iptracker.py
```

Linux (Ubuntu/Debian)

```bash
sudo apt update
sudo apt install python3 git
git clone https://github.com/fredomae730/IPGeo-Tracker.git
cd IPGeo-Tracker
chmod +x iptracker.py
```

📖 Usage

Interactive Mode (Recommended)

```bash
python3 iptracker.py
```

Then type:

· IP address (e.g., 8.8.8.8)
· Domain name (e.g., google.com)
· myip (to track your own IP)
· exit or quit (to exit)

Command-Line Mode

```bash
# Track an IP
python3 iptracker.py 8.8.8.8

# Track a domain
python3 iptracker.py google.com

# Track your own IP
python3 iptracker.py myip
```

JSON Output (for scripting)

```bash
python3 iptracker.py -q 8.8.8.8
```

📊 Example Output

Field Description
IP Address The tracked IP address
Country Country name
Region State/Region name
City City name
ISP Internet Service Provider
Latitude/Longitude Geographic coordinates
Google Maps Direct map link

🛠️ API Information

This tool uses ip-api.com - a free, no-API-key-required IP geolocation service.

Limits:

· 45 requests per minute from a single IP
· Free for non-commercial use
· No registration required

🔧 Commands

Command Description
myip Show your public IP address
exit / quit / q Exit the program
help Show help menu

📝 Examples

```bash
# Track Google DNS
python3 iptracker.py 8.8.8.8

# Track Cloudflare
python3 iptracker.py 1.1.1.1

# Track a website
python3 iptracker.py github.com

# Find your location
python3 iptracker.py myip

# Get JSON output
python3 iptracker.py -q 8.8.8.8 | jq '.'
```

🤝 Contributing

Contributions are welcome! Here's how:

1. Fork the repository
2. Create a feature branch (git checkout -b feature/AmazingFeature)
3. Commit changes (git commit -m 'Add AmazingFeature')
4. Push to branch (git push origin feature/AmazingFeature)
5. Open a Pull Request

📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

👤 Author

fredomae730

· GitHub: @fredomae730

⭐ Show your support

Give a ⭐️ if this project helped you!

📌 Note

· For educational purposes only
· Respect privacy laws in your country
· Don't use for malicious purposes
