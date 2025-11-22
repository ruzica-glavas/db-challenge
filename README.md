**Gestione biblioteca**

Per creare il diagramma della gestione di una biblioteca, sono partità dall'entità libri. Innanzittuto ho definito la relazione tra libri e autori, la quale é una relazione **molti a molti** e quindi c'era bisogno della creazione di una tabella **pivot** nella quale inserire le foreign key.
Sia la relazione tra **libri e categorie** e **libri e prestiti** é una relazione **1 a molti**. Tra libri e categorie, **una categoria può avere più libri** mentre **un libro può avere una categoria**.
Per quanto riguarda i prestiti, **un libro può avere più prestiti**, mentre **un prestito può essere associato ad un libro**.

Anche la relazione tra **prestiti e utenti** é una relazione una a molti, in quanto **utente può avere più prestiti** mentre **un prestito può essere associato ad un singolo utente**. Dopo aver definito le relazioni, ho inserito la Foreign Key nella tabella lato 'molti' (N) della relazione 1:N, in modo che ciascun record di questa tabella possa riferirsi al corrispondente record della tabella lato 'uno' (1).

**Piattaforma Food Delivery**

Per creare questo diagramma sono partita dagli ordini e ho creato le relazioni con le altre entità. Per quanto riguarda **i ristoranti**, **i clienti** e **le consegne** é presente una **relazione uno a molti** in quanto **un ordine appartiene ad una consegna, ma una consegna può avere più ordini**, **un ordine appartiene ad un ristorante, ma un ristorante può avere più ordine** e **un cliente può fare più ordini, ma un ordine appartiene ad un cliente**. Anche in questo caso l'inserimento della FK é nella tabella del lato molti, quindi negli ordini.

Invece tra l'entità **Ristoranti** e **Piatti** c'é una **relazione molti a molti** in quanto più piatti possono far parte di più ristoranti. In questo caso bisogna creare una tabella **Pivot** in cui inserire le FK del ristorante e del piatto.

**Gestione Eventi**

Per creare questo diagramma sono partita dall'entità eventi per poi creare il restante delle relazioni. Tutte le relazioni sono **uno a molti** in quanto: **un evento può avere molti biglietti, ma molti biglietti sono collegati ad un evento**; **un evento può avere tanti sponsor, ma tanti sponsor sono collegati a quell'evento**; **una location può ospitare molti eventi, ma un evento ha una sola location**. Infine c'é la relazione tra i biglietti e i partecipanti in cui **un partecipante può aver molti biglietti (per esempio la versione VIP di un biglietto), ma N biglietti sono appartenenti da un partecipante**.