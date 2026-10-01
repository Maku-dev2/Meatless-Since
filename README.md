# Meatless Since

Ein fleischfrei-Tracker als einzelne HTML-Datei: Er zählt die Tage seit dem letzten Fleisch und rechnet aus, was das für Tiere, Klima, Wasser, Fläche und Geldbeutel bedeutet. Die Oberfläche gibt es auf Deutsch und Englisch.

## Funktionen

- **Heute**: Zähler seit dem Startdatum und ein 30-Tage-Fenster statt einer Serie. Ein Fleischtag kostet einen Punkt und setzt nichts auf null zurück. Mahlzeiten lassen sich auch rückwirkend eintragen (pflanzlich, mit Ei/Milch, Fisch, Fleisch, weiß nicht mehr).
- **Weg**: Eine Zeitleiste mit Meilensteinen in den Kategorien Körper, Alltag, Tiere, Planet und Geld. Meilensteine, die an Mengen hängen, verschieben sich mit dem früheren Fleischkonsum.
- **Nährstoffe**: Hinweise, auf welche Nährstoffe man bei vegetarischer Ernährung achten sollte. Das ist ausdrücklich keine medizinische Beratung und nennt keine Dosierungen.
- **Einwände**: Gegenargumente und Grenzen der eigenen Zahlen, absichtlich vollständig aufgeführt.
- **Du**: Angaben ändern, Sprache, Einheiten (metrisch/imperial), eigene Preise, Hell-/Dunkelmodus, Sicherung exportieren und einspielen, alles zurücksetzen.

Bei der Einrichtung gibt man vier Dinge an: das Startdatum, die frühere Fleischmenge (Vorgaben für USA, Deutschland und den Weltdurchschnitt), womit das Fleisch ersetzt wurde (Hülsenfrüchte, Tofu, Eier, Käse, Fleischersatz, Nüsse) und welche Zahl oben stehen soll.

## Datengrundlage

Die Werte stammen unter anderem aus Poore & Nemecek 2018 (Emissionen, Fläche, Wasser), aus Scarborough et al. 2023 (gemessene Ernährungsmuster, an denen der Klimazähler verankert ist) und aus FAO-Statistiken. Hinter jeder Kennzahl erklärt ein „?“ Wert, Quelle, Methode und Grenzen.

## Nutzung

`index.html` im Browser öffnen. Es gibt keinen Build-Schritt und keine Abhängigkeiten außer Google Fonts. Ohne eigene Angaben zeigt die App Beispieldaten von fünf Monaten.

Gespeichert wird im `localStorage` des Browsers. Wenn die Seite als Claude-Artifact läuft, kommt zusätzlich der Datenspeicher der Seite hinzu, der die Daten zwischen Geräten synchronisiert. Wer nur den Browser-Speicher nutzt, sollte regelmäßig über „Sicherung anzeigen“ ein Backup machen.
