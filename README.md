# Acquisizione Dati

Questa guida fornisce istruzioni dettagliate sull'uso dei dispositivi, **Empatica+** e **Emotiv Epoc X**, per l'acquisizione dei dati biometrici ed EEG.

- **Empatica+** è un braccialetto smart che rileva vari dati fisiologici, come battito cardiaco, pressione sanguigna e l'attività elettrodermica (EDA).
- **Emotiv Epoc X** è un caschetto EEG wireless che misura l'attività cerebrale attraverso sensori non invasivi posizionati sulla testa.

## Indice
- [Empatica+](#Empatica)
- [Emotiv Epoc X](#Emotiv-Epoc-X)
- [Problemi Comuni](#Problemi-Comuni)
- [Manuali Ufficiali](#References)

## Empatica+

### Prerequisiti
- Bracciale Smart Empatica+
- Smartphone con [Empatica Care App](https://support.empatica.com/hc/en-us/articles/9843547409821-Download-the-Care-App)
- Computer
- Connessione Internet

### Configurazione
1. Accedere al portale [care lab](https://carelab.empatica.com/) con i dati dello studio.
2. Nella sezione **partecipants** cliccare sul pulsante **add partecipants** per inserire il numero desiderato di partecipanti.
    - Se volete che il sistema generi automaticamente gli Id dei partecipanti, selezionate Automatic IDS.
    - Se volete, potete inserire manualmente l'id per ogni partecipante.
    Verranno create le credenziali di accesso per ogni partecipante.
3. Aprire l'app Empatica Care dal dispositivo ed effettuare l'accesso con le credenziali del partecipante. Le credenziali possono essere inserite automaticamente scannerizzando il QR code creato dal sistema o inserendo manualmente le credenziali.
4. Accendere il bracciale premendo il tasto laterale superiore e seguire le informazioni a schermo per effettuare il pairing tra dispositivo e bracciale.
5. Indossare il bracciale sul braccio non dominante e attendere qualche minuto affinché il dispositivo si stabilizzi. Alla fine di questa procedura tutte le spunte nella schermata di stato diventeranno verdi e nella schermata principale vedremo i dati biometrici attuali.  
La registrazione dei dati avviene in automatico appena il bracciale riconosce il corretto posizionamento. Se ci sono errori di lettura, il bracciale ci avviserà tramite l'app.

## Emotiv Epoc X

### Prerequisiti
- USB Receiver Dongle
- EPOC X Headset
- Soluzione Salina
- Cavo di ricarica USB-C
- Computer
- Emotiv Launcher e EmotivPro installati

### Preparazione del Dispositivo
1. **Idratazione dei Feltrini**
    - Per idratare i feltrini, posizionateli in un bicchiere e aggiungete la soluzione salina.
    - Quando sono completamente imbevuti, rimuoveteli dal bicchiere, schiacciandoli leggermente per togliere la soluzione in eccesso.
    - Possono essere ora inseriti nei sensori.
    
2. **Connessione tramite Dongle**
    - Inserire il ricevitore nella porta USB, si accenderà un led sul ricevitore.
    - Accendere l'headset, emetterà un suono e un led accanto al pulsante di accensione si illuminerà.
    - L'effettiva connessione tra dongle e headset sarà confermata dall'accensione di un secondo led sul ricevitore.

3. **Indossare l'headset**
    - Effettuare l'accesso su Emotiv Launcher.
    - Aprire l'app EmotivPro e seguire le indicazioni di montaggio.
    - Nel caso in cui il partecipante abbia capelli folti, è necessario fare spazio fino al cuoio capelluto per garantire il miglior contatto possibile col sensore.

## Problemi Comuni

1. **Scarsa qualità del contatto del caschetto**
   - La qualità del segnale EEG potrebbe non essere perfetta, ma per un funzionamento ottimale è necessario ottenere il massimo contatto tra cuoio capelluto e sensori. Utilizzare la mappa fornita nell'app durante la configurazione per posizionare correttamente i sensori, spostando i capelli sottostanti finché il sensore non raggiunge il contatto massimo (colore verde).

## References
- [Empatica Health Monitoring Platform](https://s3.amazonaws.com/box.empatica.com/manuals/embraceplus_care/v1.3/en/EHMP_PatientInstructionsForUse-en-UM-74-Rev%205.0.pdf)
- [Emotiv Epoc X User Manual](https://emotiv.gitbook.io/epoc-x-user-manual)
