Enthält im Grunde Velocity und Collision

Velocity:
Kann mit getSpeed ausgegeben werden.
Kann mit setVel verändert werden. setVel nimmt einen Vector2fc entgegen.
In jedem update wird Geschwindigkeit * Deltatime auf die Position draufgerechnet (also der komplette Vektor pro sekunde bei 60fps)

Collision:
Kann mit getCollider ausgegeben werden.
SetColliderSize nimmt eine float entgegen und verändert damit die Größe.
Der Collider ist Kreisförmig und Size gibt den Radius an.