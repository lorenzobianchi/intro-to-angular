# Introduzione allo sviluppo web con Angular

## Le basi di una pagina web

I principali linguaggi con cui vengono create le pagine web sono 3 ognuno dei quali ha uno scopo ben preciso:

* __HTML__ con questo linguaggio si definisce la __struttura__ (layout) di una pagina web attraverso lutilizzo di diversi __tag__ che rappresentano i diversi componenti di una pagina. La pagina ha una struttura che si divide in 2 parti: l'_header_ dove vengono definiti i [metatags](https://it.wikipedia.org/wiki/Meta_tag) e il _body_ dove viene definito il layout della pagina.
* __CSS__ (Cascading Style Sheets) è un linguaggio che serve a definire lo _style_ degli elementi di un documento HTML. Gli stili possono essere applicati globalmente su tutti gli elementi di una certa categoria oppure attraverso l'uso di classi o id applicati su tags HTML (<code>body, p, div, button, ul, li....</code>) nel documento HTML stesso.
* __javascript__ In informatica JavaScript è un linguaggio di scripting orientato agli oggetti e agli eventi, comunemente utilizzato nella programmazione Web lato client per la creazione, in siti web e applicazioni web, di effetti dinamici interattivi tramite funzioni di script invocate da eventi innescati a loro volta in vari modi dall'utente sulla pagina web in uso (mouse, tastiera, caricamento della pagina ecc...) (da [wikipedia](https://it.wikipedia.org/wiki/JavaScript)).  
Le pagine Web non sono l'unico posto in cui viene utilizzato JavaScript. Molti programmi desktop, server e alcuni database usano JavaScript come linguaggio di programmazione. Torneremo su questo argomento in modo più approfondito nei prossimi paragrafi.

