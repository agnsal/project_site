# Mini sito per il progetto ErasmusTrip

Il team vuole sviluppare un sito vetrina responsive per il progetto ErasmusTrip, a sua volta sviluppato nell'ambito del corso "_Progettazione di Sistemi Interattivi_" A.A. 2016/2017 delle prof.sse Laura Tarantino e Tania Di Mascio. 

## Generalità

### Obiettivi generali del nuovo sito

Questo sito ha molteplici scopi:
* Far conoscere l’app ErasmusTrip, ipotizzando che si stia apprestando ad entrare in commercio, nonché promuovere la sua diffusione;
* Fornire informazioni utili agli utenti riguardo tale sistema;
* Convincere gli utenti che entrano nel sito ad effettuare il download e l’installazione della suite sul proprio smartphone.

### Utenti

Gli utenti target di questo sito coincidono con gli utenti del sistema ErasmusTrip; in particolare, tutti e soli gli utenti target sono studenti universitari che necessitano di organizzare i vari aspetti della loro esperienza Erasmus, in ogni sua fase:
* Before User: utente che si appresta a iniziare la propria esperienza Erasmus;
*  During User: utente che è già in Erasmus e vuole organizzare la sua vita in loco;
*  After User: utente che sta per tornare in Patria, avendo completato la propria esperienza Erasmus.

Una descrizione più dettagliata è descritta nel documento ”ErasmusTrip: documento delle attività”.

### Posizionamento competitivo
Al momento, non essendo stati individuati competitor di rilievo che abbiano prodotto pacchetti software simili ad ErasmusTrip, il team si trova a compiere un’attività pionieristica in tale settore; ne consegue che non sia possibile analizzare siti simili a quello che si sta progettando.

## Requisiti

### Requisiti di architettura

#### Architettura informativa

Il sito sarà strutturato secondo il seguente schema gerarchico.

* homepage
    * Che cosa offriamo:
        * Overview sul progetto
        * Overview sulle mini app
        * Iscrizione alla mailing list
        * Download dell’app
        * Testimonianze degli utenti
* Le nostre app
    * Elenco delle mini app (con breve descrizione) 
* Singola app
    * Descrizione estesa della mini app 
    * Galleria delle view della mini app
* Dicono di noi
    * Testimonianze degli utenti
* Contatti
    * Conosci il team (descrizione con foto)
    * Contatti e pagine social (Facebook, Twitter, etc...)
* Sitemap

Ogni pagina presenterà un footer con:
* Sezione social
* Sezione contatti (indirizzo, email, tel)
* Info "azienda"

#### Navigazione
* Il sito dovrà prevedere una struttura di navigazione globale, accessibile da ogni pagina, dalla quale siano sempre raggiungibili le pagine di primo livello corrispondenti alle diverse sezioni del sito, e una navigazione locale, che permetta la navigazione all’interno di ogni singola sezione;
* Navigazione globale e navigazione locale dovranno sempre essere nella stessa posizione in tutte le pagine;
* La navigazione globale dovrà essere disposta orizzontalmente (e in un burger menu in caso di dispositivi con schermo di piccole dimensioni).

### Requisiti di comunicazione

#### Identità di marca, tono e stile della comunicazione
Il sito presenterà il logo del sistema, costituito da un puzzle colorato affiancato dal nome del sistema: si è voluto stressare il parallelismo tra i pezzi che si giustappongono e le mini app che costituiranno la suite ErasmusTrip, perfettamente integrata.

Verrà riutilizzato il motto che il team ha imposto all’intero progetto, ossia ”I’ll shape your Erasmus experience”. Esso verrà inserito all’interno della Homepage del sito, essendo questo lo slogan a cui gli utenti dovranno immediatamente associare l’idea di Erasmus (il team ha intenzione di puntare ud una diffusione capillare per il sistema, essendo unico nel suo genere).
Il fatto che l’utenza è costituita esclusivamente da studenti, quindi persone giovani, e che statisticamente l’utenza è poco disposta a prestare grande attenzione alla lettura di testi lunghi e/o ampollosi, sarà utilizzato uno stile di comunicazione leggero, asciutto e di facile comprensione. Per quanto riguarda lo stile ed il tono della comunicazione, il team prenderà come esempio il sito della Apple.

#### Grafica e multimedialità
Il sito deve rispettare le specifiche del Responsive Web Design ed è sviluppato tenendo conto delle diverse dimensioni e risoluzioni degli schermi dei dispositivi fissi e mobile; in particolare, ad ogni dispositivo sarà associato il corrispettivo breakpoint:

