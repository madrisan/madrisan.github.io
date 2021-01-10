---
layout: post
category: climate-change
date: 2021-01-01
highcharts: off
image: /assets/images/blog-climate-changes-glacier.jpg
language: it
location: Nice
mathjax: 'on'
summary: A quanto viene stimato il riscaldamento globale attuale?
title: Misura del Riscaldamento Globale
titlejumbotron: 'off'
---
## Cambiamenti Climatici
### Misura del Riscaldamento Globale

Nel [post precedente]({% post_url 2020-12-29-climate-changes-physics %})
abbiamo definito come *cambiamento climatico* una modifica dei valori statistici del clima
terrestre, misurati su un periodo sufficientemente lungo da eliminare il rumore statistico
dato dalle fluttuazioni naturali del clima.

Sono disponibili numerose basi dati di misure delle temperature terrestri, ragionevolmente
complete, e fin dalla seconda metà del XIX secolo.

<div class="bd-callout bd-callout-info">
<p>
Con tecniche differenti, quali l'analisi della composizione chimica delle rocce o del ghiaccio
gli scienziati sono in grado di ricostruire le variazioni delle temperatura terrestre con un
sufficiente grado di accuratezza fino a periodi ben più remoti, coprendo centinaia di milioni
di anni.
</p>
</div>

Gli oceani sono il *serbatoio di energia dominante* nel sistema climatico terrestre, a cause della
loro grande capacità ad accumulare calore e la loro estensione sul pianeta.
Segue in importanza il calore latente associato all'aumento ed al declino delle calotte glaciali
continentali.

È quindi importante tenere in considerazione anche la temperatura oceanica, mediando i valori
ottenuti in un numero sufficiente grande di punti campione scelti a profondità differenti, dalla
superficie fino alla loro profondità media, di 4 Km.
E comparare i dati così ottenuti con quelli terrestri.

Le misurazioni risultanti vengono presentate come *anomalie* o scostamenti (positivi o
negativi) rispetto ai valori medi di un periodo scelto come riferimento.
I dati devono spesso essere corretti per cercare di annullare o almeno contenere cambiamenti nelle
tecniche o condizioni di misurazione delle temperature (soprattutto quelle oceaniche).

<div class="pb-2">
<img src="/assets/images/blog-monthly-surface-air-temperature-anomaly.png"
     class="mx-auto d-block img-fluid">
<p class="text-center"><small>
Anomalia delle temperature terrestri &mdash;
<a href="http://iridl.ldeo.columbia.edu/maproom/Global/Atm_Temp/Anomaly.html">
<small>IRI Climate Monitoring</small></a>
</small></p>
</div>

#### Base dati HadCRUT5

Il *Met Office Hadley Centre* (Had) in collaboratione con il *Climatic Research Unit* (CRU) dalla
University of East Anglia ha rilasciato a metà dicembre 2020 una
[nuova versione](https://www.metoffice.gov.uk/hadobs/hadcrut5/) della base dati *HadCRUT*, che
copre l'intero globo terrestre e contiene i dati mensili medi di ogni cella di controllo.
In particolare nella nuova versione sono stati effettuati migliori
[aggiustamenti](https://www.metoffice.gov.uk/hadobs/hadsst4/) ai valori delle temperature oceaniche
collezionati prima degli anni '70 del secolo scorso, sono stati utilizzati metodi statistici per
estendere i dati mancanti in regioni in rapido riscaldamento ma dove ancora oggi le misurazioni
sono scarse, quali la zona Artica, ed anche un utilizzo di nuovi dati derivanti dalla
digitalizzazione di valori storici (processo ancora in corso).

Il nuovo set di dati risulta consistente con altre collezioni di temperature eseguite in modo
indipendente, quali [GISTEMP](https://data.giss.nasa.gov/gistemp/),
[NOAAGlobalTemp](https://www.ncdc.noaa.gov/data-access/marineocean-data/noaa-global-surface-temperature-noaaglobaltemp),
[Berkeley Earth](http://berkeleyearth.org/) e [Reanalyses.org](https://reanalyses.org/).

<div class="pb-2">
<img src="https://www.metoffice.gov.uk/hadobs/hadcrut5/figures/HadCRUT5_figure_7.png"
     class="mx-auto d-block img-fluid">
<p class="text-center"><small>
Anomalie delle temperature nei vari dataset &mdash;
<a href="https://www.metoffice.gov.uk/hadobs/hadcrut5/">
<small>Met Office Hadley Centre</small></a>
</small></p>
</div>

La temperatura media globale negli anni 2010-2018 è
[stimata](https://www.metoffice.gov.uk/about-us/press-office/news/weather-and-climate/2020/hadcrut5-announcement)
ora a 1.07 ± 0.11°C superiore alla temperatura media del periodo 1850-1900
(che è generalmente, ma non universalmente, considerata
approssimabile a quella pre-industriale), con un incremento di 0.16°C rispetto alla versione
precedente dai dati.

Generalmente viene preso in considerazione il periodo 1961-1990 poichè nell'arco temporale
1850-1900 si sono verificati alcuni eventi vulcanici maggiori, tra cui in particolare:
 * Krakatoa (1883), che ha causato un *inverno vulcanico* di 5 anni (cioè una riduzione delle
   temperature globali causati dalla cenere vulcanica e dalle goccioline di acido solforico
   ed acqua proiettate nelle stratosfera che riflettono parte della radiazione solare verso
   lo spazio),
 * Mount Tarawera (1886), la più grande eruzione storicamente registrata in Nuova Zelanda.

L'ottimale sarebbe sarebbe usare come riferimento gli anni 1720-1800, ma purtroppo in questi
anni non esistono collezioni di dati di temperatura sufficienti a coprire l'intero pianeta.

<div class="bd-callout bd-callout-warning">
<p>
La stima del riscaldamento globale attuale che ne consegue è dunque di circa 1.2°C
(1.200410°C calcolata sul periodo 1850-1900, 0.841467 sul periodo 1961-1990).
Distribuita in modo non uniforme: maggiore nell'emisfero boreale e minore in quello australe,
crescente allontanandosi dall'equatore e superiore sulla terraferma rispetto agli oceani.
</p>
</div>

<div class="bd-callout bd-callout-info">
<p>
Il codice Python per effettuare il parsing dei dataset HadCRUT5 contenenti le temperature medie
annuali è liberamente (licenza GPL-3.0+) disponibile nel mio repository GitHub
<a href="https://github.com/madrisan/HadCRUT5/">
madrisan/HadCRUT5</a>. Il file
<a href="https://github.com/madrisan/HadCRUT5/blob/main/README.md">README</a> contiene le immagini
generabili dallo script.
</p>
</div>

<div class="pb-2">
<img src="https://github.com/madrisan/HadCRUT5/raw/main/plots/HadCRUT-1850-1900-smoother.png"
     class="mx-auto d-block img-fluid">
<p class="text-center"><small>
Anomalie delle temperature (medie su 5 anni) &mdash;
<a href="https://github.com/madrisan/HadCRUT5/">
<small>GitHub</small></a>
</small></p>
</div>
