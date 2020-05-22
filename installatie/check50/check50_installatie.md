# Check50 installatie
Voor alle cases is er een check50 ontworpen: een script waarmee je de output van je programma's kan testen.
De scripts zijn voor iedere case anders, dus zal je het ook op andere manier moeten aanroepen.
Dit kan je vinden op de pagina van de jouw case.
Hieronder staat hoe je check50 moet installeren om zo gebruik te maken van de scripts.
Voor Windows moeten een extra stap gemaakt worden en zal dus los staan van Linux en macOS.


## Windows
Voor Windows moet eerst Windows Subsystem for Linux (WSL 1) geïnstalleerd worden.
Vervolgens kunnen we Ubuntu installeren en met een terminal check50 installeren.

#### Windows Subsystem for Linux
Windows Subsystem for Linux kan geactiveerd en geïnstalleerd worden met een paar simpele commando's.

1. Activeer de optie met een terminal.
    1. Open PowerShell als administrator en run:
        ```powershell
        dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
        ```
       ![Commando in PowerShell om WSL te activeren.](powershell_wsl_enable.png)
    {:start="2"}
    2. Start vervolgens de computer opnieuw op.
    
#### Installeer Ubuntu
{:start="2"}
2. Installeer Ubuntu via de Microsoft Store.
    1. Open de Microsoft Store en zoek naar Ubuntu.
    2. Selecteer `Ubuntu` (dus zonder versie erachter!) en installeer de applicatie door op de `Get` knop te klikken.
    ![Search for Ubuntu in the Windows Store.](ws_ubuntu.png)
3. Start de Ubuntu applicatie op.
4. Geef een gebruikersnaam en wachtwoord op die je gaat gebruiken voor het Ubuntu besturingssysteem.
Dit account zal alle administrator rechten krijgen binnen Ubuntu.
5. Update Ubuntu door de volgende regel uit te voeren in de terminal:
```bash
sudo apt update && sudo apt upgrade
```

#### Installeer check50
Met de volgende stappen installeren we check50. 
Dit gebeurd allemaal binnen het Ubuntu besturingssysteem waar je in komt door de Ubuntu applicatie op te starten.
{:start="6"}
6. Installeer Python voor het Ubuntu besturingssyteem. Dit doe je door ??.
7. Open een terminal en installeer check50 met:
```bash
pip install check50
```
Vervolgens kan je de check50 scripts uitvoeren zoals aangegeven bij de door jou gekozen case.


## Linux & macOS
Zorg ervoor dat je Python en Git geïnstalleerd hebt.
Dit kan het makkelijkste gedaan worden via een Conda installatie zoals uitgelegd in ??.
Open een terminal en installeer check50 met:
```bash
pip install check50
```
Vervolgens kan je de check50 scripts uitvoeren zoals aangegeven bij de door jou gekozen case.