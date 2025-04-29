Note: 
    Questa traccia è stata svolta sul modello di "ESEMPIO_3_NODI_COMUNICANTI_PIA", facendo riferimento al suo schematico.
    IMPORTANTE: Il sistema C dello schematico presente in "architettura sistema.png", è rappresentato dal sistema A della traccia, quindi
                bisogna caricare sul motorola 7 e sulla memoria 8 il codice e le memorie del sistema A.
    Riguardo le memorie, ne sono state generate due: la prima "mem_tx.mem" è quella dei trasmettitori, identica.
    Differentemente, "mem_sys_A.mem" è la memoria del sistema A (che ricordo essere il sistema C nello schematico, DA CARICARE in memoria 8).
    Le variabili is_reading nello pseudo-codice nell'assembly sono state sostituite da "IS_REC"
COME VERIFICARE IL FUNZIONAMENTO DEL PROGRAMMA:
    Al termine dell'esecuzione, vengono caricati nei registri D4/D5/D6 e D7 i valori di "possesso - end_b - end_c - k ( contatore di iterazioni)".
    Se il programma funziona correttamente, allora i loro valori sono "IS_READING_NONE - 1 - 1 - NITER (=5)".
    Inoltre è possibile mettersi all'indirizzo 8000 della memoria 8 e verificare i messaggi salvati: Per ogni 3 messaggi omologhi devono esserci due messaggi 
    di B ( caricato sul Motorola 1) ed un messaggio di C (caricato su Motorola 4), e che inoltre i messaggi non si accavallano.