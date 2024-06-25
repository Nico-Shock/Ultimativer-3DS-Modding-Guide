Hier ist das beste Tutorial, um den 3DS zu modden: Es enthält alle notwendigen Schritte und Bilder, die du benötigst.

# 3DS SD Karten Setup

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

   ## MacOS:

Um in Macos die sd karte in fat32 zu formatieren nutze führe diese schrite aus:

1. öffne das terminal und schriebe "diskutil list" um die infos frü die disk zu bekommen
2. unmounte die sd karte zuerst mit "diskutil unmountDisk /dev/disk1" (ersetze "disk1" durch den tatsächlichen namen der sd karte)
3. führe dann den script aus um die sd karte in fat32 zu formatieren "diskutil eraseDisk FAT32 namedersdkarte MBRFormat /dev/disk1"

