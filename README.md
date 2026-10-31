# Lindoo Orca Plugins

Lindoo 维护的个人 Orca 插件市场。目前仅包含 Draw.io 插件。

| 路径 | 内容 |
| --- | --- |
| `plugins/drawio/` | Draw.io 插件源码与静态资源 |
| `orca-catalog.json` | Orca catalog v2 市场索引 |
| `scripts/release-entry.mjs` | 生成并检查插件发布元数据 |

## Draw.io

在 Orca 中离线创建和编辑 `.drawio` 与 `.drawio.xml` 图表，支持多页图表、主题同步和新建文件模板。

开发插件后运行测试：

```sh
node --test plugins/drawio/build/tests/editor.test.mjs
```

更新插件发布元数据时，需要一个已安装依赖的 Orca 源码目录：

```sh
ORCA_DIR=/path/to/orca node scripts/release-entry.mjs --write
ORCA_DIR=/path/to/orca node scripts/release-entry.mjs
```
