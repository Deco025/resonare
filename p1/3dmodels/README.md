# 3D 模型

下面 9 种器件的 3D 模型不在 KiCad 官方 3D 库里。它们来自厂家或立创商城，版权归原作者，所以**不随本仓库分发**。

只看原理图、PCB 或出生产文件时，不需要这些模型。想在 3D 查看器里看到完整外观，就按下表下载，**改成表中的文件名**，放进本目录（`p1/3dmodels/`）。两块板的封装已经指向这里，对齐参数也已设好。

| 文件名 | 器件 | 位号 | 来源 |
|---|---|---|---|
| `BSC070N10NS3G.step` | Infineon BSC070N10NS3G（PG-TDSON-8） | TX：Q1–Q4；RX：Q701、Q702、Q801 | 立创 C501502 |
| `UCC27211DRM.step` | TI UCC27211DRMR（VSON-8，4 × 4 mm） | TX：U201、U202；RX：U701 | 立创 C544677 |
| `SB2060L_PowerDI-5.step` | SB2060L（取得的模型为 TO-277 外形，作 PowerDI-5 替身） | RX：D601–D604 | 立创 C6067491 |
| `L_12x12mm_H8mm.step` | 12 × 12 mm 功率电感（TDK B82477P4 系列外形） | TX：L301 | 立创 C2042433 |
| `Vishay_WSK2512.step` | Vishay WSK2512 四端分流电阻 | TX：R101；RX：R801 | Vishay 官网 |
| `Littelfuse_NANO2_451_453.step` | Littelfuse NANO2 451 / 453 保险丝 | TX：F101 | pcb-3d.com |
| `AMASS_XT30PW-M.step` | AMASS XT30PW-M | TX：J101 | 立创 C431092 |
| `AMASS_XT60PW-M.step` | AMASS XT60PW-M | RX：J801 | 立创 C98732 |

- 立创的模型：在立创商城打开对应料号页面，从 EasyEDA 的 3D 模型处导出 STEP。也可以用开源工具 [easyeda2kicad](https://github.com/uPesy/easyeda2kicad.py)，例如：`easyeda2kicad --3d --lcsc_id C501502`。
- 完整链接与许可说明见 [SOURCES.md](SOURCES.md)。
- NR5040 电感（TX：L401、L402；RX：L901、L902）用的是 KiCad 自带的同尺寸模型 `L_APV_ANR5040`，无需下载。
