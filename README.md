# LatexMacros

The general pattern is to define things in terms of commands. For example, we can make many commands for parentheses:


\newcommand{\paren}[1]{\left ( #1 \right )}

\newcommand{\bracket}[1]{{\left [ #1 \right ]}}

\newcommand{\sparen}[1]{ (#1)}

\newcommand{\sbracket}[1]{{ [ #1  ] }}


With these commands, if I want to change the sizing or style of parenthesis or brackets I can do so very quickly by just changing the command. Because the curly brackets are already in place, I am just changing the name of the command that takes the argument. 

Likewise, defining:

\newcommand{\myequation}[1]{\begin{eqnarray} #1 \end{eqnarray}}

\newcommand{\myequationn}[1]{\begin{align*} #1 \end{align*}}

\newcommand{\myequationnn}[1]{\ensuremath{#1}}

Allows swiching between labeld, unlabeled, and inline equations with a minimum of keystrokes and jumping from start to end. Most macros here fall into this sort of pattern. 
