# The Feynman Lectures on Physics - LaTeX 中文版

费曼物理学讲义中文 LaTeX 版本，现已开放全部最新进展。

The Chinese translation of The Feynman Lectures on Physics using LaTeX, now with all latest progress publicly available.

## 📚 当前进度 Current Progress

- **第一卷（力学、辐射和热学）**: 第 1-52 章 ✅
- **第二卷（电磁学和物质）**: 第 1 章 ✅  
- **第三卷（量子力学）**: 第 1 章 ✅

共计 693 页，完整编译通过。

## 🔧 编译方法 Compilation

### 环境要求 Requirements
- XeLaTeX (TeX Live 2020 或更高版本)
- 中文字体：SimSun（宋体）
- Times New Roman 字体

### 编译命令 Build Command

```bash
# 使用 latexmk 自动处理多遍编译和交叉引用
latexmk -xelatex -interaction=nonstopmode "Feynman Lectures on Physics.tex"

# 或手动编译（需运行 2-3 次以解析引用）
xelatex "Feynman Lectures on Physics.tex"
xelatex "Feynman Lectures on Physics.tex"
```

编译成功后生成 `Feynman Lectures on Physics.pdf`（约 8.3 MB）。

## 📁 目录结构 Structure

```
├── Feynman Lectures on Physics.tex    # 主文件
├── Cover.pdf                           # 封面
├── Chapters/
│   ├── VolumeI/                       # 第一卷章节
│   ├── VolumeII/                      # 第二卷章节
│   └── VolumeIII/                     # 第三卷章节
└── Figures/
    ├── VolumeI/                       # 第一卷插图
    ├── VolumeII/                      # 第二卷插图
    └── VolumeIII/                     # 第三卷插图
```

## 🧹 仓库清理 Repository Cleanup

为保持仓库简洁，已移除所有中间编译产物：
- `*.aux` - 辅助文件
- `*.gz` - 压缩文件
- `*.fls` - 文件列表

最终的 PDF 文件保留在仓库中供直接下载使用。

## 🤝 贡献 Contributing

欢迎贡献新的章节、修正错误或改进排版！

Contributions are welcome! Feel free to:
- Add new chapters
- Fix typos or errors
- Improve typesetting

## 📄 许可 License

本项目仅用于学习交流，版权归原作者所有。

This project is for educational purposes only. All rights belong to the original authors.

## 🙏 致谢 Acknowledgments

感谢理查德·费曼教授的不朽著作，以及所有为本项目做出贡献的志愿者。

Thanks to Professor Richard Feynman for his immortal work, and to all volunteers who contributed to this project.
