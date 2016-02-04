# latex
Change section default font
```
\usepackage{sectsty}
\allsectionsfont{\usefont{OT1}{phv}{bc}{n}\selectfont}
```

Redefine font for entire document to san serif font
```
\renewcommand*{\sfdefault}{phv}
\renewcommand{\familydefault}{\sfdefault}
```
change ttdefault font 
```
\renewcommand*{\ttdefault}{pcr}
```
Or, define in premable
```
\usepackage{courier}
```
Simple and clean title page
```
\usepackage{titling}
\title{Another Title}
\author{John Dan}
\date{\today}

\begin{document}
{\raggedright \sffamily
    \LARGE \textbf{\thetitle} \\ [2mm]
    \normalsize \ \theauthor \\
    \normalsize \ \thedate \\
    \normalsize \ v-1.0 \\ % version
}
...snip...

```
Simple way to print code
```
\usepackage{xcolor}
\usepackage{listings}
\lstset{
	basicstyle=\footnotesize\ttfamily,
	breaklines=true,
	backgroundcolor=\color{gray!8},
	keepspaces=true,                                  
  	showspaces=false,                
  	showstringspaces=false,
  	showtabs=false,                  
  	tabsize=2
}

..snip..

\begin{lstlisting}
for x in customlist:
	print x
\end{lstlisting}

```

