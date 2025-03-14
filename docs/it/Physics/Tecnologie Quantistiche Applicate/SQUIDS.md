---
tags:
  - flux
  - squid
  - josephsonjunction
  - qubit
Topic: Quantum Technologies
DC SQUID: false
RF-SQUID: false
---
# **SQUIDS**
## **RF-SQUID**

### **RF SQUID immerso in un campo magnetico esterno**

Un RF SQUID (Superconducting Quantum Interference Device a radiofrequenza) è un anello superconduttivo contenente una singola giunzione Josephson. Quando viene immerso in un campo magnetico esterno, il flusso magnetico totale nel loop non è semplicemente uguale al flusso esterno, ma è influenzato anche dalla presenza della giunzione. Il comportamento del sistema è descritto dalle seguenti equazioni:

$$\begin{cases} \Phi_{\text{int}} = \Phi_{\text{ext}} + \Phi_J = \Phi_{\text{ext}} - L I_J \\ I_J = I_c \sin(\delta) = I_c \sin\left(2\pi\dfrac{\Phi_{\text{int}}}{\Phi_0}\right) \end{cases}$$

Dove:

- $\Phi_{\text{int}}$ è il flusso totale all'interno del loop,
- $\Phi_{\text{ext}}$ è il flusso magnetico esterno applicato,
- $\Phi_J = -L I_J$ è il contributo della corrente della giunzione al flusso totale,
- $I_J$ è la corrente attraverso la giunzione Josephson,
- $I_c$ è la corrente critica della giunzione,
- $\delta$ è la differenza di fase della giunzione,
- $\Phi_0$ è il quanto di flusso magnetico ($h/2e$).

Sostituendo l'espressione per la corrente della giunzione, otteniamo:

$$\Phi_{\text{int}} = \Phi_{\text{ext}} - L I_c \sin\left(2\pi\dfrac{\Phi_{\text{int}}}{\Phi_0}\right)$$

Questa relazione presenta due comportamenti che possono essere analizzati attraverso la sua derivata rispetto al flusso esterno:

$$\frac{\partial\Phi_{\text{int}}}{\partial\Phi_{\text{ext}}} = 1 - L I_c \cos\left(2\pi\dfrac{\Phi_{\text{int}}}{\Phi_0}\right)\cdot\frac{2\pi}{\Phi_0}\frac{\partial\Phi_{\text{int}}}{\partial\Phi_{\text{ext}}}$$

$$\begin{align}
\frac{\partial\Phi_{\text{int}}}{\partial\Phi_{\text{ext}}} &= \left[1+\frac{2\pi L I_c}{\Phi_0} \cos\left(2\pi\dfrac{\Phi_{\text{int}}}{\Phi_0}\right)\right]^{-1}\\\\
&=\left[1+\beta'_L \cos\left(2\pi\dfrac{\Phi_{\text{int}}}{\Phi_0}\right)\right]^{-1}
\end{align}$$

con $\beta_L'=\dfrac{2\pi LI_c}{\Phi_0}$ parametro cruciale per determinare il comportamento del sistema, poiché influenza la non linearità della risposta del flusso totale al flusso esterno applicato.

![[assets/imgs/RF-SQUID_FLUX.png]]

#### **Comportamento del sistema in funzione di $\beta_L'$**

1. **Regime non isteretico o debole ($\beta_L' < 1$)**
    
    Quando $\beta_L' < 1$, il termine non lineare $\sin\left(2\pi \frac{\Phi_{\text{int}}}{\Phi_0}\right)$ ha un effetto trascurabile. In questo regime, la relazione tra il flusso totale e il flusso esterno è **quasi lineare**, e il comportamento del sistema è monotono e prevedibile. Pertanto, il flusso totale segue in modo diretto e continuo il flusso esterno, con poca o nessuna isteresi.
    
	**NB:** La derivata del flusso totale rispetto al flusso esterno è sempre positiva.


2. **Regime isteretico o forte ($\beta_L' > 1$)**
    
    Quando $\beta_L' > 1$, il termine $\frac{L I_c}{\Phi_0}$ diventa significativo, e il termine non lineare $\sin\left(2\pi \frac{\Phi_{\text{int}}}{\Phi_0}\right)$ inizia a influenzare fortemente la risposta del sistema. In questo regime, la derivata del flusso totale rispetto al flusso esterno, $\frac{d\Phi_{\text{int}}}{d\Phi_{\text{ext}}}$, può assumere valori negativi o divergere, dando luogo alla comparsa di **isteresi**. In altre parole, il flusso interno non segue più linearmente il flusso esterno, ma può avere più stati stabili per un dato valore del flusso esterno. Questo rende il dispositivo estremamente sensibile a piccole variazioni del campo magnetico, mostrando una **risposta non lineare complessa**.

## **DC-SQUID**