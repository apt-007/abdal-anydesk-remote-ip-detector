# AnyDesk IP Leak Vulnerability


## 🎤 README Translation
- [English](README.md)
- [فارسی](README.fa.md)

## 📸 Screenshot

<video width="800" height="468" controls>
  <source src="" type="video/mp4">
  Your browser does not support the video tag.
</video>
 
## 💎 Introduction
The Abdal AnyDesk Remote IP Detector is a Proof-of-Concept (PoC) tool that exploits a vulnerability in AnyDesk’s "Allow Direct Connections" feature. When this option is enabled and the connection port is set to 7070 on the attacker's system only, it allows a user with only the AnyDesk ID of the target to retrieve their public IP address without requiring any settings to be changed on the target system. Additionally, if both systems are connected to the same network, it is also possible to obtain the private IP address of the target.


## 💀 Vulnerability Overview
This vulnerability leverages the "Allow Direct Connections" feature in AnyDesk, potentially exposing sensitive IP information of a target. Attackers can use this flaw to acquire the public IP and, under certain conditions, the private IP address of the target machine. The vulnerability highlights privacy risks associated with remote access tools when security settings are not appropriately configured.

## ✨ Features
* Retrieves public IP address of a remote system when AnyDesk ID is known.
* Private IP detection within local network connections.
* Quick setup and straightforward PoC execution.
* No complex dependencies;
 

## 🛠️ Development Environment Setup
- **.NET 6**
 

## 🔥 Requirements
There are no specific prerequisites needed to run this PoC.

## 📥 Download
To download the executable versions of this PoC, please visit the official Releases page on GitHub. This will allow you to obtain the compiled version ready for use:

- [Download Executable PoC Versions from GitHub](https://github.com/ebrasha/abdal-anydesk-remote-ip-detector/releases)

 

## 📦 Setup and Usage
1. Enable Direct Connections in AnyDesk: Open AnyDesk on your system, go to Settings > Connection, then enable the option Allow direct connections. Set the port to 7070.
2. Launch the PoC Tool: Run the Abdal AnyDesk Remote IP Detector tool.
3. Enter Target AnyDesk ID: In AnyDesk, input the AnyDesk ID of the target system you wish to check.
4. IP Retrieval: Once the target AnyDesk ID is entered, the tool will automatically detect and display the public IP address of the target. If the two systems are on the same local network, the private IP address will also be shown.

## 😎 Expected Output
The tool will output:

* The public IP address of the remote system.
* The private IP address if the two systems are within the same local network.

## ✅ Mitigation
Unfortunately, there is currently no user-side fix for this vulnerability. To fully address this issue, an update or patch from AnyDesk’s development team is required. Until then, users should remain cautious with the "Allow direct connections" setting and monitor for updates from AnyDesk.

## 🎖️ Credit
- **Bug Discovery and PoC Developer**: Ebrahim Shafiei (EbraSha)
- [Profile on Linkedin](https://www.linkedin.com/in/profshafiei/)

## ❤️ Donation
If you find this project helpful and would like to support further development, please consider making a donation:
- [Donate Here](https://ebrasha.com/abdal-donation)

## 🤵 Programmer
Handcrafted with Passion by **Ebrahim Shafiei (EbraSha)**
- **E-Mail**: Prof.Shafiei@Gmail.com
- **Telegram**: [@ProfShafiei](https://t.me/ProfShafiei)

## ☠️ Reporting Issues
If you encounter any issues or have configuration problems, please reach out via email at Prof.Shafiei@Gmail.com. You can also report issues on GitLab or GitHub.

## ⚠️  Legal Disclaimer
This Proof of Concept (PoC) is provided for educational purposes only. Unauthorized use of this code on systems you do not own or have explicit permission to test is illegal and unethical. By using this PoC, you agree to take full responsibility for any misuse or damage that may result. The author disclaims all liability for actions taken based on the information provided in this repository. Always ensure you have proper authorization before conducting any security testing.