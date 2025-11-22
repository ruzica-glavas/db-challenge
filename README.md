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

**Gestione cinema**

Per questo diagramma sono partita dall'entità film per poi collegare il restante delle relazioni. I film sono relazionati con le proiezioni in una relazione **uno a molti, in cui un film può avere più proiezioni**. Tra le proiezioni e le sale c'é una **relazione 1 a 1, in quanto una proiezione può essere proiettata in una sala**. La relazione tra sale e spettatori é di **uno a molti, in quanto molti spettatori possono stare in una sala sola**. Infine la relazione che contradistingue gli spettatori e le prenotazioni é di **uno a molti in quanto uno spettatore può avere più prenotazini ma una prenotazione é associata ad uno spettatore.**

**Piattaforma Social**

Per questo diagramma sono partita dall'entità Utenti e ho definito la relazione tra utenti e commenti che à una **relazione uno a molti, in quanto un utente può fare molti commenti, ma un commento é associato ad un utente solo.** Dopodiché ho definito la relazione tra utenti e post la quale é una **relazione uno a molti in quanto un utente può scrivere molti posti e molti post posson essere associati ad un utente.** L'entità post ha una **relazione uno a molti con i commenti, con i likes e i media, in quanto un post può avere molti commenti, molti likes e molti media.** Infine la relazione tra l'entità commenti e l'entità likes é di tipo **uno a molti in quanto un commento può avere molti likes e i likes sono associati ad un commento.**
