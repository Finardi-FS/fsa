
| Paragrafo | Argomento                                                                                   | Stato | Comprensione |
| --------- | ------------------------------------------------------------------------------------------- | :---: | :----------: |
| **P.1**   | Circuiti a giunzione superconduttiva: dalla quantizzazione macroscopica ai qubit            |   ✅   |     4/4      |
| **P.2**   | Circuiti superconduttivi: effetti di carica e flusso nella coerenza quantistica             |   ✅   |     4/4      |
| **P.3**   | Un nuovo qubit con giunzione Josephson su scala micrometrica                                |   ❓   |              |
| **P.4**   | Proprietà Quantistiche della Giunzione Josephson con Corrente di Bias                       |  ✅❓   |              |
| **P.5**   | Corrente ed Hamiltoniana                                                                    |  🤔❗  |     1/3      |
| **P.6**   | Misura dello stato del qubit tramite tunneling                                              |  🤔   |     5/6      |
| **P.7**   | Implementazione di un bias di corrente ad alta impedenza                                    |  🤔❗  |     2/10     |
| **P.8**   | Fabbricazione e filtraggio del circuito qubit                                               | 🤔ℹ️  |     5/6      |
| **P.9**   | Determinazione del bias ottimale e quantizzazione del flusso nel circuito                   | 🤔🤔  |     3/7      |
| **P.10**  | Spettroscopia del qubit: determinazione dei livelli energetici e del fattore di qualità $Q$ |   ✅   |     6/6      |
| **P.11**  | Preparazione e misura dello stato del qubit                                                 |  🤔   |     1/3      |
| **P.12**  | Fedeltà della misura dello stato                                                            | 🤔🤔  |     5/9      |
| **P.13**  | Tasso di rilassamento dello stato $\ket{1}$                                                 |  🤔   |     2/3      |
| **P.14**  | Manipolazione coerente dello stato del qubit                                                | 🤔🤔  |     2/6      |
| **P.15**  | Origine della decoerenza e possibili miglioramenti                                          | 🤔🤔  |     2/6      |
| **P.16**  | Conclusioni                                                                                 |  🤔   |     3/4      |

# P.1 - Circuiti a giunzione superconduttiva: dalla quantizzazione macroscopica ai qubit
**PARAGRAFO:**
--
The question of the applicability of the laws of quantum mechanics to macroscopic degrees of freedom triggered some 20 years ago the development of superconducting junction circuits displaying quantum behavior at the level of their macroscopic electrical variables. Energy level quantization, macroscopic quantum tunneling, and quantum superposition of states have indeed been observed in these “atomlike” circuits. More recently, the idea that quantum mechanics could be used to manipulate information efficiently has boosted interest from a different perspective for such solid-state devices: the two lowest energy states of these circuits could be used as a quantum bit (qubit) and scaled to a full quantum computer through integrated-circuit technology. However, as solid-state qubits are by necessity coupled to many electromagnetic degrees of freedom through bias and measurement wires, long coherence times requires careful circuit design.

**TRADUZIONE E ANALISI:**
--
✅La questione dell'applicabilità delle leggi della meccanica quantistica ai gradi di libertà macroscopici ha stimolato, circa 20 anni fa, lo sviluppo di circuiti a giunzione superconduttiva che mostrano un comportamento quantistico a livello delle loro variabili elettriche macroscopiche. 

✅In questi circuiti “simili ad atomi” sono stati infatti **osservati la quantizzazione dei livelli energetici, il tunneling quantistico macroscopico e la sovrapposizione quantistica degli stati**. 

✅Più recentemente, l'idea che la meccanica quantistica possa essere utilizzata per manipolare l'informazione in modo efficiente ha incrementato l'interesse per questi **dispositivi a stato solido** da una prospettiva diversa: i due stati di energia più bassi di questi circuiti potrebbero essere utilizzati come bit quantistici (qubit) e scalati fino a un computer quantistico completo attraverso la tecnologia dei circuiti integrati. 

✅Tuttavia, poiché i qubit a stato solido sono necessariamente accoppiati a molti gradi di libertà elettromagnetici tramite fili di polarizzazione e di misura, per ottenere lunghi tempi di coerenza è necessaria un'attenta progettazione del circuito.

# P.2 - Circuiti superconduttivi: effetti di carica e flusso nella coerenza quantistica
**PARAGRAFO:**
--
Circuits presently being explored combine in variable ratios the Josephson effect and single Cooper-pair charging effects. When the Josephson energy is dominant, these “flux circuits” are sensitive to external flux and its noise. Conversely, when the Coulomb energy is dominant, the “charge circuits” can decohere from charge noise generated by the random motion of offset charges. For the intermediate-energy regime, a circuit designed to be insensitive to both the charge and flux bias has recently achieved long coherence times (500 ns), demonstrating the potential of superconducting circuits.

**TRADUZIONE E ANALISI:**
--
✅I circuiti attualmente studiati combinano in proporzioni variabili l'**effetto Josephson** e gli **effetti di carica delle singole coppie di Cooper**. 

✅Quando l'energia di Josephson è dominante, questi “circuiti a flusso” (***flux circuit***) sono sensibili al flusso esterno e al rumore associato. 

✅Al contrario, quando domina l'energia di Coulomb, i “circuiti a carica” (***charge circuit***) possono perdere coerenza a causa del rumore di carica generato dal moto casuale delle cariche residue. 

✅Nel regime di energia intermedio (***phase circuit***), un circuito progettato per essere insensibile sia alla polarizzazione di carica che a quella di flusso ha recentemente raggiunto tempi di coerenza lunghi ($\pu{500 ns}$), dimostrando il potenziale dei circuiti superconduttivi.

# P.3 - Un nuovo qubit con giunzione Josephson su scala micrometrica
**PARAGRAFO:**
--
In this Letter, we present a new qubit designed around a $\pu{10 \mu m}$ scale Josephson junction in which the charging energy is very small, thus providing immunity to charge noise. Although still sensitive to flux, the circuit retains the quality of being tunable, and calculations indicate that decoherence from flux noise is small. Built into the circuit is a single-shot state measurement that has good fidelity. However, the most significant advantage is that scaling to more complex circuits will be favorable because fabrication and operation of complex superconducting integrated circuits with large junctions are well established. Moreover, the large junction capacitance enables qubits to be capacitively coupled over relatively long distances, allowing greater and more easily engineered interconnectivity.

