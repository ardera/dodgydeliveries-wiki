# Die Basics
- Innerhalb der Tunnel beschränken sich die Mechanics auf simple Ausweichmanöver, als auf, ab und seitwärts fliegen.
- Die Angriffe, denen es auszuweichen gilt, folgen dem Rhythmus der Hintergrundmusik.
- Außerhalb der Actionszenen gibt es in den Camps Ressourcenmanagement, verwaltung von Quests und generell alles,
    was mit der Story zu tun hat.
- Am wichtigsten sind wahrscheinlich die bullet hell Elemente, während wir auf den Rhythmus noch am ehesten verzichten können.

# Spieldesign
- Die Welt ist aus bisher ungeklärtem Grund auf unterirdische Camps verteilt.
- Diese Camps, sind durch Tunnel, Höhlen und Röhren miteinander verbunden. Sämtliche Gegner befinden sich in diesen Tunneln, wodurch auch die ganze Action dort stattfinden wird.
- In den Camps erhält man wichtige Hinweise und Aufträge, die einen in den meisten fällen zu anderen Camps leiten. Um dorthin zu gelangen muss man den Weg durch einen oder mehrere Tunnel nehmen, wodurch die mechanics gleichmäßig miteinander verbunden werden sollen.

## Vereinfachter Map-/Spiel-Aufbau (Tokens)

### Camps
- sind Orte die zivilisiert sind
- hier findet eine Gameplay-"Pause" statt
- Story Time
- Upgrades
- Shop
- Quests

### Tubes
- haupt Gameplay
- nicht zivilisiert

### Shop
- Kaufen von Gegenständen via Geld

### Quests
- **sehr** einfach Aufgaben

### Upgrades
- sind quasi Items aber liegen nicht im Inventar

### Story Time
- Interaktion mit Charakteren

### Hindernisse
- können dem Spieler HP abziehen

### Gegner
- Sind wie Hindernisse die sich bewegen 

## Projektil Arten
- Basic
  - fliegt in die initial Richtung mit konstanter Speed
  - hoher schaden
- Wobble
  - fliegt mit Sinuskurve
  - recht langsam
- Short
  - wie Basic aber mit geringer Lebenserwartung
- Firework
  - erst wie basic dann explodiert es
  - dabei werden weitere Short gespawned
- Sideburner
  - wie Firework aber es werden nur Short zur Seite gefeuert
  - nur Horizontal
- Laser
  - lebt sehr kurz
  - komplett vertikal
  - mit Telegraph
- Flame
  - wie Short aber mit breiter Fächerung

### Design Idee
- Steinfelsen
- Gegner werfen mit Abfall/Metallschrott(Rohre, Zahnräder, Reifen)
- Stalaktiten, die herunter fallen

> Telegraph ist ein Zeichen vor der Aktion (Audio oder Visuell)

# Steuerung
Akzeptierte Input Devices inkludieren Tastatur, Gamepad und auch Tablet.

## **In Game**  
präzise 2D Steuerung, Umsetzung kann variieren.

- Maus
- Grafiktablet
- Tastatur (nicht empfohlen)

## **Menüsteuerung**
- klassisch (trivial)

## **Ray Projection**
Da eine Maussteuerung nicht in einem 3D Spiel verwendet werden kann, wo das Spielfeld Perspektive besitzt, muss eine Projektion des ScreenSpaces auf die Spielebene passieren.

# Items
## Beim Händler kaufbar:
### Itemideen / via Shop
* Schutzschilde (unverwundbar für eine kleine Zeit nach Hit) läd auf
* Taschen Uhr (Slow Motion nach Hit) läd auf
* Ventilator (Wegpusten von Projektilen nach Aktivierung) läd auf
* Turbo Flasche (Beschleunigung bei Hit) läd auf
* Schaf (Umwandeln von Projektilen zu Wattekugeln, die lustig wegbouncen nach Aktivierung) einmalig
* Heilitems
  * kleines Herz (Sofort Heilung nach Aktivierung) einmalig
  * ? (Heilung, wenn man Damage nimmt) einmalig
  * Medipack (an bestimmten Stellen im Level kann leben regeneriert werden | durchs stehenbleiben) dauerhaft
