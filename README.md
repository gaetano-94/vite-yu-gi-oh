# Vite Yu-Gi-Oh

_Descrizione:_
Create un nuovo progetto utilizzando Vite e Vue 3 e definite i componenti necessari per strutturare il layout come da screenshot allegato.

Al caricamento della pagina, effettuate una chiama ajax all'API di Yu Gi Oh: https://db.ygoprodeck.com/api/v7/cardinfo.php
e con i dati restituiti, stampate una card per ogni carta. Oggi non preoccupatevi per la ricerca.

PS: usate il font che preferite ;)
_ATTENZIONE_: l’api restituisce tutti i risultati in un colpo solo. Per evitare attese e/o rallentamenti nelle richieste, potete diminuire il numero di risultati sfruttando i parametri num e offset
https://db.ygoprodeck.com/api/v7/cardinfo.php?num=20&offset=0