**TRADUZIONE E ANALISI:**
--
🤔In questo articolo, presentiamo un nuovo qubit basato su una giunzione Josephson di scala $\pu{10 \mu m}$, in cui l'energia di carica è molto bassa, garantendo così immunità al rumore di carica. 
	- $E_J=\hbar I_c/2e$ con $I_c$ corrente critica direttamente proporzionale all'area della giunzione. <mark style="background: #FF5582A6;">cercare una relazione che lo mostri</mark>
	- $E_J\gg E_C$: Fase localizzata e incertezza sulla carica. <mark style="background: #FF5582A6;">Più robusto rispetto alle fluttuazioni di carica</mark>

Sebbene il circuito rimanga sensibile al flusso, conserva la proprietà di essere regolabile, e i calcoli indicano che la decoerenza dovuta al rumore di flusso è ridotta. 

Il circuito integra una misura dello stato a single-shot con buona fedeltà. 

✅Tuttavia, il **vantaggio** più significativo è la possibilità di **scalare verso circuiti più complessi**, poiché la fabbricazione e il funzionamento di circuiti integrati superconduttivi con giunzioni di grandi dimensioni sono già ben consolidati. 

Inoltre, l'elevata capacità della giunzione consente l'accoppiamento capacitivo tra qubit su distanze relativamente lunghe, facilitando una maggiore e più agevole interconnessione tra di essi.

# P.4 - Proprietà Quantistiche della Giunzione Josephson con Corrente di Bias
![[Pasted image 20250308151017.png]]
**PARAGRAFO:**
--
The quantum properties of the current-biased Josephson junction [Figs. 1(a) and 1(b)] are well established. With zero dc voltage across the junction, the Josephson inductance and the junction capacitance form an **anharmonic "LC"** resonator in which the two lowest quantized energy levels are the states of the qubit. Because the junction bias current $I$ is typically driven close to the critical current $I_0$, the anharmonic potential can be well approximated by a cubic potential, parametrized by the potential barrier height $\Delta U(I) = \left( 2 \sqrt{2} I_0 \Phi_0 / 3\pi \right) [1 - I/I_0]^{3/2}$ and a (classical) plasma oscillation frequency at the bottom of the well $\omega_p (I) = 2^{1/4} (2\pi I_0 / \Phi_0 C)^{1/2} [1 - I/I_0]^{1/4}$, where $\Phi_0 = h/2e$. Note that, as $I \to I_0$, $\Delta U$ decreases rapidly to zero, while $\omega_p$ decreases much more slowly. The bound quantum states $|n\rangle$, with energy $E_n$, can be observed spectroscopically by resonantly inducing transitions with microwaves at frequencies $\omega_{mn} = E_{mn} / \hbar = (E_m - E_n) / \hbar$. For typical operation, the number of states in the well is approximately $\Delta U / \hbar \omega_p \approx 3$, the transition frequency between qubit states is $\omega_{10} \approx 0.9 \omega_p$, and the separation of the two lowest resonant frequencies is $\omega_{10} - \omega_{21} \approx 0.1 \omega_{10}$. For the $|1\rangle$ state, the decay rate is $\gamma_1 \approx \text{Re} Y(\omega_{10}) / C \approx \omega_{10} / Q$, which is approximately the classical rate of energy decay, where $\text{Re}Y$ is the real (dissipative) part of the admittance of the current bias, and $Q$ is the oscillator quality factor. The rates $\Gamma_n$ of tunneling out of states $|n\rangle$ are given by $\Gamma_0 \approx 52 (\omega_p / 2\pi) \sqrt{\Delta U / \hbar \omega_p} \exp \left[ -7.2 \Delta U / \hbar \omega_p \right]$, with a ratio $\Gamma_{n+1} / \Gamma_n \sim 1000$.

**TRADUZIONE E ANALISI:**
--
Le proprietà quantistiche della giunzione Josephson con corrente di bias [Fig. 1(a) e 1(b)] sono ben conosciute. 
- $I_B\neq0$: *Washboard Potential*  

Con una tensione continua nulla attraverso la giunzione, l'induttanza di Josephson e la capacità della giunzione formano un risonatore **"LC" anarmonico** in cui i due livelli energetici quantizzati più bassi sono gli stati del qubit. 

Poiché la corrente di bias $I$ della giunzione è tipicamente portata vicino alla corrente critica $I_0$, il potenziale anarmonico può essere ben approssimato da un potenziale cubico, parametrizzato dall'altezza della barriera potenziale $\Delta U(I) = \left( 2 \sqrt{2} I_0 \Phi_0 / 3\pi \right) [1 - I/I_0]^{3/2}$ e da una frequenza di oscillazione al plasma (classica) al fondo della buca $\omega_p (I) = 2^{1/4} (2\pi I_0 / \Phi_0 C)^{1/2} [1 - I/I_0]^{1/4}$, dove $\Phi_0 = h/2e$. 

Si noti che, quando $I \to I_0$, $\Delta U$ decresce rapidamente a zero, mentre $\omega_p$ decresce molto più lentamente. 

Gli stati quantistici vincolati $|n\rangle$, con energia $E_n$, possono essere osservati spettroscopicamente inducendo transizioni risonanti con microonde a frequenze $\omega_{mn} = E_{mn} / \hbar = (E_m - E_n) / \hbar$. 

Per il funzionamento tipico, il numero di stati nella buca è approssimativamente $\Delta U / \hbar \omega_p \approx 3$, la frequenza di transizione tra gli stati del qubit è $\omega_{10} \approx 0.9 \omega_p$, e la separazione delle due frequenze risonanti più basse è $\omega_{10} - \omega_{21} \approx 0.1 \omega_{10}$. 

Per lo stato $|1\rangle$, il tasso di decadimento è $\gamma_1 \approx \text{Re} Y(\omega_{10}) / C \approx \omega_{10} / Q$, che è approssimativamente il tasso classico di decadimento dell'energia, dove $\text{Re}Y$ è la parte reale (dissipativa) dell'ammettenza della corrente di polarizzazione, e $Q$ è il fattore di qualità dell'oscillatore. 

