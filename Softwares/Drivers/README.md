# Drivers

This repository contains only the LattePanda Mu Ultra drivers. For drivers related to the carrier board, please refer to the carrier board documentation.

## Windows 11

After installing Windows 11 OS, the OS will automatically connect to the internet to download driver updates. If it is unable to access the Windows Update service, or if there are missing drivers after the automatic updates, you can download the offline driver package here.


| Name                                | Version         | Size    | Download                                                                        |
|--------------------------------------------|-----------------|---------|---------------------------------------------------------------------------------|
| Intel Chipset Driver                       | 10.1.48.18     | 11 KB   | [⬇️](./Intel_Chipset_Driver_10.1.48.18.zip) |
| Intel Network Adapter Driver | 2.1.5.7   | 37.2 MB | [⬇️](./Intel_Wired_Lan_driver_31.1_x64_win11.zip) |
| Intel Arc Graphics Driver | Latest | /  | [⬇️](https://www.intel.com/content/www/us/en/download/785597/intel-arc-graphics-windows.html)[^1] |
| Realtek Audio Driver | 6.0.9782.1 | 37.6 MB | [⬇️](./Realtek_Audio_Driver_6.0.9782.1.zip)                      |
| Touch Panel Driver | 1.3.2.0 | 63.4 KB | [⬇️](./TouchPanel_1.3.2.0.zip)                                   |
| Intel Serial IO Driver | 30.100.2416.40 | 445 KB | [⬇️](./Intel_Serial_IO_Driver_30.100.2416.40.zip)                |
| Intel Management Engine Interface Driver | 2512.7.3.0 | 2 MB | [⬇️](./Intel_Management_Engine_Interface_Driver_2512.7.3.0.zip)  |
| Intel Platform Monitoring Technology Driver | 5.2.3.4  | 50.8 KB | [⬇️](./Intel_Platform_Monitoring_Technology_Driver_5.2.3.4.zip)  |
| Intel Smart Sound Technology Driver | 20.42.12350.0 | 40.6 MB | [⬇️](./Intel_SST_LNL_v20.42.12350.0_Prod.zip) |
| Intel NPU Driver | Latest | / | [⬇️](https://www.intel.com/content/www/us/en/download/794734/intel-npu-driver-windows.html)[^1] |

[^1]: Download from intel official website

## Linux

Linux drivers are generally provided by the distribution through kernel and kernel module updates. Please use a newer kernel version to ensure full driver support.

- Minimum Kernel Requirement: 6.11 or higher

The following two drivers need to be installed separately:

- Intel GPU Compute Driver

  - [Click here for installation guide](https://dgpu-docs.intel.com/installation-guides/index.html)

- Intel NPU Driver

  - [Click here for installation guide](https://github.com/intel/linux-npu-driver/releases)
