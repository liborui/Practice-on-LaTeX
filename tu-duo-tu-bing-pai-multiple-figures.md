# 图|多图并排 Multiple figures

如果你想要并排多张图片，并且每个图片独立编号的话，可以使用

```latex
\begin{figure*}[t]
	\centering
	\begin{minipage}[c]{.29\linewidth}
		\centering
		\includegraphics[width=\linewidth]{fig/application-eeg}
		\vspace{-2em}
		\caption{Application EEG}
		\label{fig:application-eeg}
	\end{minipage}%
	\hfill
	\begin{minipage}[c]{.29\linewidth}
	\centering
	\includegraphics[width=\linewidth]{fig/application-eeg}
	\vspace{-2em}
	\caption{Application EEG}
	\label{fig:application-eeg}
\end{minipage}%
\hfill
	\begin{minipage}[c]{.4\linewidth}
	\centering
	\includegraphics[width=\linewidth]{fig/memory-footprint}
	\vspace{-2em}
	\caption{Memory footprint comparison with baselines. The red line indicates the RAM upper bound.}
	\label{fig:memory-footprint}
\end{minipage}
	\vspace{-1.5em}
\end{figure*}
```

如果你想要并排多张图片，并且每个图片独立使用（a）（b）之类的编号的话

```latex
\begin{figure*}[t]
	% 	\vspace{-1em}
	\centering
	\subfigure[TelosB]{
		\includegraphics[width=5.5em,height=4em]{fig/iot-node-telosb.png}
		\label{fig:iot-node-telosb}
	}
	\subfigure[Arduino Mega]{
		\includegraphics[width=5.5em,height=4em]{fig/iot-node-mega.png}
		\label{fig:iot-node-mega}
	}
	\subfigure[Arduino Uno]{
		\includegraphics[width=5.5em,height=4em]{fig/iot-node-uno.png}
		\label{fig:iot-node-uno}
	}
	\subfigure[ESP32]{
		\includegraphics[width=5.5em,height=4em]{fig/iot-node-esp32.png}
		\label{fig:iot-node-esp32}
	}
	\subfigure[nRF52840]{
		\includegraphics[width=5.5em,height=4em]{fig/iot-node-nrf52840.png}
		\label{fig:iot-node-nrf52840}
	}
	\subfigure[STM32 F103]{
		\includegraphics[width=5.5em,height=4em]{fig/iot-node-stm32.png}
		\label{fig:iot-node-stm32}
	}
	\subfigure[AOS DevKit]{
		\includegraphics[width=5.5em,height=4em]{fig/iot-node-developerkit.png}
		\label{fig:iot-node-developerkit}
	}
	\subfigure[HaaS100]{
		\includegraphics[width=5.5em,height=4em]{fig/iot-node-haas100.jpeg}
		\label{fig:iot-node-haas100}
	}
	\vspace{-1em}
	\caption{\nsdidiff{IoT devices deployment in LinkLab~2.0.}}
	\vspace{-1.5em}
	\label{fig:iot-node}
\end{figure*}
```