I tassi $\Gamma_n$ di tunneling fuori dagli stati $|n\rangle$ sono dati da $\Gamma_0 \approx 52 (\omega_p / 2\pi) \sqrt{\Delta U / \hbar \omega_p} \exp \left[ -7.2 \Delta U / \hbar \omega_p \right]$, con un rapporto $\Gamma_{n+1} / \Gamma_n \sim 1000$.

# P.5 - Corrente ed Hamiltoniana
**PARAGRAFO:**
--
The qubit state can be fully manipulated with dc and microwave pulses of bias current
$$I(t) = I_{dc} + \delta I_{dc}(t) + I_{\mu wc}(t) \cos \omega_{10} t + I_{\mu ws}(t) \sin \omega_{10} t.$$
Under the condition that $\delta I_{dc}, I_{\mu wc},$ and $I_{\mu ws}$ are varied in time slowly compared to $2\pi / (\omega_{10} - \omega_{21}) \sim 1 \text{ ns}$, the dynamics of the system is restricted to the Hilbert space spanned by the lowest two states and has a Hamiltonian in the $\omega_{10}$ rotating frame
$$H = \hat{\sigma}_x I_{\mu wc}(t) \sqrt{\hbar / 2 \omega_{10} C} / 2 + \hat{\sigma}_y I_{\mu ws}(t) \sqrt{\hbar / 2 \omega_{10} C} / 2 + \hat{\sigma}_z \delta I_{dc}(t) (\partial E_{10} / \partial I_{dc}) / 2,$$
where $\hat{\sigma}_{x,y,z}$ are Pauli operators.

**TRADUZIONE E ANALISI:**
--
- ✅Lo stato del qubit può essere completamente manipolato con impulsi a corrente di polarizzazione DC e a microonde
	$$
	I(t) = I_{dc} + \delta I_{dc}(t) + I_{\mu wc}(t) \cos \omega_{10} t + I_{\mu ws}(t) \sin \omega_{10} t.
	$$
- 🤔Sotto la condizione che $\delta I_{dc}$, $I_{\mu wc}$ e $I_{\mu ws}$ variano nel tempo lentamente rispetto a $2\pi / (\omega_{10} - \omega_{21}) \sim 1 \text{ ns}$, la dinamica del sistema è ristretta allo spazio di Hilbert generato dai due stati più bassi e ha un Hamiltoniano nel frame rotante a $\omega_{10}$
	$$
	🤔H = \hat{\sigma}_x I_{\mu wc}(t) \sqrt{\hbar / 2 \omega_{10} C} / 2 + \hat{\sigma}_y I_{\mu ws}(t) \sqrt{\hbar / 2 \omega_{10} C} / 2 + \hat{\sigma}_z \delta I_{dc}(t) (\partial E_{10} / \partial I_{dc}) / 2,
	$$
	dove $\hat{\sigma}_{x,y,z}$ sono gli operatori di Pauli.

**([[04_Trasformazione Hamiltoniana Phase qubit e RWA]])**

# P6 - Misura dello stato del qubit tramite tunneling
**PARAGRAFO:**
--
The measurement of the qubit state utilizes the escape from the cubic potential via tunneling. To measure the occupation probability $p_1$ of state $|1\rangle$, we pulse microwaves at frequency $\omega_{21}$, driving a $1\rightarrow 2$ transition. The large tunneling rate $\Gamma_2$ then causes state $|2\rangle$ to rapidly tunnel. After tunneling, the junction behaves as an open circuit, and a dc voltage of the order of the superconducting gap ( $\sim 1\text{ mV}$ ) appears across the junction. c . Thus the occupation probability $p_1$ is equal to the probability $p_v$ of observing a voltage across the junction after the measurement pulse.


**TRADUZIONE E ANALISI:**
--
- ✅La misura dello stato del qubit sfrutta l'escape dal potenziale cubico tramite effetto tunnel. 

