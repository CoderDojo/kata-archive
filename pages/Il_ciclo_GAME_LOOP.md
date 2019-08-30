Le prime istruzioni riportate nella sezione precedente sono necessarie
per :

  - importare la libreria pygame
  - attivare la libreria pygame
  - creare la finestra grafica delle dimensioni desiderate
  - scrivere un titolo sulla finestra grafica

Queste operazioni sono da eseguire una sola volta e quindi vengono messe
all'inizio del programma.

Le operazioni che seguono, invece, hanno un altro significato perché, a
differenza delle altre, devono essere eseguite più volte. Vediamo
perché.

Un videogioco termina quando il giocatore o la giocatrice decidono di
chiudere il programma.

Il videogioco, da parte sua, deve controllare ogni momento se il
giocatore o la giocatrice hanno premuto qualche tasto (per spostare un
oggetto, per colpire un bersaglio, ecc) e ogni volta che questo succede
deve svolgere i comandi necessari per completare l'operazione richiesta.

Ecco perché queste istruzioni vengono chiamate **GAME LOOP**, cioè il
ciclo di gioco (o ciclo del gioco):

    1.  while stop == False:
    2.      for event in pygame.event.get():
    3.          if event.type == pygame.QUIT:
    4.              stop = True
    
    5.  pygame.quit()

  - Nel comando di riga 1 il ciclo while verrà ripetuto finché la
    variabile stop rimmarrà falsa: questo sta a significare che fino a
    quando non verrà eseguito il comando QUIT (che corrisponde alla
    chiusura della finestra grafica) le istruzioni che seguono dovranno
    essere eseguite all'infinito

<!-- end list -->

  - Per evitare che i comandi vadano perduti, il programma conserva in
    un elenco tutti i comandi che gli vengono inviati dal giocatore o
    dalla giocatrice. La riga 2 estrae un comando alla volta da questo
    elenco e poi lo invia al programma perché sia riconosciuto ed
    eseguito. In genere questi comandi rappresentano un tasto premuto
    sulla tastiera, la posizione del mouse oppure la posizione di un
    joystick

<!-- end list -->

  - Nella riga 3 è presente un comando che controlla se è stato premuto
    un comando QUIT. In questo caso viene cambiato il valore contenuto
    nella variabile stop (che era False) con il valore True. Questa
    azione porta alla conseguenza che il ciclo della riga 1 terminerà e
    il controllo passerà alla prima istruzione che verrà incontrata dopo
    le istruzioni del ciclo

<!-- end list -->

  - La riga n.5 viene eseguita solo quando alla variabile stop verrà
    assegnato il valore True (come spiegato nel punto precedente) e
    serve per chiudere la libreria grafica prima che il programma venga
    terminato.

È chiaro che le istruzioni grafiche per disegnare sulla finestra grafica
andranno aggiunte a questo blocco tra le righe 4 e 5 del GAME LOOP, come
vedremo in seguito.
