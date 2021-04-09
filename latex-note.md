split, multi-lign and align:

Align, from amsmath package:
numbered equations aligned at points marked
with \verb|&| usually just before a relation.

```
\begin{align}
a_1& =b_1+c_1\\
a_2& =b_2+c_2-d_2+e_2
\end{align}
```

split, also from amsmath,
similar alignment to align, but the whole construct fits within
equation (or other display math) and is numbered as a unit.
```
\begin{equation}\label{xx}
\begin{split}
a& =b+c-d\\
 & \quad +e-f\\
 & =g+h\\
 & =i
\end{split}
\end{equation}
```

multline, from amsmath
for lonq expressions taking more than one line,
with no specifed alignment points.
```
\begin{multline}
a+b+c+d+e+f+g+h+i+j+k+\\
l+m+n+o+p+q+r+s+t+w+x+y+z
\end{multline}
```
---
There are three commands here that work the same in the example:
```
    \\ (two backslashes)
    \newline
    \hfill \break 
```
--- 
Force image position:  
```
\usepackage{float}  
...
\begin{figure}[H]  
\centering
\includegraphics{slike/visina8}
\caption{Write some caption here}\label{visina8}
\end{figure}
```
--- 
make two column: 
```
\documentclass[twocolumn]{article}
...
\twocolumn

\onecolumn
```
---
clean latex:  
latexmk -C

---
--- 
multiline in table:  
1. using nested tabular
2. using p insteal of l, c, or r



latex-suite cheatsheet:  
https://michaelgoerz.net/refcards/vimlatexqrc.pdf