- ✅Per misurare la probabilità di occupazione $p_1$ dello stato $|1\rangle$, si applica un impulso a microonde alla frequenza $\omega_{21}$, inducendo una transizione $1\rightarrow 2$. 
	- [[05_Verifica dello stato di occupazione del qubit#Misura della probabilità di occupazione dello stato $ ket{1}$]]

- ✅L'elevato tasso di tunneling $\Gamma_2$ provoca quindi una rapida transizione dello stato $|2\rangle$ tramite effetto tunnel. 

- 🤔Dopo il tunneling, la giunzione si comporta come un circuito aperto e una tensione continua dell'ordine del gap superconduttivo ($\sim 1\text{ mV}$) compare ai capi della giunzione. [^7]

- ✅Questa tensione è facilmente misurabile con un **amplificatore a temperatura ambiente**. 

- ✅Di conseguenza, la probabilità di occupazione $p_1$ è uguale alla probabilità $p_v$ di osservare una tensione ai capi della giunzione dopo l'impulso di misura.

**([[05_Verifica dello stato di occupazione del qubit]])**

# P.7 - Implementazione di un bias di corrente ad alta impedenza
![[Circuito_articolo.png|400]]^FIG-1C

**PARAGRAFO:**
--
The manipulation of the qubit over many logic pulses requires a large $Q$. In turn, this imposes both a small energy relaxation rate $\gamma_1$ and a small dephasing rate from low-frequency noise in the bias current. Both of these conditions are met using a current bias with high impedance from DC to frequencies $\gtrsim \omega_p/2\pi \sim \pu{10 GHz}$. We can obtain $Q \gtrsim 10^5$ for junctions of area $\sim \pu{100 \mu m^2}$ ($C \sim \pu{10 pF}$) with $1/\text{Re}Y \gtrsim \pu{160 k\Omega}$. This cannot be achieved with a conventional current bias since typical wire impedances at microwave frequencies are low ($\sim \pu{100  \Omega}$).
[FIG-1C](04_PARAGRAFI#^FIG-1C) shows a circuit that realizes this high-impedance current bias using broadband transformers. Because of the large loop inductance $L \gg L_{J0} = \Phi_0 / 2 \pi I_0$, the circuit creates a current divider from the external biases to the bias current of the qubit junction $I \simeq (M/L)I_{\phi} + (L_{jf}/L)I_V$. These current dividers produce transformations in $1/\text{Re}Y$of $(L/M)^2$and $(L/L_{jf})^2$. Here the "filter" junction (labeled $i_0$) behaves as an inductor (When the qubit junction switches to the voltage state, the loop current I is interrupted. Because $I_V > i_0$, the filter junction then also switches) with value $L_{jf} = \Phi_0 / 2 \pi i_0$ because its current $I_V - (M/L)I_{\phi}$is made small by adjusting the biases such that $I_V \simeq (M/L)I_{\phi}$. For the particular design of Fig. 1(c), a full calculation shows that the dominant dissipation source gives $1/\text{Re}Y \simeq (L/L_{jf})^2 R_V \simeq \pu{560 k}\Omega$.

**TRADUZIONE E ANALISI:**
--
✅La manipolazione del qubit attraverso numerosi impulsi logici richiede un **fattore di qualità $Q$** elevato:
	1. **Elevato Fattore di Qualità ($Q$) Necessario**  
	   - La manipolazione del qubit avviene tramite una serie di impulsi logici. Per garantire che il qubit mantenga la coerenza quantistica durante l'intera sequenza di operazioni, è essenziale che il sistema presenti un alto $Q$.  
	   - Un elevato $Q$ significa che le perdite energetiche (rilassamento) e la perdita di coerenza della fase (dephasing) sono molto contenute, permettendo operazioni logiche accurate e ripetibili.

- ✅Questo, a sua volta, impone sia un basso tasso di rilassamento energetico $\gamma_1$ sia un basso tasso di decoerenza dovuto al rumore a bassa frequenza nella corrente di polarizzazione. 
	1. **Basso Tasso di Rilassamento Energetico e di Dephasing**  
	   - **Rilassamento Energetico:** Un tasso di rilassamento basso indica che il qubit riesce a mantenere il proprio stato eccitato per un tempo sufficiente, riducendo la probabilità di decadimento spontaneo verso lo stato fondamentale.
	   - **Dephasing:** Un basso tasso di dephasing è cruciale perché il rumore a bassa frequenza, che può disturbare la fase del qubit, è minimizzato. In altre parole, il qubit conserva la sua coerenza, essenziale per il corretto funzionamento delle operazioni logiche.
	   
- 🤔Entrambe queste condizioni vengono soddisfatte utilizzando una **corrente di bias con alta impedenza** dal DC (corrente continua) fino a frequenze $\gtrsim \omega_p/2\pi \sim \pu{10 GHz}$. 

- 🤔Possiamo ottenere $Q \gtrsim 10^5$ per giunzioni di area $\sim \pu{100 \mu m^2}$ ($C \sim \pu{10 pF}$) con $1/\text{Re}Y \gtrsim \pu{160 k\Omega}$. 

- 🤔Questo non può essere ottenuto con una corrente di bias convenzionale, poiché le impedenze tipiche dei fili alle frequenze a microonde sono basse ($\sim \pu{100 \Omega}$). 

- 🤔[FIG-1C](04_PARAGRAFI#^FIG-1C) mostra un circuito che realizza questa corrente di bias ad alta impedenza utilizzando trasformatori a banda larga. 

- 🤔A causa della grande induttanza dell'anello $L \gg L_{J0} = \Phi_0 / 2 \pi I_0$, il circuito crea un partitore di corrente dalle polarizzazioni esterne alla corrente di polarizzazione della giunzione del qubit $I \simeq (M/L)I_{\phi} + (L_{jf}/L)I_V$. 
	![[Circuito_1.jpg|300]]
	$$
	\begin{cases}
	V_{AB}=V_Z=V_R=I_R\cdot R_V=I_Z\cdot Z_{eq}\
	I_V=I_Z+I_R
	\end{cases}
	$$
	$$I_Z=I_V\cdot\frac{R_V}{R_V+Z_{eq}}$$
	![[Circuito_2.jpg|400]]
	$$
	\begin{cases}
	V_{AB}=V_{f}=V_q+V_L\
	I_Z=I+I_f\
	I_{\phi}'=I_{\phi}\cdot\dfrac{R_{\phi}}{R_{\phi}+j\omega L_{\phi}}\
	V_L=L\cdot\dfrac{dI}{dt}+M\cdot\dfrac{dI'_{\phi}}{dt}\
	V_q=L_q\cdot\dfrac{dI}{dt}\
	V_f=L_f\cdot\dfrac{dI_f}{dt}
	\end{cases}
	$$
	$$L_f\cdot\dfrac{dI_Z}{dt}=(L_f+L_q+L)\cdot\dfrac{dI}{dt}+M\cdot\dfrac{dI'_\phi}{dt}$$
	$$
	\begin{cases}
	L_fI_Z=(L_f+L_q+L)I+MI'_{\phi}\
	L_f+L_q+L = L_{eq}
	\end{cases}
	$$
	$$I=\left(\dfrac{L_f}{L_{eq}}\right) I_Z-\left(\dfrac{M}{L_{eq}}\right) I_{\phi}'$$
	$$
	\begin{cases}
	L_q=\dfrac{\Phi_0}{2\pi I_0}\
	L_f=\dfrac{\Phi_0}{2\pi i_0}
	\end{cases}
	$$
	Valori numerici:
	
	- **Corrente critica giunzione qubit:** $I_0\simeq\pu{21 \mu A}$ 
	- **Capacità qubit:** $C\simeq \pu{6 pF}$
	- **Corrente critica giunzione filtro:** $i_0\simeq \pu{10.5 \mu A}$
	- **Induttanza circuito:** $L\simeq\pu{3.3 nH}$
	- **Mutua induttanza:** $M\simeq L/160$
	- **Induttanza sul circuito del generatore di corrente $I_{\Phi}$:** $L_{\phi}\simeq \pu{0.4 nH}$
	- $R_V\simeq\pu{50 \Omega}$
	- $R_{\Phi}\simeq\pu{2 \Omega}$
	Basandoci sui valori numerici dell'articolo si ottiene che:
	$$L_{eq}\simeq L$$
	$$
	\begin{cases}
	I_Z=I_V\cdot\dfrac{R_V}{R_V+Z_{eq}}\
	I_{\phi}'=I_{\phi}\cdot\dfrac{R_{\phi}}{R_{\phi}+j\omega L_{\phi}}
	\end{cases}
	$$
	
	**Relazione dell'articolo:**
	$$I \simeq \left(\frac{M}{L}\right) I_\phi + \left(\frac{L_{Jf}}{L}\right) I_V$$
	**Relazione ricavata da me:**
	$$I \simeq -\left(\frac{M}{L}\right) I_\phi' + \left(\frac{L_{Jf}}{L}\right) I_Z$$

- 🤔Questi partitori di corrente producono trasformazioni in $1/\text{Re}Y$ di $(L/M)^2$ e $(L/L_{jf})^2$.

- 🤔Qui la giunzione "filtro" (etichettata $i_0$) si comporta come un induttore (quando la giunzione del qubit commuta nello stato di tensione, la corrente dell'anello $I$ viene interrotta. Poiché $I_V > i_0$, la giunzione filtro commuta anch'essa) con valore $L_{jf} = \Phi_0 / 2 \pi i_0$ poiché la sua corrente $I_V - (M/L)I_{\phi}$ viene ridotta regolando le polarizzazioni in modo che $I_V \simeq (M/L)I_{\phi}$. 

- 🤔Per il particolare design di Fig. 1(c), un calcolo completo mostra che la sorgente di dissipazione dominante fornisce $1/\text{Re}Y \simeq (L/L_{jf})^2 R_V \simeq \pu{560 k\Omega}$.



# P.8 - Fabbricazione e filtraggio del circuito qubit
![[Circuito_articolo.png|500]] ^FIG-1C2

**PARAGRAFO:**
--
The qubit circuit in [FIG-1C](04_PARAGRAFI#^FIG-1C2) is fabricated using a **standard trilayer niobium process** using **optical lithography**. The inductor $L$ is a six-turn spiral to minimize radiation damping and keep its self-resonance frequency $\sim\pu{15 GHz}$ much greater than $\omega_p/2\pi$. The chip is mounted inside a double-shielded $\text{Cu}$ and $\text{Al}$ box anchored to the mixing chamber of a dilution refrigerator whose base temperature is $\pu{25 mK}$. The microwave line is attenuated and the bias lines are heavily filtered with $\text{Cu}$ powder and $\text{RC}$ filters. The low-noise bias currents are generated with $\pu{4 K}$ resistors connected to optically isolated battery-powered voltage sources that have a total noise of about $\text{10 ppm}$. The resistor $R_V$ limits switching to a subgap voltage $\sim\pu{1 mV}$ to minimize quasiparticle generation.

**TRADUZIONE E ANALISI:**
--
- 🤔Il circuito qubit in [FIG-1C](04_PARAGRAFI#^FIG-1C2) è fabbricato utilizzando un **processo standard a tre strati di niobio** con **litografia ottica**. 
	- Accennare qualcosa

- ✅L'induttore $L$ è un solenoide a sei spire per ==minimizzare lo smorzamento delle radiazioni== e ==mantenere la sua frequenza di auto-risonanza (SRF) a== $\sim\pu{15 GHz}$ molto maggiore di $\omega_p/2\pi$. 

> [!important] **Solenoide $L$ a 6 spire**
>1. **Minimizzare lo smorzamento delle radiazioni** → Probabilmente vogliono evitare che l'induttore agisca come un'antenna indesiderata, il che può accadere quando le dimensioni fisiche dell'induttore diventano paragonabili alla lunghezza d'onda del segnale. Ridurre il numero di spire aiuta a limitare le perdite per radiazione.
>
>1. **Mantenere $f_{\text{SRF}}$​ alta ($\sim\pu{15 GHz}$)** → Hanno scelto il numero di spire in modo che la frequenza di auto-risonanza sia **molto maggiore di $\omega_p / 2\pi$** (la corrente di bias ha una frequenza che varia tra dc e $\omega_p / 2\pi\sim \pu{10 GHz}$). Questo garantisce che l'induttore si comporti ancora come un induttore puro nella banda di funzionamento desiderata.
>
>Se avessero usato **più di sei spire**, l'induttanza sarebbe aumentata, ma anche la **capacità parassita**, abbassando la **SRF** e aumentando il rischio di comportamento capacitivo indesiderato (vedi [[Self Resonant Frequency (SRF) di un induttore]]).

---

- ✅Il chip è montato all'interno di una scatola a doppia schermatura in $\text{Cu}$ e $\text{Al}$ ancorata alla camera di miscelazione di un refrigeratore a diluizione la cui temperatura base è $\pu{25 mK}$. 

- ℹ️La linea a microonde è attenuata e le linee di polarizzazione sono fortemente filtrate con polvere di $\text{Cu}$ e filtri $\text{RC}$. 

- ℹ️Le correnti di bias a basso rumore sono generate con resistori a temperature di $\pu{4 K}$ collegati a sorgenti di tensione alimentate a batteria isolate otticamente che hanno un rumore totale di circa $\text{10 ppm}$. 

- 🤔Il resistore $R_V$ limita la commutazione a una tensione subgap di $\sim\pu{1 mV}$ per minimizzare la generazione di quasiparticelle.


# P.9 - Determinazione del bias ottimale e quantizzazione del flusso nel circuito
![[Pasted image 20241025105404.png|400]]^FIG-2

**PARAGRAFO:**
--
The initial test of this circuit measures the device parameters and **finds optimum biasing**. [FIG-2](04_PARAGRAFI#^FIG-2) shows the values of $I_V$ and $I_\phi$ at which the circuit switches into the voltage state. Here the bias currents follow a triangular trajectory, and the full range of currents is sampled by sweeping in time the initial ratio of $I_V$ and $I_\phi$. Analysis of the circuit shows that the center of the vertical step corresponds to the optimal bias condition $I_V = (M/L)I_\phi$ discussed previously. At this point, $I_0 = I_V$ and the ratio of the two currents is $L/M$. The step height is $2i_0$ and its slope is $-L/L_{Jf}$. Multiple vertical lines at the step arise from flux quantization in the superconducting loop, with the line spacing in $I_{\phi}$ giving $M$.


**TRADUZIONE E ANALISI:**
--
- ✅Il test iniziale di questo circuito misura i parametri del dispositivo e **trova il bias ottimale**. 

- ✅La [FIG-2](04_PARAGRAFI#^FIG-2) mostra i valori di $I_V$ e $I_\phi$ ai quali il circuito passa allo stato di tensione.

- ✅Qui le correnti di bias seguono una traiettoria triangolare, e l'intero intervallo di correnti viene campionato variando nel tempo il rapporto iniziale tra $I_V$ e $I_\phi$. 

- 🤔L'analisi del circuito mostra che il centro del passo verticale corrisponde alla condizione di bias ottimale $I_V = (M/L)I_\phi$ discussa in precedenza. 

- 🤔In questo punto, $I_0 = I_V$ e il rapporto tra le due correnti è $L/M$. 

- 🤔L'altezza del passo è $2i_0$ e la sua pendenza è $-L/L_{Jf}$. 

- 🤔Le linee verticali multiple nel passo derivano dalla quantizzazione del flusso nel loop superconduttore, con la spaziatura delle linee in $I_{\phi}$ che dà $M$.

# P.10 -  Spettroscopia del qubit: determinazione dei livelli energetici e del fattore di qualità $Q$
![[Pasted image 20241025120100.png|400]]^FIG-3

**PARAGRAFO:**
--
We first determine the energy-level spacings and $Q$ spectroscopically. [FIG-3](04_PARAGRAFI#^FIG-3) shows the measured escape rate as a function of the qubit bias current $I$ in the presence of a microwave signal at a fixed frequency $\omega / 2\pi = \pu{6.80 GHz}$. A resonance is observed because $\omega_{10}$ varies with current bias. The temperature $T \simeq \pu{25 mK}$ is low enough so that without microwaves the measured escape rate is consistent with the quantum-tunneling prediction $\Gamma_0$. The resonance in the escape rate arises from the resonant increase in population of state $\ket{1}$, which tunnels at a higher rate than the ground state. [FIG-3](04_PARAGRAFI#^FIG-3) also shows an expanded current scale for resonance curves obtained with slightly different values of $\omega / 2\pi$. The full width at half maximum of these resonances is $\pu{6.1 MHz}$, implying a quality factor $Q \simeq 1000$.

**TRADUZIONE E ANALISI:**
--
- ✅Prima determiniamo le separazioni dei livelli energetici e $Q$ spettroscopicamente. 

- ✅La [FIG-3](04_PARAGRAFI#^FIG-3) mostra il tasso di fuga misurato in funzione della corrente di bias del qubit $I$ in presenza di un segnale a microonde a una frequenza fissa $\omega / 2\pi = \pu{6.80 GHz}$. 
	- **([[05_Verifica dello stato di occupazione del qubit#Controllo variando la corrente di Bias $I_B$​ (con $f_{ text{gen}}$ fisso)|Controllo in funzione di I_B e f_gen costante]])**

- ✅Si osserva una risonanza poiché $\omega_{10}$ varia con la corrente di bias. 
	$$\omega_{10}\propto\omega_p(I_B)$$
- ✅La temperatura $T \simeq \pu{25 mK}$ è sufficientemente bassa da fare in modo che, senza microonde, il tasso di fuga misurato sia coerente con la previsione del tunneling quantistico $\Gamma_0$. 
	- **N.B.** $K_BT\ll\hbar\omega_{10}$. In questo modo se si osserva qualche tunneling, sappiamo che non è per effetto termico.

- ✅La risonanza nel tasso di fuga deriva dall'**aumento risonante della popolazione dello stato** $\ket{1}$, che tunnelizza con un rate maggiore rispetto allo stato fondamentale. 
	- **([[Dinamiche di decadimento e tunneling in un Phase qubit#Tunneling quantistico|Tasso di tunneling]])**

- ✅La [FIG-3](04_PARAGRAFI#^FIG-3) mostra anche una scala di correnti allargate per mostrare le curve di risonanza ottenute con valori leggermente diversi di $\omega / 2\pi$ ($\pu{6.80 GHz}$ e $\pu{6.78 GHz}$). La larghezza a metà altezza di queste risonanze è $\pu{6.1 MHz}$, il che implica un fattore di qualità $Q \simeq 1000$.
	$$Q=\omega\times\frac{\text{Energia immagazzinata}}{\text{Dissipazione di potenza}}=\frac{f_{\text{0}}}{\Delta f}$$
	con $f_0$, frequenza di picco e $\Delta f$, larghezza di banda. 
	Quindi:
	$$Q=\frac{\pu{6.80 GHz}}{\pu{6.61 MHz}}\simeq\frac{\pu{6.78 GHz}}{\pu{6.61 MHz}}\simeq1000$$

# P.11 - Preparazione e misura dello stato del qubit
![[FIG-4.png|400]]^FIG-4

![[FIG-5.png|400]]^FIG-5

![[FIG-6.png|400]]^FIG-6

**PARAGRAFO:**
--
Figures 4-6 demonstrate preparation and measurement of the qubit state. For these data, $Q \simeq 350$ and a bias current is selected such that $\Gamma \simeq 1.2 \times 10^3 \, \text{s}^{-1}$ ($\Delta U / \hbar \omega_p \simeq 2.8$) for no microwaves. The qubit remains on resonance during the entire microwave pulse sequence by using a current bias with a slow ramp rate.

**TRADUZIONE E ANALISI:**
--
- ✅Le Figure 4-6 mostrano la **preparazione e la misura dello stato del qubit**. 
	- Imposto il sistema su uno stato, lo eccito col segnale a microonde e misuro la tensione per verificare il tunneling.

- 🤔Per questi dati, $Q \simeq 350$ e si seleziona una corrente di bias tale che $\Gamma \simeq 1.2 \times 10^3 \, \text{s}^{-1}$ $(\Delta U / \hbar \omega_p \simeq 2.8)$ **in assenza di microonde**.[^8]

- 🤔Il qubit rimane in risonanza durante l'intera sequenza di impulsi a microonde grazie all'uso di una corrente di bias con un tasso di variazione lento.[^6]
	- Far variare la corrente implica una variazione anche della risonanza.
	- La corrente di bias è prodotta anche dal trasformatore che contiene una parte oscillante. la frequenza di tale corrente è necessario sia bassa in maniera tale da avere piccole variazioni.

# P.12 - Fedeltà della misura dello stato
![FIG-4](04_PARAGRAFI#^FIG-4)
**PARAGRAFO:**
--
The fidelity of the state measurement is determined with the data of [FIG-4](04_PARAGRAFI#^FIG-4). State $\ket{1}$ is populated incoherently via an excitation pulse with frequency $\omega_{10}$, power $P_{10}$, and duration $\pu{0.7 μs}$ that is much longer than the coherence time. The state measurement pulse of duration $\pu{25 ns}$ is applied about $\pu{40 ns}$ before the end of the excitation pulse to ensure the population does not decay before measurement. We measure the probability $p_v$ as the ratio of the number of events that switch to the voltage state during the measurement pulse to the total number of events. For $P_{10} = 0$, we obtain $p_1 = 0.003$. [FIG-4](04_PARAGRAFI#^FIG-4) shows a linear increase in the population of state $\ket{1}$ with increasing $P_{10}$ until saturation occurs at $p_1 = 0.43 \pm 0.05$ for high power. We see good agreement between the data and the expected theoretical behavior $p_1 = 0.5/(1 + P_{\text{sat}}/{P_{10}})$, where the saturation power $P_{\text{sat}} = 0.065$ is chosen for best fit. We think the slight decrease in $p_1$ at the highest power is due to off resonant $1 \to 2$ transitions. The optimum setting of $P_{21}$ is chosen by maximizing the ratio of $p_v$ between $P_{10} \simeq 10P_{\text{sat}}$ and $P_{10} = 0$. These results imply that the $\ket{0}$ state is prepared and measured with greater than $99\%$ fidelity, whereas the $\ket{1}$ state is measured with $85\%$ fidelity.

**TRADUZIONE E ANALISI:**
--
- ✅La fedeltà della misura dello stato è determinata con i dati della [FIG-4](04_PARAGRAFI#^FIG-4). 

- ✅Lo stato $\ket{1}$ è popolato incoerentemente attraverso un **impulso di eccitazione** con: 
	- frequenza $\omega_{10}$
	- potenza $P_{10}$ (studio la probabilità di occupazione al variare della potenza)
	- durata $\pu{0.7 μs}$ (**molto più lunga del tempo di coerenza** - $\pu{500 ns}$). Poiché l'impulso ha una durata **molto più lunga** del tempo di coerenza, il sistema perde coerenza prima che l'impulso termini. Dopo che la coerenza si è persa, il sistema non si trova più in una sovrapposizione coerente $c_0\ket{0} + c_1 \ket{1}$, ma piuttosto in una miscela statistica in cui la probabilità di trovarlo in $\ket{1}$ dipende solo dalla potenza $P_{10}$​ e non da eventuali effetti coerenti del segnale di drive.

- ✅L'**impulso di misura** dello stato, della durata di $\pu{25 ns}$, è applicato circa $\pu{40 ns}$ prima della fine dell'impulso di eccitazione **per garantire che la popolazione non decada prima della misura**. 

- ✅Misuriamo la probabilità $p_v$ come il rapporto tra il numero di eventi che commutano nello stato di tensione durante l'impulso di misura e il numero totale di eventi. 
$$p_v=\frac{\text{N° eventi di tunneling}}{\text{N° eventi totali}}\propto p_1$$

- ✅Per $P_{10} = 0$, otteniamo $p_1 = 0.003$. La [FIG-4](04_PARAGRAFI#^FIG-4) mostra un aumento lineare della popolazione dello stato $\ket{1}$ con l'aumento di $P_{10}$ fino a che si verifica la saturazione a $p_1 = 0.43 \pm 0.05$ per alta potenza. 

- 🤔Vediamo un buon accordo tra i dati e il comportamento teorico atteso $p_1 = 0.5/(1 + P_{\text{sat}}/{P_{10}})$[^3] dove la potenza di saturazione $P_{\text{sat}} = 0.065$ è scelta per il miglior fit. 

- ✅Pensiamo che la leggera diminuzione di $p_1$ alla massima potenza sia dovuta a transizioni fuori risonanza $1 \to 2$. 

- 🤔L'impostazione ottimale di $P_{21}$ è scelta massimizzando il rapporto di $p_v$ tra $P_{10} \simeq 10P_{\text{sat}}$ e $P_{10} = 0$. 

- 🤔Questi risultati implicano che lo stato $\ket{0}$ è preparato e misurato con una fedeltà superiore al $99\%$, mentre lo stato $\ket{1}$ è misurato con una fedeltà dell’$85\%$.

# P.13 - Tasso di rilassamento dello stato $\ket{1}$
![FIG-5](04_PARAGRAFI#^FIG-5)
**PARAGRAFO:**
--
The measured relaxation rate of state $\ket{1}$ is shown in [FIG-5](04_PARAGRAFI#^FIG-5). Here $p_1$ is obtained as in [FIG-4](04_PARAGRAFI#^FIG-4), but with a time delay between excitation and measurement. We observe a nonexponential decay, initially with rate $\sim(20 \, \text{ns})^{-1}$, but later becomes significantly slower $\sim(300 \, \text{ns})^{-1}$.

**TRADUZIONE E ANALISI:**
--
- ✅Il **tasso di rilassamento** misurato dello stato $\ket{1}$ è mostrato in [FIG-5](04_PARAGRAFI#^FIG-5). 

- ✅Qui $p_1$ è ottenuto come in [FIG-4](04_PARAGRAFI#^FIG-4), ma con un **ritardo temporale tra l'eccitazione e la misura**. 

- 🤔Osserviamo un **decadimento non-esponenziale**, inizialmente con un tasso di circa $\sim (\pu{20 ns})^{-1}$, che successivamente diventa significativamente più lento, circa $\sim(\pu{300 ns})^{-1}$.

# P.14 - Manipolazione coerente dello stato del qubit
![FIG-6](04_PARAGRAFI#^FIG-6)
**PARAGRAFO:**
--
Coherent manipulation of the qubit state is demonstrated by the observation of Rabi oscillations, as shown in [FIG-6](04_PARAGRAFI#^FIG-6). These data are obtained as in [FIG-4](04_PARAGRAFI#^FIG-4), but with a $\pu{25 ns}$ excitation pulse that allows coherence to be maintained during the pulse. The phase of the Rabi oscillations is the product of the microwave amplitude and pulse length. Because the coherence time is short, the data of [FIG-6](04_PARAGRAFI#^FIG-6) are obtained by fixing the duration of the pulse and varying the amplitude. For an initial pulse of $\pu{17 ns}$ (data not shown), the Rabi oscillations have similar magnitude but a period $1.36$ times longer, consistent within experimental uncertainties to the ratio of the pulse widths. Full modulation of the oscillations between $0$ and $1$ is expected without decoherence; the observed amplitude of $15\%$ points to a coherence time of $\sim \pu{10 ns}$, consistent with our other observations.

**TRADUZIONE E ANALISI:**
--
- 🤔La manipolazione coerente dello stato del qubit è dimostrata dall'osservazione delle **oscillazioni di Rabi**[^5], come mostrato in [FIG-6](04_PARAGRAFI#^FIG-6). 

- 🤔Questi dati sono ottenuti come in [FIG-4](04_PARAGRAFI#^FIG-4), ma con un impulso di eccitazione di $\pu{25 ns}$[^4] che permette di mantenere la coerenza durante l'impulso. 
	- **Durata dell'impulso COSTANTE**. 

- ✅La fase delle oscillazioni di Rabi è il **prodotto dell'ampiezza delle microonde e della durata dell'impulso**. 

- ✅Poiché il tempo di coerenza è breve, i dati di [FIG-6](04_PARAGRAFI#^FIG-6) sono ottenuti **fissando la durata dell'impulso e variando l'ampiezza**. 

- 🤔Per un impulso iniziale di $\pu{17 ns}$ (dati non mostrati), le oscillazioni di Rabi hanno magnitudine simile ma un periodo $1.36$ volte più lungo, in accordo, entro le incertezze sperimentali, con il rapporto tra le larghezze degli impulsi. 

- 🤔Una modulazione completa delle oscillazioni tra $0$ e $1$ è attesa in assenza di decoerenza; l'ampiezza osservata del $15\%$ indica un tempo di coerenza di $\sim \pu{10 ns}$, coerente con le nostre altre osservazioni.

# P.15 - Origine della decoerenza e possibili miglioramenti
**PARAGRAFO:**
--
The data in Figs. 4–6 consistently give a qubit coherence time much shorter than the predicted value $\pu{4 μs}$. Clearly, a source of noise and dissipation other than that of the circuit admittance must be present. The nonexponential energy decay possibly indicates that the qubit couples to a *small* number of other degrees of freedom that can transfer energy back to the qubit. We also observe that the measured $Q$ randomly changes over time by a factor of $\sim 2$ when the junction is at base temperature $\pu{25 mK}$, and by a factor of $\sim 4$ when heated briefly to $\pu{300 mK}$. These observations suggest that the extra decoherence comes from dissipation in the thin ($\sim \pu{2 nm}$) capacitor formed by the tunnel junction, probably from trap states in niobium oxides. Since long coherence and energy relaxation times have been measured in $\text{Al/Al}_2\text{O}_3\text{/Al}$ and $\text{NbN/AlN/NbN}$ tunnel junctions, we expect our qubit circuit will attain coherence times $> \pu{1 μs}$ after improving or changing our junction fabrication process.

**TRADUZIONE E ANALISI:**
--
- 🤔I dati nelle Figs. 4–6 indicano costantemente un **tempo di coerenza del qubit molto più breve rispetto al valore previsto** di $\pu{4 μs}$. 

- ✅È evidente che deve essere **presente una sorgente di rumore e dissipazione** diversa da quella dovuta all'ammettenza del circuito. 

- 🤔Il decadimento energetico non esponenziale potrebbe indicare che il **qubit si accoppia a un _numero ridotto_ di altri gradi di libertà**, i quali possono trasferire energia nuovamente al qubit. 

- 🤔Osserviamo inoltre che il **valore misurato di $Q$ cambia casualmente nel tempo** di un fattore $\sim 2$ quando la giunzione è alla temperatura base di $\pu{25 mK}$, e di un fattore $\sim 4$ quando viene riscaldata brevemente fino a $\pu{300 mK}$. 

- 🤔Queste osservazioni suggeriscono che la **decoerenza aggiuntiva derivi dalla dissipazione nel sottile condensatore** ($\sim \pu{2 nm}$) formato dalla giunzione tunnel, probabilmente a causa di stati di trappola negli ossidi di niobio. 

- ✅Poiché tempi di coerenza e rilassamento energetico lunghi sono stati misurati in giunzioni tunnel $\text{Al/Al}_2\text{O}_3\text{/Al}$ e $\text{NbN/AlN/NbN}$, ci aspettiamo che il nostro circuito per il qubit raggiunga tempi di coerenza $> \pu{1 μs}$ dopo un miglioramento o una modifica del processo di fabbricazione della giunzione.

# P.16 - Conclusioni
**PARAGRAFO:**
--
In conclusion, we have devised a new Josephson-junction circuit based on large-area junctions that is a good candidate for a scalable solid-state quantum computer. This circuit uses broadband impedance transformers to isolate the qubit from dissipation of the bias and measurement leads. Although decoherence is stronger than expected, proper operation has been clearly demonstrated. Observation of Rabi oscillations shows coherent manipulation of the qubit states, and preparation and measurement is accomplished with high fidelity.

**TRADUZIONE E ANALISI:**
--
- ✅In conclusione, abbiamo progettato un nuovo circuito a giunzione Josephson basato su giunzioni di grande area, che rappresenta un **buon candidato per un computer quantistico scalabile a stato solido**. 

- 🤔Questo circuito utilizza trasformatori di impedenza a banda larga per isolare il qubit dalla dissipazione dovuta alle linee di polarizzazione e misura. 

- ✅Sebbene la decoerenza sia più forte del previsto, il corretto funzionamento è stato chiaramente dimostrato. 

- ✅L'osservazione delle oscillazioni di Rabi mostra una manipolazione coerente degli stati del qubit, e la preparazione e la misura vengono effettuate con alta fedeltà.




---

[^3]: Da dove arriva la relazione attesa?

[^4]: Cosa mi garantisce che 25 ns sono adeguati per mantenere la coerenza?

[^5]: Fare la spiegazione teorica.

[^6]: Cosa significa che la corrente varia lentamente? non dovrebbe rimanere fissa?
	I termini a microonde hanno frequenze alte. come mai non causano variazione della frequenza di risonanza da che sono parte della corrente di bias?

[^7]: perché non aumenta se abbiamo detto che si ha un'accelerazione?

[^8]: La scelta del bias è vincolata al contenere 3 livelli nella barriera e rispettare il bias ottimale ottenuto nel paragrafo 9?
