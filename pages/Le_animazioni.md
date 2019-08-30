Per poter muovere gli oggetti presenti in un videogioco si possono
utilizzare diverse tecniche, non tutte facili.

Esiste però un trucco che può essere utilizzato e che ci aiuterà nella
scrittura dei comandi necessari.

Questo trucco sfrutta il fatto che la nostra finestra dove abbiamo
disegnato lo sfondo è aggiornata in modo molto veloce da un componente
che si chiama **timer** e che avevamo incontrato all'interno del game
loop:

``` 
...
# Inizio del GAME LOOP
while stop == False:

    # Avvio del timer
    clock.tick(10)

    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            stop = True

    # Qui vanno inseriti i comandi per disegnare
    # Per il momento disegnamo solo un piccolo cerchio
    pygame.draw.circle(finestra,rosso,[20,200],20,1)
    
    # Comando per aggiornare la finestra grafica con le modifiche richieste
    pygame.display.flip()
...   
```

Il timer funziona esattamente come un cronografo che conta il passare
del tempo:

  - Aspetta fino a quando il tempo non è scaduto ( a volte anche pochi
    millisecondi, quindi è velocissimo\!)

<!-- end list -->

  - disegna le immagini che abbiamo deciso di mostrare (in questo caso i
    comandi che deve eseguire sono legati ad un piccolo cerchio che
    sposteremo da un parte all'altra dello schermo).

Se noi ogni volta che il timer decide di ridisegnare la finestra,
spostiamo gli oggetti anche di pochissimo, il timer sarà costretto a
disegnarli esattamente nel punto dove li abbiamo messi, creando
l'illusione che gli oggetti si siano spostati da soli\!
