<html>
 <h2>ROG Zephyrus G14 GA402RK – Hackintosh (macOS 15.5 Sequoia)</h2>
<p><strong>Status</strong>: ✅ Working<br>
<strong>Model</strong>: GA402RK (Ryzen 9 6900HS + Radeon RX 6800S), GA402RJ will work too<br>
<strong>macOS Version</strong>: macOS Sequoia 15.5<br>
<strong>EFI Source</strong>: <a href="https://drive.google.com/file/d/1m7VaAxh2oUaFYqP6vWavmVwGE0ntqzhM/view?usp=sharing">EFI Download (Google Drive)</a></p>
<hr>
<h3>✅ What works</h3>

Feature | Status | Notes
-- | -- | --
GPU Acceleration (RX6800S) | ✅ Yes | Using NootRx.kext + proper device injection
Audio | ✅ Yes | AppleALC working with internal speakers and mic
USB Ports | ✅ Yes | USBMap completed
Keyboard / Trackpad | ✅ Yes | Basic functionality (no gestures on trackpad)
Battery Status | ✅ Yes | Battery percentage shows correctly
HDMI Output | ✅ Yes | Fully working with RX6800S
Sleep / Wake | ⚠️ Partial | Works but can be unstable sometimes
Wi-Fi (Intel AX210) | ✅ Yes | Using itlwm.kext + HeliPort
Bluetooth (Intel AX210) | ✅ Yes | Using BTPatch.kext
iServices (iCloud, etc) | ✅ Yes | All work after SMBIOS + Ethernet fix


<hr>
<h3>📂 EFI Info</h3>
<ul>
<li>
<p>Based on OpenCore 1.0.4</p>
</li>
<li>
<p>Patched with AMD Vanilla (15.4 support) lastest patch</p>
</li>
<li>
<p>Includes:</p>
<ul>
<li>
<p><code inline="">NootRx.kext</code></p>
</li>
<li>
<p><code inline="">Lilu</code>, <code inline="">VirtualSMC</code>, <code inline="">WhateverGreen</code>, <code inline="">AppleALC</code></p>
</li>
<li>
<p><code inline="">itlwm.kext</code>, <code inline="">HeliPort</code>, <code inline="">BTPatch.kext, ...</code> (for AX210)</p>
</li>
<li>
<p>USBMap.kext</p>
</li>
<li>
<p>ACPI: <code inline="">SSDT-EC</code>, <code inline="">SSDT-USBX</code>, <code inline="">SSDT-PLUG</code></p>
</li>
</ul>
</li>
<li>
<p><code inline="">SMBIOS</code>: MacPro7,1</p>
</li>
</ul>
<hr>
<h3>📝 Notes</h3>
<ul>
<li>
<p>System can use for development (Xcode with ios simulator support, browsing, media) </p>
</li>
<li>
<p>You <em>must</em> disable iGPU and use dGPU-only mode</p>
</li>
<li>
<p>First boot may take time — let it finish!</p>
</li>
<li>
<p>HeliPort auto-launch recommended for Wi-Fi</p>
</li>
<li>
<p>You can use Bluetooth keyboard/mouse normally with BTPatch</p>
</li>
</ul>
<hr>
<h3>🔗 Links</h3>
<ul>
<li>
<p>EFI (Google Drive): <a href="https://drive.google.com/file/d/1m7VaAxh2oUaFYqP6vWavmVwGE0ntqzhM/view?usp=sharing">EFI Folder</a></p>
</li>
<li>
<p>Reference: <a href="https://github.com/b00t0x/ROG-Zephyrus-G14-GA402-Hackintosh">b00t0x GA402 GitHub</a></p>
</li>
<li>
<p>itlwm repo: <a href="https://github.com/OpenIntelWireless/itlwm">OpenIntelWireless</a></p>
</li>
</ul>
<hr>
<h3>🗨️ Credits</h3>
<ul>
<li>
<p>AMD OS X Community</p>
</li>
<li>
<p>Dortania OpenCore Guide</p>
</li>
<li>
<p>OpenIntelWireless for AX210 support</p>
</li>
<li>
<p>@b00t0x for base structure</p>
</li>
<li>
<p>@your-name (replace with Reddit or GitHub handle) for macOS 15.4 port on GA402RK</p>
</li>
</ul>
<hr>
<p>✅ Bạn muốn mình đóng gói lại thành <code inline="">README.md</code> + folder chuẩn GitHub để bạn upload không? Mình có thể tạo bản <code inline="">.zip</code> sẵn để bạn chỉ việc push lên GitHub nếu cần.</p></body></html><!--EndFragment-->
</body>
</html>Tuyệt vời! Mình sẽ cập nhật lại nội dung theo đúng cấu trúc GitHub như trước, nhưng **chính xác hơn với thông tin bạn cung cấp**:

