## How to Use

#### Requirements
- Download [**MacTex**](https://www.tug.org/mactex/mactex-download.html)
- Ensure [**Titillium Web**](https://fonts.google.com/specimen/Titillium+Web?query=titi) is downloaded

#### Optional but recommended 
- Use **LaTeX Workshop** on VScode for easy editing and viewing

## Usage

In terminal, cd into desired whitepaper directory

```bash
cd /{directory}
```
Generate files with the following command. *If using the **LaTeX Workshop**, it will auto generate on file save*

```bash
xelatex {your-cv}.tex
```

this should result in the creation of ``{your-cv}.pdf``


## Using Covalent Template

Copy Template from `template.tex` in the root folder or the following code block

```tex
\documentclass{article}

% Set page size and margins
\usepackage[letterpaper,top=2cm,bottom=2cm,left=1.5cm,right=1.5cm,marginparwidth=1.75cm]{geometry}
\usepackage{setspace}
\setstretch{1.5}
% Set column length
\usepackage{multicol}
\setlength{\columnsep}{25pt}

% Useful packages
\usepackage{amsmath}
\usepackage{graphicx}
\usepackage[colorlinks=true, allcolors=blue]{hyperref}
\usepackage{titlesec}
\usepackage{xcolor}
\usepackage{fontspec}

\title{Covalent Network Whitepaper}
\author{Niall}
\definecolor{pink}{RGB}{255,76,139}  % Customize RGB values
\titleformat{\section}{\color{pink}\Large}{\thesection}{18pt}{}

\setmainfont{Titillium Web}

\begin{document}
\fontsize{12}{14}\selectfont
\maketitle

\begin{multicols}{2}

% Content goes here

\nocite{ref1,ref2,ref3}
\bibliographystyle{alpha}
\bibliography{sample}
\end{multicols} 
\end{document}
```

