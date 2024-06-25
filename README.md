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
