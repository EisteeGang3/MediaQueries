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