* ✅ HDMI hoạt động
* ✅ Wi-Fi + Bluetooth (Intel AX210) hoạt động qua HeliPort + BTPatch

---

## ROG Zephyrus G14 GA402RK – Hackintosh (macOS 15.4 Sequoia)

**Status**: ✅ Working
**Model**: GA402RK (Ryzen 9 6900HS + Radeon RX 6800S)
**macOS Version**: macOS Sequoia 15.4 (Developer Beta)
**EFI Source**: [[EFI Download (Google Drive)](https://drive.google.com/file/d/1m7VaAxh2oUaFYqP6vWavmVwGE0ntqzhM/view?usp=sharing)](https://drive.google.com/file/d/1m7VaAxh2oUaFYqP6vWavmVwGE0ntqzhM/view?usp=sharing)

---

### ✅ What works

| Feature                    | Status     | Notes                                           |
| -------------------------- | ---------- | ----------------------------------------------- |
| GPU Acceleration (RX6800S) | ✅ Yes      | Using `NootRx.kext` + proper device injection   |
| Audio                      | ✅ Yes      | AppleALC working with internal speakers and mic |
| USB Ports                  | ✅ Yes      | USBMap completed                                |
| Keyboard / Trackpad        | ✅ Yes      | Basic functionality (no gestures on trackpad)   |
| Battery Status             | ✅ Yes      | Battery percentage shows correctly              |
| HDMI Output                | ✅ Yes      | Fully working with RX6800S                      |
| Sleep / Wake               | ⚠️ Partial | Works but can be unstable sometimes             |
| Wi-Fi (Intel AX210)        | ✅ Yes      | Using `itlwm.kext` + HeliPort                   |
| Bluetooth (Intel AX210)    | ✅ Yes      | Using `BTPatch.kext`                            |
| iServices (iCloud, etc)    | ✅ Yes      | All work after SMBIOS + Ethernet fix            |

---

### ❌ What doesn’t work

| Feature               | Status        | Notes                                    |
| --------------------- | ------------- | ---------------------------------------- |
| Internal iGPU (RDNA2) | ❌ Not Working | Ryzen 6900HS iGPU not supported in macOS |
| Brightness keys       | ❌ Not working | Use `MonitorControl.app` instead         |
| Touchscreen           | ❌ Not working | No macOS support                         |

---

### 📖 Requirements

* macOS installer (create via [[GibMacOS](https://github.com/corpnewt/gibMacOS)](https://github.com/corpnewt/gibMacOS) or [[OCLP](https://dortania.github.io/OpenCore-Legacy-Patcher/)](https://dortania.github.io/OpenCore-Legacy-Patcher/))
* OpenCore 1.0.0+
* A USB drive (16GB+)
* BIOS set to **Discrete Graphics (dGPU only)**

---

### 🛠️ BIOS Settings

1. Enter BIOS by pressing `DEL` during boot
2. Set the following:

| Setting      | Value             |
| ------------ | ----------------- |
| GPU Mode     | Discrete Graphics |
| Fast Boot    | Disabled          |
| Secure Boot  | Disabled          |
| AMD SVM Mode | Enabled           |


---

### 📂 EFI Info

* Based on OpenCore 1.0.4
* Patched with AMD Vanilla (15.5 support) lastest
* Includes:

  * `NootRx.kext`
  * `Lilu`, `VirtualSMC`, `WhateverGreen`, `AppleALC`
  * `itlwm.kext`, `HeliPort`, `BTPatch.kext` (for AX210)
  * USBMap.kext
  * ACPI: `SSDT-EC`, `SSDT-USBX`, `SSDT-PLUG`
* `SMBIOS`: MacPro7,1

---

### 📝 Notes

* System is stable for development use (Xcode, browsing, media)
* You *must* disable iGPU and use dGPU-only mode
* First boot may take time — let it finish!
* HeliPort auto-launch recommended for Wi-Fi
* You can use Bluetooth keyboard/mouse normally with BTPatch

---

### 🔗 Links

* EFI (Google Drive): [[EFI Folder](https://drive.google.com/file/d/1m7VaAxh2oUaFYqP6vWavmVwGE0ntqzhM/view?usp=sharing)](https://drive.google.com/file/d/1m7VaAxh2oUaFYqP6vWavmVwGE0ntqzhM/view?usp=sharing)



---

### 🗨️ Credits

* AMD OS X Community
* Dortania OpenCore Guide
* OpenIntelWireless for AX210 support
* @b00t0x for base structure
* @neoncuber129 for macOS 15.4 port on GA402RK