* Smartphone portrait: >= 320px;
* Tablet portrait: >= 768px;
* Desktop: >= 1224px.

Si terrà conto di tali breakpoint sia per le immagini che per eventuali video (tutti fluidi). Nella fattispecie, questi ultimi saranno in formato YouTube-embedded per minimizzare i tempi di risposta del server host.

Per quanto concerne la palette di colori utilizzata per il sito, il team utilizzerà un set di colori coerente con quello della suite ErasmusTrip e con quello del logo scelto.

#### Lingua e localizzazione

Tutti e soli gli utenti target del sito che si vuole progettare, almeno in concomitanza con la prima versione di ErasmusTrip, saranno studenti italiani. Tuttavia, essendo l’inglese la lingua principalmente utilizzata nei contesti internazionali, il team non si impone vincoli nell'utilizzarla nel sito (per quanto in minima parte).

#### Requisiti di contenuto

* **Home**: contiene la headline e la tagline del sistema, immagini coerenti con il sistema stesso accompagnate da slogan e da alcuni dei migliori commenti degli utenti di ErasmusTrip. Presenta il collegamento al download del sistema
    * Headline: _I'll shape your Erasmus experience!_
    * Sub-headline: _Quando vai in Erasmus, hai un compagno su cui contare_
* **Chi siamo**: contiene le foto dei membri del team e dati, il loro ruolo e i link ai social media;
* **Dicono di noi**: contiene le testimonianze e commenti più rilevanti degli utenti dell’app (nella forma foto dell’utente, nome completo dell’utente e breve testimonianza testuale);
* **Le nostre app**: contiene una breve descrizione di tutte le mini app che compongono ErasmusTrip. È corredato da informazioni aggiuntive quali un’indicazione del main purpose del sistema, nonché da immagini delle stesse componenti ed alcuni slogan sulla mini app
    * _Ubi - Dove vado?_: contiene una descrizione estesa della mini app Ubi (che permette di trovare un’università estera per l’esperienza Erasmus, nonché un alloggio in loco), corredata da alcune immagini illustrative delle view;
    * _Eventa - A cosa partecipo?_: Contiene una descrizione estesa della mini app Eventa (che permette di trovare attività ed eventi nella città dell’Erasmus tenendo conto degli interessi dell’utente), corredata da alcune immagini illustrative delle view.
* **Sitemap**

### Requisiti di Accessibilità

#### Prestazioni

Per motivi legati alla Search Engine Optimization, sarà necessario minimizzare il ”peso” delle pagine, in particolare la Homepage. Nel dettaglio:
* Le immagini devono essere opportunamente compresse in modalità lossless per non perdere in qualità (preferibilmente JPEG e PGN);
* Gli eventuali video saranno Youtube embedded, per favorire il caricamento asincrono degli stessi.

#### Reperibilità

Il nome scelto per il dominio è _www.erasmustrip.example_. Tenendo conto della mappa di navigazione del sito saranno stabiliti i seguenti path:
* Per la pagina ”Le mini App”: /apps/
* Per la singola pagina di ogni mini app: /apps/ < nomeapp > • per la pagina ”Dicono di noi”: /opinions/
* Per la pagina ”Contatti”: /contacts/

Puntiamo ad un alto ranking nelle SERP dei motori di ricerca Google, Yahoo e Bing, mediante l’ottimizzazione SEO. In particolare si utilizzeranno le seguenti parole chiave:

* Primary keyword: ErasmusTrip;
* Other:
    * App
    * Erasmus
    * Trip
    * Scegliere
    * Destinazione
    * Corsi
    * Organizzare
    * Viaggio
    * Trovare
    * Alloggio
    * Pianificare
    * Studio
    * Tempo libero
    * Vendere
    * Acquistare/Comprare
    
#### Compatibilità con i Browser
Per motivi legati all’ottimizzazione SEO si farà uso esclusivo della tecnologia HTML5+CSS3 secondo lo standard W3C, ne consegue che saranno supportati esclusivamente i browser che supportano questo requisito. In particolare, si ottimizzerà il sito per i seguenti browser (versioni desktop e mobile):
- Google Chrome; 
- Mozilla Firefox; 
- Apple Safari.

#### Accessibilità da parte di utenti disabili

Il sito, come è stato fatto anche per il sistema ErasmusTrip, dovrà poter essere utilizzato da utenti che siano ipovedenti o che soffrano delle più comuni disfunzioni visive (daltonismo, visione bicromatica). Si effettuerà una verifica del rispetto di tale specifica sfruttando appositi tool online.
