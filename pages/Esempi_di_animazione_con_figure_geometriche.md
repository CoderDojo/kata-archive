Ora proviamo a realizzare una semplice animazione basata sullo
spostamento di un cerchio che si fermerà una volta che avrà raggiunto il
bordo della finestra grafica:

    # Comando per caricare la libreria pygame
    import pygame
    
    # Comandi per le operazioni preparatorie
    stop = False
    clock = pygame.time.Clock()
    
    # Definizione di alcuni colori da utilizzare per disegnare
    bianco = (255,255,255)
    rosso = (255,0,0)
    verde = (0,255,0)
    blu = (0,0,255)
    
    # Comando per attivare la libreria grafica
    pygame.init()
    
    # Comandi per la creazione della finestra grafica
    finestra = pygame.display.set_mode((400,300))
    pygame.display.set_caption("Esempio di finestra grafica")
    
    # Comando per colorare di bianco tutta la finestra (sfondo)
    finestra.fill(bianco)
    
    # Posizione di inizio orizzontale del cerchio in movimento
    x = 20
        
    # Inizio del GAME LOOP
    while stop == False:
    
        # Avvio del timer
        clock.tick(10)
    
        for event in pygame.event.get():
            if event.type == pygame.QUIT:
                stop = True
    
        # Sfondo colorato di bianco
        finestra.fill(bianco)
    
        # Qui vanno inseriti i comandi per disegnare
        # Per il momento disegnamo solo un piccolo cerchio
        # Attenzione: questa volta il cerchio viene disegnato
        # sempre più spostato a sinistra fino a quando
        # non toccherà il bordo destro della finestra
        pygame.draw.circle(finestra,rosso,[x,200],20,1)
    
        # Aggiornamento della posizione orizzontale
        # Controllo se spostamento è giunto sul bordo destro della finestra
        if x<380:
            x+=10
        
        # Comando per aggiornare la finestra grafica con le modifiche richieste
        pygame.display.flip()                    
    
    # Chiusura della libreria e fine del programma
    pygame.quit()

Una volta lanciato il programma produrrà questo risultato:

![bitmap\_04.png](../files/img/bitmap_04.png "bitmap_04.png")

## Miglioramenti

Si potrebbe fare in modo che il cerchio potesse tornare indietro alla
posizione iniziale.

Per fare questo occorre impostare un meccanismo di andata e ritorno in
modo che fino a quando la coordinata orizzontale non avrà raggiunto il
bordo della finestra potrà aumentare di valore, ma appena raggiunge il
valore massimo consentito, il valore della coordinata dovrà diminuire
fino a tornare al punto di partenza.

Vediamo le modifiche da apportare per ottenere un effetto rimbalzo:

    # Comando per caricare la libreria pygame
    import pygame
    
    # Comandi per le operazioni preparatorie
    stop = False
    clock = pygame.time.Clock()
    
    # Definizione dei colori da utilizzare per disegnare
    bianco = [255,255,255]
    rosso = [255,0,0]
    verde = [0,255,0]
    blu = [0,0,255]
    
    # Comando per attivare la libreria grafica
    pygame.init()
    
    # Comandi per la creazione della finestra grafica
    finestra = pygame.display.set_mode([400,300])
    pygame.display.set_caption("Esempio di finestra grafica")
    
    # Comando per colorare di bianco tutta la finestra (sfondo)
    finestra.fill(bianco)
    
    # Posizione di inizio orizzontale del cerchio in movimento
    x = 20
    andata = True
        
    # Inizio del GAME LOOP
    while stop == False:
    
        # Avvio del timer
        clock.tick(10)
    
        for event in pygame.event.get():
            if event.type == pygame.QUIT:
                stop = True
    
        # Sfondo colorato di bianco
        finestra.fill(bianco)
    
        # Qui vanno inseriti i comandi per disegnare
        # Per il momento disegnamo solo un piccolo cerchio
        # Attenzione: questa volta il cerchio viene disegnato
        # sempre più spostato a sinistra fino a quando
        # non toccherà il bordo destro della finestra
        pygame.draw.circle(finestra,rosso,[x,200],20,1)
    
        # Aggiornamento della posizione orizzontale
        # Controllo se spostamento è giunto sul bordo destro della finestra
        # per attivare il ritorno
        if andata == True:
            if x<380:
                x+=10
            else:
                andata = False
        else:
            if x>20:
                x-=10
            else:
                andata = True
        
        # Comando per aggiornare la finestra grafica con le modifiche richieste
        pygame.display.flip()                    
    
    # Chiusura della libreria e fine del programma
    pygame.quit()
