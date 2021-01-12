---
layout: post
category: climate-change
date: 2020-12-29
highcharts: off
image: /assets/images/blog-climate-changes.jpg
language: it
license: 'CC BY-SA 3.0'
location: Nice
mathjax: 'on'
summary: Una breve carrellata sulla fisica dei Cambiamenti Climatici.
title: Fisica dei Cambiamenti Climatici
titlejumbotron: 'off'
---
## Cambiamenti Climatici
### Riscaldamento Globale

Cominciamo col definire *cambiamento climatico* la modifica dei valori statistici del clima
terrestre (variazione dei valori medi ed estremi delle temperature e delle precipitazioni o di
altri parametri meteorologici importanti), misurati su un periodo di alcuni decenni.
La misura su un lungo periodo ha lo scopo di rimuovere il rumore delle fluttuazioni statistiche
naturali (per esempio le variazioni stagionali) e mettere in evidenza le linee di tendenza.

Nei prossimi paragrafi introduciamo brevemente alcuni principi fisici di base utili a comprendere
i fenomeni che sono alla base del clima, con lo scopo di rendere spero meno astratta una
espressione ormai comunemente usata da tutti, e che costituisce un importante aspetto dei
cambiamenti climatici: il *riscaldamento globale*.

#### Energia, temperatura e radiazione elettromagnetica

Tutti i corpi possiedono una *energia interna* che si manifesta a livello microscopico come
movimento o oscillazione degli atomi che lo costituiscono.

La *temperatura* di un corpo è la misura *macroscopica* di questa energia interna.
Quando quest'ultima aumenta, cioè il movimento interno dei suoi atomi aumenta, la temperatura del
corpo cresce.
E viceversa, una diminuzione della sua energia interna risulta in una diminuzione della
temperatura globale del corpo.

<div class="bd-callout bd-callout-info">
<h6>La scala Kelvin delle temperature</h6>
<p>
I fisici utilizzano di preferenza la <i>scala Kelvin</i> delle temperature (introdotta dal fisico
britannico William Thomson, meglio conosciuto come Lord Kelvin), poichè la temperatura espressa in
questo modo è proporzionale all'energia interna di un corpo. Ad esempio un raddoppio della
temperatura in gradi Kelvin di un corpo si traduce in un raddoppio della sua energia interna.
Questa proprierà non è valida per una misura in gradi centrigradi.

Si passa facilmente da una temperatura espressa in gradi centigradi all'equivalente temperatura
in gradi Kelvin aggiungendo 273 gradi (più precisamente 273,15 gradi) e sottraendo 273 gradi
nella conversione inversa.
$$
\begin{array}{l|rcl}
conversione & \rm{°C}& \xrightarrow[]{\text{ + 273 }}     & °\rm{K} \\
            & \rm{°K}& \xleftarrow[]{\text{ &minus; 273 }}& °\rm{C}
\end{array}
$$

Ad esempio la temperatura media sulle superficie terrestre è di 15°C, corrispondente a
273 + 15 = 288°K.

Lo <i>zero assoluto</i> (0°K) è la <i>temperatura minima possibile teorica</i> di un qualsiasi
sistema termodinamico.
Si può dimostrare in base alle leggi della fisica che si tratta di una temperatura limite non
raggiungibile.
</p>
</div>

L'energia di un corpo si diffonde nello spazio, anche in assenza di materia, come
*radiazione elettromagnetica*. È così che l'energia emessa dal sole raggiunge l'atmosfera e la
superficie terrestre, sotto forma di un *flusso di fotoni di luce*
(piccoli pacchetti o quanti di energia), dopo aver percorso la distanza di circa 150 milioni di
kilometri che ci separa dalla nostra stella.

Dal punto di vista ondulatorio, un fotone ha una sua *frequenza* di vibrazione $$\nu$$ ed una
sua *lunghezza d'onda* $$\lambda$$

$$
\lambda = \frac{c}{\nu}
$$

