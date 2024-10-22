# Acquisizione Dati 
Questa guida fornisce istruzioni dettagliate sull'uso dei dispositivi , **Empatica+** e **Emotiv Epoc X**, per l'acquisizione dei dati biometrici ed EEG.
- **Empatica+** è un braccialetto smart che rileva vari dati fisiologici, come battito cardiaco, pressione sanguina e l'attività elettrodermica (EDA).
- **Emotiv Epoc X** è un caschetto EEG wireless che misura l'attività cerebrale attraverso sensori non invasivi 
    posizionati sulla testa.
## Indice
- [Empatica+](#Empatica+)
- [Emotiv Epoc X](#Emotiv-Epoc-X)
- [Problemi Comuni](#Problemi-Comuni)
- [Manuali Ufficiali](#References)



## Empatica+

### Prerequisiti

- Bracciale Smart Empatica+
- Dispositivo con Empatica Care App
- Computer
- Connessione Internet

### Configurazione
1. Accedere al portale [care lab](https://carelab.empatica.com/) con i dati dello studio.
2. Nella sezione **partecipants** cliccare sul pulsante **add partecipants** per inserire il numero desiderato di partecipanti.
    - Se volete che il sistema generi automaticamente gli Id dei partecipanti, selezionate Automatic IDS.
    - Se volete potete inserire manualmente l'id per ogni partecipante.
    Verrano create le credenziali di accesso per ogni partecipante. 
3. Aprire l'app Empatica Care dal dispositivo ed effettuare l'accesso con le credenziali del partecipante da analizzare. Le credenziali possono essere inserite
automaticamente scannerizzando il qr code creato dal sistema, o inserendo manualmente le credenziali.
4. Accendere il bracciale premendo il tasto laterale superiore e seguire le informazioni a schermo per effettuare il pairing tra dispositivo e bracciale. 
5. Indossare il bracciale sul braccio non dominante e attendere qualche minuto affinche il dispositivo si stabilizzi. Alla fine di questa procedura tutte le spunte nella schermata di stato diventeranno verdi e nella schermata principale vedremo i dati biometrici attuali.
La registrazione dei dati avviene in automatico appena il bracciale riconosce il corretto posizionamento, lo schermo del dispostivo diventa chiaro. Nel caso in cui ci siano errori di lettura il bracciale ci avviserà dall'app. 

## Emotiv Epoc X

### Prerequisiti

- USB Receiver Dongle
- EPOC X Headset
- Soluzione Salina
- Cavo di ricarica USB-C
- Computer
- Emotiv Launcher e EmotivPro installati

### Preparazione del Dispositivo
1. Idratazione dei Feltrini
    - Per idratare i feltrini, posizionateli in un bicchiere e aggiungete la soluzione salina.
    - Quando sono completamente imbevuti, rimuoveteli dal bicchiere, schiacciandoli leggermente per togliere la soluzione in eccesso.
    - Possono essere ora inseriti nei sensori.
    
2. Connessione tramite Dongle
    - Inserire il ricevitore nella porta USB, si accenderà un led sul ricevitore.
    - Accendere l'headset, emetterà un suono e un led accanto al pulsante di accensione si illuminerà.
    - L'effettiva connessione tra dongle e headset sarà confermata dall'accensione di un secondo led sul ricevitore.

3. Indossare l'headset
    - Effettuare l'accesso su Emotiv Launcher.
    - Aprire l'app EmotivPro e seguire le indicazioni di montaggio.
    - Nel caso in cui il partecipante abbia capelli folti bisogna farsi spazio fino al cuoio capelluto
      per garantire il miglior contatto possibile col sensore.

### Problemi Comuni
1. Scarsa Contact Quality del caschetto
   - L'eeg quality può anche essere non perfetta ma al fine del corretto funzionamento bisogna ottenere il massimo
     contatto tra cuoio capelluto e sensori. Per posizionare correttamente i sensori, aiutarsi con la mappa fornita nell'app durante la configurazione
     e lavorare sui singoli sensori. Aggiustarne il posizionamento, spostando i capelli sottostanti finchè il sensore non raggiunge il contatto massimo (colore verde).

### References
- [Empatica Healt Monitoring Platform](https://s3.amazonaws.com/box.empatica.com/manuals/embraceplus_care/v1.3/en/EHMP_PatientInstructionsForUse-en-UM-74-Rev%205.0.pdf)
- [Emotiv Epoc X User Manual](https://emotiv.gitbook.io/epoc-x-user-manual)

