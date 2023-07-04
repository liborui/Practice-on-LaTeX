# Practice-on-LaTeX

```latex
\begin{figure}[t]
\centering
\begin{minipage}[c]{.48\linewidth}
    \centering
	\includegraphics[width=\textwidth]{fig/eval-tc-network-small.pdf}
	\vspace{-2em}
	\caption{Provisioning time of new experiments when another experiment is running on the edge device with and without \texttt{resGuard}.}
	\label{fig:eval-tc-network}
\end{minipage}%
\hfill
\begin{minipage}[c]{.48\linewidth}
    \centering
	\includegraphics[width=\textwidth]{fig/eval-multi-tenancy-small.pdf}
	\vspace{-2em}
	\caption{Average programming latency different concurrent request for tenant G1 (80 devices maximum) and G2 (20 devices maximum).}
	\label{fig:eval-multi-tenancy}
\end{minipage}
\vspace{-1.5em}
\end{figure}
```

