<img src="./assets/journal-scout-logo.webp" alt="Journal Scout logo" width="112" height="112">

# Journal Scout for Zotero

在 Zotero 文献列表与右侧面板中查看、归档和筛选期刊指标及 CCF 会议等级。

![Journal Scout 在 Zotero 文献列表显示期刊指标，右侧面板可选择显示指标与显示位置](./assets/zotero-overview.webp)

[下载安装与图文说明](https://journal.scansci.com/extension-install.html#zotero-install) · [发行版本](https://github.com/Rimagination/journal-scout-zotero/releases) · [问题反馈](https://github.com/Rimagination/journal-scout-zotero/issues)

Journal Scout for Zotero displays, archives and filters journal metrics and CCF conference rankings in Zotero. Published by ScanSci.

## 功能

- 在 Journal Scout 列和侧栏查看影响因子、JCR 分区、中科院分区、Top、CCF、中文核心等指标；未收录或无法确认的数据保留为空。
- 高级搜索提供独立的 Journal Scout 指标菜单。影响因子支持完整小数的等于、不等于、大于和小于比较，可组合条件并保存搜索。
- 将确认的指标存入条目 Extra（附加信息），复用本地归档和期刊缓存；网站发布数据版本后优先更新当前查看的文献。
- 可逐项选择显示的指标，切换「列表列与侧边栏」或「仅侧边栏」，调整配色、字号、圆角与间距。
- 在「设置 → Journal Scout」中按需补全文库期刊指标，运行时显示进度并支持取消；已完成的归档会保留。
- 支持 Zotero 原生自动更新。原生标签兼容筛选也会保留，数值范围筛选使用独立指标字段。

![Zotero 中的 Journal Scout 列及兼容原生标签筛选示例](https://journal.scansci.com/assets/install-guide/zotero-tag-filter.webp)

## 安装与兼容性

当前版本为 **v0.1.1**。安装清单声明支持 **Zotero 7–10**；已在 **10.0.8** 实测，7–9 尚未逐版测试。Zotero 6 不支持。

1. 从[发行页](https://github.com/Rimagination/journal-scout-zotero/releases/latest)或[官网](https://journal.scansci.com/extension-install.html#zotero-install)下载 `.xpi`。
2. 打开 Zotero「工具 → 插件」，点击右上角齿轮，选择「从文件安装插件 / Install Plugin From File」。
3. 选择安装包，安装后选中文献即可查看指标。显示选项位于「编辑 → 设置 → Journal Scout」（Windows）。

更新遵循 Zotero 插件管理器中的设置；需要立即更新时，点击齿轮菜单「检查更新 / Check for Updates」。

## 数据与同步

插件查询期刊服务时只使用条目已有的刊名或 ISSN，不上传论文全文或附件；会议等级按会议名称匹配 CCF 目录。指标数据可能存在缺失或更新延迟，使用时请核对对应年度和原始来源。

自动归档会修改条目的 Extra 和插件管理的原生标签，保留已有正文及用户标签。这些条目修改可能随 Zotero 同步，并可能包含在部分导出文件中。本地显示设置不影响完整归档。只读或正在编辑的条目会跳过。

原生更新清单：[updates/zotero.json](https://journal.scansci.com/updates/zotero.json)。数据版本信号：[zotero-data-release.json](https://journal.scansci.com/data/zotero-data-release.json)。

本仓库用于发布 Journal Scout for Zotero 的安装包与使用说明。产品主页：[Journal Scout](https://journal.scansci.com/)。
