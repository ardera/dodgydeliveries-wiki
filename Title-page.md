![Title](https://github.com/janekx21/JackTheFishman/wiki/assets/dd3.png)

# How
## Framework
Wir nutzen [Jack the Fishman](https://github.com/janekx21/JackTheFishman/wiki/Jack-the-Fishman)
als Framework, also als Basis, für das Spiel. Es abstrahiert viele Vorgänge, darunter z.B. die
Interaktion mit der Grafik API oder das Laden von Ressourcen. Dabei ist das Build System so
aufgesetzt das DD3 (Dodgy Deliveries 3) als Teilpaket eingebunden ist.

## Issue Management
Die grund Idee ist es sich **ausschließlich** auf Github zu konzentrieren, um Redundanz zu vermeiden.
Zudem ist alles an einem Ort und gut miteinander verbunden.
- Wiki
  - Dokumentation die nicht automatisch generiert ist
- Issues (Git-Flow)
  - Tracken von Tasks
  - Bugs
- Github Projects
  - Kanban Board mit Issues

## Entity System
So nennen wir unser komponentenbasiertes System mit dem wir neue Gameplay Features implementieren.
Es hat genau 3 Schichten: `Scene`, `GameObject` und `Component`.

![ER vom Entity System](https://github.com/janekx21/JackTheFishman/wiki/assets/er-entity-system.png)

# What
## Idee Story-Spiel
*Retten in der Zeit*

### Gameplay
- Jemanden retten (Freund wird entführt)
- man folgt in der Zeit
- Zeit reisen
- first Person
- Entweder Rätsellastig

### Alternativen im Gameplay
#### Rätsel
Freund ist beim Treffen nicht da man muss folgen Viele Personen wurden entführt.
Man muss andere Personen retten, um an Infos zu kommen / weiterzukommen.

##### Action
Man folgt der Person ins Portal, reist in eine andere Zeit landet vielleicht im Schloss des Bösen etc.
Man muss viele Gegner töten. Böse flieht in eine andere Welt mit Freund.
Der Böse dropt ein Gerät um in der Zeit zu reisen? Gerät geht bei der ersten Zeitreise kaputt?
Man muss in den Welten Reparaturteile finden.

### Alternative Story 
#### Zeitreise mit Gerät
Am Ende der Level funktioniert das Gerät noch nicht komplett.
Man reist in die falschen Zeiten.

#### Zeitreise mit Portalen
Zeitportale sind nur am Ende des Levels.
Man sieht die Portale vom Anfang des Levels und muss diese erreichen.
Man hofft im Portal in die richtige Zeit zu reisen. Ende. Freund in Wirklichkeit böse?

#### Ending Ideen
- Man bekommt das Geld zusammen aber der Hooligan gibt alles in der Gefängnisbar für Bier aus anstatt sich freizukaufen (quasi lustiges bad ending).
- Die Leute, die ihn gefangen haben sind der Grund für die Wesen in den Tunneln. Man deckt das Ganze auf und es gibt einen Aufstand.
- Der MC kommt auf die Idee nur die Hälfte zu sammeln und das Geld im Casino zu verdoppeln --> RNG entscheidet über good/bad ending.
- Die Wesen in den Tunneln sind quasi Insekten. Man findet zufällig die Höhle, in der sich das Nest befindet und zündet es an.
    ↣ Reisen ist nicht mehr gefährlich und man wird als Held gefeiert (der Hooligan wird daraufhin freigelassen).

### Level
#### Anfangslevel
Freund wird vor den eigenen Augen entführt
Man verfolgt den Bösen (mit Freunden?) (man sprint mit ins Portal des Bösen, kurz bevor es schließt?)

### Alternativen
#### Statt zeitreisen: Teleporter 
Man muss an einen Ort gelangen, an den man sich nur teleportieren kann mit dem Gerät

## Idee Sound Dodger
*Rougelike Bullethell Sound Dodger mit Story*

### Map
### Gameplay
Man reist von Camp zu Camp um Quests zu erledigen und Items zu sammeln. Die Reise ist dabei das actionlastige Gameplay. Die Story kann innerhalb der Camps erzählt werden.

# Art Style
Das Spiel hat einen Stiel mit vielen Pastellfarben wie bie Flip Flappers.
![Beispiel Graphik](https://images2.alphacoders.com/753/thumb-1920-753003.png)

