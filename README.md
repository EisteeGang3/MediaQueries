# MediaQueries
Media Queries Crash Kurs

## Terminal wichtigste Befehle
|Befehl|Bedeutung
|---|---|
|'dir','ls'|Inhaltsverzeichnis anzeigen|
|'cd'| Verzeichnis Wechseln|

### GIT
|Befehl|Bedeutung
|---|---|
|'git clone'| Klont ein Git-Repo|
|'git add .'| Alle Dateien ins Repo übernehmen|
|'git commit -m "Text zum Commit"'| Commit erstellen|
|'git push'| Commit ins Remote Repo übernehmen|
|'git pull'| Daten vom Remote Repo ziehen|





### Media Queries im CSS
```css
@media (Bedingung) {

}
```

### Typische Bedingungen
|Bedingungen|Bedeutung|
|---|---|
|'max-width'|Stile gelten bis zu dieser Größe|
|'min-width'|Stile gelten ab dieser Größe|
|'orientation'| Bildschirmausirhctung 'landscape' oder 'portrait'|
|'screen'|Für Bildschirme gültig|
|'print'|Für Drucker gültig|


## Aufgaben

### 1. Breakpoints nach Bootstrap

setze die breakpoints nach Bootstrap so um, das die jeweilige Bildschirmgröße ausgegben wird und die BackgroundFarbe wechselt. (siehe ganz unten)

### 2. Horizontal, Vertikal

Zeige an, ob der Bildschrim Querformat oder Hochformat ist.

### 3. Ausdrucken

Wenn die Seite ausgedruckt wird, soll der 'large'-Inhalte ausgegeben werden und das Aussehen angepasst werden:

- Hintergrund Weiss
- Schriftfarbe Schwarz
- Bilder weg




### Beispiel HintergrundFarbe ändern
```css
html,body{
    width: 100%;
    height: 100%;
    background-color: green;
}

/*Sichtbarkeit grundlegend ausschalten*/



.extrasmall{
    display: none;
}

.small{
    display: none;
}

.medium{
    display: none;
}

.large{
    display:none;
}

.extralarge{
    display: none;
}

.extraextralarge{
    display: none;
}

/*Extra Small*/
@media (max-width: 576px){
    html, body{
        background-color: red;
    }
    .extrasmall{
        display: block;
    }
}

/*small*/

@media (min-width: 577px) and (max-width: 767px){
    html, body{
        background-color: blue;
    }
    .small{
        display:block;
    }
}

/*medium*/

@media (min-width: 768px) and (max-width: 991px){
    html, body{
        background-color: purple;
    }
    .medium{
        display:block;
    }
}


/*Large*/

@media (min-width: 992px) and (max-width: 1199px){
    html, body{
        background-color: yellow;
    }

    .large{
        display: block;
    }
}

/*ExtraLarge*/

@media (min-width: 1200px) and (max-width: 1399px){
    html, body{
        background-color: pink;
    }

    .extralarge{
        display: block;
    }
}

/*ExtraExtraLarge*/

@media (min-width: 1400px){
    html, body{
        background-color: white;
    }

    .extraextralarge{
        display: block;
    }
}

```