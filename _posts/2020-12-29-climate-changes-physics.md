---
layout: post
category: climate-change
date: 2020-12-29
highcharts: off
image: /assets/images/blog-climate-changes.jpg
language: it
location: Nice
mathjax: 'on'
summary: Una breve carrellata sulla fisica dei Cambiamenti Climatici.
title: Cambiamenti Climatici - parte I
titlejumbotron: 'off'
---

## Cambiamenti Climatici - parte I
### Fondamenti fisici

Cominciamo con alcuni brevi principi fisici di base per comprendere i fenomeni che sono alla base
del clima terrestre e rendere meno astratta l'espressione ormai comunemente usata da tutti:
"*i cambiamenti climatici*".

#### Energia, temperatura e radiazione elettromagnetica

Tutti i corpi possiedono una *energia interna* che si manifesta a livello microscopico come
movimento o oscillazione degli atomi che lo costituiscono.

La *temperatura* di un corpo à la misura macroscopica di questa energia interna.
Quando quest'ultima aumenta, cioè il movimento interno dei suoi atomi aumenta, la temperatura del
corpo cresce.
E viceversa, una diminuzione della sua energia interna risulta in una diminuzione della
temperatura globale del corpo.

<div class="bd-callout bd-callout-info">
<h6>La scala Kelvin delle temperature</h6>
<p>
I fisici utilizzano di preferenza la <i>scala Kelvin</i> (introdotta dal fisico britannico
William Thomson, meglio conosciuto come Lord Kelvin), poichè la temperatura espressa in questo
modo è proporzionale all'energia interna di un corpo. Ad esempio un raddoppio della temperatura
in gradi Kelvin di un corpo si traduce in un raddoppio della sua energia interna.
Questa proprierà non è valida per una misura in gradi centrigradi.

Si passa facilmente da una temperatura espressa in gradi Kelvin all'equivalente temperatura
in gradi centigradi sottraendo 273 gradi (più precisamente 273,15 gradi) ed aggiungendo
273 gradi nella conversione inversa.
$$
\begin{array}{l|rcl}
conversione & °C & \xrightarrow[]{\text{ + 273 }}      & °K \\
            & °K & \xleftarrow[]{\text{ &minus; 273 }} & °C
\end{array}
$$

Lo <i>zero assoluto</i> (0°K) è la temperatura minima possibile teorica di un qualsiasi sistema
termodinamico. Si può dimostrare in base alle leggi della fisica che è una temperatura limite non
raggiungibile.
</p>
</div>

L'energia di un corpo si diffonde nello spazio anche in assenza di materia, come
*radiazione elettromagnetica*. È così che l'energia emessa dal sole raggiunge l'atmosfera e la
superficie terrestre, sotto forma di un flusso di fotoni di luce, dopo aver percorso la distanza di
circa 150 milioni di kilometri che ci separa dalla nostra stella.

La luce si può convenientemente immaginare come un fascio di onde che si propagano nello spazio
vuoto ad una velocità $$c$$ pari a quasi 300000 km/s.
Ogni onda è caratterizzata da una *frequenza* $$\nu$$ pari al suo numero di oscillazioni
(o *cicli*) al secondo e da una *lunghezza d'onda* $$\lambda$$

$$
\lambda = \frac{c}{\nu}
$$

<div class="pb-2">
<img src="/assets/images/blog-spettro-elettromagnetico.png" class="mx-auto d-block img-fluid">
<p class="text-center"><small>
Spettro elettromagnetico &mdash; da scienzeescienze.blogspot.com
</small></p>
</div>

I nostri occhi, a seguito dell'evoluzione biologica, sono diventati sensibili ad una parte dei
fotoni emessi dal sole e le cui frequenze definiamo per questo *visibili*.
Le frequenze superiori comprendono gli *ultravioletti* (*UV*), e radiazioni che trasportano ancora
più energia e pertanto estremamente pericolose perchè interferiscono con la chimica degli
organismi viventi.
Delle frequenze inferiori a quelle visibili notiamo in particolare gli *infrarossi*
(*IR*) che pur essendo invisibili all'occhio umano, svolgono come vedremo un ruolo chiave nel clima
della terra.

