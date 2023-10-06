# c snake unive
Snake game implementation in C.

# Idee sulla realizzazione.
1. Mappa
La mappa sarà nient'altro che una matrice di oggetti.
Ogni oggetto avrà delle coordinate espresse in interi.
Ogni oggetto avrà delle proprietà diverse, come la sua rappresentazione grafica e altre proprietà, come, per esempio, cosa succede quando il serpente occupa determinate celle.
2. Tipologia di celle
- <b>Muro</b>: un muro è un blocco che non può essere attraversato dal serpente.
Quando viene pestato, determina la fine del gioco.
- <b>Cibo</b>: un blocco di cibo, quando viene pestato, diventa graficamente invisibile. Oltre a questo, aumenta il punteggio e la lunghezza del serpente.
Allo scomparire di un unità di cibo, potrebbe comparirne un'altra.
- <b>Uscita</b>: Quando il serpente entra in questo blocco, il gioco finisce, e l'utente ha vinto.

Tutti questi blocchi possono essere occupati dal serpente.

Il serpente avrà una testa a un corpo. Inizialmente ha una testa e poi mangiando cibo sviluppa il corpo. Per ogni unità di cibo assunta, il punteggio aumenta di uno e con esso la lunghezza del corpo.

Il punteggio sarà quindi:

`punteggio = cibo_mangiato`

`lunghezza_corpo = cibo_mangiato`

`lunghezza_snake = lunghezza_corpo + 1 (testa)`