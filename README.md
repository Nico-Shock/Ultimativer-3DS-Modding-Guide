Hier ist das beste Tutorial, um den 3DS zu modden: Es enthält alle notwendigen Schritte und Bilder, die du benötigst.

# 3DS SD Karten Setup

Du benötigst eine SD-Karte mit mindestens 2 GB Speicherplatz. Optimalerweise sollte sie mehr als 2 GB haben, am besten 32 GB.

2. Windows:

Um die SD-Karte auf "Fat32" zu formatieren, führe die folgenden Schritte aus:

1. Rechtsklicke auf die SD-Karte und wähle "Formatieren".
2. Wähle als Dateisystem "Fat32" aus und klicke auf "Formatieren". 
   
   **Hinweis:** Wenn "Fat32" nicht als Option angezeigt wird:
   - Öffne die Eingabeaufforderung (cmd) als Administrator.
   - Gib die folgenden Befehle ein:

     ```
     diskpart
     list disk
     sel disk 2   // Wähle die Nummer der SD-Karte, z.B. Disk 2
     format fs=fat32 quick
     ```

Stelle sicher, dass du die richtige Disk-Nummer für deine SD-Karte auswählst.