Si definisce *corpo nero* un corpo ideale in grado di assorbire tutta la radiazione
elettromagnetica incidente senza rifletterla (da cui il nome).
La radiazione emessa da un corpo nero viene detta *radiazione del corpo nero* e la densità di
energia irradiata, in funzione della lunghezza d’onda $$\lambda$$, *spettro di corpo nero*.
Tale spettro presenta una caratteristica forma a campana (più o meno asimmetrica e più o meno
schiacciata) dipendente unicamente dalla sua temperatura $$T$$.
Dall'immagine che segue si nota che all'aumentare della temperatura l'area sottesa dalla curva
aumenta ed il picco si sposta verso frequenza sempre più alte, indice dell'aumento dell'energia
interna del corpo.

<div class="pb-3">
<img src="/assets/images/blog-blackbody-spectra.jpg" class="mx-auto d-block img-fluid">
</div>

La maggior parte dei <i>solidi</i> e <i>liquidi</i> sulla superficie della terra sono
approssimabili a corpi neri.
L'atmosfera terrestre si comporta invece in modo <i>molto differente</i>:
i gas che la compongono interagiscono con la luce esclusivamente a specifiche frequenze.
I loro legami chimici e molecolari entrano infatti in risonanza solo se illuminati da una luce
avente una frequenza prossima o uguale ad uno dei suoi punti di risonanza, caratteristici di
ogni tipo di gas perchè legati alla loro particolare struttura atomica.

Il meccanismo di trasferimento dell'energia funziona anche in senso inverso:
l'energia dalla materia viene *riemessa verso l'esterno* sotto forma di fotoni di luce.
Tutti gli oggetti che ci stanno intorno emettono in continuazione fotoni.

<div class="bd-callout bd-callout-info">
<h6>Legge di Stephan-Boltzmann</h6>
<p>
I dati sperimentali mostrano che la quantità di energia emessa da un corpo nero è direttamente
proporzionale alla potenza quarta della temperatura, secondo la relazione nota come
<i>legge di Stephan-Boltzmann</i>:
$$
E_{emessa} = \sigma T^4
$$
</p>
</div>

