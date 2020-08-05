## What
Jack the Fishman ist ein 3D game framework.

## Why
Jack the Fishman ist als Lernprojekt gedacht und wurde für die Lehrveranstaltung [3D Game Projekt](https://www.acagamics.de/pages/forschung-veranstaltungen-3d-game-project-sose2020/) gebaut.

## How
Die basis bildet eine kombination aus Kotlin + LWJGL.
Dazu kommt Github für VC, Issue Management und Dokumentation.
Der Stack sieht im genauen wie folgt aus:
- Kotlin + LWJGL
    - [Kotlin](https://kotlinlang.org/
        -ist eine Java ähnliche Sprache die sich in JVM Bytecode kompiliert
    - [LWJGL](https://www.lwjgl.org/)
        - OpenGL ist eine Grafik Api, über Statemachine, die alt aber bekannt ist
            - stellt das Interface zum Grafiktreiber da
        - GLFW ist ein native Window wrapper der cross platform ist
            - er sorgt für Input Output aka Mouse, Keyboard und Bildschirm
        - Assimp ist für Model-Loading
        - STB ist für Texture-Loading
        - OpenAL ist eine Audio library
- Serialisierung
    - [Klaxon](https://github.com/cbeust/klaxon)
- Build verfahren
    - [Gradle](https://gradle.org/)
    - in kombination mit der [Kotlin Scrip Language](https://kotlinlang.org/docs/reference/using-gradle.html)
    - das Ganze ist cross platform
- Dokumentation
    - JavaDoc bzw Dokka zum Generieren von Code Dokumentation
- Tools
    - IntelliJ IDE (Coding)
    - Blender (3D Modeling)
    - RenderDoc (OpenGL Debugger)

## Who
[Meet the Team](https://github.com/janekx21/JackTheFishman/wiki/Meet-the-Team)
