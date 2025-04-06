# Phase Qubit
Quando $E_J \gg E_C$, il potenziale periodico domina e $\delta$ assume valori ben definiti nei minimi, mentre $N$ diventa continuo.
- **Fase localizzata**
- **Incertezza sulla carica**

In tali condizioni la fase della giunzione Josephson è considerata una **buona quantità per rappresentare il sistema**.

## Energia Cinetica

Sappiamo che la carica accumulata su un condensatore è data da $Q = C V$, e il potenziale ai capi della giunzione è $V = \dot{\Phi}$, dove $\Phi$ è il flusso magnetico.

L'energia immagazzinata in un condensatore è:

$$U_C = \frac{1}{2} C V^2 = \frac{1}{2} C \dot{\Phi}^2$$

Poiché nella formulazione lagrangiana l'energia cinetica è positiva, questo termine compare come:

$$T = \frac{1}{2} C \dot{\Phi}^2$$

---

## Energia Potenziale

La giunzione Josephson introduce un termine di energia potenziale legato alla corrente che attraversa la giunzione, data dalla relazione di Josephson:

$I_J = I_c \sin(\delta)$

dove $I_c$ è la corrente critica e $\delta$ è la differenza di fase della funzione d'onda superconduttiva tra i due lati della giunzione.

L'energia associata a questa corrente è ottenuta integrando rispetto al flusso:

$$U_J = \int V I_J dt = \int \dot{\Phi} I_c \sin(\delta) dt$$

Poiché il flusso e la fase sono legati dalla relazione:

$$\delta = \frac{2e}{\hbar} \Phi$$

possiamo esprimere l'energia potenziale in termini di $\Phi$:

$$U_J = -E_J \cos\left(\frac{2e}{\hbar} \Phi\right)$$

dove $E_J = \frac{\hbar I_c}{2e}$ è l'energia di Josephson.

---

## Scrittura della Lagrangiana

Ora che abbiamo identificato l'energia cinetica e l'energia potenziale, possiamo scrivere la lagrangiana come:

$$\mathcal{L}_0 = T - U = \frac{1}{2} C \dot{\Phi}^2 + E_J \cos\left(\frac{2e}{\hbar} \Phi\right)$$

Questo descrive il comportamento di una giunzione Josephson senza alcuna corrente di bias applicata.

## Aggiunta di un generatore di corrente di bias $I_B$

![[Pasted image 20241119180323.png|200]]

**A cosa serve?** 
Per poter osservare il tunneling di fase attraverso la configurazione di **Tilted washboard potential**
![[Washboard-potential-with-zero-bias-upper-and-non-zero-bias-lower.jpg|300]]

![[Pasted image 20241119180410.png|300]]

Quando si introduce un generatore di corrente $I_B(t)$ in serie con la giunzione, bisogna considerare che la corrente che attraversa la giunzione è la somma della corrente dovuta all'effetto Josephson e della corrente esterna $I_B(t)$. La corrente totale in una giunzione Josephson è quindi data da:

$$
I(t) = I_{J}(t) + I_B(t)=I_c \sin(\delta) + I_B(t)
$$

### **Potenza della corrente $\mathcal{P}_I$**
La potenza fornita dal generatore di corrente è:

$$
\mathcal{P}_I = V I_B
$$

Il potenziale $V$ è legato al flusso magnetico $\Phi$ tramite:

$$
V = \dot{\Phi}.
$$

### **Energia potenziale associata al generatore**
L'energia potenziale associata alla corrente $I_B$ può essere ricavata attraverso il lavoro applicato dal generatore:

$$
W_I=-\Delta U_{\text{gen}}=U_i-U_f=-U_f\equiv-U_I=\int\mathcal{P}_Idt=\int I_B \, d\Phi = I_B \Phi,
$$

### **Termine di interazione $\mathcal{L}_I$**

$$
\mathcal{L}_I =K_I - U_I = -U_I=I_B \Phi.
$$

### **Lagrangiana totale**

$$
\mathcal{L} = \mathcal{L}_0 + \mathcal{L}_I,
$$

ovvero:

$$
\mathcal{L} = \frac{1}{2} C \dot{\Phi}^2 + E_J \cos\left(\frac{2e}{\hbar} \Phi\right) + I_B \Phi.
$$

