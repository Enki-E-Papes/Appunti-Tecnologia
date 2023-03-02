# ***Cos’è Javascript?***
Javascript è un linguaggio di programmazione che viene utilizzato soprattutto nella programmazione lato client in ambiente web (ovvero nella parte di presentazione): gli script possono essere utilizzati per arricchire le pagine “statiche” con effetti “dinamici”, per implementare funzionalità di controllo, modificare il contenuto di una pagina web, gestire eventi relativi agli elementi presenti in una pagina web e altro ancora. 
Inizialmente i produttori di browser hanno sviluppato delle versioni proprietarie di sistemi di scripting lato client; a partire dal 1997 si è creato uno standard (ECMAScript) e questo ha permesso di rendere gli script totalmente compatibili sui diversi tipi di browser.
Negli ultimi anni sono stati sviluppati diversi framework e librerie basati su questo linguaggio (a partire da jQuery, passando per KnockOut, fino alle tecnologie più utilizzate attualmente come Angular, Vue e React; attraverso Node.js è possibile utilizzare il linguaggio Javascript non soltanto a livello client, permettendo quindi di realizzare applicazioni web facendo uso di un unico linguaggio di programmazione). 

## Caratteristiche principali di Javascript

Tra le caratteristiche principali di Javascript (in seguito JS) vale la pena sottolineare queste:


   - è un linguaggio interpretato: il codice non viene compilato ma eseguito direttamente (dall’interprete del browser).

   - è un linguaggio orientato agli oggetti (anche se in modalità differente rispetto ad altri linguaggi come C++ o Java; sarebbe più corretto dire che è un linguaggio orientato ai prototipi: infatti in JS ogni istanza di un oggetto è una copia di una sorta di meta-oggetto definito prototipo da cui eredità le funzionalità).
    
   - è un linguaggio orientato agli eventi (permette di gestire gli eventi relativi agli elementi del DOM, ovvero della pagina web).

   - ha una sintassi abbastanza simile a quella di linguaggi come C++ o Java (sia come sintassi in senso stretto che come strutture di controllo e iterazione).

   - è un linguaggio non fortemente tipizzato: le variabili hanno tipi che possono cambiare durante l’esecuzione dello script (es: assegnamenti diversi) in maniera dinamica


## Dichiarazione di variabili e costanti
In JS è possibile dichiarare le variabili in due modi:
- utilizzando la parola chiave **var** 
- utilizzando la parola chiave **let**

Le costanti in JS sono di fatto delle variabili che devono essere inizializzate contestualmente alla dichiarazione e che non possono essere modificate nè ridichiarate. Le costanti vengono dichiarate utilizzando la parola chiave const.

Per capire la differenza tra le variabili dichiarate con var e quelle dichiarate con let o const occorre introdurre il concetto di scope (che in italiano potremmo tradurre con ambito o contesto): lo scope indica l’area di validità di una variabile, ovvero in quale porzione di codice una variabile “vive”.
Con l’espressione global scope si indica tutto il codice; mentre con local scope si indica un blocco di codice, sia esso una funzione (functional scope), un ciclo o un ramo di una struttura di controllo (block scope).

In generale valgono queste regole:

- Le variabili di tipo **var** hanno uno scope globale, o di funzione (locale), mentre quelle dichiarate con **let** e **const** hanno scope di blocco (locale).

- Le variabili **var** possono essere aggiornate o ridichiarate dentro il loro scope
Le variabili **let** possono essere aggiornate ma non ridichiarate.

- Le variabili const non possono essere né aggiornate né ridichiarate
Le variabili var sono inizializzate automaticamente con undefined, mentre le variabili **let** e const non sono inizializzate.

- Le variabili **var** e **let** possono essere dichiarate senza essere inizializzate, const deve essere inizializzato durante la sua dichiarazione.

- le variabili **var** possono essere utilizzate prima della loro dichiarazione (hoisting).

Bisogna quindi fare attenzione a dichiarare nella maniera corretta le variabili; in particolare la dichiarazione di variabili globali con il **var** potrebbe portare a ridichiarare variabili involontariamente (soprattutto nel caso in cui vengono inclusi più script in una pagina). Per la dichiarazione di variabili globali è quindi preferibile l’utilizzo del **let**.
