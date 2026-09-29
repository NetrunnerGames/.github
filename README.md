<div align="center">

<img src="logo.jpg" width="160" height="160" style="border-radius: 50%; border: 2px solid #00ffff; box-shadow: 0 0 20px rgba(0, 255, 255, 0.4);" alt="NetrunnerGames Logo" />

# ⚡ NETRUNNER GAMES ⚡

### *Next-Generation Open Source Steam Ecosystem & Netrunning Toolsuite*

<a href="https://github.com/NetrunnerGames"><img src="https://img.shields.io/badge/Ecosystem-Active-090a0f?style=for-the-badge&labelColor=090a0f&logo=github&logoColor=00ffff" height="38" alt="Ecosystem Active" /></a>
<a href="https://github.com/NetrunnerGames/DataJackUI"><img src="https://img.shields.io/badge/Core_Client-DataJackUI-090a0f?style=for-the-badge&labelColor=090a0f&logo=dotnet&logoColor=512bd4" height="38" alt="DataJackUI Client" /></a>
<a href="https://github.com/NetrunnerGames/Jack-in"><img src="https://img.shields.io/badge/CEF_Plugin-Jack--in-090a0f?style=for-the-badge&labelColor=090a0f&logo=steam&logoColor=00adf0" height="38" alt="Jack-in Plugin" /></a>
<a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-090a0f?style=for-the-badge&labelColor=090a0f&logo=open-source-initiative&logoColor=3da639" height="38" alt="License" /></a>

---

</div>

> [!NOTE]
> **NETRUNNER GAMES ORGANIZATIONAL DIRECTORY**  
> We build high-performance desktop clients, CEF storefront plugins, native DLL hook loaders, and manifest distribution services designed for game management, preservation, and client customization.

---

## 🛰️ Description & Mission

**NetrunnerGames** is an open-source development collective dedicated to crafting modular, resilient, and aesthetically refined utilities for desktop gaming platforms. 

Our core focus spans:
* **Client UI Engineering**: Modern WPF interfaces built with custom Acrylic backdrops, DoH network fallback, and real-time Steam storefront search engines.
* **Native Hook Systems**: Modular C++ payload loaders (`version.dll` / IceBreaker framework) and dynamic CloudRedirect hooks.
* **Storefront Integration**: Asynchronous CEF store plugins (`Jack-in`) enabling seamless 1-click manifest operations directly inside the Steam client interface.

---

## 🎮 Organization Projects

| Project | Description | Primary Tech Stack | Status |
| :--- | :--- | :--- | :--- |
| 🎛️ **[DataJackUI](https://github.com/NetrunnerGames/DataJackUI)** | Modern WPF client for Steam manifest acquisition, DoH resolution, and hook management. | .NET 8, WPF, C# | **v2.00.0 (Active)** |
| 🔌 **[Jack-in](https://github.com/NetrunnerGames/Jack-in)** | Native Steam CEF store plugin enabling 1-click manifest addition inside Steam. | JavaScript, Lua, CSS | **v1.0 (Active)** |
| ⚡ **IceBreaker** | High-performance C++ `version.dll` hook loader and CloudRedirect payload handler. | C++, Win32 API | **Core Module** |
| 📦 **DepotBox / Ryuu** | Automated manifest indexing services and fix repositories. | Cloudflare Pages, JSON APIs | **Service Active** |

---

## 🛠️ Architecture & Core Principles

```
  +-------------------------------------------------------------+
  |                   NetrunnerGames Ecosystem                  |
  +-------------------------------------------------------------+
             |                                     |
             v                                     v
   +-------------------+                 +-------------------+
   |   DataJackUI      | <--- IPC ---->  |   Jack-in Plugin  |
   | (WPF .NET 8 Client)|                 |  (Steam CEF Store)|
   +-------------------+                 +-------------------+
             |                                     |
             +------------------+------------------+
                                |
                                v
                   +-------------------------+
                   |  IceBreaker / Netrunning |
                   |  (version.dll Loader)   |
                   +-------------------------+
```

1. **Zero-Trust Network Fallback**: Native DNS-over-HTTPS (Cloudflare DoH `https://1.1.1.1/dns-query`) engine ensuring reliable store search queries even under restricted network environments.
2. **Decoupled Architecture**: Clean separation between desktop management clients, frontend browser plugins, and low-level DLL hooks.
3. **Open Standards & Security**: Fully open-source codebase with configurable telemetry defaults and secure local key management.

---

## 📬 Contact & Community

* **GitHub Organization**: [github.com/NetrunnerGames](https://github.com/NetrunnerGames)
* **Bug Reports & Feature Requests**: Please submit issues on the respective project repository:
  * [DataJackUI Issues](https://github.com/NetrunnerGames/DataJackUI/issues)
  * [Jack-in Issues](https://github.com/NetrunnerGames/Jack-in/issues)
* **Contributions**: Pull requests are welcome across all repositories! Please adhere to our coding conventions and test guidelines.

---

<div align="center">

*Designed for Netrunners. Powered by Open Source.*

</div>
