# LatexMacros

The general pattern is to define things in terms of commands. For example:


\newcommand{\paren}[1]{\left ( #1 \right )}
\newcommand{\bracket}[1]{{\left [ #1 \right ]}}
\newcommand{\sparen}[1]{ (#1)}
\newcommand{\sbracket}[1]{{ [ #1  ] }}


So if I want to change the sizing or style of parenthesis or brackets I can do so very quickly because the curly brackets are already in place, and I am just changing the name of the command that takes the argument. Likewise, if we define:

\newcommand{\myequation}[1]{\begin{eqnarray} #1 \end{eqnarray}}
\newcommand{\myequationn}[1]{\begin{align*} #1 \end{align*}}
\newcommand{\myequationnn}[1]{\ensuremath{#1}}

which allows you to switch around environments quickly with a minimum of keystrokes and jumping from start to end. Most macros here fall into this sort of pattern. 
