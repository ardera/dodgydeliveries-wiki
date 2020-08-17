# Physics Component
Enthält im Grunde Velocity und Collision

Velocity:
Kann mit getSpeed ausgegeben werden.
Kann mit setVel verändert werden. setVel nimmt einen Vector2fc entgegen.
In jedem update wird Geschwindigkeit * Deltatime auf die Position draufgerechnet (also der komplette Vektor pro sekunde bei 60fps)

Collision:
Kann mit getCollider ausgegeben werden.
SetColliderSize nimmt eine float entgegen und verändert damit die Größe.
Der Collider ist Kreisförmig und Size gibt den Radius an.

# Smooth follow Kamera
Kamera soll dem Spieler immer smooth folgen.

Variablen:
follow: Transform des Spielers
distance: die Distanz die die Cam zum Spieler einhält
relative Rotation: die position relativ zum Spieler (wird normalisiert und mit disctance multipliziert)
smoothAmount: wie smooth gefolgt werden soll. wird bei kleinerem Wert smoother

# Kamera
* Fixed Cameraposition
* Winkel ändert sich zum Spieler hin