### **Riscrittura in funzione di $\delta$ ed $N$**
Descrivere il sistema in termini di fase $\delta$ e numero di coppie di Cooper $N$ è più naturale rispetto a flusso e carica perché queste variabili formano una coppia canonica ben definita, con una relazione di commutazione semplice. Inoltre, nel regime $E_C \ll E_J$, la fase $\delta$ è un buon parametro dinamico per descrivere il comportamento della giunzione, mentre $N$ rappresenta direttamente il numero di coppie trasferite.

$$\delta=2\pi\frac{\Phi}{\Phi_0}=\frac{2e}{\hbar}\Phi$$

$$N=\frac{Q}{2e}=\frac{C}{2e}\dot{\Phi}=\frac{\hbar C}{(2e)^2}\dot{\delta}$$

$$\begin{align}
	\mathcal{L}(\delta,N)&=4\frac{e^2}{2C}N^2+E_J\cos(\delta)+\frac{\hbar I_B}{2e}\delta=\\\\
	&=4E_CN^2+E_J\cos(\delta)+\frac{\hbar I_B}{2e}\delta
\end{align}$$

**NB:**
$$
\begin{align}
&\begin{cases} 
	\Phi & \text{Coordinata} \\ 
	Q=\frac{\partial\mathcal{L}}{\partial\dot{\Phi}} & \text{Momento coniugato} \\
	[\Phi,Q]=i\hbar &\text{Relazione di commutazione}
\end{cases}\\\\
&\text{quindi:} \\\\
&\begin{cases} 
	\delta & \text{Coordinata} \\ 
	N=\frac{1}{\hbar}\frac{\partial\mathcal{L}}{\partial\dot{\delta}} & \text{Momento coniugato} \\
	 [\delta,N]=i &\text{Relazione di commutazione}
\end{cases}
\end{align}
$$

### **Hamiltoniana**

$$\begin{align}
	\mathcal{H}&=Q\dot{\Phi}-\mathcal{L}=\hbar N\dot\delta-\mathcal{L}=2 \cdot(4E_CN^2)-\mathcal{L}=K_J+U_J+U_I=\\\\
	&=4E_CN^2-E_J\cos(\delta)-\frac{\hbar I_B}{2e}\cdot\delta
\end{align}$$

## Approssimazione del potenziale armonico a **potenziale cubico (anarmonico)**

$$U(\delta)=-E_J\cos(\delta)-\frac{\hbar I_B}{2e}\cdot\delta=-E_J\cdot\left[\cos(\delta)+\frac{I_B}{I_0}\cdot\delta\right]$$

Intorno al minimo:

$$U(\delta)=U(\delta_{\text{min}})+U'(\delta)\lvert_{\delta_{\text{min}}}\cdot\,(\delta-\delta_{\text{min}})+\frac{1}{2}\cdot U''(\delta)\lvert_{\delta_{\text{min}}}\cdot\,(\delta-\delta_{\text{min}})^2+\cdots$$

$$U'(\delta)=-\sin(\delta)+\frac{I_B}{I_0}$$

Sui punti critici la derivata prima del potenziale è nulla:

$$\sin(\delta_c)=\frac{I_B}{I_0}$$

la quale ammette due soluzioni distinte, ossia $\delta_c$ e $\pi-\delta_c$:

$$\begin{cases} 
	\delta_{\text{min}}&=\arcsin\left(\frac{I_B}{I_0}\right)\\
	\delta_{\text{max}}&=\pi-\arcsin\left(\frac{I_B}{I_0}\right)
\end{cases}$$

**NB:** Sperimentalmente si sceglie $I_B\sim 0.95\cdot I_0$, in modo da avere il rapporto tra le due quantità di circa $1$. Tale scelta permette una maggior stabilità del sistema trovandosi vicino allo stato stazionario e permette inoltre di approssimare il potenziale in una forma più semplice:

Considerando $\frac{I_B}{I_0}\rightarrow 1$, riscriviamo il rapporto come $\frac{I_B}{I_0}=1-\varepsilon$ in cui $\varepsilon\rightarrow 0$.
In questo modo possiamo approssimare l'arcoseno ad una forma più semplice:

$$\arcsin(1-\varepsilon)\sim\frac{\pi}{2}-\sqrt{2\varepsilon}$$

**Dimostrazione:**
Poniamo $\varepsilon=t^2$:

$$g(t)=\arcsin(1-t^2)$$

$$g'(t)=-\frac{2}{\sqrt{2-t^2}}$$

Sapendo che $t\rightarrow0$:

