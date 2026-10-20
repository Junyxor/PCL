# Plain Craft Launcher

> **⚠ 本项目是特殊时期的临时解决方案**
>
> 本仓库是 [PCL](https://github.com/Meloong-Git/PCL) 的非官方临时分支。由于 PCL 上游在 2.99.0.0 中出于合规考虑移除了 Minecraft 下载与整合包安装功能，本分支临时恢复这些入口，供已了解并自行承担相关责任的使用者使用。
>
> **一旦 PCL 官方恢复下载功能，本仓库将立即归档，不再维护。**
>
> 本分支与原作者龙腾猫跃及 PCL 贡献者无隶属、合作或背书关系。PCL 的著作权归原作者所有，本分支仅依据其公开许可证进行修改与分发。本程序按「现状」提供，不附带任何担保，使用风险由使用者自行承担。

## 三个版本

| 版本 | 构建方式 | MC 下载 | 整合包 | 版本修改页 MC 卡片 | 内置凭据 | 更新通道 | 下载 |
|---|---|---|---|---|---|---|---|
| **开源版** | 源码重编译 | ✅ | ✅ | ✅ | ✅ | `-source` | [v2.99.0.0-source](https://github.com/Junyxor/PCL/releases/tag/v2.99.0.0-source) |
| **完整补丁版** | 官方 exe 全量 IL 补丁 | ✅ | ✅ | ✅ | ❌ | `update/fullpatch` | [v2.99.0.0-fullpatch](https://github.com/Junyxor/PCL/releases/tag/v2.99.0.0-fullpatch) |
| **最小补丁版** | 官方 exe 41 字节补丁 | ✅ | ❌ | ❌ | ❌ | `update/minpatch` | [v2.99.0.0-minpatch](https://github.com/Junyxor/PCL/releases/tag/v2.99.0.0-minpatch) |

- **开源版**：功能最全，有本项目的定制弹窗、关于页与内置凭据，更新检测只认 `-source` 标签。
- **完整补丁版**：基于官方 exe 重建被删除的 IL 逻辑，功能与开源版对齐，但界面保持官方原样、不内置凭据。
- **最小补丁版**：只改 41 字节恢复下载页入口，其余完全保持官方原样。

三个版本的更新检测完全独立，互不覆盖。补丁版内置的官方更新器已指向本仓库的 `update/` 静态配置，不会把程序更新回官方受限版。

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
