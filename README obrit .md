[README.md](https://github.com/user-attachments/files/33275651/README.md)
# 文档索引

| 文档 | 内容 |
|---|---|
| [README](../README.md) | 仓库总览、安装、用法、已知限制、推送命令 |
| [orbit-parameters.md](orbit-parameters.md) | **具体轨道参数总表**：天体常数、二体公式、地球/Kerbin 常用轨道全量数值 |
| [上传到GitHub.cmd](../上传到GitHub.cmd) | 双击即用的推送脚本（init → add → commit → pull → push，含文件清单核对） |

## 代码入口

| 文件 | 作用 |
|---|---|
| [kerbin_orbit.ks](../Ships/Script/kerbin_orbit.ks) | 主脚本：点火 → 重力转弯 → MECO → 滑行 → 圆化 → 打印参数 |
| [orbit_params.ks](../Ships/Script/orbit_params.ks) | 只读：打印当前飞船完整轨道参数 |
| [lib/orbit_lib.ks](../Ships/Script/lib/orbit_lib.ks) | 轨道数学库 + 参数报表 |
| [lib/orbit_presets.ks](../Ships/Script/lib/orbit_presets.ks) | kOS 侧轨道预设表 |
| [EarthOrbit.cfg](../GameData/KerbinEarthOrbit/EarthOrbit.cfg) | 地球天体参数（MM 数据节点 + 可选 Kopernicus 补丁） |
| [OrbitPresets.cfg](../GameData/KerbinEarthOrbit/OrbitPresets.cfg) | 轨道预设数据节点（纯数据） |

## 数据来源

- WGS84 / IERS Conventions — 地球形状、自转、$J_2$、$J_3$、$J_4$
- NASA JPL — 地球日心轨道根数（J2000）、$\mu_\odot$
- KSP 原版数据 — Kerbin 半径 600 km、$\mu = 3.5316\times10^{12}$、恒星日 21 549.425 s
