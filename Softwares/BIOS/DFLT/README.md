# BIOS Release Notes

## [2026-04] Initial Release

### 📂 BIOS Files
| Compatible Model | Filename | Build Date |
| :--- | :--- | ---- |
| LattePanda Mu Ultra 226V 16GB | `SBCLNLCXR120-A.bin` | 2026/04/30 |
| LattePanda Mu Ultra 256V 16GB | `SBCLNLCXR120-A.bin` | 2026/04/30 |


### 📝 Changelog
- Initial BIOS firmware release

---

## Interface Configuration

### Special Notes

- **USB2_P1**: Dedicated for USB Type-C, must be used in conjunction with a PD controller, **cannot be used as a standard USB port**.
- **USB2_P2**: Dedicated for USB Type-C, must be used in conjunction with a PD controller, **cannot be used as a standard USB port**.
- **USB2_P6**: Dedicated for Bluetooth, must be used in conjunction with M.2 wireless module, **cannot be used as a standard USB port**.

### PCIe Bifurcation

| PCIe Lane    | BIOS Configuration   | Associated REFCLK   |
| ------------ | -------------------- | ------------------- |
| PCIe Lane #3 | PCIe 4.0 x1          | REFCLK0             |
| PCIe Lane #4 | PCIe 4.0 x1          | REFCLK3             |
| PCIe Lane #5 | PCIe 4.0 x4 (Lane 0) | REFCLK2             |
| PCIe Lane #6 | PCIe 4.0 x4 (Lane 1) | Shared with REFCLK2 |
| PCIe Lane #7 | PCIe 4.0 x4 (Lane 2) | Shared with REFCLK2 |
| PCIe Lane #8 | PCIe 4.0 x4 (Lane 3) | Shared with REFCLK2 |
| PCIe Lane #1 | PCIe 4.0 x2 (Lane 0) | REFCLK4             |
| PCIe Lane #2 | PCIe 4.0 x2 (Lane 1) | Shared with REFCLK4 |

### DDI&TCP

- **DDIA**: eDP (FPC connector on LattePanda Mu Ultra)
- **TCP0**: USB Type-C (requires external PD controller)
- **TCP1**: USB Type-C (requires external PD controller)
- **TCP2**: HDMI

### GPIO

- **I2C0**: Touch panel (FPC connector on LattePanda Mu Ultra)
- **I2C1**: Communication with Type-C PD controller
- **GPP_B05**: Communication interrupt with Type-C PD controller
- **GPP_E22**: Communication interrupt with Type-C PD controller
- **GPP_B07**: Output blink signal in Modern Standby state

Other GPIOs not listed are not allocated specific functions.
