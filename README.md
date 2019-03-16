# Introduzione allo sviluppo web con Angular

## Le basi di una pagina web
I principali linguaggi con cui vengono create le pagine web sono 3 ognuno dei quali ha uno scopo ben preciso: 
* __HTML__ con questo linguaggio si definisce la __struttura__ (layout) di una pagina web attraverso lutilizzo di diversi __tag__ che rappresentano i diversi componenti di una pagina. La pagina ha una struttura che si divide in 2 parti: l'_header_ dove vengono definiti i [metatags](https://it.wikipedia.org/wiki/Meta_tag) e il _body_ dove viene definito il layout della pagina.
* __CSS__ (Cascading Style Sheets) è un linguaggio che serve a definire lo _style_ degli elementi di un documento HTML. Gli stili possono essere applicati globalmente su tutti gli elementi di una certa categoria oppure attraverso l'uso di classi o id applicati su tags HTML (<code>body, p, div, button, ul, li....</code>) nel documento HTML stesso.
* __javascript__ In informatica JavaScript è un linguaggio di scripting orientato agli oggetti e agli eventi, comunemente utilizzato nella programmazione Web lato client per la creazione, in siti web e applicazioni web, di effetti dinamici interattivi tramite funzioni di script invocate da eventi innescati a loro volta in vari modi dall'utente sulla pagina web in uso (mouse, tastiera, caricamento della pagina ecc...) [wikipedia](https://it.wikipedia.org/wiki/JavaScript). Torneremo su questo argomento in modo più approfondito nei prossimi paragrafi.


## Come funziona internet
Ora parleremo in modo introduttivo di alcuni argomenti che riguardano il funzionamento del web e che, a mio avviso, è necessario sapere se si vuole intraprendere la professione del web developer nel 2019.  
Non serve imparare alla perfezione i dettagli tecnici, ma avere un'idea di come funzionana internet ci aiuta a prendere le giuste decisioni nello sviluppare web app, siti....

### __Browsers__
In informatica il web browser, traducibile come navigatore) è un'applicazione per l'acquisizione, la presentazione e la navigazione di risorse sul web. Tali risorse (come pagine web, immagini o video) sono messe a disposizione sul World Wide Web (la rete globale che si appoggia su Internet), su una rete locale o sullo stesso computer dove il browser è in esecuzione. Il programma implementa da un lato le funzionalità di client per il protocollo HTTP, che regola il download delle risorse dai server web a partire dal loro indirizzo URL; dall'altro quelle di visualizzazione dei contenuti ipertestuali (solitamente all'interno di documenti HTML) e di riproduzione di contenuti multimediali. [wikipedia](https://it.wikipedia.org/wiki/Browser)  

In pratica un browser Web o browser è un programma che recupera e visualizza pagine dal Web e consente agli utenti di accedere a ulteriori pagine tramite l'utilizzo di _hyperlinks_.
I broweser più utilizzati sono:
* [Google Chrome](https://www.google.com/chrome/) 
* [Internet Explorer](https://it.wikipedia.org/wiki/Internet_Explorer)
* [Mozilla Firefox](https://www.mozilla.org/it/firefox/new/)
* [Microsoft Edge](https://it.wikipedia.org/wiki/Microsoft_Edge)
* [Safari](https://www.apple.com/it/safari/)
* [Opera](https://www.opera.com/it)

### __http__
L'_HyperText Transfer Protocol_ (HTTP) (protocollo di trasferimento di un ipertesto) è un protocollo utilizzato come principale sistema per la trasmissione d'informazioni sul web. L'architettura tipicamente impiegata è quella _client-server_ in cui il client invia un messaggio di richiesta al serve al sever che risponde inviando file HTML, dati estratti da un database o altri contenuti.

### JSON & XML


### Domain Name System
In informatica e telecomunicazioni il sistema dei nomi di dominio (in inglese: _Domain Name System_, DNS), è un sistema utilizzato per la risoluzione di nomi dei nodi della rete (in inglese: host) in indirizzi IP. Il servizio è realizzato tramite un database distribuito, costituito dai server DNS. Il DNS ha una struttura gerarchica ad albero rovesciato ed è diviso in domini (com, org, it, ecc.). Ad ogni dominio o nodo corrisponde un nameserver, che conserva un database con le informazioni di alcuni domini di cui è responsabile e si rivolge ai nodi successivi quando deve trovare informazioni che appartengono ad altri domini.

Ogni nome di dominio termina con un “.” (punto). Ad esempio l'indirizzo wikipedia.org termina con il punto. La stringa vuota che segue il punto finale è chiamata dominio radice (DNS root zone). I server responsabili del dominio radice sono i cosiddetti root nameservers. Essi possiedono l'elenco dei server autoritativi di tutti i domini di primo livello (TLD) riconosciuti e lo forniscono in risposta a ciascuna richiesta. I root nameserver sono 13 in tutto il mondo, di cui 10 negli Stati Uniti, due in Europa (Inghilterra e Svezia) ed uno in Giappone.[wikipedia](https://it.wikipedia.org/wiki/Domain_Name_System)

## Git

### __Cos'è un VCS__