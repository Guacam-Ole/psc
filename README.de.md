# psc-Importer für Wordpress
Kleines Script zum auslesen von PSC-Dateien in Wordpress

# Warnung
Benutzung auf eigene Gefahr! Keine Garantie für Schäden, verlorene Beiträge, weggelaufene Katzen, o.ä.

## Was macht das Script?
Es liest eine beliebige PSC (Podlove simple Chapter) - Datei ein und zeigt sie im Wordpress-Beitrag an

### Installation
1. Kopiere den psc-Ordner nach wp-content/plugins
2. Aktiviere das Plugin

### Konfiguration
Es gibt drei Variablen im Code, die sich anpassen lassen:
 $pscClass="entry-meta";
 $pscHeader="Pingbacks:";
 $pscUrlsOnly=true;

```php
$pscClass
```
Definiert die CSS-Klasse, die für das DIV verwendet wird.
```php
$pscHeader
``` 
Die Überschrift

```php
$pscUrlsOnly
```
Wenn *true*: Zeigt nur Einträge mit URLs an
Wenn *false*: Zeigt alle Einträge an

### Benutzung
Füge `[PSC]yourUrl[/PSC]` irgendwo im Artikel ein.
Beispiel: `[PSC]http://cdn.podseed.org/blathering/blathering_008.psc[/PSC]`

Nach dem speichern sollte der PSC-Bereich ersetzt worden sein mit dem Inhalt der PSC-Datei

### Fehler
Falls ein Fehler auftritt, sollte er an der PSC-Stelle angezeigt werden

### Leichte Installation
Gibt es nicht :) Du wirst das Plugin nicht bei Wordpress finden. 



