# Acquisizione Dati 
Guida all'uso dei dispositivi per l'acquisizione di dati...

## Indice

- [Empatica+](#empatica+)
- [Quick Start](#quick-start)
- [Game Rules](#game-rules)
- [Features](#features)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)




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
- Se volete potente inserire manualmente l'id per ogni partecipante.
Verrano create le credenziali di accesso per ogni partecipante. 
3. Aprire l'app Empatica Care dal dispositivo ed effettuare l'accesso con le credenziali del partecipante da analizzare. Le credenziali possono essere inserite
automaticamente scannerizzando il qr code creato dal sistema, o inserendo manualmente le credenziali.
4. Seguire le informazioni a schermo per effettuare il pairing tra dispositivo e bracciale. 
5. Indossare il bracciale e attendere qualche minuto affinche il dispositivo si stabilizzi. Alla fine di questa procedura tutte le spunte nella schermata di stato diventeranno verdi e nella schermata principale vedremo i dati biometrici attuali.
### Clone the Repository

To get the source code, clone this repository using Git:

```bash
git clone https://github.com/Riccardohihello/sette_e_mezzo.git
```

### Build
```bash
cd sette_e_mezzo
mvn clean install
mvn dependency:copy-dependencies
```
### Run

After compiling the project, you can run the game from the bin folder:
``` bash
mvn javafx:run
or
java --module-path target/dependency --add-modules javafx.controls,javafx.fxml -cp target/sette_e_mezzo-1.0-SNAPSHOT.jar it.uniparthenope.sette_e_mezzo.Main
```

## Quick Start
1. **New Game**: Start a new game, you can select the number of players and modify their names.
2. **Save/Load Game**: You can save the game state and resume where you left off.
3. **Computer Stats**: See how many wins has the computer.
4. **Statistics**: At the end of the game, player stats are displayed.

## Game Rules
- The goal is to reach a score as close as possible to 7.5 without exceeding it.
- Each player can request additional cards or stop.
- If a player's score exceeds 7.5, they automatically lose.
- The game ends when all players either stop or lose.

## Features
- **Save and Load** game sessions using the **Memento** desing pattern.
- AI for computer-controlled dealer behavior.
- Leaderboard to view past games and player statistics.
- Graphical User Interface (UI) that allows managing all phases of the game intuitively.

## Project Structure

``` less
src/
└── main/
    └── java/
        └── it/uniparthenope/sette_e_mezzo/
            ├── Game        // Main game logic
            ├── Player      // Represents a player
            ├── Deck        // Manages the deck of cards
            ├── Card        // Represents a single card
            ├── GameUI      // User interface
            ├── Memento     // Handles game state saving/loading
            └── Main.java   // Entry point of the program

```
## Contributing

Contributions and suggestions are welcome! Feel free to open a pull request or report issues in the issues section of the repository.

## License

This project is distributed under the [MIT](https://choosealicense.com/licenses/mit/) License. See the LICENSE file for more information.
