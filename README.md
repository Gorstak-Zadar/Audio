# 🔊 Audio

> Windows PowerShell utility to enable **Acoustic Echo Cancellation (AEC)** and **Noise Suppression** on all audio devices.

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 🔇 **AEC** | Reduces echo in voice calls and recordings |
| 🎚️ **Noise Suppression** | Reduces background noise for clearer audio |
| 📻 **All Devices** | Applies settings to every audio render device |
| 🔧 **Registry-based** | Uses Windows MMDevices API configuration |

---

## 📋 Requirements

| Requirement | Details |
|-------------|---------|
| **OS** | Windows 10/11 |
| **PowerShell** | 5.1+ |
| **Privileges** | Administrator |

---

## 🚀 Usage

```powershell
# Run as Administrator
.\Audio.ps1
```

---

## 🔧 What It Does

- Takes ownership of `FxProperties` registry keys under `HKLM:\SOFTWARE\Microsoft\Windows\CurrentVersion\MMDevices\Audio\Render`
- Enables **Acoustic Echo Cancellation** (`{1c7b1faf-caa2-451b-b0a4-87b19a93556a},6 = 1`)
- Enables **Noise Suppression** (`{e0f158e1-cb04-43d5-b6cc-3eb27e4db2a1},3 = 1`)

---

<p align="center">
  <sub>🔧 Gorstak Windows Security Tooling</sub>
</p>
