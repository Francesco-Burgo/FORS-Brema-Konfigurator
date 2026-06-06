FORS BREMA EISMASCHINEN KONFIGURATOR – Interner Prototyp
=========================================================

SCHNELLSTART
------------
1. Datei "brema-konfigurator.html" doppelklicken -> öffnet im Browser.
2. Fertig. Logos und alle 92 BREMA-Geräte sind bereits enthalten.
   Mit Internet werden die Produktbilder automatisch live von fors.ch angezeigt.

ORDNERSTRUKTUR
--------------
brema-konfigurator.html        -> Das komplette Tool (eine einzige Datei)
README.txt                     -> Diese Anleitung
assets/logos/                  -> FORS- und BREMA-Logo (für lokale Verwendung)
assets/brema/produktbilder/    -> optionaler alternativer Bildordner
Brema Geräte Bilder/           -> Hier lokale Produktbilder ablegen
   Bilder-Liste.csv            -> Dateiname <-> Original-URL für jedes Gerät

BILDER OFFLINE NUTZEN (optional)
--------------------------------
Standardmässig zeigt das Tool die echten FORS-Bilder online an.
Wer offline arbeiten will:
1. Bilder gemäss "Brema Geräte Bilder/Bilder-Liste.csv" herunterladen
   und mit dem dort angegebenen Dateinamen in den Ordner "Brema Geräte Bilder/" legen.
2. Im HTML (Bereich CONFIG, ganz oben im <script>) setzen:
   ONLINE_BILDER: false

DATEN PFLEGEN
-------------
Im <script>-Block zwischen den Markern:
   ▼▼▼ HIER GERÄTEDATEN PFLEGEN ▼▼▼   ...   ▲▲▲ ENDE GERÄTEDATEN ▲▲▲
Einen { ... }-Block kopieren, einfügen, Werte anpassen.
- aktiv: true / false  -> Gerät ein-/ausblenden
- preisInkl leer lassen -> wird automatisch aus preisExkl + 8.1% MwSt. berechnet
- fehlende Links -> Button wird automatisch deaktiviert ("Link fehlt")

LOGOS TAUSCHEN
--------------
Im <header> die beiden <img>-Quellen (IDs logoFors / logoBrema) auf die
lokalen Dateien umstellen, z.B.:
   src="assets/logos/fors-logo.jpg"
   src="assets/logos/brema-logo.png"

HINWEIS
-------
Die Empfehlung ersetzt keine technische Prüfung vor Angebotserstellung.
FORS AG · Interner Prototyp · BREMA Ice Makers.
