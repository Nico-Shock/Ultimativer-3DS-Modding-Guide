# **3DS Hacken mit MSET9**

# Was du brauchst

1. Eine SD Karte mit mindestens 2 GB Speicherplatz. Optimalerweise sollte sie mehr als 2 GB haben, am besten 32 GB.
2. Einen 3DS oder 2DS, egal ob Old, New, XL oder normal.
3. Einen PC, Laptop oder ähnliches, um Daten auf der SD Karte zu ändern oder hinzuzufügen.

# SD Karten Vorbereitung

## Windows

1. Ladet euch [Fat32 Format](http://ridgecrop.co.uk/index.htm?guiformat.htm) herunter.
2. Startet die "guiformat.exe".
3. Wählt eure SD Karte aus (z.B. "D:").
4. Falls eure SD Karte über 32 GB hat, wählt "32768" bei "allocated unit size" aus, damit der 3DS die SD Karte erkennen kann.

## MacOS

1. Startet das "Festplattendienstprogramm".
2. Rechtsklickt auf die SD Karte und wählt dann "Löschen" aus. Formatiert sie als Fat32 (es wird eventuell als "MS-DOS-Dateisystem" angezeigt).
3. Wählt anschließend "Löschen".

## Linux

1. Öffnet die "Disk" App.
2. Wählt die Festplatte aus, klickt dann auf das Zahnradsymbol oder macht einen Rechtsklick und wählt "Formatieren".
3. Wählt beim Typ "Fat32" aus (eventuell müsst ihr unter "Other" oder "Weitere" nach Fat32 suchen).

# 3DS Vorbereitung

1. Stecke die SD Karte in deinen 3DS und warte, bis die Daten auf die SD Karte erstellt wurden.
2. Gehe auf Mii Maker und warte, bis die Daten dafür angelegt wurden, wenn sie nicht schon vorhanden sind.
3. Gehe auf die Systemeinstellungen, wähle "Allgemeine Einstellungen" aus und gehe dann ganz rechts auf "System Update" (du müsstest auf v.11.17.0-50 sein; der Buchstabe hinter der Zahl zeigt nur die Region an).4
4. In den Systemeinstellungen gehe auf "Datenverwaltung". Entferne deine SD Karte und stecke sie in deinen PC (Du solltest deinen 3DS eingeschaltet lassen).

# SD Karten Setup

1. Lade die 3DS Modding Setup Daten (MSET9) vom [3DS-Nitro-Pack](https://github.com/Nico-Shock/3DS-Nitro-Pack) herunter und entpacke sie.
2. Installiere Python von der offiziellen Webseite.
3. Platziere den "dbs" Ordner im Nintendo 3DS Ordner, in den beiden Unterordnern mit den langen Ziffern, wo sich auch der Ordner "extdata" befindet.
4. Kopiere alle Daten aus dem "SD" Verzeichnis direkt ins Stammverzeichnis der SD Karte.
5. Packe die SD Karte in den 3DS.

# Payload Vorbereiten

1. Gehe auf deinem 3DS in den Systemeinstellungen auf Datenverwaltung (wo wir schon sein müssten), wähle "Software" und dann "Zurücksetzen" (deine Daten werden nicht gelöscht).
2. Entferne danach deine SD Karte und stecke sie in deinen PC.

# Payload einfügen

1. Öffne die Datei "mset9.bat" (in Windows), "mset9.py" (in Windows und Linux) oder "mset9.command" (in macOS).
2. Wähle im Script aus, ob du einen New 3DS oder Old 3DS hast.
3. Wähle dann "Inject MSET9 Payload".
4. Stecke die SD Karte wieder in den 3DS ein (lass den 3DS eingeschaltet).

# Payload laden

1. Gehe auf dem 3DS in die Datenverwaltung und wähle "Zusatzdaten".
2. Gebe die oben angezeigte Tastenkombination ein.
3. Nachdem der 3DS neu gestartet ist, schalte ihn aus.

# Payload Entfernen

1. Stecke die SD Karte wieder in deinen PC.
2. Öffne erneut das mset9 Script.
3. Wähle deine 3DS Version erneut aus.
4. Wähle "Remove MSET9 Payload".
5. Stecke deine SD Karte wieder in den 3DS.

# NAND Backup

1. Starte erneut GodMode9 beim Starten des 3DS.
2. Drücke die "Home" Taste.
3. Wähle "Scripts".
4. Wähle dann "GM9Megascript".
5. Wähle schließlich "Backup Options".
6. Wähle "SysNAND".
7. Schalte den 3DS aus.
8. Stecke die SD Karte in deinen PC.
9. Gehe auf der SD Karte in den Ordner "gm9" und dann in den Ordner "out".
10. Speichere die Dateien (mit der endung) `.bin`, `.bin.sha` und `.exefs` in einen Backup Ordner.

# Aktiviere "Enable loading external FIRMs and modules" und "Enable Game patching"

1. Halte vor dem Starten die "Select" Taste gedrückt, um in das Luma3DS Menü zu gelangen.
2. Setze ein Haken bei den Optionen, die in dieser Überschrift stehen.
3. Starte den 3DS anschließend neu.

# Homebrews und zusätzliche Software installieren

1. Starte eine beliebige App außer den Systemeinstellungen.
2. Drücke gleichzeitig L + Steuerkreuz nach unten + Select, um das Rosalina Menü zu öffnen.
3. Scrolle herunter zu "Miscellaneous options".
4. Wähle "Switch the HB title to the current app".
5. Schließe das Rosalina Menü und starte die App anschließend neu.
6. Öffne dann im Homebrew Launcher "FBI".
7. Hier kannst du unter "SD" dann "cias" aus dem "current directory" auswählen.
8. Wähle dann "Install and Delete all CIAs".


# CFW (Luma3DS) deinstallieren

1. Starte GM9 (Godmode9), indem du beim Starten die "Start" Taste gedrückt hältst. Wähle dann "GM9Megascript" oder drücke im Godmode9 die "Home" Taste.
2. Wähle "Scripts" und dann "GM9Mega Script".
3. Gehe zu "Hax options".
4. Wähle "Uninstall Hax".
5. Gehe dann immer weiter und gib die benötigten Tastenkombinationen ein.
