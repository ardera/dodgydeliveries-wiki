# GDD

## Inhalt

- Inhalt

- Team

- Kurzbeschreibung

- Genre

- Erfolgskriterien

- unique selling points

- gameplay

- setting

- feedback

- sound

- weitere details

## Team

## Kurzbeschreibung

DD3 ist ein rythmusbasiertes Bullet Hell Spiel im Stil von Touhou und Rhythmy. Die Challenge besteht darin, bis zum Ende jedes Levels durchzuhalten ohne eine gewisse Maximalzahl an Treffern abzubekommen. unterstützt wird der Spieler durch die Hintergrundmusik und das dauerhaft sichtbare Grid, auf dem sich die Projektile der Gegner entlangbewegen.

## Genre

Ganz einfach Rhythm + Bullet Hell. Daher entsprechend schwer.

## Erfolgskriterien

Erfolgreich sind wir dann, wenn sich alles richtig anfühlt. Bei einem so simplen Produkt sollte Qualität stat Quantität gelten. Daher setzen sich unsere Erfolgskriterien aus den Punkten, Schwierigkeit, Präzision und Präsentation zusammen. 

Die richtige Schwierigkeit ist dann erreicht, wenn es nahezu unmöglich ist, ein Level auf den ersten Versuch zu bestehen, es aber gleichzeitig nicht unfair wirkt und eine klare Lernkurve festzustellen ist. Präzision bezieht sich auf Timing und Platzierung. Das ganze Prinzip funktioniert nur, wenn man sich auf den Beat verlassen kann und jederzeit weiß, ob man auch zwischen zwei Objekten durchpasst, bzw. einfach ab wann man weit genug entfernt ist. Präsentation beschreibt zum einen Effekte, Farben und Grafik, die das ganze schön aussehen lassen, wie auch Sichtbarkeit, damit es nicht vorkommt, dass der Spieler ein Objekt übersieht.

## Unique Selling Points

Im Grunde genommen ist DD3 nichts neues, es gibt bereits mehrere Produkte, die dem gleichen Prinzip folgen und das auch so gut hinkriegen, dass man infrage stellen könnte, ob man so etwas nochmal braucht. Was unser Projekt von den anderen abhebt ist die dritte Dimension. Da die grundlegende Bewegung auf der Ebene stattfindet, ist es ein logischer Gedanke, die Grafik dem Ganzen anzupassen. Allerdings liefert die Dritte Dimension die Möglichkeit von Tiefe, möglichen auf-ab Bewegungen und verschedenen (dynamischen) Perspektiven.

# TDD

- Inhalt
- Technische Mindestanforderungen
- Verwendete Software und Libs
- Softwarearchitektur
- Projektmanagement
    - Versionierung
    - Kommunikationsmittel
    - Doku
    - Workpackages (Aufgabenverteilung)
    - Meilensteine
    - Coding Conventions

## Inhalt

** Unfertig:
Zuerst Verwendete Mittel, dann Architektur, dann Anforderungen und n smooth segway zu Management

## Tools und Libs

Das Komplette Projekt wurde in IntelliJ IDEA in Kotlin geschrieben, weswegen natürlich die Kotlin standard Library nötig war. Weiters verwenden wir LWJGL für Rendering, OpenGL für Shader und JBox2D für unsere Physik (Collider, Vektoren usw.). Extern haben wir unsere Modelle in Blender modelliert und Concept Art in Affinity Designer erstellt. Versionierung, Dokumentation und Management läuft dabei komplett über Github.

## Architektur

Das Spiel läuft in der eigens erstellten JackTheFishman Engine, die auch einen großen Teil des Projekts darstellt. Die Engine ist im groben auf 4 Packages aufgeteilt: 

- Audio
- Graphics
- Math
- Util

Wobei, zum besseren Verständnis, Math hauptsächlich lineare Algebra (Vektoren und Matrizen) enthält und Util aus diversen Skripten für Type Conversion, Scene Loading, Serialisation usw. besteht.

Das Spiel selbst enthält dann ebenfalls ein Util Package, ein weiteres für Shader und das wahrscheinlich wichtigste, das Compnents Package. Components ist stark vom Component System der Unity Engine inspiriert, wobei man jederzeit an ein Objekt die nötigen Components einfach anhängen und mit GetComponent Zugriff darauf bekommen kann.

## Technische Anforderungen

Zum einen soll die JackTheFishman Engine eine möglichst simple und angenehme Arbeitsumgebung für das Spiel schaffen. Im endeffekt steckt in der Engine auch die meiste Arbeit. DD3 ist kein besonders kompliziertes Spiel, weswegen wir nach dem Prinzip Qualität statt Quantität hoffen, dass wir ein durch und durch fertig wirkendes Spielerlebnis bieten wollen. Speziell die Placement der Gegner im Bezug auf die Musik soll, mit hilfe von Analyse des Rhythmus, einfach gesagt funktionieren und nicht frustrieren.

## Management

### Version Control

Für die Versionierung wurde Github verwendet, wobei für jedes neue Feature, jeden Bugfix und jeden Refactor ein neuer Branch erstellt wurde. War die Arbeit fertig, hat der Autor eine Pullrequest angelegt. Waren sich alle einig wurde das Feature dann auf Develop gemerged.

### Kommunikation

Für kurze Nachrichten hatten wir eine Telegram Gruppe, die auch die Links zu unseren beiden Zoom Meetings als angepinnte Nachricht enthalten hat. Concept Art und Demo Videos hatten ihren eigenen Channel in einem unserer Discord Server und Meetings werden, wie erwähnt, auf Zoom abgehalten.

### Dokumentation

Für jedes Feature hatten wir im Meeting ein Issue mit einer groben auflistung der Anforderungen erstellt. War das Feature fertig, wurde eine Seite im Wiki auf Github angelegt, in der Anweisungen zur Nutzung und eventuelle Dependencies gelistet waren.

### Packages

kommt noch

Gegner

Movement

Playercondition

Spawner

Steuerung

Loading

Cleanup

Serialization

Kameracontroller (look at)

Physik

Audio und Musik

Alles zusammenfügen

Modellierung

Renderer

Entity framework



### Meilensteine und Zeitplan

Direkt Meilensteine hatten wir keine. Die Issues wurden einfach immer an unser Kanban-Board geheftet und nacheinander abgearbeitet. Welches Feature angeheftet wird, wurd vorher im Meeting abgesprochen. Aus diesem Grund hatten wir auch keinen richtigen Zeitplan, sondern haben alles eher nach Gefühl gemanaged. Zwar hat das nicht wirklich zu Problemen geführt, jedoch hat sich die Arbeit doch tendenziell etwas nach hinten verlagert. Unerwartet war das nicht und die Vorlesungsfreie Zeit erlaubt uns auch noch genug zu Arbeiten.