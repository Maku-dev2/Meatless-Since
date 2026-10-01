# Meatless Since

**Deutsch** · [English](#english)

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

---

<a id="english"></a>

[Deutsch](#meatless-since) · **English**

A meat-free tracker in a single HTML file: it counts the days since you last ate meat and works out what that means for animals, climate, water, land and your wallet. The interface is available in German and English.

## Features

- **Today**: A counter since your start date and a 30-day window instead of a streak. A meat day costs one dot and never resets anything to zero. Meals can be logged after the fact too (plant-based, with eggs/dairy, fish, meat, can't remember).
- **Journey**: A timeline of milestones in the categories body, habit, animals, planet and money. Milestones tied to a quantity move with how much meat you used to eat.
- **Nutrition**: Which nutrients need more attention on a vegetarian diet. This is explicitly not medical advice and states no dosages.
- **Caveats**: The case against the app's own numbers, deliberately given in full.
- **You**: Edit your setup, language, units (metric/imperial), your own prices, light/dark mode, export and restore a backup, reset everything.

Setup asks for four things: your start date, how much meat you ate before (defaults for the US, Germany and the global average), what replaced it (pulses, tofu, eggs, cheese, meat substitutes, nuts) and which number goes on top.

## Data sources

Figures come from Poore & Nemecek 2018 (emissions, land, water), Scarborough et al. 2023 (measured diets, which anchor the climate counter) and FAO statistics, among others. Behind every figure, a “?” explains its value, source, method and limits.

## Usage

Open `index.html` in a browser. There is no build step and no dependencies apart from Google Fonts. Until you enter your own numbers, the app shows five months of sample data.

Data is saved in the browser's `localStorage`. When the page runs as a Claude artifact, it also uses the page's own store, which syncs across devices. If you rely on browser storage alone, make regular backups via “Show backup”.
