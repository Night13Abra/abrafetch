# Abrafetch

Abrafetch ist ein einfaches und anpassbares System-Info-Tool, das in der Kommandozeile ausgeführt werden kann. Es zeigt verschiedene Systeminformationen und ermöglicht es Benutzern, ein benutzerdefiniertes Logo und Zitate anzuzeigen.

## Features
- Zeigt Systeminformationen wie Betriebssystem, CPU, GPU und mehr.
- Ermöglicht benutzerdefinierte Logos, die in einer `.txt`-Datei gespeichert werden.
- Zitate aus Marx, Engels und Lenin für etwas politische Philosophie.

## Installation

### 1. Repository klonen

Zuerst musst du das Repository auf dein System klonen:

```bash
git clone https://github.com/Night13Abra/abrafetch.git
cd abrafetch
```

### 2. Skript nach `/usr/bin/` kopieren

Um **Abrafetch** von überall im Terminal auszuführen, kopiere das Skript nach `/usr/bin/`:

```bash
sudo cp abrafetch /usr/bin/
```

Nun kannst du **Abrafetch** ausführen, indem du einfach `abrafetch` in das Terminal eingibst.

### 3. Abrafetch anpassen

#### Logo anpassen

Du kannst dein eigenes Logo verwenden, indem du eine `.txt`-Datei im Verzeichnis `~/.abrafetch/logos/` speicherst. Das Skript sucht nach einem benutzerdefinierten Logo in diesem Verzeichnis. Wenn es keine findet, wird das Standard-Logo verwendet.

Erstelle das Verzeichnis für die Logos:

```bash
mkdir -p ~/.abrafetch/logos
```

Lade dein eigenes Logo hoch oder erstelle eine `.txt`-Datei mit deinem gewünschten Logo und speichere es im `~/.abrafetch/logos/` Verzeichnis.

Beispiel für das Erstellen eines benutzerdefinierten Logos:

1. Erstelle eine Datei mit dem Namen `custom_logo.txt`.
2. Füge dein ASCII-Logo in die Datei ein.
3. Speichere die Datei im `~/.abrafetch/logos/` Verzeichnis.

#### Zitate anpassen

Die Zitate werden zufällig aus einer Auswahl von Marx-, Engels- und Lenin-Zitaten angezeigt. Du kannst die Zitate im Skript anpassen, indem du die Liste der Zitate bearbeitest:

```bash
quote=$(shuf -n1 -e \
    "„Religion ist das Opium des Volkes. – Karl Marx“" \
    "„Die Philosophen haben die Welt nur verschieden interpretiert; es kommt aber darauf an, sie zu verändern. – Marx“" \
    "„Ein Schritt wirklicher Bewegung ist mehr wert als ein Dutzend Programme. – Marx“" \
    "„Proletarier aller Länder, vereinigt euch! – Marx“" \
)
```

### 4. Abrafetch ausführen

Nun kannst du **Abrafetch** jederzeit ausführen, indem du einfach `abrafetch` in deinem Terminal eingibst.

```bash
abrafetch
```

Du solltest jetzt dein benutzerdefiniertes Logo und die Systeminformationen angezeigt bekommen!

## Beispiele

### Standardausgabe:

![grafik](https://github.com/user-attachments/assets/ed86e06f-2ff9-4671-b7ad-02851be0a2d3)



## Beiträge

Beiträge sind willkommen! Wenn du neue Features hinzufügen oder Fehler beheben möchtest, erstelle bitte ein Pull-Request.

## Lizenz

Dieses Projekt ist unter der MIT-Lizenz lizenziert – siehe die [LICENSE](LICENSE)-Datei für Details.
