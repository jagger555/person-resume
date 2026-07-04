# 个人简历

中文简历 LaTeX 源码。

## 编译

需要 XeLaTeX 编译器，推荐以下两种方式：

### 本地编译

```bash
make
```

### Overleaf 在线编译

将整个项目打包为 zip，上传至 [Overleaf](https://www.overleaf.com)，编译器选择 **XeLaTeX**。

## 自定义

编辑 `resume-zh_CN.tex`，修改个人信息和经历即可。主要区域：

| 区域 | 说明 |
|------|------|
| 个人信息 | 姓名、籍贯、生日、电话、邮箱 |
| 教育背景 | 学校、专业、GPA、课程、荣誉 |
| 项目经历 | 使用 `\datedsubsection` 添加 |
| 竞赛经历 | 直接文本排版 |
| 个人评价 | 自由描述 |

### 字体

- 已安装 Adobe 宋楷黑仿四套字体 → 使用 `zh_CN-Adobefonts_internal`
- 未安装 → 使用 `zh_CN-Adobefonts_external`（默认，已内置在 `fonts/`）

在 `resume-zh_CN.tex` 开头切换：

```latex
\usepackage{zh_CN-Adobefonts_external}  % 默认
%\usepackage{zh_CN-Adobefonts_internal}  % 已安装 Adobe 字体时
```

## License

MIT
