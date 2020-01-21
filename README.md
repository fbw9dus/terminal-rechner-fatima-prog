# Summe und Mittelwert

- Schreib ein Programm, dem man mehrere Argumente übergeben kann.
- Im ersten Argument gibt man die Rechenart an: "sum" für Addieren oder "avg" für Mittelwert
- Die übrigen Argumente sind für Zahlen, mit denen das Programm rechnen soll.
- Das Ergebnis soll im Terminal ausgegeben werden

## Anforderungen:

- Im ersten Argument darf nur `"sum"` oder `"avg"` angegeben werden. Wenn etwas anderes angegeben wird, sollte das Programm sich automatisch beenden und eine Fehlermeldung für den Benutzer ausgeben. (Siehe Beispiele unten)

- Alle weiteren Argumente müssen Zahlen sein. Wenn eins der Argumente keine Zahl ist sollte das Programm beendet werden und eine Fehlermeldung ausgegeben werden. (Siehe Beispiele unten)

## Beispiele:

### Summe berechnen

```bash
$ node index.js sum 1 2 3 4
> 10
```

### Mittelwert berechnen

```bash
$ node index.js avg 1 2 3 4
> 2.5
```

### Falscher Rechenart-Parameter

```bash
$ node index.js oops 1 2 3 4
> "I cannot calculate that, please type either "sum" (to calculate the sum) or "avg" (To calculate the Average)"
```

### Falsche Art von Parameter

```bash
$ node index.js sum 1 hello 3 4
> "Sorry, the argument 'hello' is not a number, please try again"
```