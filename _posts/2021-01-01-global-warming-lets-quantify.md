---
layout: post
category: climate-change
date: 2021-01-01
e-ighcharts: off
image: /assets/images/blog-climate-changes-glacier.jpg
language: it
license: 'CC BY-SA 3.0'
location: Nice
mathjax: 'on'
post-title: Cambiamenti Climatici
summary: Sono disponibili numerose basi dati di misure delle temperature terrestri, ragionevolmente complete, e fin dalla seconda metà del XIX secolo. Il <i>Met Office Hadley Centre</i> in collaboratione con il <i>Climatic Research Unit</i> dalla University of East Anglia ha rilasciato a metà dicembre 2020 una nuova versione della base dati <i>HadCRUT</i>, che copre l'intero globo terrestre e contiene i dati mensili medi di ogni cella di controllo. In questo post visualizziamo questo dataset e calcoliamo una stima del riscaldamento globale attuale.
title: Misura del Riscaldamento Globale
titlejumbotron: 'off'
---
#### Misura del Riscaldamento Globale

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

<picture>
    <img src="/assets/images/blog-monthly-surface-air-temperature-anomaly.png"
         class="mx-auto d-block img-fluid pt-3">
</picture>
<p class="text-center pt-3 pb-3">
    <small>
       Anomalia delle temperature terrestri &mdash;
       <a href="http://iridl.ldeo.columbia.edu/maproom/Global/Atm_Temp/Anomaly.html">
          <small>IRI Climate Monitoring</small></a>
    </small>
</p>

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

<picture>
    <img src="https://www.metoffice.gov.uk/hadobs/hadcrut5/figures/HadCRUT5_figure_7.png"
         class="mx-auto d-block img-fluid">
</picture>
<p class="text-center pb-2">
    <small>
        Anomalie delle temperature nei vari dataset &mdash;
        <a href="https://www.metoffice.gov.uk/hadobs/hadcrut5/">
           <small>Met Office Hadley Centre</small></a>
    </small>
</p>

La temperatura media globale negli anni 2010-2018 è
[stimata](https://www.metoffice.gov.uk/about-us/press-office/news/weather-and-climate/2020/hadcrut5-announcement)
ora a 1.07 ± 0.11°C superiore alla temperatura media del periodo 1850-1900
(che è generalmente, ma non universalmente considerata approssimabile a quella pre-industriale),
con un incremento di 0.16°C rispetto alla versione precedente dei dati.

Generalmente viene preso in considerazione il periodo 1961-1990 poichè nell'arco temporale
1850-1900 si sono verificati alcuni eventi vulcanici maggiori, tra cui in particolare:
 * Krakatoa (1883), che ha causato un *inverno vulcanico* di 5 anni (cioè una riduzione delle
   temperature globali causati dalla cenere vulcanica e dalle goccioline di acido solforico
   ed acqua proiettate nelle stratosfera che riflettono parte della radiazione solare verso
   lo spazio),
 * Mount Tarawera (1886), la più grande eruzione storicamente registrata in Nuova Zelanda.

Alternativamente viene preso come base di riferimento il periodo 1880-1920,
con l'ipotesi che il limitato riscaldamento causato dai gas ad effetto serra emessi fino a
questo periodo sia compensato dall'alta attività vulcanica di cui si è accennato.

<div class="bd-callout bd-callout-warning">
<p>
La stima del riscaldamento globale attuale che ne consegue è dunque di circa 1.3°C
(1.29°C calcolata sul periodo 1850-1900,
 1.32°C sul periodo 1880-1920, e di
 0.93°C relativamente al 1961-1990).
Distribuita in modo non uniforme: maggiore nell'emisfero boreale e minore in quello australe,
crescente allontanandosi dall'equatore e superiore sulla terraferma rispetto agli oceani.
</p>
</div>

<picture>
    <img src="https://github.com/madrisan/HadCRUT5/raw/main/plots/HadCRUT5-global-1880-1920.png"
         alt="Global average temperature difference 1850-2020"
         class="mx-auto d-block img-fluid pt-3 pb-2">
</picture>
<p class="text-center pb-2">
    <small>
        Anomalie delle temperature rispetto al periodo 1850-2020 &mdash;
        <a href="ihttps://github.com/madrisan/HadCRUT5/">
           <small>GitHub</small></a>
    </small>
</p>

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

<picture>
    <img src="https://github.com/madrisan/HadCRUT5/raw/main/plots/HadCRUT5-1880-1920-smoother.png"
         alt="HadCRUT5 1880-1920 based with 5-years averages"
         class="mx-auto d-block img-fluid">
</picture>
<p class="text-center">
    <small>
        Anomalie delle temperature (medie su 5 anni) &mdash;
        <a href="https://github.com/madrisan/HadCRUT5/">
           <small>GitHub</small></a>
    </small>
</p>
