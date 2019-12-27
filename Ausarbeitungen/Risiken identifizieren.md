# Risiken identifizieren

## Arten von Risiken

Zum Einschätzen von Gefahren die zum Ausfall von Geschäftsprozessen führen können, müssen diese vorher identifiziert werden.

### Interne Risiken
Entstehen aus der Unternehmenstätigkeit selber
- Ausfall von Maschinen
- Fehlbedientung von Mitarbeitern bei Vorgängen

### Externe Risiken
Wirken von außen auf eine Institution
- Umweltauflagen können Produktionsprozesse beeinflussen
- Stillstand der Produktion durch Unwetter
- Wechselkursänderung können Produkt unrentabel machen

### Direkt wirkende Risiken
Gefährungen, die unmittelbar zu Ausfällen im Geschäftsprozess führen, sind direkt zu erkennen
- Ausfall Maschine -> Produktionsunterbrechung

### Indirekt wirkende Risiken
Gefährungen, die nicht direkt im Zusammenhang mit einem Ausfall von Geschäftsprozessen stehen
- Stabilität Herstellungsprozess
    - Wartungsintervalle Produktionsanlagen

### Durch Institution beeinflussbare Risiken
Können durch Institution selbst bestimmt werden
- Wartungsintervalle eigener Produktionsanlagen

### Durch Institution nicht beeinflussbare Risiken
Gesetzliche Auflagen haben feste Rahmenbedingungen und wenig Spielraum für eine Institution zur konkreten Umsetzung.

### Höhere Gewalt
- Personalausfall
- Unwetter
- Ausfall von Lieferanten
- Technische Katastrophen

### Organisatorische Mängel
- Fehlbediendung
- Fehlverhalten

### Technisches Versagen
- Ausfall von IT-Systemen
- Stromausfall

### Vorsätzliche Handlungen
- Missbrauch
- Vandalismus
- Diebstahl

### Beispiel
Die RECPLAST GmbH hat bereits bei der Entwicklung ihrer Informationssicherheitskonzepte Risikoanalysen durchgeführt. Ein Teil der Ergebnisse konnte auch bei der Notfallplanung verwendet werden. Zwei mehrstündige Workshops dienten außerdem dazu, weitere Risiken für die als besonders kritisch bewerteten Geschäftsprozesse zu identifizieren, beispielsweise für die Prozesse "Fertigung Endprodukte" und "IT-Wartung" sowie den Server-Betrieb in Bad Godesberg und Bonn-Beuel. Aufgrund der guten Erfahrungen, die bereits mit dieser Methode gewonnen wurden, wurde die Brainstorming-Technik eingesetzt, um mögliche Gefährdungen für die Verfügbarkeit der kritischen Geschäftsprozesse zu finden. Die angesprochenen Risiken deckten das gesamte Spektrum an Gefährdungsszenarien ab, beispielsweise Naturkatastrophen (Erdbeben, Überflutungen – beides kann prinzipiell die Standorte des Unternehmens betreffen), technische Mängel, die einen längeren Produktionsstillstand bewirken können, gezielte Angriffe auf die IT, der Ausfall von Schlüsselpersonen oder von wichtigen Lieferanten.

## Schritt 1: Abgenzung des Analysebereiches
- Bereich spezifizieren, deren Risiken erkannt werden sollen, zB.
    - IT-Systeme
    - Gebäude
    - Infrastruktur
- Festlegen, ob und in welchem Maße diese berücksichtigt werden sollen

## Schritt 2: Identifikation der bedrohten Objekte
- Erfassung aller bedrohten Objekte (Assets), die im Analyseberteich liegen

## Schritt 3: Identifizierung der Risiken zu den Assets
- Mögliche Schwachstellen aller Assets prüfen
- Prüfen, ob vorhandene Schutzmaßnahmen ausreichend sind
- (Grundschutzkataloge BSI)

## Schritt 4: Bewertung der Risiken zu den Assets
- Schadenshöhe für Eintritt aller bekannten Risiken abschätzen
- Wahrscheinlichkeit und Dauer eines Ausfalls beurteilen

## Quellen
[BSI: 4.2 Risiken identifizieren](https://www.bsi.bund.de/DE/Themen/ITGrundschutz/ITGrundschutzSchulung/Webkurs1004/4_RisikenAnalysieren/1_Risiken%20identifizieren/RisikenIdentifizieren_node.html)
[disn-blog](https://www.dsin-blog.de/2014/02/10/it-risikoanalyse/)
[Projektmagazin](https://www.projektmagazin.de/glossarterm/risikoidentifikation)


# Risiken (nur) Identifizieren am Beispiel

## Schritt 1: Abgenzung der bedrohten Objekte
- Es soll eine Benutzerschnittstelle zu einer Serveranwendung im Intranet abgesichert werden, welche keine Benutzeranmeldung erfordert
    - Speiseplan Mensa

## Schritt 2: Identifikation der der bedrohten Assets
- Infrastruktur Server
- Infrastruktur Client
- Serveranwendung
- Browser
- Kommunikationskanal Server <--> Client
- Hardware Server
- Hardware Client

## Schritt 3: Identifizierung der Risiken zu den Assets

Zur Risikoidentifizierung gehört:
- Vollständige Benennung der Risiken
- Ihre Faktoren (Ursachen)
- Ihre Indikatoren (Symptome).

Für eine bessere Übersicht werden die Risiken hier nur benannt, eine vollständige Beschreibung folgt Stichprobenartig während der Präsentation.

- Infrastruktur Server
    - Strom- und Netzwerkausfälle
        - Server
        - Switch
        - Rack
        - RZ
        - Region
    - Ausfall Klimatisierung
        - Klimagerät
        - Serverlüfter für CPU, RAM, PCIe, HDD/SSD/NVMe, Chipsatz
    - Backbone überlastet
- Infrastruktur Client
    - Stromausfall
    - Netzwerkausfall
    - Inkompatible Software
- Serveranwendung
    - Unbehandelter Fehlerfall
    - Unerwartete Benutzereingabe
    - Datenschutz Benutzerdaten
- Browser
    - Keine Unterstützung genutzter Webstandards
    - Darstellungsfehler durch Addons
- Kommunikationskanal Server <--> Client
    - Netzwerkangriffe
    - Blockade durch FW auf Client
    - Verbindungsabbrüche
    - IP-Adressenwechsel bei mobilen Geräten
- Hardware Server / Client
    - Ausfall einzelner Primärspeicher
    - Ausfall einzelner Sekundärspeicher
    - Gleichzeitiger Ausfall von bis zu 3 Sekundärsapeicher
    - Ausfall Backplane für Sekundärspeicher
    - Ausfall Netzteil
    - Ausfall Netzwerkkarte
    - Skalierungseinschränkungen (nur Server)
        - Horizontal
        - Vertikal
    - Kernelpanic durch Hardwaredefekt oder Treiberprobleme
- Hardware Client
    - Ausfall Primär- u. Sekundärspeicher
    - Ausfall Netzteil
    - Anzeigeprobleme Monitor
    - Treiberprobleme Grafikkarte (zB. WebGL)

## Schritt 4: Risikobewertung
Separater Teil des Vortrags