$$\begin{align}
	g(t)&=g(0)+g'(t)\lvert_0\cdot t+\cdots\\\\
	&\sim\frac{\pi}{2}-\sqrt{2}\cdot t=\frac{\pi}{2}-\sqrt{2\varepsilon}
	\end{align}$$

Possiamo dunque riscrivere le fasi:

$$\begin{cases} 
	\delta_{\text{min}}&\sim\dfrac{\pi}{2}-\sqrt{2\varepsilon}\\\\
	\delta_{\text{max}}&\sim\dfrac{\pi}{2}+\sqrt{2\varepsilon}
\end{cases}$$

A questo punto la differenza di potenziale può essere facilmente approssimata nel seguente modo:

$$\begin{align}
	\Delta U(I_B)=&\,U(\delta_{\text{max}})-U(\delta_{\text{min}})=\\
	\lvert&\\
	\sim&-E_J\left[\cos\left(\frac{\pi}{2}+\sqrt{2\varepsilon}\right)+(1-\varepsilon)\cdot\left(\frac{\pi}{2}+\sqrt{2\varepsilon}\right)+\right.\\\\
	&\left.-\cos\left(\frac{\pi}{2}-\sqrt{2\varepsilon}\right)-(1-\varepsilon)\cdot\left(\frac{\pi}{2}-\sqrt{2\varepsilon}\right)\right]=\\
	\lvert&\\
\sim\,&E_J\left[2\sin(\sqrt{2\varepsilon})-2(1-\varepsilon)\sqrt{2\varepsilon}\right]=\\
	\end{align}$$

Sviluppando il seno fino al secondo ordine si ottiene:

$$\begin{align}
&2E_J\left[\sqrt{2\varepsilon}-\frac{1}{6}(2\varepsilon)^{3/2}-\sqrt{2\varepsilon}+\sqrt{2}\cdot\varepsilon^{3/2}\right]=\\\\
=&\,2\sqrt{2}\cdot E_J\cdot\varepsilon^{3/2}\cdot\left(1-\frac{1}{3}\right)=\\\\
\Delta U(I_B)\sim&\,\frac{2^{5/2}}{3}\cdot E_J\cdot\left(1-\frac{I_B}{I_0}\right)^{3/2}=2\sqrt{2}\cdot \frac{I_0\cdot\Phi_0}{3\pi}\cdot\left(1-\frac{I_B}{I_0}\right)^{3/2}
\end{align}$$

**NB:** La differenza di potenziale appena ricavata rappresenta l'altezza della barriera e dipende dalla corrente di bias (fornita dal generatore di corrente). **Più $I_B$ tende a $I_0$ e più la barriera si abbassa**.

## Frequenza di plasma per $I_B\rightarrow I_0$:
$$L(\delta)=\frac{\Phi_0}{2\pi I_0\cos(\delta)}=\frac{L_0}{\cos(\delta)}$$
	$$\omega_p(\delta)=\frac{1}{\sqrt{LC}}=\frac{1}{L_0C}\cdot\sqrt{\cos(\delta)}=\omega_0\cdot\left[1-\sin^2(\delta)\right]^{1/4}$$
	Sapendo che per $\delta\rightarrow\delta_{\text{min}}$, il seno tende a $I_B/I_0$, possiamo fare delle approssimazioni:
	$$\omega_p(I_B)\sim\omega_0\cdot\left[1-\left(\frac{I_B}{I_0}\right)^2\right]^{1/4}$$
	
Sapendo inoltre che $I_B\sim0.95\cdot I_0$, allora $\frac{I_B}{I_0}=(1-\varepsilon)\rightarrow 1$, con $\varepsilon\rightarrow 0$:
	
	$$\begin{align}
	\omega_p(I_B)&\sim\omega_0\cdot\left[1-(1-2\varepsilon)\right]^{1/4}=\omega_0\cdot(2\varepsilon)^{1/4}\\\\
	\omega_p(I_B)&\sim2^{1/4}\cdot\omega_0\cdot\left(1-\frac{I_B}{I_0}\right)^{1/4}
	\end{align}$$ 
**NB:** 
	- $\omega_p<\omega_0$;
	- Inoltre, siccome $L$ e $C$ sono rispettivamente inversamente e direttamente proporzionali all'area della giunzione, le frequenze $\omega_0$ e $\omega_p$ **non** dipendono dalla sua geometria.
	
## Seconda quantizzazione
Operatori di innalzamento e abbassamento (creazione e distruzione):