Gli oggetti a temperatura ambiente (mediamente 300°K circa), emettono fotoni che, come indica
la legge di Stephan-Boltzmann, hanno una energia molto inferiore di quelli di origine solare.
Il sole ha infatti ha una temperatura superficiale stimata a circa 6000°K.
La loro lunghezza d'onda si trova quindi *nella zona degli infrarossi*.
Possiamo "visualizzarli" con una telecamera speciale (ad infrarossi per l'appunto), come quelle
che vengono comunemente installate per la video-sorveglianza notturna.

I corpi dunque emettono e ricevono fotoni.
Il *bilancio energetico*, dato dalla differenza tra energia emessa ed energia assorbita, determina
la temperatura di un corpo nel tempo. Nel caso limite in cui le due quantità di energia si
eguaglino, la sua temperatura non cambia.
Si dice allora che è in una situazione di *equilibrio termodinamico*.

#### Gas ad effetto serra

Il sole costituisce la nostra sorgente naturale di energia.
Essa viene emessa dalla nostra stella in ogni direzione e a seconda della stagione
terrestre, la parte di potenza intercettata dalla terra varia tra 168500 TW e 180000 TW
(1 TW, terawatt, corrisponde ad un miliardo di Watt).
Una quantità enorme, che se riuscissimo ad utilizzare anche solo in minima parte, coprirebbe il
fabbisogno energetico dell'umanità intera, attualmente di circa 18 TW.

Non tutta l'energia raggiunge la superficie terrestre.
Parte della luce solare viene riflessa dalle nuvole e dall'atmosfera.
Una frazione viene anche riflessa dalla superficie terrestre.
La frazione della luce riflessa è detta *albedo* e viene indicata con il simbolo $$\alpha$$.
La terra ha un albedo pari a circa 0.3 (cioè del 30%).

<div class="bd-callout bd-callout-warning">
<h6>Albedo terrestre</h6>
<p>
Le superfici ricoperte di neve o ghiaccio e le nuvole sono particolarmente riflettenti e
provocano un aumento dell'albedo. Gli oceani hanno invece un effetto contrario, essendo di colore
scuro. Le zone emerse del pianeta e coperte da vegetazione hanno un influsso variabile sull'albedo,
dipendente dal tipo (colore) di vegetazione prevalente.
</p>
</div>

Circa il 78% dell'atmosfera terrestre è composto da azoto (nella forma $$N_2$$), il 21% da
ossigeno (come $$O_2$$), lo 0,93% da gas Argon. Questi gas sono trasparenti ai fotoni provenienti
dal sole, cioè non ne ostacolano il cammino verso la superficie terrestre e gli oceani, ed anche
alla radiazione infrarossa emessa dalla terra.
La ragione è che la vibrazione dei loro legami chimici non provoca uno sbilanciamento del campo
elettrico della molecola, essendo questa perfettamente simmetrica.

Il costituente atmosferico che segue in pencentuale è il *vapore acqueo*, che deriva
principalmente dall'evaporazione delle superfici oceaniche, e la cui abbondanza percentuale
varia da luogo a luogo della terra: più presente nelle zone calde tropicali e meno in quelle
fredde polari. La sua concentrazione è regolata dal *ciclo dell'acqua*:
quando raggiunge un livello critico, dipendente dalla temperatura e da altri fattori come le
impurità e gli inquinanti presenti nell'aria, essa ricade sulla terra sotto forma di pioggia o
neve.

Al vapor acqueo segue in scala di importanza l'*anidride carbonica* (nota anche come
*diossido di carbonio*; formula chimica: $$CO_2$$) che costituiste attualmente lo 0.0415%
dell'atmosfera e viene misurata per questo con una unità di misura più pratica: in
*parti per milione* (*ppm*).

<div class="bd-callout bd-callout-warning">
<p>
Il valore 0.0415% corrisponde a 415 ppm, 415 molecole di anidride carbonica ogni milione di
molecole d'aria. Tale valore è stato misurato nel mese di novembre 2020 dalla strumentazione
dell'osservatorio Mauna Loa, Hawaii.
</p>
</div>

<div pb-2>
<img src="/assets/images/blog-nasa-CO2-level.png" class="mx-auto d-block img-fluid">
<p class="text-center">
<small>
Livello di diossido di carbonio in ppm misurato dal 2005
&mdash; dati <a href="http://www.noaa.gov/"><small>NOAA</small></a>
</small>
</p>
</div>

Contrariamente al vapore acqueo, il diossido di carbonio rimane stabilmente nell'atmosfera per
tempi molto lunghi. Occorrono alcuni secoli o millenni affinchè venga assorbito dagli oceani e
dalla vegetazione terrestre, ma una parte consistente, pari a circa il 25%, rimarrà attivo
pressochè *indefinitamente* (per centinaia di migliaia di anni), spostandosi essenzialmente
tra atmosfera, oceani e vegetazione.
L'interessante ciclo del carbonio terrestre è descritto in modo dettagliato nel libro
"*The Long Thaw*" di David Archer e sarà descritto in un prossimo post.

Altri gas presenti in parti ancora minori sono il metano ($$CH_4$$) e l'ozono ($$O_3$$) che
in alta armosfera è fondamentale per la preservazione della vita sulla terra, poichè assorbe
buona parte dei raggi ultravioletti ad alta energia provenienti dal sole.

