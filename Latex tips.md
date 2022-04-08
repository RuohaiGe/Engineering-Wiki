## Two figure side by side
```TeX
\begin{figure}[H]
    \centering
    \begin{subfigure}[b]{0.45\textwidth} %adjust this for n pictures(0.9/n)
        \centering
        \includegraphics[width=\textwidth]{}
    \end{subfigure}
    \hfill
    \begin{subfigure}[b]{0.45\textwidth}
        \centering
        \includegraphics[width=\textwidth]{}
    \end{subfigure}
    \hfill
    \caption{Left side is and right side is}
\end{figure}
```
    
## One figure
```TeX
\begin{figure}[H]
    \centering
        \includegraphics[width=0.8\textwidth,height=0.4\textwidth,keepaspectratio]{}
        \caption{}
\end{figure}
```
    
## Matrix
```TeX
\[
    \begin{bmatrix}
      1 & 2 & 3\\
			4 & 5 & 6\\
			7 & 8 & 9\\
    \end{bmatrix}
\]
```

## Latex symbols
https://www.caam.rice.edu/~heinken/latex/symbols.pdf