$$\hat{a}^\dagger=\frac{\left(\Phi-izQ\right)}{\sqrt{2\hbar z}};\hspace{2cm}\hat{a}=\frac{\left(\Phi+izQ\right)}{\sqrt{2\hbar z}}$$

con $z=\sqrt{L/C}$ 

$$\Phi=\sqrt{\frac{\hbar z}{2}}\cdot\left(\hat{a}^\dagger+\hat{a}\right);\hspace{2cm}Q=i\sqrt{\frac{\hbar}{2z}}\cdot\left(\hat{a}^\dagger-\hat{a}\right)$$

Passando allo spazio di $\{\delta, N\}$, otteniamo:

$$\delta=e\cdot\sqrt{\frac{2z}{\hbar}}\cdot\left(\hat{a}^\dagger+\hat{a}\right);\hspace{2cm}N=\frac{i}{2e}\cdot\sqrt{\frac{\hbar}{2z}}\cdot\left(\hat{a}^\dagger-\hat{a}\right)$$

Per semplificare la scrittura, d'ora in avanti ometteremo il simbolo del cappuccio sugli operatori e scriveremo $\sqrt{\hbar/2z}=\Lambda$.

**Hamiltoniana del sistema:**

$$\mathcal{H}(\delta,N)=4E_CN^2-E_J\cos(\delta)-\frac{\hbar I_B}{2e}\cdot\delta$$

Prendiamo un sottospazio del sistema in cui consideriamo solo i primi due livelli energetici:

$$\mathcal{B}=\{\ket{0},\ket{1}\}$$

Tenendo presente che i primi due livelli energetici sono vicini al minimo della buca di potenziale, possiamo sviluppare in serie di Taylor il coseno dell'Hamiltoniana:

$$\cos(\delta)\sim1-\frac{\delta^2}{2}+\cdots$$

$$\mathcal{H}(\delta,N)\sim4E_CN^2-E_J+\frac{1}{2}E_J\delta^2-\frac{\hbar I_B}{2e}\cdot\delta$$

Trascuriamo il termine costante $-E_J$, in quanto contribuisce solamente allo shift dei livelli energetici e non influisce sulla differenza tra di essi per quanto riguarda le transizioni energetiche.

$$\mathcal{H}(\delta,N)\sim4E_CN^2+\frac{1}{2}E_J\delta^2-\frac{\hbar I_B}{2e}\cdot\delta$$

Esplicitiamo ora gli operatori di innalzamento e abbassamento a partire dalle variabili canoniche $\delta$ ed $N$:

$$\begin{align}
\mathcal{H}_C&=4E_C\cdot\left(-\frac{\Lambda^2}{4e^2}\right)\cdot\left(a^{\dagger2}-a^2\right)^2=\\
&=\frac{E_C\Lambda^2}{e^2}\cdot\left(2a^\dagger a+1-a^{\dagger2}-a^2\right)
\end{align}$$

$$\begin{align}
\mathcal{H}_J&=\frac{1}{2}E_J\cdot\left(\frac{e}{\Lambda}\right)^2\cdot\left(a^{\dagger2}+a^2\right)^2=\\
&=\frac{E_Je^2}{2\Lambda^2}\cdot\left(2a^\dagger a+1+a^{\dagger2}+a^2\right)
\end{align}$$

$$\begin{align}
\mathcal{H}_{I_B}&=-\frac{\hbar I_B}{2\Lambda}\cdot\left(a^\dagger+a\right)
\end{align}$$

Ricordando le seguenti relazioni:

$$\omega_0=\frac{1}{\sqrt{L_0C}}=\frac{\sqrt{8E_CE_J}}{\hbar};$$

$$E_C=\frac{e^2}{2C};$$

$$E_J=E_L=\frac{1}{L_0}\left(\frac{\hbar}{2e}\right)^2=\frac{\hbar I_0}{2e}$$

Possiamo riscrivere le costanti dei primi termini dell'Hamiltoniana come:

$$\begin{align}
\frac{E_C\Lambda^2}{e^2}&=\frac{\hbar\omega_0}{4}\\
\frac{E_Je^2}{2\Lambda^2}&=\frac{\hbar\omega_0}{4}\\
\frac{\hbar I_B}{2\Lambda}&=I_B\cdot\sqrt{\frac{\hbar\omega_0L_0}{2}}=I_B\cdot\sqrt{\frac{\hbar}{2\omega_0C}}
\end{align}$$