dove $$c$$ è la [velocità della luce](https://it.wikipedia.org/wiki/Velocit%C3%A0_della_luce)
nel vuoto.
I fotoni trasportano un'energia $$E$$ proporzionale alla frequenza $$\nu$$

$$
E = h \nu
$$

dove $$h$$ è la [costante di Planck](https://it.wikipedia.org/wiki/Costante_di_Planck).
 
<div class="pb-2">
<img src="/assets/images/blog-spettro-elettromagnetico.jpg" class="mx-auto d-block img-fluid">
<p class="text-center"><small>
Spettro elettromagnetico &mdash; da scienzeescienze.blogspot.com
</small></p>
</div>

I nostri occhi, a seguito dell'evoluzione biologica, sono diventati sensibili ad una parte dei
fotoni emessi dal sole, le cui frequenze definiamo per questo *visibili*.
La lunghezza d'onda della luce visibile nell'aria va indicativamente dai 390 ai 700 nm
(*nanometri*, unità di lunghezza corrispondente a $$10^{-9}$$ metri), un ordine di grandezza
pari a circa un centesimo dello spessore di un capello.

Le frequenze superiori comprendono gli *ultravioletti* (*UV*), e radiazioni che trasportano ancora
più energia e pertanto estremamente pericolose perchè interferiscono con la chimica degli
organismi viventi.
Delle frequenze inferiori a quelle visibili notiamo in particolare gli *infrarossi*
(*IR*) che pur essendo invisibili all'occhio umano, svolgono come vedremo un ruolo chiave nel clima
della terra e quindi influenzano la nostra vita di tutti i giorni.

Si definisce *corpo nero* un corpo ideale in grado di assorbire tutta la radiazione
elettromagnetica incidente senza rifletterla (da cui il nome).

Il meccanismo di trasferimento dell'energia funziona anche in senso inverso:
l'energia dalla materia viene *riemessa verso l'esterno* sotto forma di fotoni di luce.
La radiazione emessa da un corpo nero viene detta *radiazione del corpo nero* e la densità di
energia irradiata, in funzione della lunghezza d’onda $$\lambda$$, *spettro di corpo nero*.
Tale spettro presenta una caratteristica forma a campana (più o meno asimmetrica e più o meno
schiacciata) dipendente unicamente dalla sua temperatura $$T$$.

<div class="pb-3">
<img src="/assets/images/blog-blackbody-spectra.jpg" class="mx-auto d-block img-fluid">
</div>

Dall'immagine si nota come, all'aumentare della temperatura, l'area sottesa dalla curva aumenti
ed il picco si sposti verso frequenze più alte (e quindi lunghezze d'onda $$\lambda$$ più
piccole), indice dell'aumento dell'energia interna del corpo, come visto precedentemente.

<div class="bd-callout bd-callout-info">
<h6>Legge dello spostamento di Wien</h6>
<p>
Più precisamente il picco di emissione dello spettro segue la semplice relazione nota con il
nome di <i>legge dello spostamento di Wien</i>
$$
\lambda_{max} = \frac{b}{T} \approx \frac{3000}{T}
$$
dove <i>b</i> vale circa 2898 m K.
Per <i>T</i> pari a 6000°K per esempio (vicina alla temperatura della superficie solare),
il picco di emissione è a circa 0.5 micrometri (500 nm), nel campo visibile.
Ad una temperatura ambiente <i>T</i> di 300°K corrisponde invece un picco a circa 10 micrometri,
nella zona degli infrarossi.
</p>
</div>

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

La maggior parte dei <i>solidi</i> e <i>liquidi</i> sulla superficie della terra sono
approssimabili a corpi neri.
L'atmosfera terrestre si comporta invece in modo <i>molto differente</i>:
i gas che la compongono interagiscono con la luce esclusivamente a specifiche frequenze.
I loro legami chimici e molecolari entrano infatti in risonanza solo se illuminati da una luce
avente una frequenza prossima o uguale a valori particolari e caratteristici di ogni tipo
di gas perchè legati alla sua struttura atomica.

Tutti gli oggetti a temperatura ambiente e la terra stessa, da quanto abbiamo visto, emettono
fotoni *nella zona degli infrarossi*.
Possiamo "visualizzare" quelli emessi da oggetti a noi vicini con una macchina fotografica
o una telecamera speciali (ad infrarossi per l'appunto), come quelle che vengono comunemente
installate per la video-sorveglianza notturna.

<div class="pb-3">
<img src="/assets/images/blog-infrared-photo.jpg" class="mx-auto d-block img-fluid">
</div>

Il *bilancio energetico*, dato dalla differenza tra l'energia emessa da un corpo e l'energia
assorbita, determina la temperatura di un corpo nel tempo.
Nel caso limite in cui le due quantità di energia si eguaglino, la sua temperatura rimane
costante. Si dice allora che è in una situazione di *equilibrio termodinamico*.

#### Gas ad effetto serra

Il sole costituisce la nostra sorgente naturale di energia.
Essa viene emessa dalla nostra stella in ogni direzione e a seconda della stagione
terrestre, la parte di potenza intercettata dalla terra varia tra 168500 TW e 180000 TW
(1 TW, terawatt, corrisponde ad un miliardo di Watt).
Una quantità enorme, che se riuscissimo ad utilizzare anche solo in minima parte, coprirebbe il
fabbisogno energetico dell'umanità intera, attualmente di circa 18 TW.

Non tutta l'energia raggiunge la superficie terrestre e viene assorbita.
Parte della luce solare viene essenzalmente riflessa dalle nuvole ($$H_2O$$) e
dall'[*aerosol atmosferico*](https://it.wikipedia.org/wiki/Particolato) di origine umana
(inquinamento) e di origine vulcanica.
Parte viene riflessa anche dalla superficie terrestre.
La frazione totale riflessa è detta *albedo* e viene indicata con il simbolo $$\alpha$$.
La terra ha attualmente un albedo pari a circa 0.3 (cioè del 30%).

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
fredde polari. È importante notare che la sua concentrazione è *regolata* da quelle che viene
chiamato il *ciclo dell'acqua*: quando raggiunge un livello critico, dipendente dalla temperatura
e da altri fattori come le impurità e gli inquinanti presenti nell'aria, essa ricade sulla terra
sotto forma di pioggia o neve.

Al vapor acqueo segue in scala di importanza l'*anidride carbonica* (nota anche come
*diossido di carbonio*; formula chimica: $$CO_2$$) che costituiste attualmente (2020) lo 0.0415%
dell'atmosfera.
Vista la sua presenza nell'atmosfera in quantità così limitate, viene misurata con una unità
di misura più pratica: in *parti per milione* (*ppm*).

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
Livello di CO2 in ppm misurato dal 2005 &mdash;
dati <a href="http://www.noaa.gov/"><small>NOAA</small></a>
</small>
</p>
</div>

<div class="bd-callout bd-callout-warning">
<p>
Nel 2021 sarà probabilmente superato per alcune settimane tra aprile e giugno il valore di
417 ppm. Un incremendo del 50% rispetto al valore di 278 ppm di fine secolo XVIII, epoca
in cui l'attività industriale ha cominciato a diffondersi in modo capillare.
Il livello di 348 ppm, 25% superiore a quelle  pre-industriale è stato raggiunto nel 1986.
L'accumulo di diossido di carbonio nell'atmosfera sta accelerendo.
Sono stati infatti necessari più di 200 anni per raggiungere l'incremento del 25% e solo altri
35 per raggiungere il 50%.
</p>
</div>

Contrariamente al vapore acqueo, il diossido di carbonio rimane stabilmente nell'atmosfera per
tempi molto lunghi. Occorrono alcuni secoli o millenni affinchè venga assorbito dagli oceani e
dalla vegetazione terrestre, ma una parte consistente, pari a circa il 25%, rimane attivo
pressochè *indefinitamente* (per centinaia di migliaia di anni), spostandosi essenzialmente
tra atmosfera, oceani e vegetazione.
L'interessante ciclo del carbonio terrestre è descritto in modo dettagliato nel libro
"*The Long Thaw*" di David Archer e sarà descritto in un prossimo post.

Altri gas presenti in parti ancora minori sono il metano ($$CH_4$$) e l'ozono ($$O_3$$).
Quest'ultimo, in alta armosfera, è fondamentale per la preservazione della vita sulla terra,
poichè assorbe buona parte dei raggi ultravioletti ad alta energia provenienti dal sole.
Il metano rimane nell'atmosfera per alcune decine di anni, per poi degradarsi in $$CO_2$$.
La sua concentrazione in atmosfera, che si misura in *ppb* (parti per miliardo), è aumentata da
700 ppb nel periodo 1000-1750 a quasi
[1.877](https://www.esrl.noaa.gov/gmd/ccgg/trends_ch4/?fbclid=IwAR3_8r1Y_gPP9W2Chj8kek7CVFP7h-V4uAxeOwdv2zsQG2-INiB1l-N6XkE)
ppb nell'agosto 2020, con un incremento vicino al 270%.

<div class="bd-callout bd-callout-warning">
<p>
Questi ultimi gas descritti (<i>vapore acqueo</i>, <i>diossido di carbonio</i> e <i>metano</i>i
essenzialmente), pur essendo presenti soltanto in tracce nell'atmosfera, hanno un ruolo vitale e
vengono indicati con il nome di <i>gas ad effetto serra</i>.
Essi infatti assorbono parte dei fotoni infrarossi emessi dalla superficie terrestre, impedendone
la dispersione nello spazio cosmico.
Questo fatto provoca un riscaldamento della zona bassa dell'atmosfera (la <i>troposfera</i>) che
raggiunge così la temperatura media di 288°K (15°C) invece dei 255°K (&minus;18°C) che ci
sarebbero in loro assenza.
Svolgono dunque un ruolo vitale per la vita sulla terra, che non sarebbe possibile così come la
conosciamo oggi in un pianeta integralemente coperto da ghiacci perenni.
</p>
</div>

Le figura seguente da una idea del ruolo dei differenti gas serra, e nell'ultimo riquadro del
loro effetto totale, nell'assorbimento dell'energia infrarossa emessa dalla terra.

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
Le prime misurazioni della quantità di calore assorbita dai vari gas serra risalgono agli
esperimenti di laboratorio condotti dal fisico inglese John Tyndall nel 1859.
Tyndall concluse correttamente che la parte principale dell'effetto serra è provocato dal vapore
acqueo a causa della sua relativa alta concentrazione nell'atmosfera.
I suoi esperimenti mostrarono anche che il diossido di carbonio è un altro importante gas ad
effetto serra ed egli arrivò anche a provare un'altra importante conclusione:
senza gas ad effetto serra le temperature notturne terrestri sarebbere inferiori a quanto misuriamo.
Questi risultati furono riaffermati sperimentalmente dal chimico e fisico svedese Svante Arrhenius
verso la fine degli anni 1890.
Arrhenius calcolò anche che un raddoppio della quantità di anidride carbonica nell'atmosfera
avrebbe causato un <i>incremento di temperatura</i> da 5 a 6 gradi centigradi.
Una stima che è più elevata di quella
<a href="https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2019RG000678">attuale</a>
(da 2.6 a 4.1°C), ma che gli ha comunque valso il titolo di
"<i>padre dei cambiamenti climatici</i>".
</p>
</div>

#### Riscaldamento globale

La temperatura degli oceani e della superficie terrestre è determinata dall'interazione 
(bilancio) tra il flusso di energia proveniente dal sole e quello irraggiato della terra verso
lo spazio.

L'attività umana, caratterizzata dal rilascio nell'atmosfera di quantità sempre crescenti di
$$CO_2$$ (ormai dell'ordine dei miliardi di tonnellate all'anno) e di metano, derivanti
dall'utilizzo su larga scala dei *combustibili fossili*, ha portato nei circa 250 anni trascorsi
dall'inizio della rivoluzione industriale ad un aumento significativo della quantità di energia
intrappolata nella troposfera dall'effetto serra.
E dunque ad un incremento della sua temperatura media di quasi
[1.2°C]({% post_url 2021-01-01-global-warming-lets-quantify %}) rispetto al periodo 1850-1900
(la cui temperatura media si considera pressochè assimilabile a quella del periodo
pre-industriale) o di [1°C](https://climate.nasa.gov/vital-signs/global-temperature/) rispetto ai
valori del 1951-1980:

<div pb-2>
<img src="/assets/images/blog-nasa-global-temp.png"
     class="mx-auto d-block img-fluid">
<p class="text-center">
<small>
Andamento della temperatura terrestre &mdash;
<a href="https://climate.nasa.gov/vital-signs/global-temperature/"><small>NASA</small></a>
</small>
</p>
</div>

Incidentalmente, il rafforzamento dell'effetto serra provoca anche un abbassamento della
temperatura nelle zone alte dell'atmosfera terrestre, a causa della diminuzione del flusso di
fotoni emessi dalla terra che riescono a raggiungerla.
Anche questo fenomeno è stato verificato da misurazioni sperimentali satellitari cominciate nei
primi anni '80 del secolo scorso.

Lo squilibrio termico attuale è
[stimato](https://www.pnas.org/content/116/30/14881) a 0,5 W/$$m^2$$ (watt al metro
quadrato), ben superiore al valore di 0,2 W/$$m^2$$ che si è mantenuto più o meno costante
dall'ultima glaciazione ed ha permesso all'umanità di diventare stanziale e sostentarsi con una
agricoltura su larga scala, resa possibile dalla sostanziale stabilità del clima degli ultimi
10000 anni. Ed alla fine di costruire la società globalizzata ed articolata che conosciamo.

<div class="bd-callout bd-callout-info">
<p>
Oppure nella versione alternativa, descritta da James C. Scott nel suo libro
"<i>Against the Grain &mdash; A deep history of the earliest states</i>",
di abbandonare una vita di caccia e raccolta per una vita sedentaria in comunità
dipendenti dall'allevamento del bestiame e dei cereali, perdendo la sua libertà personale e
lavorativa. Costretto finanche a subire malattie imprevedibili causate dalla convivenza promiscua
di uomini ed animali addomesticati, in comunità sempre più affollate.
</p>
</div>

Questa fase di riscaldamento continuerà fino al raggiungimento di un nuovo equilibrio termico,
ad una temperatura media della troposfera superiore all'attuale ma non prevedibile, perchè
dipendente dalle emissioni *future* di gas ad effetto serra, oltre che da quelle
*cumulate fino ad ora* nell'atmosfera.
Il mondo sarà molto diverso da quello attuale, come leggiamo nel libro di Mark Lynas
"<i>Six Degrees: Our Future on a Hotter Planet</i>", nei cui sei capitoli che lo costituiscono,
uno per ogni grado di scostamento progressivo dalla temperatura del periodo pre-industriale, sono
descritti i gradi crescenti dell'impatto dei cambiamenti climatici sull'ambiente e le popolazioni,
per quanto ci è possibile scientificamente e ragionevolmente ipotizzare, al netto delle
conoscenze attuali.

<div class="bd-callout bd-callout-warning">
<h6>Breve nota su Covid-19 e Lockdown</h6>
<p>
La diminuzione delle emissioni di diossido di carbonio a seguito del periodo di lockdown
generalizzato sul pianeta <i>non ne hanno ridotto la concentrazione</i> nell'atmosfera, ma
solo rallentata temporaneamente la crescita. Il riscaldamento globale è causato dai gas ad effetto
serra <i>accumulatisi</i> nell'atmosfera (dall'inizio del periodo industriale o persino prima,
quando sono cominciati i grandi disboscamenti delle foreste europee).
Questo è un punto chiave che sfugge a molti.
</p>
</div>

I risultati scientifici, ottenuti soprattutto negli ultimi trenta anni di esplosiva ricerca nel
campo, ci mostrano come il clima terrestre sia un *sistema complesso*, costituito da molteplici
elementi strettamente correlati e mutualmente interconnessi tra loro, in equilibrio instabile,
almeno su una scala temporale di centinaia di migliaia di anni.
Un tempo praticamente infinito per noi umani.

Stiamo eseguendo su scala planetaria un esperimento di cui non sappiamo calcolare pienamente le
conseguenze, ma di cui la scienza ci indica in modo sempre più chiaro l'*estrema pericolosità*.
Non abbiamo un pianeta e neppure un ecosistema di riserva, dove migrare nel caso il risultato
fosse disastroso.
Affidarsi all'idea che la tecnologia del futuro saprà risolvere il problema è un rischio
insensato il cui prezzo maggiore sarà pagato da altri: le generazioni future.
