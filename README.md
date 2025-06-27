🐚 MiniShellPokemon
Una mini shell interattiva ispirata all’universo Pokémon, sviluppata in C come progetto scolastico per approfondire la gestione dei processi, il parsing dei comandi e l’uso di segnali Unix.

🎯 Obiettivo
Simulare una shell Unix-like con funzionalità base, arricchita da elementi estetici e testuali ispirati al mondo Pokémon. Il progetto ha lo scopo di migliorare la comprensione del funzionamento di una shell e del comportamento dei processi nel sistema operativo.

⚙️ Funzionalità
Esecuzione di comandi esterni (ls, cat, etc.)

Supporto per comandi interni come cd, exit

Parsing avanzato di input con gestione di:

Pipe (|)

Redirezioni (>, >>, <)

Variabili d'ambiente

Gestione dei segnali (Ctrl+C, Ctrl+D)

Prompt personalizzato a tema Pokémon

📁 Struttura del progetto
makefile
Copia
Modifica
MiniShellPokemon/
├── src/               # File sorgente
├── include/           # Header files
├── Makefile           # Build system
├── README.md          # Questo file
└── assets/            # Immagini e media (es. sprite, suoni)
🛠️ Compilazione
Per compilare il progetto:

bash
Copia
Modifica
make
Per pulire i file oggetto:

bash
Copia
Modifica
make clean
🚀 Esecuzione
Dopo la compilazione, esegui:

bash
Copia
Modifica
./minishell
🎨 Screenshot / Video
https://github.com/tuo-user/tuo-progetto/assets/demo.mp4
MiniShellPokemon in azione, con un prompt animato e comandi eseguiti in stile trainer battle!

💡 Ispirazione
Il progetto è un mix tra la didattica dei sistemi operativi e l'amore per il mondo Pokémon. È pensato per imparare divertendosi, proprio come un vero Allenatore impara dalle sue battaglie.

📚 Tecnologie usate
C (standard ISO C99)

GNU Make

GDB / Valgrind per debugging

Linux Terminal API
