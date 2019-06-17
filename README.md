# Introduzione allo sviluppo web con Angular  
Per poter utilizzare in modo efficace Angular, un moderno framework di Google per lo sviluppo di applicazioni Web, abbiamo bisogno di avere alcune conoscenze sullo sviluppo web in generale.

## Le basi di una pagina web

I principali linguaggi con cui vengono create le pagine web sono 3 ognuno dei quali ha uno scopo ben preciso:

* __HTML__ (_HyperText Markup Language_) con questo linguaggio si definisce la __struttura__ (layout) di una pagina web attraverso lutilizzo di diversi __tag__ che rappresentano i diversi componenti di una pagina. La pagina ha una struttura che si divide in 2 parti: l'_header_ dove vengono definiti i [metatags](https://it.wikipedia.org/wiki/Meta_tag) e il _body_ dove viene definito il layout della pagina.  
Quindi cos'è esattamente l'HTML? HTML fornisce una struttura al contenuto (immagini, testo o video) che appare su un sito Web. Se provi a far clic con tasto destro su qualsiasi pagina Internet e selezioni "Ispeziona" oppure "Visualizza sorgente pagina", vedrai il codice HTML della pagina che stai visualizzando.  
Imparare l'HTML è sicuramente il primo passo da fare per poter realizzare siti web e applicazioni.
* __CSS__ (Cascading Style Sheets) è un linguaggio che serve a definire lo _style_ degli elementi di un documento HTML. Gli stili possono essere applicati globalmente su tutti gli elementi di una certa categoria oppure attraverso l'uso di classi o id applicati su tags HTML (<code>body, p, div, button, ul, li....</code>) nel documento HTML stesso.
* __javascript__ In informatica JavaScript è un linguaggio di scripting orientato agli oggetti e agli eventi, comunemente utilizzato nella programmazione Web lato client per la creazione, in siti web e applicazioni web, di effetti dinamici interattivi tramite funzioni di script invocate da eventi innescati a loro volta in vari modi dall'utente sulla pagina web in uso (mouse, tastiera, caricamento della pagina ecc...) (da [wikipedia](https://it.wikipedia.org/wiki/JavaScript)).  
Le pagine Web non sono l'unico posto in cui viene utilizzato JavaScript. Molti programmi desktop, server e alcuni database usano JavaScript come linguaggio di programmazione. Torneremo su questo argomento in modo più approfondito nei prossimi paragrafi.

