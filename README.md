# ~~寻找 taffy~~ 传递闭包算法仓库

在终端中执行 `git clone https://github.com/YuxuanQin/closure.git` 可以把本仓库的所有文件下载到本地。

## 构建说明 (命令行界面)

> （注意，这是针对命令行下的编译指导，如果用的是 IDE，可以略过）

要是下了完整的 TeXLive，构建应该不会有什么大问题，不过要注意，由于种种因素，存在目录的 `.tex` 文档需要**多次编译**！

在终端中执行至少两次

```
xelatex paper.tex
```


针对代码本身的说明请看注释。

## 编译注记
使用 [tectonic](https://github.com/tectonic-typesetting/tectonic) 来编译会获得更好的体验：

- 自动下载缺少的各种文件，例如 `.otf`、`.sty`。
- 自动清理冗余的辅助文件，例如 `.aux`、`.log`。
- **忠实地完成一个程序应该做的所有事情**：使用 `xelatex` 或者 `latex` 编译带目录的文件时，需要你**手动**多次编译，这是为何？作为一个只想要结果 —— pdf —— 的用户而言，实在是太烦人了。

一切只需要遵从 [How to: Install Tectonic](https://tectonic-typesetting.github.io/book/latest/installation/) 的指示，执行那段 “Copy-paste terminal command”，再放进你的路径中，最后：

```
tectonic file.tex
```

一切就完成了，谁 tm 关心那些 `.aux`、`.out` :laughing:？
