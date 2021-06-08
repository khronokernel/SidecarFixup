SidecarFixup
==============

[![Build Status](https://github.com/acidanthera/SidecarFixup/workflows/CI/badge.svg?branch=master)](https://github.com/acidanthera/SidecarFixup/actions) [![Scan Status](https://scan.coverity.com/projects/23155/badge.svg?flat=1)](https://scan.coverity.com/projects/23155)

[Lilu](https://github.com/acidanthera/Lilu) Kernel extension for enabling Sidecar support on the following SMBIOS:

```
iMac13,x - iMac16,x
MacBook8,1
MacBookAir5,x - MacBookAir7,x
MacBookPro9,x - MacBookPro12,x
Macmini6,x - Macmini7,1
MacPro5,1 - MacPro6,1
```

Additionally whitelists the following iPad Models:

```
iPad4,x - iPad6,x
```

**Note**: Requires a machine with an Intel iGPU enabled and active, dGPU-only machines will not work.

#### Boot arguments

- `-caroff` (or `-liluoff`) to disable
- `-cardbg` (or `-liludbgall`) to enable verbose logging (in DEBUG builds)
- `-carbeta` (or `-lilubetaall`) to enable on macOS newer than 12

#### Credits

- [Apple](https://www.apple.com) for macOS  
- [vit9696](https://github.com/vit9696) for [Lilu.kext](https://github.com/vit9696/Lilu)
- [Osy](https://github.com/Osy/Polaris22Fixup/) and [DhinakG](https://github.com/dhinakg/Polaris22Fixup/) for Polaris22Fixup base
- [Ben-z](https://github.com/ben-z/free-sidecar) for original patch SidecarCore patch set