Ecco un [esempio](http://embed.plnkr.co/hVwcOWilsbU0T2IjV6Da/) di come questi 3 linguaggi lavorano insieme.  
Prima di passare a cose più avanzate ti consiglio di prendere familiarità con questi 3 pilastri dello sviluppo web.  

## Come funziona internet 🤔

Ora parleremo in modo introduttivo di alcuni argomenti che riguardano il funzionamento del web e che, a mio avviso, è necessario sapere se si vuole intraprendere la professione del web developer nel 2019.  
Non serve imparare alla perfezione i dettagli tecnici, ma avere un'idea di come funzionana internet ci aiuta a prendere le giuste decisioni nello sviluppare web app, siti....

### __Browsers__

In informatica il web browser (traducibile come _navigatore_) è un'applicazione per l'acquisizione, la presentazione e la navigazione di risorse sul web. Tali risorse (come pagine web, immagini o video) sono messe a disposizione sul World Wide Web (la rete globale che si appoggia su Internet), su una rete locale o sullo stesso computer dove il browser è in esecuzione. Il programma implementa da un lato le funzionalità di client per il protocollo HTTP, che regola il download delle risorse dai server web a partire dal loro indirizzo URL; dall'altro quelle di visualizzazione dei contenuti ipertestuali (solitamente all'interno di documenti HTML) e di riproduzione di contenuti multimediali. (da [wikipedia](https://it.wikipedia.org/wiki/Browser))  

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

Git è un software di controllo versione distribuito utilizzabile da interfaccia a riga di comando, creato dal grande [Linus Torvalds](https://it.wikipedia.org/wiki/Linus_Torvalds) nel 2005.
Questo strumento nacque con lo scopo di facilitare lo sviluppo del [kernel Linux](https://it.wikipedia.org/wiki/Linux_(kernel)) ed è diventato uno degli strumenti di controllo versione più diffusi al mondo.
Imparare ad utilizzare questo strumento è fondamentale per sviluppare software al giorno d'oggi. Questo sistema di lavoro collabarativo consente di lavorare al codice aggiungendo le nuove modifiche man mano vengono fatte. Se si sbaglia o se per qualche altro motivo ne abbiamo la necessità, possiamo tornare indietro alle modifiche precedenti e correggere il codice.  
Git, tra le alre cose, consente di creare nuovi _branches_ (cloni del codice sorgente al momento della creazione) per sviluppare in parallelo versioni diverse partendo dalla stessa basa di codice.  
Le possibilità date da _git_ sonno davvero tante e danno ai developers uno strumento potentissimo che li aiuta a creare codice di qualità, mantenibile e scalabile.
Permettetemi di dire che git ci "salva la vita" quando siamo responsabili dello sviluppo del nostro codice, ci permette di correggere gli errori che spesso facciamo (come è normale che sia) e ci costringe ad avere un approccio al codice davvero intelligente. Quindi IMPARATELO! È a vostro esclusivo vantaggio.

### __Cos'è un VCS__

I _Version Control System_ (sistemi di controllo versione) sono una categoria di strumenti software che aiutano un team di software a gestire le modifiche al codice sorgente nel tempo. Il software di controllo della versione tiene traccia di ogni modifica al codice in un tipo speciale di database. Se viene commesso un errore, gli sviluppatori possono tornare indietro nel tempo e confrontare le versioni precedenti del codice per aiutare a correggere l'errore riducendo al minimo l'interruzione di tutti i membri del team.  
(tradotto dalla [guida Bitbucket](https://it.atlassian.com/git/tutorials/what-is-version-control))

## Il successo di javascript negli ultimi anni

![JS icon](./covers/JS.png)

JavaScript è un linguaggio di scripting orientato agli oggetti e agli eventi, comunemente utilizzato nella programmazione Web lato client per la creazione, in siti web e applicazioni web, di effetti dinamici interattivi tramite funzioni di script invocate da eventi innescati a loro volta in vari modi dall'utente sulla pagina web in uso (mouse, tastiera, caricamento della pagina ecc...). ( da [wikipedia](https://it.wikipedia.org/wiki/JavaScript)).  

JS fu creato da [Brendan Eich](https://it.wikipedia.org/wiki/Brendan_Eich) per [Netscape](https://it.wikipedia.org/wiki/Netscape_Navigator) nel lontano 1995 e fu chiamato così perchè a quei tempi _Java_ era uno dei linguaggi più popolari.
Nel 1997 diventa per la prima volta uno __standard__ per opera della [ECMA](https://www.ecma-international.org/default.htm), un'associazione internazionale formata da [membri delle maggiori società del settore](https://www.ecma-international.org/memento/members.htm), che ha lo scopo di definire degli standards per il settore informatico.  
Per avere una buona introduzione e capire cos'è questo linguaggio e iniziare a capire quali grandi potenzialità ha JS potete leggere [questo articolo](https://developer.mozilla.org/it/docs/Learn/Getting_started_with_the_web/JavaScript_basics) su [MDN](https://developer.mozilla.org/it/) un sito dove troverete documentazione aggiornata su Javascript e sullo sviluppo web in generale.

Negli ultimi anni lo standard JS definito negli [ECMAScripts](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Language_Resources) è stato rilasciato più di frequente, indice del successo che Javascript sta risquotendo negli ultimi anni.

| Versione       | Anno di rilascio |
| -------------- |:----------------:|
| ECMAScript 1   | 1997             |
| ECMAScript 2   | 1998             |
| ECMAScript 3   | 1999             |
| ECMAScript 4   | Abbandonata      |
| ECMAScript 5   | 2009             |
| ECMAScript 5.1 | 2011             |
| ECMAScript 6   | 2015             |
| ECMAScript 7   | 2016             |
| ECMAScript 8   | 2017             |

Nei ultimi anni (dal 2009), JS è impiegato anche al di fuori del contesto dei browsers ed è utilizzato per la gestione di server, database, applicazioni desktop e mobile, internet of things e altro ancora. 

Inoltre Javascript è anche conosciuto per essere "_The Most Misunderstood Programming Language_"  😂 come ci dice _Douglas Crockford_ in un [articolo del suo blog](https://crockford.com/javascript/javascript.html) intitolato proprio così. Questo per motivi come il nome che ricorda Java, con cui ha qualche similitudine nella sinstassi, ma che è un liguaggio completamente diverso, per alcuni comportamenti "bizzarri" di Javascript che generano confusione nei programmatori, soprattutto i meno espereti e per altri motivi ancora. A tal proposito vi segnalo questo fantastico repository: [wtfjs](https://github.com/denysdovhan/wtfjs) dove potete trovare un sacco di esempi di molti comportamenti "poco logici" di JS con la rispettiva spiegazione.

## __[Node.js](https://nodejs.org/it/)__

![node icon](./covers/node.png)

Uno dei pricipali motici del successo di Javascript negli ultimi anni è proprio __Node.js__.

Node.js è una piattaforma Open source event-driven per l'esecuzione di codice JavaScript Server-side, costruita sul motore JavaScript [V8](https://v8.dev/) di Google Chrome. Molti dei suoi moduli base sono scritti in JavaScript, e gli sviluppatori possono scrivere nuovi moduli in JavaScript.  
 In origine JavaScript veniva utilizzato principalmente lato client. In questo scenario gli script JavaScript, generalmente incorporati all'interno dell'HTML di una pagina web, vengono interpretati da un motore di esecuzione incorporato direttamente all'interno di un Browser. Node.js consente invece di utilizzare JavaScript anche per scrivere codice da eseguire lato server, ad esempio per la produzione del contenuto delle pagine web dinamiche prima che la pagina venga inviata al Browser dell'utente. Node.js in questo modo permette di implementare il cosiddetto paradigma "JavaScript everywhere" (Javascript ovunque), unificando lo sviluppo di applicazioni Web intorno ad un unico linguaggio di programmazione : __JavaScript__.  
(da [wikipedia](https://it.wikipedia.org/wiki/Node.js))

### __Concetto di modulo e di package 📦__

I moduli in Node.js non sono molto diversi dai _packages_ di Java o di Python per esempio. Se non li conosci, non ti preoccupare. I moduli sono semplici file JavaScript che contengono del codice per uno scopo specifico. Il pattern dei moduli è pensato per rendere più facile il lavoro del programmatore, dandogli modo di usare codice implemetato da altri. Questo ci fa risparmiare tempo e ci aiuta a sviluppare codice di qualità senza doverci "_re-inventare la ruota_" ogni volta. Esistono due tipi di moduli in Node.js:

* __Core Modules__: sono quelli che vengono precompilati con la libreria Node.js. Lo scopo dei core modules è quello di fornire agli sviluppatori funzionalità spesso ricorrenti (HTTP, URL, EVENTS, FILE SYSTEM..) che, se non fossero disponibili, comporterebbero un compito noioso per gli sviluppatori perché dovrebbero riscriverle ogni volta.
* __User Defined Modules__: questi moduli, definiti dagli utenti, sono quelli che vengono sviluppati per uno scopo specifico e sono necessari quando i _core modules_ non sono in grado di soddisfare la funzionalità desiderata.

Un package può essere un modulo o contenere più node's modules. Questi pacchetti vengono gestiti con __npm__ e nei prossimi paragrafi ne parleremo in modo più approfondito.

### __npm__

![npm icon](./covers/npm.png)

NPM è uno strumento pensato per la gestione e la condivisione di pacchetti javascipt e, come dice la [documentazione ufficiale](https://docs.npmjs.com/about-npm/), si divide in 3 principali entità:

* __website__ che serve per scoprire i packages, leggere la documentazione e, in caso si vogliano pubblicare dai pacchetti, gestire le impostazioni del proprio package;
* __Command Line Interface (CLI)__ che viene eseguito da un terminale ed è il modo in cui la maggior parte degli sviluppatori interagisce con npm;
* __registry__ un grande database che racchiude tutti i software javascript pubblicati su npm e da dove è possibile scaricarli,

## __Installazione di node sulla tua macchina 💻__

Dopo averti annoiato con la teoria è ora di iniziare un po di pratica  💪😃🎉.
Vai sul [sito ufficiale di node](https://nodejs.org/it/) e scarica l'ultima versione stabile (nel momento in cui scrivo è la 10.15.3) per il tuo sistema operativo (macOS, Windows, Linux).
Come puoi vedere ci viene proposta l'ultima versione stabile e la versione con le ultime features.
Segui la guida (se hai problemi cerca su Google è pieno di articoli e tutorial) e completa l'installazione di node.

## Pwa e Angular

![angular logo](./covers/angular.png)  

Progressive Web App (PWA, in italiano applicazioni web progressive) è un termine, coniato in origine da Google, che si riferisce ad applicazioni web che vengono sviluppate e caricate come normali pagine web, ma che si comportano in modo simile alle applicazioni native quando utilizzate su un dispositivo mobile. Diversamente dalle applicazioni tradizionali, le progressive web apps sono un ibrido tra le normali pagine web (o siti web) e le applicazioni mobili. Questo modello di applicazioni cerca di combinare le possibilità offerte dalla maggior parte dei moderni browser con i benefici dell'utilizzo in mobilità.  
Il termine Progressive si riferisce al fatto che, dal punto di vista dell'esperienza utente (UX), queste applicazioni possono abilitare una serie di funzionalità aggiuntive alle normali pagine web a seconda delle funzionalità offerte dal dispositivo (da [wikipedia](https://it.wikipedia.org/wiki/Progressive_Web_App)).

Esistono diversi frameworks e librerie per sviluppare App e Web App al giorno d'oggi tra queste ricordiamo:

* [Angular](https://angular.io/)
* [React.js](https://reactjs.org/)
* [Vue.js](https://vuejs.org/)
* [Ember.js](https://emberjs.com/)
* [Preact.js](https://preactjs.com/)
* e molti altri...

Se siete curiosi di sapere quanto e come vengono utilizzati queste fantastiche tecnologie, date un'occhiata a [The State of JavaScript 2018](https://2018.stateofjs.com/), una fotografia del mondo di javascript moderno in una spendida web app, sviluppata con React e Gatsby, che di sicuro potrà ispirarvi.

In questo corso, come dice il titolo, abbiamo deciso di usare Angular, un framework sviluppato e mantenuto da Google e che è uno degli strumenti tra i più usati e richiesti nell'ambito dello sviluppo web moderno.  

[Qui](https://stackblitz.com/edit/angular-qxsypd) è possibile trovare un esempio di un'app Angular.

### __Introduzione ad angular__

__Cos'è Angular?__  
Angular è un framework Javascript per creare app web interattive. È progettato per piattaforme Web, desktop e mobile. Per creare un app con Angular utilizzamo HTML, CSS e Javascript. Anzi non utilizziamo direttamente javascript, ma Typescript (un superset tipizzato di Javascript scalabile), una specie di versione più severa di Javascript fornita di funzionalità di aggiuntive. Il codice Typescript viene successivamente compilato in javascript così da poter essere eseguito nei browsers.

__Angualr CLI__  
Così come node, anche Angular viene fornito con una _Command Line Interface_ o CLI, uno strumento che ci consente di lanciare comandi da un terminale. Questi comandi ci consentono di creare nuove applicazioni, creare componenti, moduli e services, eseguire localmente la nosta app e moltissime altre cose.

## __Installazione dell'Angular cli  💻__

Il CLI di Angualr deve essere installato a livello globale sulla tua macchina in modo da poterlo usare da qualsiasi parte del filesystem.  
Per installare il CLI di Angular usando npm, apri una finestra del terminale/console e lancia il seguente comando:

`npm install -g @angular/cli`

Fatto, ora siamo pronti per fare bootstrap della nosta prima app Angular 🎊!

## La tua prima app Angular 🚀

La app Angular vengono sviluppare nel contesto di un'_Angular workspace_, che sarebbe una _directory_ (cartella) che contiene i files per uno o più progetti.  
Per creare un nuovo workspace e un app iniziale dobbiamo lanciare il comando "__ng new__" seguito dal nome che vogliamo dare al progetto/app:

`ng new my-angular-app`

Dopo aver lanciato questo comando ci vengono chieste alcune cose come:  

* il linguaggio di styling che vogliamo utilizzare => selezioniamo CSS
* se vogliamo che la nostra app abbia il routing => diciamo di si

Inoltre il CLI di Angular si occupa di installare i pacchetti npm necessari e alcune altre dipendenze (questo processo può durare qualche minuto a seconda della macchina che utilizziamo).
In pratica verranno creati:

* un nuovo workspace con una cartella root chiamata col nome che abbiamo deciso
* un boilerplate iniziale della nostra app nella sotto-directory __src__ che contiene una semplice app di benvenuto, pronta per essere eseguita,
* un progetto di test end-to-end (nella sottocartella __e2e__)
* i file di configurazione correlati

(dalla [doc ufficiale di Angular](https://angular.io/guide/quickstart))

### __Start the project__

Angular include un web server, quindi possiamo facilmente eseguire una _build_ e servire la nostra app in locale sul nostro pc. Per far questo dobbiamo utilizzare un terminale su mac oppure su windows possiamo utilizzare la _Windows Command Prompt_, o la _Powershell_ ma io consiglio di installare anche la Git bash, puoi trovarla [qui](https://git-scm.com/downloads).  
Inoltre utilizzeremo alcuni comandi unix per muoverci nel filesystem da terminale.  

1- Entra nella directory del tuo workspace  

`cd my-angular-app`

2- Fai partire il web server eseguendo il comando "__ng serve__" con l'opzione "__--open__" per aprire direttamente la pagina nel browser del tuo computer.  

`ng serve --open`

Il comando `ng serve` fa partire il server e tiene sotto controllo (in inglese _watches your files_) i tuoi files. Se vengono eseguite modifiche al codice mentre il server sta "girando" e si salva, viene eseguiuta una nuova build con codice aggionarto. In pratica l'app riparte aggiornandosi all'ultimo codice salvato.  
L'opzione `--open` (che si può lanciare anche con la shortcut `--o`) fa aprire una finestra del tuo browser su [http://localhost:4200/](http://localhost:4200/).  

(anche questo tradotto dalla [doc ufficiale di Angular](https://angular.io/guide/quickstart))

Fantastico! Se è andato tutto secondo i piani la tua prima app Angular è in eseguzione su [http://localhost:4200/](http://localhost:4200/) 🎉🎉🎉✌️😺!!!

La web app servita su [http://localhost:4200/](http://localhost:4200/) è solo un _boilerplate_, un punto di partenza per iniziare a creare la tua app personalizzata. Ora puoi creare le tue pagine e i tuoi componenti per strutturare la tua app come vuoi.  

Apri la cartella dove hai creato la tua app nel tuo __editor di testo__ preferito, io personalmete uso [Visual Studio Code](https://code.visualstudio.com/) a mio avviso uno strumento di lavoro fantastico e di cui si parla anche [qui](https://angular.io/guide/language-service#visual-studio-code), nella doc ufficiale di Angular, ma usa l'editor che vuoi, ce ne sono molti validi ([Atom](https://atom.io/), [Sublime Text ](https://www.sublimetext.com/), [Vim](https://www.vim.org/), [Brackets](http://brackets.io/)...) e troverai una struttura del genere:

> ├── e2e  
> │   ├── protractor.conf.js  
> │   ├── src  
> │   │   ├── app.e2e-spec.ts  
> │   │   └── app.po.ts  
> │   └── tsconfig.e2e.json  
> ├── node_modules  
> │   ├── .........  
> ├── src  
> │   ├── app  
> │   │   ├── app-routing.module.ts  
> │   │   ├── app.component.html  
> │   │   ├── app.component.scss  
> │   │   ├── app.component.spec.ts  
> │   │   ├── app.component.ts  
> │   │   └── app.module.ts  
> │   ├── assets  
> │   ├── browserslist  
> │   ├── environments  
> │   │   ├── environment.prod.ts  
> │   │   └── environment.ts  
> │   ├── favicon.ico  
> │   ├── index.html  
> │   ├── karma.conf.js  
> │   ├── main.ts  
> │   ├── polyfills.ts  
> │   ├── styles.scss  
> │   ├── test.ts  
> │   ├── tsconfig.app.json  
> │   ├── tsconfig.spec.json  
> │   └── tslint.json  
> ├── .gitignore  
> ├── angular.json  
> ├── package-lock.json  
> ├── package.json  
> ├── README.md  
> ├── tsconfig.json  
> └── tslint.json  

😵😱 Ma è un sacco di roba! Come farò a capire qualcosa in mezzo a tutti questi files e cartelle?  
Non ti preoccupare, un pò alla volta imparerai. Per adesso iniziamo a dare un'occhiata al primo livello di files e cartelle che viene creato dal CLI di Angular quando lanciamo il comando `ng new`:

> * __e2e/__ => questa serve per i test end to end  
> * __node_modules/__ => moduli node, cioè dipendenze installate attraverso npm
> * __src/__  => IL CODICE VA QUI!!  
> __.gitignore__ => lista di files che devono essere ignorati da git  
> __angular.json__ => file di configurazione per angular  
> __package-lock.json__ => output delle dipendenze node e altro  
> __package.json__ => file di configurazione npm  
> __README.MD__ => descrizione testuale dell'app  
> __tsconfig.json__ => file di configurazione typescript  
> __tslint.json__ => configurazione del linter  

Per ora non preoccupiamoci di tutti questi files di configurazione e iniziamo a dire che il codice in un app Angular viene scritto all'interno della directory __src__. Apriamo questa cartella:

> * app/
> * assets/
> * environments/  
> browserslist  
> favicon.ico  
> index.html  
> karma.conf.js  
> main.ts  
> polyfills.ts
> styles.css  
> test.ts  
> tsconfig.app.json  
> tsconfig.spec.json  
> tslint.json  

e guardiamo il file __index.html__:  
![index.html image](./covers/index-html.png)  

Questo documento html è il punto di partenza della nosta app e il codice viene iniettato nel tag `<app-root></app-root>`.  

Il motivo per cui queste app vengono definite __SPA__ (_Single Page Application_) è proprio questo: al contrario di un sito web che tipicamente carica dal server più documenti html (`index.html, about.html, contacts.html` per esempio) in questo tipo di app ce n'è solo uno. Il codice necessario (`HTML`, `CSS` e `javascript`) viene ricompilato dinamicamente in base alle azioni dell'utente e ad altri fattori. Tutto ciò grazie a _Javascript_ e grazie alle `api` dei moderni Browsers.

Ora apriamo la cartella __app/__ e diamo un'occhiata al file __app.component.ts__:
![index.html image](./covers/app.component.ts.png)  

Questo è un file _Typescript_ dove viene definito un componente angular, per la precisione qui viene definito il __root__ component, cioè il componente alla base della struttura di _components_ di un app Angular. Il componente viene creato attraverso l'utilizzo del _decorator_ `@Component` che serve proprio per questo scopo. Se guardiamo il valore della chiave `selector` (che definisce il selettore html del componente) vediamo che è `app-root`, cioè lo stesso di `<app-root></app-root>` che c'è nel nostro __index.html__.  

Quindi le opzioni di questo _decorator_ `@Component` sono:

* `selector`: definisce il selector cioè il tag da usare per questo componente  
* `templateUrl`: è il path del file html dove viene definito il layout del componete, in questo caso _app.component.html_  
* `styleUrls`: array con i paths dei "_fogli di stile" del componente, in questo caso c'è _app.component.scss_

Infatti qui, in __app.component.html__ viene definito il layout del componente attraverso l'uso di tags html e di _directives_ angular che consentono di utilizzare typescript e di rendere dinamica la nostra app:
![snippet image](./covers/app.component.html.png)  

Mentre __app.component.scss__ (`scss` è che è un'evoluzione del css per dirla in un modo semplice) serve a definire lo stile del componente.  

### ___Cos’è un framework css___  

A proposito di stile, nei processi di sviluppo web moderni per uniformare lo stile ed avere una base di css più moderna vengono utilizzati i __frameworks CSS__.  

> Un framework CSS è un framework software progettato per consentire una progettazione Web più semplice e conforme agli standard utilizzando il linguaggio Cascading Style Sheets. La maggior parte di questi framework contiene almeno una griglia. I framework più funzionali sono inoltre dotati di più funzioni e funzioni aggiuntive basate su JavaScript, ma sono principalmente orientati al design.  
(https://en.wikipedia.org/wiki/CSS_framework)

### __Aggiungiamo bootstrap al progetto__

Per la nostra app ho scelto di usare [Bootstrap](https://getbootstrap.com/) il primo dei framerworks CSS creato per _Twitter_ da Mark Otto e Jacob Thornton per uniformare i componenti che componevano l'interfaccia web. Ancora oggi è uno dei framework più utilizzati nella sua catgorie e, nella mia esperienza, conoscerlo bene velocizza il processo produttivo in modo devastante.  

Quindi procediamo, aggiungiamo bootstrap come dipendenza della nostra app utilizzando __npm__. Vai sul terminale dove hai lanciato `ng serve --open` e premi `ctrl + c` per fermare il processo. Ora scrivi:  

`npm install bootstrap`  

Poi vai nel file __angular.json__ (al primo livello dell'app) e fai questa modifica:
![img snippet](./covers/bb.png)  


Ultimo passo vai in __src/styles.css__ e aggiungi:  
![img snippet](./covers/aa.png)  

Fatto abbiamo il css di bootstrap nella nosta app 😎👍!!

### __Il tuo primo componente__

In questa guida sto citando continuamete la parola "componente", ma che cos'è un componente in questo contesto? Un componente controlla una parte dell'interfaccia grafica, per esempio può essere una pagina oppure un footer o una lista. In pratica i componenti sono i "_blocchi_" con cui costruiamo la nostra app.  
Un componente detto _parent_ può essere costruito avendo al suo interno uno o più componenti _child_.
Come ho detto prima per implementare un componente dobbiamo utilizzare il _decorator_ `@Component` settando opzioni tipo `template`, `templateUrl`, `stylesUrls`, `selector` e tanti altri (se sei curioso guarda [qui](https://angular.io/api/core/Component)).  

Possiamo scrivere tutto a mano, oppure possiamo generare un componente utilizzare il potentissimo CLI di Angular. Genera la navbar della tua app, vai sul terminale e scrivi:

`ng g c navbar`  

Come vedi è stata generata una cartella `navbar` con 4 files:  

* navbar.component.scss  
* navbar.component.html  
* navbar.component.spec.ts  
* navbar.component.ts  

I files `.scss`, `.ts`, `.html` fuzionano esattamente come per `app.component`: abbiamo un controller (il file _.ts_) dove viene scritta la logica del componente, un template che è il file _.html_ dove viene definito il _layout_ del componente e infine abbiamo un foglio di stile dedicato al componente, cioè nel nostro caso il file _.scss_.  

Ho deciso di creare una `navbar` (conosciuta anche come `topbar`) come componente perchè è un componente __comune__ a tutte le pagine e quindi lo inserireremo in `app.component.html` in modo che sia sempre presente nella nostra app (vedi file `src/app/app.component.html`).  


Ora vai sulla _doc_ di _bootstrap_ a [questo link](https://getbootstrap.com/docs/4.3/components/navbar/#placement), copiati questo snippet di codice da cui potrai partire.
![code snippet](./covers/navbar.png)  

Perfetto ora incollalo in `navbar.component.html` al posto del contenuto che c'è ora e salva il file.  
Ti ho fatto andare nella pagina di doc di bootstrap perchè è quello che faccio io quando devo creare un componente basato sullo stile di bootstrap in Angular.  Come vedi la documentazione di bootstrap è molto dettagliata e si possono trovare una serie di componenti con i relativi esempi che possiamo usare come _boilerplate_ per il layout dei componenti della nostra app.  

## __Link utili per proseguire da soli__

Il pattern degli argomenti trattati in questo `README` è stato ispirato da [questo bellissimo repo](https://github.com/kamranahmedse/developer-roadmap) che vi consiglio di guardare e dove potrete trovare una vera e propria _road map_ degli argomenti da imparare per esercitare al meglio da professione del __web developer__.

__Link utili__:  

* [__Front-End Developer Handbook 2018__](https://frontendmasters.com/books/front-end-handbook/2018/) Written by Cody Lindley  
* [__gitconnected.com__](https://gitconnected.com/learn) Find Coding Tutorials & Courses  
* [__egghead__](https://egghead.io/) learn to code by awesome tutorials
