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

---

## Disclaimer

**NO WARRANTY.** THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.

**Limitation of Liability.** IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
