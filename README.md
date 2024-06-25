Hier ist das beste Tutorial, um den 3DS zu modden: Es enthält alle notwendigen Schritte und Bilder, die du benötigst.

# SD Karten Setup

Du benötigst eine SD-Karte mit mindestens 2 GB Speicherplatz. Optimalerweise sollte sie mehr als 2 GB haben, am besten 32 GB.

## Windows:

Um die SD-Karte auf "Fat32" zu formatieren, führe die folgenden Schritte aus:

1. Rechtsklicke auf die SD-Karte und wähle "Formatieren".
2. Wähle als Dateisystem "Fat32" aus und klicke auf "Formatieren". 
   
   **Hinweis:** Wenn "Fat32" nicht als Option angezeigt wird, öffne die Eingabeaufforderung (cmd) als Administrator und führe die folgenden Befehle aus:

   ```sh
   diskpart
   list disk
   sel disk 2   // Wähle die Nummer der SD-Karte, z.B. Disk 2
   format fs=fat32 quick

Falls du eine SD-Karte hast, die größer als 32 GB ist und dein 3DS sie nicht erkennt, lade das Programm "Fat32 Format" herunter (von beliebiger Quelle). Wähle deine SD-Karte aus und setze die Größe auf 32768, um sie auf 32 GB zu begrenzen.

## Linux:

Um die SD-Karte in Linux zu formatieren, führe diese Schritte aus:

1. Öffne das Terminal und führe `lsblk` aus, um die Disk-Informationen zu erhalten.
2. Wähle die SD-Karte aus, indem du `sudo fdisk /dev/disk1` eingibst (ersetze `disk1` durch den tatsächlichen Namen der SD-Karte)
3. Führe diesen Befehl aus, um die Partition in FAT32 zu formatieren:

   ```bash
   sudo mkfs.vfat -F 32 /dev/disk1

## macOS:

Um in macOS die SD-Karte in FAT32 zu formatieren, führe diese Schritte aus:

1. Öffne das Terminal und schreibe `diskutil list`, um die Infos für die Disk zu bekommen.
2. Unmounte die SD-Karte zuerst mit `diskutil unmountDisk /dev/disk1` (ersetze `disk1` durch den tatsächlichen Namen der SD-Karte).
3. Führe dann den Befehl aus, um die SD-Karte in FAT32 zu formatieren: `diskutil eraseDisk FAT32 namedersdkarte MBRFormat /dev/disk1`.

# 3DS Setup

1. Stecke die SD-Karte in deinen 3DS und warte, bis die Daten auf die SD-Karte erstellt wurden.
2. Gehe auf Mii Maker und warte, bis die Daten dafür angelegt wurden, wenn sie nicht schon vorhanden sind.
3. Gehe auf die Systemeinstellungen, wähle "Allgemeine Einstellungen" aus und gehe dann ganz rechts auf "System-Update" (du müsstest auf v.11.17.0-50 sein; der Buchstabe hinter der Zahl zeigt nur die Region an).4
4. In den Systemeinstellungen gehe auf Datenverwaltung. Entferne deine SD-Karte und stecke sie in deinen PC (Du solltest deinen 3DS eingeschaltet lassen).

# SD Karten Vorbereitung

1. Lade die 3DS Modding Setup Daten aus der "Downloads.txt" Datei herunter und entpacke sie.
2. Installiere Python von der offiziellen Webseite.
3. Platziere den "dbs" Ordner im Nintendo 3DS Ordner, in den beiden Unterordnern mit den langen Ziffern, wo sich auch der Ordner "extdata" befindet.
4. Kopiere alle Daten aus dem "SD" Verzeichnis direkt ins Stammverzeichnis der SD-Karte.
5. Packe die SD Karte in den 3DS.

# Payload Vorbereiten

1. Gehe auf deinem 3DS in den Systemeinstellungen auf Datenverwaltung (wo wir schon sein müssten), wähle "Software" und dann "Zurücksetzen" (deine Daten werden nicht gelöscht).
2. Entferne danach deine SD-Karte und stecke sie in deinen PC.

# Payload einfügen

1. Öffne die Datei "mset9.bat" (in Windows), "mset9.py" (in Windows und Linux) oder "mset9.command" (in macOS).
2. Wähle im Script aus, ob du einen New 3DS oder Old 3DS hast.
3. Wähle dann "Inject MSET9 Payload".
4. Stecke die SD-Karte wieder in den 3DS ein (lass den 3DS eingeschaltet).

# Payload laden

1. Gehe auf dem 3DS in die Datenverwaltung und wähle "Zusatzdaten".
2. Gebe die oben angezeigte Tastenkombination ein.
3. Nachdem der 3DS neu gestartet ist, schalte ihn aus.

# Payload Entfernen

1. Stecke die SD-Karte wieder in deinen PC.
2. Öffne erneut das mset9 Script.
3. Wähle deine 3DS-Version erneut aus.
4. Wähle "Remove MSET9 Payload".
5. Stecke deine SD-Karte wieder in den 3DS.

# Aktiviere "Enable loading external FIRMs and modules" und "Enable Game patching" um Mods zu installieren

1. Halte vor dem Starten die "Select"-Taste gedrückt, um in den "Luma3DS Firmware"-Konfigurationsmodus zu gelangen.
2. Setze ein Haken bei den Optionen, die in dieser Überschrift genannt sind.
3. Starte den 3DS anschließend neu.

# Dump DSP Firmware

1. Drücke gleichzeitig "L + Steuerkreuz Unten + Y".
2. Wähle "Miscellaneous Options".
3. Wähle dann "Dump DSP Firmware und Nullify User Time Offset".

# Homebrews und zusätzliche Software installieren

1. Halte vor dem Starten des 3DS die "Start"-Taste gedrückt, um in den "GodMode9" zu booten.
2. Wähle dann die "Home"-Taste.
3. Wähle "Scripts".
4. Wähle dann "Finalize (Backup auch automatisch die NAND)".
5. Drücke nur "A" und anschließend die Tastenkombination, die auf dem unteren Bildschirm angezeigt wird.
6. Starte deinen 3DS neu.
7. Öffne "FBI".
8. Gehe zu "SD".
9. Gehe dann zu "CIAs".
10. Wähle "<current directory>".
11. Wähle "Install and Delete all CIAs".

# Backup der NAND (Manuell)

1. Starte erneut GodMode9 beim Starten des 3DS.
2. Drücke die "Home"-Taste.
3. Wähle "Scripts".
4. Wähle dann "GM9Megascript".
5. Wähle schließlich "Backup Options".
6. Wähle "SysNAND".
7. Schalte den 3DS aus.
8. Stecke die SD-Karte in deinen PC.
9. Gehe auf der SD-Karte in den Ordner "gm9" und dann in den Ordner "out".
10. Speichere die Dateien `.bin`, `.bin.sha` und `.exefs` in einen Backup-Ordner.