Ecco un [esempio](http://embed.plnkr.co/hVwcOWilsbU0T2IjV6Da/) di come questi 3 linguaggi lavorano insieme  

## Come funziona internet

Ora parleremo in modo introduttivo di alcuni argomenti che riguardano il funzionamento del web e che, a mio avviso, è necessario sapere se si vuole intraprendere la professione del web developer nel 2019.  
Non serve imparare alla perfezione i dettagli tecnici, ma avere un'idea di come funzionana internet ci aiuta a prendere le giuste decisioni nello sviluppare web app, siti....

### __Browsers__

In informatica il web browser, traducibile come navigatore) è un'applicazione per l'acquisizione, la presentazione e la navigazione di risorse sul web. Tali risorse (come pagine web, immagini o video) sono messe a disposizione sul World Wide Web (la rete globale che si appoggia su Internet), su una rete locale o sullo stesso computer dove il browser è in esecuzione. Il programma implementa da un lato le funzionalità di client per il protocollo HTTP, che regola il download delle risorse dai server web a partire dal loro indirizzo URL; dall'altro quelle di visualizzazione dei contenuti ipertestuali (solitamente all'interno di documenti HTML) e di riproduzione di contenuti multimediali. (da [wikipedia](https://it.wikipedia.org/wiki/Browser))  

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

### __JSON & XML__

[JSON](https://it.wikipedia.org/wiki/JavaScript_Object_Notation) (_Javascript Object Notation_) e [XML](https://it.wikipedia.org/wiki/XML) (_Extended markup language_), sono degli standards di formattattazione pensati per lo scambio di informazioni/dati nel web.

### __Domain Name System__

In informatica e telecomunicazioni il sistema dei nomi di dominio (in inglese: _Domain Name System_, DNS), è un sistema utilizzato per la risoluzione di nomi dei nodi della rete (in inglese: host) in indirizzi IP. Il servizio è realizzato tramite un database distribuito, costituito dai server DNS. Il DNS ha una struttura gerarchica ad albero rovesciato ed è diviso in domini (com, org, it, ecc.). Ad ogni dominio o nodo corrisponde un nameserver, che conserva un database con le informazioni di alcuni domini di cui è responsabile e si rivolge ai nodi successivi quando deve trovare informazioni che appartengono ad altri domini.

Ogni nome di dominio termina con un “.” (punto). Ad esempio l'indirizzo wikipedia.org termina con il punto. La stringa vuota che segue il punto finale è chiamata dominio radice (DNS root zone). I server responsabili del dominio radice sono i cosiddetti root nameservers. Essi possiedono l'elenco dei server autoritativi di tutti i domini di primo livello (TLD) riconosciuti e lo forniscono in risposta a ciascuna richiesta. I root nameserver sono 13 in tutto il mondo, di cui 10 negli Stati Uniti, due in Europa (Inghilterra e Svezia) ed uno in Giappone.(da [wikipedia](https://it.wikipedia.org/wiki/Domain_Name_System))

## Git

![Git logo](./covers/git-logo.png)

Git è un software di controllo versione distribuito utilizzabile da interfaccia a riga di comando, creato dal grande Linus Torvalds nel 2005.
Qusto strumento nacque con lo scopo di facilitare lo sviluppo del kernel Linux ed è diventato uno degli strumenti di controllo versione più diffusi al mondo.
Imparare ad utilizzare questo strumento è fondamentale per sviluppare software al giorno d'oggi. Questo sistema di lavoro collabarativo consente di lavorare al codice aggiungendo le nuove modifiche man mano vengono fatte,se si sbaglia o per qualche altro motivo possiamo tornare indietro alle modifiche precedenti e correggere il codice. 
Git, tra le alre cose, consente di creare nuovi _branches_ (cloni del codice sorgente al momento della creazione) per sviluppare in parallelo versioni diverse partendo dalla stessa basa di codice. 
Le possibilità date da _git_ sonno davvero tante e danno ai developers uno strumento potentissimo che li aiuta a creare codice di qualità, mantenibile e scalabile.
Permettetemi di dire che git ci "salva la vita" quando siamo responsabili dello sviluppo del nostro codice, ci permette di correggere gli errori che spesso facciamo (come è normale che sia) e ci costringe ad avere un approccio al codice davvero intelligente. Quindi IMPARATELO! È a vostro esclusivo vantaggio.

### __Cos'è un VCS__

I _Version Control System_ (sistemi di controllo versione) sono una categoria di strumenti software che aiutano un team di software a gestire le modifiche al codice sorgente nel tempo. Il software di controllo della versione tiene traccia di ogni modifica al codice in un tipo speciale di database. Se viene commesso un errore, gli sviluppatori possono tornare indietro nel tempo e confrontare le versioni precedenti del codice per aiutare a correggere l'errore riducendo al minimo l'interruzione di tutti i membri del team (dalla [guida Bitbucket](https://it.atlassian.com/git/tutorials/what-is-version-control))

## Il successo di javascript negli ultimi anni

JavaScript è un linguaggio di scripting orientato agli oggetti e agli eventi, comunemente utilizzato nella programmazione Web lato client per la creazione, in siti web e applicazioni web, di effetti dinamici interattivi tramite funzioni di script invocate da eventi innescati a loro volta in vari modi dall'utente sulla pagina web in uso (mouse, tastiera, caricamento della pagina ecc...). ( da [wikipedia](https://it.wikipedia.org/wiki/JavaScript)).  

JS fu creato da [Brendan Eich](https://it.wikipedia.org/wiki/Brendan_Eich) per [Netscape](https://it.wikipedia.org/wiki/Netscape_Navigator) nel lontano 1995 e fu chiamato così perchè a quei tempi _Java_ era uno dei linguaggi più popolari.
Nel 1997 diventa per la prima volta uno __standard__ per opera della [ECMA](https://www.ecma-international.org/default.htm), un'associazione internazionale formata da [membri delle maggiori società del settore](https://www.ecma-international.org/memento/members.htm), che ha lo scopo di definire degli standards per il settore informatico.


## __[Node.js](https://nodejs.org/it/)__

![node icon](./covers/node.png)

### __Concetto di package__

### __npm__

## __installazione di node sulla tua macchina__


## Pwa e Angular

### __cosa sono le pwa__

### __introduzione ad angular__

### __angular cli__

### __installazione di angular cli__


## La tua prima app Angular

### __il tuo primo progetto Angular__

### __start the project__

### __aggiungiamo bootstrap al progetto__

### ___cos’è un framework css___

### __il tuo primo componente__

### __navab__

### __home page__

### __about page__

### __routing__


## Link e informazioni utili per continuare da soli
