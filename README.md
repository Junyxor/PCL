# Plain Craft Launcher

> **⚠ 本项目是特殊时期的临时解决方案**
>
> 本仓库是 [PCL](https://github.com/Meloong-Git/PCL) 的非官方临时分支。由于 PCL 上游在 2.99.0.0 中出于合规考虑移除了 Minecraft 下载与整合包安装功能，本分支临时恢复这些入口，供已了解并自行承担相关责任的使用者使用。
>
> **一旦 PCL 官方恢复下载功能，本仓库将立即归档，不再维护。**
>
> 本分支与原作者龙腾猫跃及 PCL 贡献者无隶属、合作或背书关系。PCL 的著作权归原作者所有，本分支仅依据其公开许可证进行修改与分发。本程序按「现状」提供，不附带任何担保，使用风险由使用者自行承担。

## 下载

同一个上游版本只发一条 Release，里面包含三个构建，按需选择：

**[v2.99.0.0](https://github.com/Junyxor/PCL/releases/tag/v2.99.0.0)**

| 资产 | 构建方式 | MC 下载 | 整合包 | 版本修改页 MC 卡片 | 内置凭据 | 界面 |
|---|---|---|---|---|---|---|
| `PCL2_2.99.0.0_Source.exe` | 源码修改后重编译 | ✅ | ✅ | ✅ | ✅ | 本项目定制 |
| `PCL2_2.99.0.0_FullPatch.exe` | 官方 exe 全量 IL 补丁 | ✅ | ✅ | ✅ | ❌ | 官方原版 |
| `PCL2_2.99.0.0_MinPatch.exe` | 官方 exe 41 字节补丁 | ✅ | ❌ | ❌ | ❌ | 官方原版 |

- **Source**：功能最完整，带本项目定制的启动弹窗、协议弹窗、关于页与免责声明，内置微软登录与 CurseForge 凭据。
- **FullPatch**：重建官方 exe 中因 `Const` 编译期折叠而删除的逻辑（下载页 Loader、版本修改页卡片、整合包 7 个分派分支），界面保持官方原样。
- **MinPatch**：只改 41 字节恢复下载页入口，其余完全保持官方原样。

三个构建共用同一版本号与同一更新通道。Source 查询本仓库最新 Release；两个补丁版内置的官方更新器已指向本仓库 `update/` 下的静态配置，不会把程序更新回官方受限版。

[![Stars](https://img.shields.io/github/stars/Meloong-Git/PCL?style=flat&logo=data:image/svg%2bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZlcnNpb249IjEiIHdpZHRoPSIxNiIgaGVpZ2h0PSIxNiI+PHBhdGggZD0iTTggLjI1YS43NS43NSAwIDAgMSAuNjczLjQxOGwxLjg4MiAzLjgxNSA0LjIxLjYxMmEuNzUuNzUgMCAwIDEgLjQxNiAxLjI3OWwtMy4wNDYgMi45Ny43MTkgNC4xOTJhLjc1MS43NTEgMCAwIDEtMS4wODguNzkxTDggMTIuMzQ3bC0zLjc2NiAxLjk4YS43NS43NSAwIDAgMS0xLjA4OC0uNzlsLjcyLTQuMTk0TC44MTggNi4zNzRhLjc1Ljc1IDAgMCAxIC40MTYtMS4yOGw0LjIxLS42MTFMNy4zMjcuNjY4QS43NS43NSAwIDAgMSA4IC4yNVoiIGZpbGw9IiNlYWM1NGYiLz48L3N2Zz4=&logoSize=auto&label=Stars&labelColor=444444&color=eac54f)](https://github.com/Meloong-Git/PCL/)
[![Issues](https://img.shields.io/github/issues/Meloong-Git/PCL?style=flat&label=Issues&labelColor=444444&color=1F883D)](https://github.com/Meloong-Git/PCL/issues)
[![哔哩哔哩](https://img.shields.io/badge/动态-BiliBili-00A4DB?style=flat&labelColor=444444&logoSize=auto)](https://space.bilibili.com/11343203/dynamic)
[![爱发电](https://img.shields.io/badge/赞助-爱发电-946ce6?style=flat&labelColor=444444&logoSize=auto)](https://meloong.com/afd/a/LTCat)

包含 PCL 的大部分源代码，包括 UI 库、动画模块、下载模块、Minecraft 启动模块等！<br/>
代码并不是实时更新的，它会在每次 PCL 发布更新时同步一次。<br/>
非常感谢社区的大力支持！

<br/>

### 相关资源
- [PCL 下载](https://meloong.com/pcl)：下载可免费使用的正式版 PCL！
- [PCL 功能投票](https://github.com/Meloong-Git/PCL/discussions/2)：来参加投票吧，开发者会优先处理票数较高的项目！
- [帮助文档库](https://github.com/LTCatt/PCL2Help)：PCL 内置帮助文档的存储库
