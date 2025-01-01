# Windows-Exfil-BadUsb 💻🔌

Welcome to **Windows-Exfil-BadUsb**! This repository contains a set of two PowerShell scripts that help gather sensitive data from a Windows machine and exfiltrate it to a Discord Webhook. The first script collects system information and sensitive files, while the second script uploads the collected data to a Discord channel for easy access. 🕵️‍♂️🚨

> **Warning:** These scripts are intended for educational purposes only. **Do not use these scripts maliciously**. Unauthorized access to computer systems is illegal.

---

## 📁 Scripts

### 1. **EXFIL.txt**
This script collects a variety of system information and stores it in a `results.txt` file. The data includes:
- **System Information** 🖥️
- **Local Users** 👤
- **Network Profiles and Passwords** 🌐
- **Installed Hotfixes** 🔧
- **Environment Variables** 🌍
- **Running Services** ⚙️
- **Active IPv4 Addresses** 🌐
- **Exfiltrated Files** 📂

After running this script, you'll have a `results.txt` file that contains valuable system data.

### 2. **send_file.txt**
Once the `results.txt` is generated, this script uploads the file to a Discord Webhook using multipart form data. After the file is uploaded, it deletes the local copy to ensure no traces are left behind. ✉️📤

---

## ⚙️ Setup

1. **Clone this repository**:
   ```bash
   git clone https://github.com/Retr0-0Sec/Windows-Exfil-BadUsb
2. **Open the EXFIL.txt script and replace the placeholder with your Discord Webhook URL**:
 
  > $webhookUrl = "YOUR_DISCORD_WEBHOOK_URL"

3. **Set the path where the results.txt file will be saved**:
 
 >  $outputFile = "C:\PATH\TO\YOUR\results.txt"
 
4. **Run the Scripts**:

>Run EXFIL.txt to collect data from the system. This will create the results.txt file.

>Run send_file.txt to upload the file to Discord and delete it from the local machine.

## 📝 Usage
1. **Run the scripts in a PowerShell window on a Windows machine**.

2. **After the first script runs and creates the results.txt file, run the second script to upload it to Discord**.

3. **Monitor your Discord webhook for the uploaded data**.

## 🔒 License
**Distributed under the MIT License. See LICENSE for more information**.

## 💬 Contact
**For questions, issues, or suggestions, feel free to open an issue or reach out to me on Discord: @retr0_0sec**

## 🤖 Disclaimer
**This tool is designed for educational use only. Please respect privacy and legal boundaries when using this script. Unauthorized access to computer systems is illegal and punishable by law.**

## 📜 License
MIT License

Copyright (c) 2024 Retr0_0Sec

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
