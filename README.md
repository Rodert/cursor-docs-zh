# Cursor 文档

这个仓库包含了 [Cursor 的文档](https://docs.cursor.com) 的源代码。

欢迎提交 Pull Request 来帮助改进文档！

## 开发

安装 [Mintlify CLI](https://www.npmjs.com/package/mintlify) 来在本地预览文档更改。使用以下命令安装：

```bash
npm install mintlify
```

在文档根目录（包含 mint.json 的目录）运行以下命令：

```bash
mintlify dev
```

## 部署

文档会在推送到 main 分支时自动构建和部署。只需要：

```bash
git add .
git commit -m "docs: update documentation"
git push
```

GitHub Actions 会自动构建并部署最新的文档到 GitHub Pages。

### 故障排除

- Mintlify dev 无法运行 - 运行 `mintlify install` 重新安装依赖。
- 页面显示 404 - 确保你在包含 `mint.json` 的文件夹中运行命令。