* Bombe (die Feinde im Umkreis zerstört) einmalig
* Feder (Springt und verlässt die Ebene) läd auf
* Hupe (alle ängstlichen Feinde fliehen) einmalig
* Musik Box (schiebt Gegner weg die nach an einem sind)
* Turbo (speed up) dauerhaft
* Laser Kanone (kleine Projektile verschwinden zufällig selten) dauerhaft
* Magnet (zieht Ressourcen an) dauerhaft
* Hufeisen (wenn man sterben würde, 30% Chance zu überleben) dauerhaft
* Koffer (halbes leben aber doppelte Ressourcen) einmal pro Level
* Dritter Arm (wie ein Herzkontainer) dauerhaft
* Pille (schupfen für eine kurze zeit) einmalig

Im Tunnel aufhebbar:
* kleinere Wertobjekte, die man bei Händlern verkaufen kann aka Ressourcen
  * Goldmünzen
  * seltene Pflanzen
  * Monsterteile / Souvenir

### Kaufbedingungen
* Ansehen beim Händler

# Gegner
Lebendige Gegner:
- Gegner, der einem Lieferungen / Wertgegenstände klauen kann (ähnlich wie Ratte in _Enter the Gungeon_)

Nicht-lebendige Gegner:
- Kugeln oder so
- Beschleunigt Projektile mit Portal oder so

Gegner Design:
Feinde des Kraken (Haie und Aale)
Haie Spawnen die Projektile, anderes Projektil je nach Hai

- Normaler Hai, normaler Schuss (entweder einfach ne Kugel oder Hai-Ei)
- Hammerhai, spawnt den Aal (wobble Gegner, siehe Game Ideas Page)
- Katzenhai, = Laserhai
- Laternenfisch, schickt eine Leuchtkugel los, die keinen Schaden verursacht (soll ablenken)
- Walhai, Explosives; spalten sich auf mehrere Lanes auf

Standard:
![](https://cdn.discordapp.com/attachments/720258966046900265/728157106145853470/Standard_Shark_Concept.png)

Hammerhead:
![](https://cdn.discordapp.com/attachments/720258966046900265/728157112701681664/Hammerhead_Concept.png)

Lasershark:
![](https://cdn.discordapp.com/attachments/720258966046900265/728157118342889482/Lasersharl_Concept.png)

Laternenfisch:
![](https://cdn.discordapp.com/attachments/720258966046900265/728157115104886814/Laternenfisch_Concept.png)

# Welt
## Spieler in der Stadt/Camp
### Perspektive und Kamera
<details> 
  <summary>Three-Quarters View</summary>
   A method of portraying three dimensional space in a two-dimensional plane. Basically, it's a tilted bird's eye view perspective in which both the top and front of an object is seen at the same time, and the vertical axis indicates both height and depth.

<b>Beispiele</b>
<ol style="list-style:upper-roman">
<li>Pokémon</li>
<li>Zelda until the debut of The Legend of Zelda Ocarina of Time</li>
</ol>
</details>

- Kamera folgt dem Spieler

### Steuerung
- Spieler ist nicht an "Felder" gelockt
- in dem Bereich frei bewegbar

### Aufbau
- großer Raum, der durch Felsen begrenzt ist
- alle Häuser befinden sich in diesem Raum
- es gibt mehrere Ausgänge, durch die man die Tunnel betritt

![](https://pokemonexperte.de/frbg/wandelhoehle.png.pagespeed.ce.X2Ajthpa1P.png)

### Design der Häuser
- ebenfalls in der Farbpalette des Tunnelgameplays

Beispielhaus:

![](https://static.miraheze.org/allthetropeswiki/3/38/Kakarikovillage.gif)

### Interaktion
- NPCs stehen vor dem Eingang der Häuser
- Alternative: s. Zusatz

### Zusatz:
- eigene Szenen für den Teil in den Häusern

# Ressourcen
- Leben (in form von Schild oder einem Stabilitätswert) 
    - Es gibt einen Default, zu dem man zurückgesetzt wird, wenn man alle Punkte verliert.
    - Leben kann man in den camps auffüllen oder erweitern.

- Treibstoff
    - Man kann in manchen Quests für wenig Treibstoff einen schweren Tunnel oder für viel mehrere leichte fliegen.