Ottenendo infine sia il termine armonico che quello **anarmonico**:

$$\mathcal{H}\sim\hbar\omega_0\cdot\left(a^\dagger a+\frac{1}{2}\right)-I_B\cdot\sqrt{\frac{\hbar}{2\omega_0C}}\cdot\left(a^\dagger+a\right)$$

---
Quando limitiamo il nostro interesse ai primi due livelli, $\ket{0}$ e $\ket{1}$, si crea una **proiezione** da uno spazio di Hilbert di dimensione infinita a uno spazio a due dimensioni, in cui gli unici stati ammissibili sono i due stati fondamentali $\ket{0}$ e $\ket{1}$.

Gli operatori di innalzamento e abbassamento $a^\dagger$ e $a$ possono essere espressi tramite le matrici di Pauli e i loro operatori associati.

In un sistema di tipo qubit (due livelli), gli operatori $a^\dagger$ e $a$ sono associati a combinazioni lineari di $\sigma_x$ e $\sigma_y$. In particolare, possiamo scrivere le seguenti relazioni per $a$ e $a^\dagger$:

$$a^\dagger = \frac{1}{2}(\sigma_x + i \sigma_y), \hspace{2cm}a = \frac{1}{2}(\sigma_x - i \sigma_y)$$

Le matrici $\sigma_x$ e $\sigma_y$ sono le matrici di Pauli che agiscono come operatori di innalzamento e abbassamento nei sistemi a due livelli:

$\sigma_x = \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix}$;  $\sigma_y = \begin{pmatrix} 0 & -i \\ i & 0 \end{pmatrix}$;  $\sigma_z = \begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix}$;

$a^\dagger = \begin{pmatrix} 0 & 0 \\ 1 & 0 \end{pmatrix}$;  $a^\dagger = \begin{pmatrix} 0 & 1 \\ 0 & 0 \end{pmatrix}$;  $a^\dagger a = \begin{pmatrix} 0 & 0 \\ 0 & 1 \end{pmatrix}$; 

Per semplificare l'hamiltoniana, traslo l'energia di una quantità $\hbar \omega_0$, in modo da centrare il sistema attorno al livello di energia zero. Questo spostamento permette di scrivere l'hamiltoniana in una forma più semplice, che coinvolge direttamente le matrici di Pauli, facilitando così l'analisi del sistema:

$$\mathcal{H}\rightarrow\mathcal{H}-\hbar\omega_0$$

In questo modo la nuova Hamiltoniana si potrà scrivere nel seguente modo:

$$\mathcal{H}\sim\hbar\omega_0\cdot\left(a^\dagger a-\frac{1}{2}\mathbb{I}\right)-I_B\cdot\sqrt{\frac{\hbar}{2\omega_0C}}\cdot\left(a^\dagger+a\right)$$

A questo punto possiamo osservare che:

$$a^\dagger a-\frac{1}{2}\mathbb{I}=-\frac{\sigma_z}{2}$$

$$a^\dagger+a=\sigma_x$$

ottenendo quindi:

$$\mathcal{H}\sim-\frac{\hbar\omega_0}{2}\cdot\sigma_z-I_B\cdot\sqrt{\frac{\hbar}{2\omega_0C}}\cdot\sigma_x$$

Per poter esplicitare le energie, è necessario diagonalizzare l'hamiltoniana:

$$\mathcal{H}=a\cdot\sigma_z+b\cdot\sigma_x=\begin{pmatrix} a & b \\ b & -a \end{pmatrix}$$

dove

$$a=-\frac{\hbar\omega_0}{2};$$

$$b=-I_B\cdot\sqrt{\frac{\hbar}{2\omega_0C}}$$

$$\det(\mathcal{H}−\lambda\mathbb{I})=0$$

$$\begin{align}
	-(a-\lambda)(a+\lambda)-b^2=0\\
	-b^2-a^2+\lambda^2=0\\
	\lambda_{1,0}=\pm\sqrt{a^2+b^2}=E_{1,0}
\end{align}$$

$$\mathcal{H}_{\text{diag}}=\begin{pmatrix} \lambda_0 & 0 \\ 0 & \lambda_1 \end{pmatrix}=-\sqrt{a^2+b^2}\cdot\sigma_z$$

Definiamo ora la transizione energetica tra i due stati:

$$\hbar\omega_{01}=E_1-E_0=2\sqrt{a^2+b^2}$$

L'hamiltoniana può essere riscritta nel seguente modo:

$$\mathcal{H}_0\equiv\mathcal{H}_{\text{diag}}=-\frac{\hbar\omega_{01}}{2}\sigma_z$$

**NB:**
Questa Hamiltoniana:
-  Descrive le **oscillazioni quantistiche** tra i due livelli $\ket{0}$ e $\ket{1}$ di un qubit superconduttore.
- Descrive la possibilità di **manipolare il qubit** controllando la corrente $I_B$​, che modifica la frequenza di oscillazione $\omega_{01}$.
- Descrive la **riduzione a un sistema a due livelli** valida in regime **fortemente anarmonico**, ossia vicino alla corrente critica $I_0$.
Inoltre descrive un sistema **isolato** a due livelli, in cui:
1. Non ci sono **interazioni** con campi esterni o altri sistemi.
2. Non ci sono termini di **eccitazione** o **diseccitazione** (nessun $\sigma_x$​ o $\sigma_y$​).
3. Le energie dei livelli $\ket{0}$ e $\ket{1}$ sono semplicemente definite dalla frequenza $\omega_{10}$.
Si tratta quindi di un **sistema statico** che evolve solo in base alla sua energia interna.

## Termine di interazione
Aggiungendo (in serie) una corrente variabile nel tempo, possiamo controllare il qubit a piacimento. Tale aggiunta determinerà un termine di interazione $\mathcal{H}_{\text{int}}$, il quale provoca l'inizio della rotazione dello stato nella sfera di Bloch.

$$\mathcal{H}(t)=\mathcal{H}_0+\mathcal{H}_{\text{int}}(t)$$

La corrente possiamo riscriverla nel seguente modo:

$$I_B=I_{B_0}+\Delta I(t)$$

dove $I_{B_0}$ rappresenta il termine di corrente costante contenuto nell'Hamiltoniana senza interazioni e $\Delta I(t)$ rappresenta il termine variabile e dipendente dal tempo contenuto nell'Hamiltoniana di interazione.

**NB:**
I livelli energetici dei rispettivi stati $\ket{0}$ e $\ket{1}$, sono determinati dal termine di corrente costante $I_{B_0}$.  

$$\begin{align}
\mathcal{H}(t)&\sim-\frac{\hbar\omega_0}{2}\cdot\sigma_z-I_B(t)\cdot\sqrt{\frac{\hbar}{2\omega_0C}}\cdot\sigma_x=\\
&\sim-\frac{\hbar\omega_0}{2}\cdot\sigma_z-I_{B}(t)\cdot\Phi=\\
&\sim\left(-\frac{\hbar\omega_0}{2}\cdot\sigma_z-I_{B_0}\cdot\Phi\right)-\Delta I(t)\cdot\Phi=\\
&\sim-\frac{\hbar\omega_{01}}{2}\sigma_z-\Delta I(t)\cdot\Phi
\end{align}$$

con $\mathcal{H}_{\text{int}}(t)=-\Delta I(t)\cdot\Phi=-\Delta I(t)\cdot\dfrac{\Phi_0}{2\pi}\cdot\delta$ 
Tale termine di interazione non risulta diagonale e per poterlo trattare in maniera più semplice si sfrutta la **Rotating Wave Approximation (RWA)** ottenendo così:

$$\begin{align}
\mathcal{H}_{\text{RWA}}\approx -\dfrac{\hbar}{2}\left(\omega_{01}-\omega_d\right)\cdot\hat{\sigma}_z -\sqrt{\dfrac{\hbar}{2\omega_0C}}\cdot\left\{\frac{I_{RFC}}{2}\hat{\sigma}_x+\frac{I_{RFS}}{2}\hat{\sigma}_y\right\}+ \frac{I_{LF}(t)}{2} \frac{\partial E_{10}}{\partial I_{B_0}}\cdot\hat{\sigma}_z\end{align}$$

con $\Delta I(t)$ riscritta come combinazione lineare dei contributi a bassa e ad alta frequenza per rappresentare i diversi effetti che un segnale esterno può avere sul qubit (con frequenza alta corrispondente alla frequenza di drive):

$$
\begin{align}
\Delta I(t) &= I_{LF}(t) + I_{RF}(t)\cos(\omega_dt+\phi)=\\\\ 
&= I_{LF}(t)+I_{RFC}(t,\phi)\cos(\omega_d t) + I_{RFS}(t,\phi)\sin(\omega_d t)
\end{align}
$$