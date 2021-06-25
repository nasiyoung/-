文件后缀：.tex

文档内容结构

```
（导言区）
\documentclass{article}
    <宏包引用>
（正文区）
\begin{document}
    <正文>
\end{document}
```

查看帮助文档：texdoc 宏包名

注释：%

快速注释：Ctrl+T

取消注释：Ctrl+U

加入年月日：\maketitle

换行符：\\\ 没有产生新段落，不会自动生成首行缩进

换段落符：①空行②\par  会自动生成首行缩进

# 字体
## 1.族
### A 罗马字

```
\textrm{...}
\rmfamily ...
```

### B 无衬线

```
\textsf{...}
\sffamily ...
```

### C 等宽

```
\texttt{...}
\ttfamily ...
```

## 2 系列
### A 细字体
中文为楷体
```
\textmd{...}
\mdseries ...
```

### B 粗字体
中文为黑体

```
\textbf{...}
\bfseires ...
```

## 3 形状
### A 直立

```
\textup{...}
\upshape ...
```
### B 斜体

```
\textit{...}
\itshape ...
```
### C 伪斜体

```
\textsl{...}
\slshape ...
```
### D 小型大写

```
\textsc{...}
\scshape ...
```
## 4 中文字体
分别对应其中文拼音

```
宋体 \songti
黑体 \heiti
仿宋 \fangsong
楷书 \kaishu
```
## 5 字号
均是与 ```normal size``` 的相对大小

设置```normal size```
```
\documentclass[xxpt]{}
通常只有10，11，12pt
```

```
Huge  huge  LARGE  Large  large  normalsize  
small  footnotesize  scriptsize tiny
```

# 文档结构
## 一级标题
```
\section{...}
```
当```documentclass{ctexart}```则一级标题默认居中
## 二级标题
```
\subsection{...}
```

## 三级标题
```
\subsubsection{...}
```

## 带第x章的标题
```
\chapter{...}
需用\documentclass{ctexbook}
此时三级标题不起作用
```

## 产生整个文档的目录
```
\tableofcontents
```

# 特殊字符
## 1 空白
正文中加入一个或多个空格效果一样

中文：无空格

英文：一个空格

中英文混排时，交替处会自动产生一个空格

可以使用命令产生指定宽度的空白如```\quad```

```
 % 1em的空白
    a\quad b
    
    % 2em空白
    a\qquad b
    
    % 1/6em空白
    a\,b
    
    a\thinspace b
    
    % 1/2空白
    a\enspace b
    
    % 空格
    a\ b
    
    % 硬空格（不可分割）
    a~b
    
    % 1pc = 12pt = 4.218mm
    a\kern 1pc b
    
    a\kern -1em b
    
    a\hskip 1em b
    
    a\hspace{35pt}b
    
    % 占位宽度
    a\hphantom{xyz}b
    
    % 弹性长度
    a\hfill b
```

## 2 控制符
```
符号 | 代码
-----|----
#    | \#
$    | \$
{}   | \{  \}
~    | \~{}
_    | \_{}
^    | \^{}
\    | \textbackslash
&    | \&
```

## 3 引号
```
`左侧单引号
'右侧单引号
``左双引号
''右双引号
```

## 4 特殊字符表
![](https://github.com/nasiyoung/Miscellaneous/blob/main/images/%E5%B8%8C%E8%85%8A%E5%AD%97%E6%AF%8D)
