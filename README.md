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
{\raggedright
	\LARGE \textbf{The Page Documentation}  \\
	\normalsize  by John Due \\
	\today \\
}
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
```

