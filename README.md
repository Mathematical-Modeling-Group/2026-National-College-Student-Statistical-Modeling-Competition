# 低碳城市试点与减污降碳压力研究

本仓库整理了统计建模论文的最终 LaTeX 文稿、图表资源和复现实证分析所需代码。

## 项目结构

```text
.
├── 统计建模论文.tex          # 论文 LaTeX 源文件
├── 统计建模论文.pdf          # 已编译论文 PDF
├── requirements.txt          # Python 代码依赖
├── assets/
│   ├── figures/              # 论文图片资源
│   └── fonts/                # LaTeX 编译所需中文字体
└── code/
    ├── did_critic_lnco2_3poll_baseline.ipynb
    ├── final_code.ipynb
    ├── parallel_trend_from_notebook.png
    └── placebo_from_notebook.png
```

## 编译论文

建议使用 XeLaTeX 编译：

```powershell
xelatex -interaction=nonstopmode "统计建模论文.tex"
xelatex -interaction=nonstopmode "统计建模论文.tex"
```

中文字体位于 `assets/fonts/`。如果公开发布仓库前需要避免字体版权风险，可以删除该目录，并在本地自行安装或配置对应字体后再编译。

## 运行代码

安装 Python 依赖：

```powershell
pip install -r requirements.txt
```

随后在 Jupyter 环境中运行 `code/` 目录下的 notebook。

## 说明

仓库保留最终论文、必要图表、字体文件和核心代码；原始参考资料、临时编译文件、旧版本文稿和大体积压缩包未纳入此整理目录。
