# Recon Raptor

```
 /$$$$$$$                                                /$$$$$$$                        /$$                        
| $$__  $$                                              | $$__  $$                      | $$                        
| $$  \ $$  /$$$$$$   /$$$$$$$  /$$$$$$  /$$$$$$$       | $$  \ $$  /$$$$$$   /$$$$$$  /$$$$$$    /$$$$$$   /$$$$$$ 
| $$$$$$$/ /$$__  $$ /$$_____/ /$$__  $$| $$__  $$      | $$$$$$$/ |____  $$ /$$__  $$|_  $$_/   /$$__  $$ /$$__  $$
| $$__  $$| $$$$$$$$| $$      | $$  \ $$| $$  \ $$      | $$__  $$  /$$$$$$$| $$  \ $$  | $$    | $$  \ $$| $$  \__/
| $$  \ $$| $$_____/| $$      | $$  | $$| $$  | $$      | $$  \ $$ /$$__  $$| $$  | $$  | $$ /$$| $$  | $$| $$      
| $$  | $$|  $$$$$$$|  $$$$$$$|  $$$$$$/| $$  | $$      | $$  | $$|  $$$$$$$| $$$$$$$/  |  $$$$/|  $$$$$$/| $$      
|__/  |__/ \_______/ \_______/ \______/ |__/  |__/      |__/  |__/ \_______/| $$____/    \___/   \______/ |__/      
                                                                            | $$                                    
                                                                            | $$                                    
                                                                            |__/
```

```
  _____                _                
 |  __ \              | |               
 | |__) |___  __ _  __| |_ __ ___   ___ 
 |  _  // _ \/ _` |/ _` | '_ ` _ \ / _ \
 | | \ \  __/ (_| | (_| | | | | | |  __/
 |_|  \_\___|\__,_|\__,_|_| |_| |_|\___|
```

## ABOUT

Recon raptor is an asynchronous multi network scanning tool employed to perform enumeration and vulnerability assessment using a range of widely used tools such as Nmap, enum4linux, gobuster, nikto and more.

The tool automates the tedious early stages of pen-testing to free up professionals to perform the more exciting tasks!

Recon raptor automatically generates structured, professional reports, including a visual vulnerability snap shot.

## Getting Started

```
   _____      _   _   _                _____ _             _           _ 
  / ____|    | | | | (_)              / ____| |           | |         | |
 | |  __  ___| |_| |_ _ _ __   __ _  | (___ | |_ __ _ _ __| |_ ___  __| |
 | | |_ |/ _ \ __| __| | '_ \ / _` |  \___ \| __/ _` | '__| __/ _ \/ _` |
 | |__| |  __/ |_| |_| | | | | (_| |  ____) | || (_| | |  | ||  __/ (_| |
  \_____|\___|\__|\__|_|_| |_|\__, | |_____/ \__\__,_|_|   \__\___|\__,_|
                               __/ |                                     
                              |___/       
```

## Prerequisites

The tool is developed to work natively within a Linux environment. However, if users have any issues please make sure to have the following tools installed:

- Python 3.8+
- Gobuster Installed
- Nikto Installed 
- Enum4linux Installed
- Internet Access For Vulners API

## Installation

Recon raptor employs mostly native python libraries for execution, keeping it lightweight and scalable. However, for functionality the following non-native libraries have been included in 'requirements.txt'.

To install, please execute the following command within your kali terminal:

```bash
pip install -r requirements.txt
```

If requirements.txt is unavailable or you have any issues please ensure Nmap is installed with the following command:

```bash
pip install python-nmap
```

## Usage

Recon raptor was designed with automation in mind. This means that minimal user input is required. However, for the tool to work as intended it is critical that the following syntax requirements are met:

```bash
sudo python recon-raptor.py <Target IP> <Target IP>
```

**Example Usage:**

```bash
sudo python recon-raptor.py 192.168.10.132 192.168.10.133
```

**Options:**

- target_ips (specify one or more target IP Addresses)

## Tool Functionality

Recon raptor performs several scanning and enumeration tasks to ascertain key information about a target network(s) including:

- **OS Detection:** Identify the target networks operating system
- **Service Detection:** Discovers open ports and their corresponding versions 
- **Nikto Scan:** Identifies web based vulnerabilities and misconfigurations
- **Gobuster Scan:** Identifies web related hidden files and directories
- **NFS Enumeration:** Discovers network shares and attempts to mount a directory if root is shared
- **SMB enumeration:** Identifies SMB shares and more comprehensive information using enum4linux
- **Vulnerability Scan:** Employs Nmap to execute a Vulners scan to identify vulnerabilities
- **Critical CVE Extraction:** Employs the Vulners API to provide more descriptive details of critical vulnerabilities 
- **Report generation:** Automatically generates a structured HTML report, including scan results and visualize critical vulnerabilities

## Disclaimer

Recon raptor is intended for educational and professional purposes only.
Recon raptor must be used legally and ethically, with no testing to occur without consent.
The developer takes no legal responsibility for use outside its permitted use.

## Contact Information

If you have any issues with Recon raptor or have any questions please send a detailed subjected email to:

2103490@uad.ac.uk

**Thank You!**
