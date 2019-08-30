Vediamo ora alcune dei comandi che permetteranno di disegnare delle
semplici figure geometriche ( per la discussione dettagliata relativa ai
colori esiste una sezione dedicata nella terza parte):

## Riempimento

Per colorare lo sfondo con un colore diverso dal nero si può comporre un
nuovo colore usando le sue componenti di rosso (R), verde (G) e blu (B)
in questo modo:

    bianco = (255,255,255)
    finestra = pygame.display.set_mode((400,300))
    finestra.fill(bianco)

Se invece si desidera colorare una figura con un colore pieno, basta
impostare la dimensione della linea a 0:

    verde = (0,255,0)
    pygame.draw.circle(finestra, verde, (200,150), 20,0)

## Linea

per disegnare una linea (a volte chiamata anche segmento) occorre
conoscere il nome della superficie dove visualizzare la linea, il colore
della linea, le coordinate dei due punti sullo schermo (punto iniziale e
punto finale) e lo spessore della linea

    rosso = (255,0,0)
    pygame.draw.line(finestra, rosso, (0,0),(100,100),1) 

## Linee

Per disegnare una figura che collega tutti i punti presenti nell'elenco
occorre aggiungere l'elenco di tutti i punti che formano la figura: il
parametro True/False indica se si desidera collegare (True) l'ultimo
punto al primo dell'elenco oppure lasciare la figura aperta (False)

    verde = (0,255,0)
    pygame.draw.lines(finestra, verde,True,((0,0),(100,100),(200,200)),1) 

## Rettangolo

Per disegnare un rettangolo occorre il nome della superficie dove
visualizzare il rettangolo, il colore del bordo del rettangolo, le
coordinate del vertice in alto a sinistra e del vertice in basso a
destra e lo spessore della linea

    giallo = (255,255,0)
    pygame.draw.rect(finestra, (255,255,0), (0,0,300,200),1)

## Cerchio

Per disegnare un cerchio occorre il nome della superficie dove
visualizzare il cerchio, il colore del bordo del cerchio, le coordinate
del centro, la dimensione del raggio e lo spessore della linea

    verde = (0,255,0)
    pygame.draw.circle(finestra, verde, (200,150), 20,1)

## Arco

Per disegnare un arco di cerchio occorre il nome della superficie, il
colore del bordo dell'arco, il rettangolo che conterrà l'arco, l'angolo
di partenza, l'angolo di fine e lo spessore della linea

    pi = 3.141592653
    blu = (0,0,255)
    pygame.draw.arc(finestra,(0,0,255),(190,200,210,220),20,3/2*pi, 1)

## Esempio di utilizzo

Ecco le istruzioni aggiunte allo scheletro:

    #Comando per caricare la libreria pygame
    import pygame
    
    #Comandi per le operazioni preparatorie
    stop = False
    #clock = pygame.time.Clock()
    pi = 3.141592653
    
    #Comando per attivare la libreria
    pygame.init()
    
    finestra = pygame.display.set_mode([400,300])
    pygame.display.set_caption("Esempio di finestra grafica")
    
    # Definizione dei colori da utilizzare per disegnare
    bianco = [255,255,255]
    rosso = [255,0,0]
    verde = [0,255,0]
    blu = [0,0,255]
    
    #Comando per colorare di bianco tutta la finestra
    finestra.fill(bianco)
    
    while stop == False:
        for event in pygame.event.get():
            if event.type == pygame.QUIT:
                stop = True
    
        #Comando per disegnare una linea
        pygame.draw.line(finestra, rosso, (0,0), (400,300),1)
        
        #comando per aggiornare la finestra grafica con le modifiche richieste
        pygame.display.flip()                    
    
    pygame.quit()

## Esercizi

Ora invece aggiungiamo proviamo a realizzare le seguenti modifiche:

1.  Disegnare la stessa linea ma di colore blu e riportare nel riquadro
    i comandi usati

<!-- end list -->

1.  Aggiungere una linea in modo che venga formata una croce per tutto
    lo schermo e riportare nel riquadro i comandi usati

<!-- end list -->

1.  Aggiungere un cerchio al centro della finestra di colore verde e di
    raggio 50

<!-- end list -->

1.  Disegnare una figura a piacere (macchina, persona, albero, ecc) e
    riportare nel riquadro i comandi utilizzati
