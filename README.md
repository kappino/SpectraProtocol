# Acquisizione Dati

Questa guida fornisce istruzioni dettagliate sull'uso dei dispositivi, **Empatica+** e **Emotiv Epoc X**, per l'acquisizione dei dati biometrici ed EEG.

- **Empatica+** è un braccialetto smart che rileva vari dati fisiologici, come il battito cardiaco, la pressione sanguigna e l'attività elettrodermica (EDA).
- **Emotiv Epoc X** è un caschetto EEG wireless che misura l'attività cerebrale attraverso sensori non invasivi posizionati sulla testa.

## Indice
- [Empatica+](#Empatica)
- [Emotiv Epoc X](#Emotiv-Epoc-X)
- [Procedura Test](#Procedura-Test)
- [Problemi Comuni](#Problemi-Comuni)
- [Manuali Ufficiali](#Manuali-Ufficiali)

## Empatica+

### Prerequisiti
- Bracciale Smart Empatica+
- Smartphone con [Empatica Care App](https://support.empatica.com/hc/en-us/articles/9843547409821-Download-the-Care-App)
- Computer
- Connessione Internet

### Configurazione
1. Accedere al portale [care lab](https://carelab.empatica.com/) con i dati dello studio.
2. Nella sezione **participants** cliccare sul pulsante **add participants** per inserire il numero desiderato di partecipanti.
    - Se si desidera che il sistema generi automaticamente gli Id dei partecipanti, selezionare Automatic IDS.
    - Altrimenti è possibile inserire manualmente l'id per ogni partecipante.
    Verranno create le credenziali di accesso per ogni partecipante.
3. Aprire l'app Empatica Care dallo smartphone ed effettuare l'accesso con le credenziali del partecipante. Le credenziali possono essere inserite automaticamente scannerizzando il QR code creato dal sistema o inserite manualmente.
4. Accendere il bracciale premendo il tasto laterale superiore e seguire le informazioni a schermo per effettuare il pairing tra smartphone e bracciale.
5. Indossare il bracciale sul braccio non dominante e attendere qualche minuto affinché il bracciale si stabilizzi. Alla fine di questa procedura tutte le spunte nella schermata di stato diventeranno verdi e nella schermata principale vedremo i dati biometrici attuali.  
La registrazione dei dati avviene in automatico non appena il bracciale riconosce il corretto posizionamento. Se ci sono errori di lettura, il bracciale ci avviserà tramite l'app.

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
    - Per idratare i feltrini, posizionarli in un bicchiere e aggiungere la soluzione salina.
    - Quando sono completamente imbevuti, rimuoveri dal bicchiere, schiacciandoli leggermente per togliere la soluzione in eccesso.
    - Possono essere ora inseriti nei sensori.
    
2. **Connessione tramite Dongle**
    - Inserire il ricevitore nella porta USB, si accenderà un LED sul ricevitore.
    - Accendere l'headset, emetterà un suono e un LED accanto al pulsante di accensione si illuminerà.
    - L'effettiva connessione tra dongle e headset sarà confermata dall'accensione di un secondo LED sul ricevitore.

3. **Indossare l'headset**
    - Effettuare l'accesso su Emotiv Launcher.
    - Aprire l'app EmotivPro e seguire le indicazioni di montaggio.
    - Nel caso in cui il partecipante abbia capelli folti, è necessario farsi spazio fino al cuoio capelluto per garantire il miglior contatto possibile col sensore.
## Procedura Test
### Prerequisiti
- Creare il loop fra la porta COM8 e COM7
- Impostare emotiv pro in ascolto sulla porta COM7
- Aprire il gioco sull'emulatore
- Aprire OBS Studio
### Fasi Da Seguire
1. **Montaggio Bracciale**
   - Con collegamento su app in base a credenziali pregenerate.
3. **Montaggio Headset**
4. **Avvio Registrazione Obs**
    - Avviare la registrazione video e audio tramite hotkey ctrl+r
5. **Avvio Registrazione Emotiv**
    - Inserendo id paziente e spuntando la baseline.
6. **Fase Gioco**
    - Riaprire l'emulatore, **inserire id paziente** e iniziare i livelli (durata ca 7 minuti).
7. **Fase Video**
   - Lanciare script python per visualizzare clip video e premere **avvia**
8. **Terminare Registrazioni**
   - Fermare OBS con hotkey ctrl+s e manualmente su emotiv pro. 
## Problemi Comuni

1. **Scarsa qualità del contatto del caschetto**
   - La qualità del segnale EEG potrebbe non essere perfetta, ma per un funzionamento ottimale è necessario ottenere il massimo contatto tra cuoio capelluto e sensori. Utilizzare la mappa fornita nell'app durante la configurazione per posizionare correttamente i sensori, spostando i capelli sottostanti finché il sensore non raggiunge il contatto massimo (colore verde).
2. **Emotiv Pro non riceve i marker dal player video**
    - Controllare che sia stato creato il loop fra la porta COM8 e la porta COM7, nel caso in cui il loop sia già attivo, chiudere emotiv pro, chiudere il player e lanciare lo script flush_port.py. Rieseguire il setup della porta su emotiv pro e lanciare di nuovo il videoplayer.

## Manuali Ufficiali
- [Empatica Health Monitoring Platform](https://s3.amazonaws.com/box.empatica.com/manuals/embraceplus_care/v1.3/en/EHMP_PatientInstructionsForUse-en-UM-74-Rev%205.0.pdf)
- [Emotiv Epoc X User Manual](https://emotiv.gitbook.io/epoc-x-user-manual)
