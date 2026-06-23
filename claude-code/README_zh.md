# Claude Code技能

[英文版本](../README.md) | [中文版本](./README_zh.md)

---

> 针对[Claude Code](https://claude.ai/code) IDE的生产力自动化和快速命令扩展。

**← [返回主目录](../README.md)**

---

## 可用技能

| 技能 | 描述 | 类型 |
|------|------|------|
| **[`perplexity-downloader`](./perplexity-downloader/)** | 下载并导出Perplexity.ai对话为Markdown文件 | 技能 |
| **[`readme-i18n`](./readme-i18n/)** | 同步README.md到简体中文，保持英文为主源
| **[`twitter-bookmarks-exporter`](./twitter-bookmarks-exporter/)** | 导出X/Twitter书签为带元数据的Markdown文件 |

---

## 前置条件

- 已安装并验证[Claude Code](https://claude.ai/code)
- Python 3.8+

---

## 安装

### 技能

1. 在Claude Code中进入 **设置** → **技能**
2. 点击 **导入** 或 **+** 添加自定义技能
3. 选择此目录中的 `.skill` 文件
4. 该技能即可在Claude Code中使用

### 命令（项目级）

```bash
cp -r ../.claude /your/project/
```

### 命令（全局）

```bash
cp -r ../.claude ~/.claude/
```

---

## 用法

在任何Claude Code会话中，通过技能名调用:

```
/perplexity-downloader https://www.perplexity.ai/search/...
/export-twitter-bookmarks
/readme-i18n
```

详见各技能文件夹的README.md

---

## 贡献

详见[`../CONTRIBUTING.md`](../CONTRIBUTING.md)的通用规则

针对Claude Code技能:

1. 新建目录: `mkdir my-skill-name`
2. 添加你的技能文件: `my-skill-name.skill` (包含SKILL.md)
3. 添加README.md说明安装和使用
4. 在本地导入Claude Code中测试
5. 提交PR

---

## 许可证

遵循MIT许可证。