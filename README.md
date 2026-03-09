# SPIEGAZIONE REPOSITORY "AR-MULTI"

In questa repo son presenti 5 cartelle, create nel seguente ordine cronologico:  
1. **test_cosmin:** rappresenta il file di test effettuato da Cosmin, rappresentante un grafico statico in un pannello (è stato utile per prendere spunto per l'interfaccia grafica).
2. **versione_base:** rappresenta una prova effettuata col marker 3 rappresentate un grafico simile a quello effettuato da Cosmin ma dinamico, con valori aggiornati in tempo reale (generati randomicamente); il grafico mostra il valore attuale all'estremo destro e a sinistra i valori dei secondi precedenti fino a -8s; inoltre in alto è presente la data e l'ora dell'ultimo aggiornamento (ottenute tramite clock del dispositivo).
3. **elementi_grafici:** in questa cartella son state sperimentate 4 applicazioni differenti:
    - ***pannello_dati_variabili:*** questo test è lo stesso del punto 2, identico.
    - ***pannello_allarmi:*** in questo test si è provato un pannello con una spia che, al variare di una variabile (es. Temp.) rispetto ad un valore soglia (es 75°C) genera tre colori diversi: verde, giallo e rosso. Il colore è derivato dalla gravità dello scostamento e si aggiorna in tempo reale. Anche qua son stati utilizzati dati randomici per simulare un caso reale.
    - ***sensore_co2:*** in questo test si è provato un pannello per un eventuale sensore IAQ, dove la concentrazione di CO2 in ppm viene aggiornata in tempo reale e rappresentata su una scala cromatica che va dal verde al rosso all'aumentare della concentrazione; inoltre son presenti altri dati come temperatura, umidità rel. ecc.. 
    - ***flussi_3d:*** in questo test infine si è immaginato di porre il marker in mezzo a due tubi trasportanti fluidi diversi (es. vapore e acqua ref.); tramite delle frecce in 3d è possibile visualizzare la direzione dei flussi e inoltre è anche possibile stampare il valore in tempo reale della temperatura di quei flussi.
4. **dati_endpoint:** in questa cartella è presente un test per valutare la possibilità di collegare dei dati reali ad un pannello in AR tramite endpoint. In un primo momento questo è stato raggiunto tramite file .json ma la prova definitiva verrà effettuata in EC collegati alla rete locale con un database di prova.
5. **all:** in questa cartella son stati implementati tutti i risulati ottenuti dai test precedenti in un unico codice in grado di riconoscere 5 marker contemporaneamnte, mostrando per ognuno di essi le informazioni desiderate. 
    - ***all_pulsanti:*** in questa sotto-cartella si vogliono integrare al test *all* le funzionalità di pulsanti cliccabili quali:
        - **Zoom +/-**
        - **Fissaggio a schermo**