<div class="bd-callout bd-callout-warning">
<p>
Questo gruppo di gas (<i>vapore acqueo</i>, <i>diossido di carbonio</i> e <i>metano</i>
principalmente), pur essendo presenti soltanto in tracce nell'atmosfera, hanno un ruolo vitale e
vengono indicati col il nome di <i>gas ad effetto serra</i>.
Essi infatti assorbono parte dei fotoni infrarossi emessi dalla superficie terrestre.
Questo fatto provoca un riscaldamento della zona bassa dell'atmosfera (la <i>troposfera</i>) che
raggiungere la temperatura media di 288°K (15°C) invece dei 255°K (&minus;18°C) che ci sarebbero in
loro assenza.
</p>
</div>

<div pb-2>
<img src="/assets/images/blog-infrared-absoption-spectra-of-major-gases.png"
     class="mx-auto d-block img-fluid">
<p class="text-center">
<small>
Spettro di assorbimento dei principali gas atmosferici &mdash;
<a href="https://www.spectralcalc.com"><small>SpectralCalc.com</small></a>
</small>
</p>
</div>

<div class="bd-callout bd-callout-info">
<p>
Le prime misurazioni della quantità di calore assorbita dai vari gas serra risale agli esperimenti
di laboratorio condotti dal fisico inglese John Tyndall nel 1859. Tyndall concluse correttamente
che la parte principale dell'effetto serra è provocato dal vapore acqueo a causa della sua
relativa alta concentrazione nell'atmosfera. I suoi esperimenti mostrarono anche che il diossido
di carbonio è un altro importante gas ad effetto serra ed egli arrivò anche a provare un'altra
importante conclusione: senza gas ad effetto serra le temperature notturne terrestri sarebbere
inferiori a quanto misuriamo.
Questi risultati furono riaffermati dal chimico e fisico svedese Svante Arrhenius verso la fine
degli anni 1890. Arrhenius calcolò anche che un raddoppio della quantità di anidride carbonica
nell'atmosfera avrebbe causato un <i>incremento di temperatura</i> da 5 a 6 gradi centigradi.
Una stima che è più elevata di quella
<a href="https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2019RG000678">attuale</a>
(da 2.6 a 4.1°C), ma che gli ha comunque valso il titolo di
"<i>padre dei cambiamenti climatici</i>".
</p>
</div>

#### Bilancio termico terrestre

La temperatura degli oceani e della superficie terrestre è determinata dall'interazione tra il
flusso di energia proveniente dal sole e quello irraggiato della terra verso lo spazio.
Il flusso di energia infrarossa aumenta con il crescere della temperatura, verso un nuovo
equilibrio termico terrestre, che tuttavia non può essere raggiunto perchè ogni anno vengono
rilasciati nell'atmosfera dalle attività umane miliardi di tonnellate di $$CO_2$$, bruciando
combustibili fossili e distruggendo foreste che ne assorbirebbero una parte considerevole
(transformandola per mezzo della fotosintesi in ossigeno ed altre sostanze organiche).
Miliardi di tonnellate che anno dopo anno si accumulano nell'atmosfera e provocano un aumento
dell'effetto serra naturale e della temperatura media della troposfera.

I risultati scientifici, soprattutto degli ultimi trenta anni, ci mostrano che il
clima terrestre è un *sistema complesso* costituito da molteplici elementi strettamente correlati
tra loro ed in equilibrio instabile, almeno su una scala di centinaia di migliaia di anni.
Stiamo eseguendo su scala planetaria un esperimento di cui non sappiamo calcolare pienamente le
conseguenze, ma di cui la scienza ci indica in modo sempre più chiaro l'estrema pericolosità.

Non abbiamo un pianeta o un ecosistema di riserva, dove migrare nel caso il risultato fosse
disastroso.
Ed affidarsi all'idea che la tecnologia del futuro saprà risolvere il problema è un rischio
insensato ed il cui prezzo maggiore sarà pagato da altri: le generazioni future.
