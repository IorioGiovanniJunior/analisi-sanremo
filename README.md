# analisi sanremo
🎶 **Analisi del Festival di Sanremo (1951–oggi)**
📌 **Descrizione del progetto**

Questo progetto nasce dall’analisi dei dataset di Sanremo (fonte GitHub giuschil) con l’obiettivo di studiare l’evoluzione del Festival nel tempo, dai partecipanti ai conduttori, dalla durata agli artisti vincitori, fino alla popolarità dei brani su Spotify.

Il lavoro è stato sviluppato in Excel, Jupyter Lab (Python/Pandas) e Looker Studio, con una parte finale di storytelling a supporto dei dati.

**🛠️ Diario di bordo – Fasi del lavoro**
1. Preparazione dei dati

Apertura iniziale dei file in Excel per una panoramica generale.

Cancellate righe e colonne vuote.

In Jupyter Lab ho cercato e gestito duplicati → trovati circa 50 duplicati di canzoni.

Nel file delle classifiche, la prima colonna non era utilizzabile come index (manca il valore 135) → droppata intera colonna.

Pulizia e normalizzazione: nomi colonne standardizzati in lower case, rimosse colonne non utili (es. url immagine).

2. Merge e gestione dati mancanti

Merge dei file puliti.

Alcune colonne risultano incomplete, in particolare canzoni vincitrici del 1951 senza dati Spotify.

Ho scelto di non cancellarle, per mantenere la coerenza storica dell’analisi.

Questo punto è stato usato nello storytelling (mancanza dovuta a limiti nei dati Spotify disponibili).

Esportazione del file merge in CSV per analisi successive ed import in Looker Studio.

3. Analisi esplorativa

Utilizzo di groupby per capire i trend principali.

Verifica su Excel: la colonna partecipanti indica effettivamente il numero totale di interpreti di quell’anno.

Split degli interpreti in caso di duetti/multipli.

4. Analisi tematiche

a) Trend del Festival

Grafico partecipanti per decade → crescita forte negli anni ’60 (da ~10 a ~60 partecipanti), poi calo progressivo fino ai ~30 del 2020.

Grafico numero conduttori nel tempo (da 5 negli anni ’50 a 7 negli ’80, poi 1 nei 2020).

Calcolo durata media del Festival (inizio/fine date → da 2 giorni anni ’50 a 4 giorni nei 2020).

b) Partecipazioni & Vittorie

Tabella con numero di partecipazioni per interprete.

Analisi vincitori: i grandi artisti storici hanno più vittorie, mentre i cantanti più recenti ne hanno solo una.

Attenzione ai duetti/collaborazioni → corretto lo schema per riflettere entrambe le voci.

c) Popolarità delle canzoni

Popolarità media: dagli anni ’50 (~13 punti Spotify) agli anni recenti (~46).

I brani vincitori hanno in media +10% popolarità rispetto agli altri, ma non è determinante.

Tabella: canzoni non vincitrici che hanno superato la popolarità dei brani vincitori del loro anno.

**📊 Visualizzazione in Looker Studio**

Dati preparati e puliti per facile integrazione.

Creazione di un report interattivo con:

KPI principali (partecipanti, durata, popolarità, vittorie multiple).

Grafici temporali sull’evoluzione del Festival.

Analisi dettagliate su interpreti, conduttori e canzoni.

Storytelling per accompagnare i dati e mostrare i cambiamenti nel tempo del Festival di Sanremo.
