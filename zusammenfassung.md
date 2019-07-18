# Fragen

MM kommt nicht dran.

----
| SAP | Erläuterung | real-life |
|-----|-------------|----|
| Mandant | übergeordnetes Element aller Organisationseinheiten | Unternehmen |
| Buchungskreis | Eine bilanzierende Einheit im Sinne einer rechtlich selbstständigen Firma oder Tochter mehrere Buchungskreise pro Mandant (für nationale Bilanzierungsrichtlinien) | Firma / Tochter |
| Werk | ???? Fabrik die mit der Herstellung von Gütern / Dienstleistungen beauftragt ist  | Fabrik |
| Verkaufsorganisation | Zuständig für den Verkauf bestimmter Produkte / bereitstellung von DL | Verkaufs-orga|
| Sparte | OE mit Vertriebsverantwortung für bestimmte Materialien oder DL \n untergliedert Vertriebs-organisation Ermöglicht Gliederung des Produktspektrums | Abteilung/ Sparte/ Geschäftsbereich
| Lagerort | OE zur Abgrenzung von Materialien | Lager |

-------
#### ? - Definiere Begriffe Buchungskreis, Lagerort, Arbeitsplatz mit eigenen Worten und beschreibe die Zusammenhänge
Buchungskreis kleinste OE für die eine Bilanz / Abrechnung erstellt werden kann. / rechtliche Einheit
Lagerort : OE zur trennung von Lagerbeständen innerhalb eines Werkes. Räumlich abgegrenzt in dem materialien für Produktionsbetrieb aufbewahrt werrden,
Ort der Leistungserbringung Wertschöpfung


#### ? - Nenne und erkläre 3 SAP Transaktionen, die die Integration mit anderen Unternehmensbereichen aufzeigen. Wie sind die Bereiche miteinander integriert?

- **Rechnungen im Vertrieb** -> generieren FI Hauptbuchbeleg über Verkauf  
 Debitorenbuchhaltung integriert Vertrieb mit Finanzbuchhaltung indem Informationen über Umsätze und Zahlungen im Bezug auf Kunden, Waren und DL verarbeitet werden

-  **Einkaufs- und Wareneingangsaktivitäten** in der Materialwirtschaft  (MM) generieren Hauptbuchbelege im FI  
Kreditorenbuchhaltung

- Absatz und Produktionsgrobplanung
  - integriert Informationen aus allen Bereichen

- Bestellanforderung(BANF) - geht aus von Materialwirtschaft betrifft Vertrieb der Lieferant beauftragt

- Produktionsauftrag - MM beauftragt PP

#### ? - Welche Aktivitäten werden im SAP-System bei einem Warenausgang zu einem Kundenauftrag ausgeführt?  
Der Bestand wird reduziert und die Selbstkosten geschrieben.  
Kontendaten werden Aktualisiert  
Der Versandvorgang wird beendet

#### ? - erkläre Profit Centre und Kostenstelle mit Beispiel
Kostenstelle: Ort der Kostenentstehung / Leistungserbringung

ProfitCentre -> Buchungskreise


#### ? - Was ist ein Debitor?
Der Debitor ist ein Kunden

Kreditoren sind Lieferanten
  - **K**reditoren sind **k**eine **K** unden

#### ? - Was sind Stamm und Bewegungsdaten jeweils ein Beispiel aus Fallstudien
Stammdaten:  
  - längerfristige Daten
  - repräsentieren Datensätze
  - Bsp. Kundenstammdaten / Material-/ Konditions-

Bewegungsdaten:  
  - Vorgangsbezogene Daten (auch Transaktionsdaten)
  - kurzlebig
  - werden bestimmten Stammdaten zugeordnet
  - beinhalten meist OEbene, Stammdaten, SituationsbedingteDaten
  - Bsp. Kundenauftrag (bezieht sich auch Kunden- und Materialstammdaten)  

#### ? - Erkläre das Belegprinzip + zwei Beispiele für Belege

- Bei Bestellung entsteht Rechnungsbeleg
- Bestellanforderung (interner Beleg der den Einkauf Anfordert)


#### ? - nenne drei Anwendungen die neben SAP anwendung finden und es richtung integriertes Lieferketten Management erweitern
Orderbuch



#### ? - Beispiele für einstufige und Mehrstufige Stückliste
Liste aller Komponenten aus denen ein Produkt oder eine Baugruppe besteht


#### ? - Nenne die OE die einen Vertriebsbereich im SAP definieren
1. Verkaufsorganisation
2. Vertriebsweg
3. Sparte


#### ? - Was ist eine Transaktion + Beispiele
Eine Folge zusammenhängender Dialogschritte für einen in sich geschlossenen betriebswirtschaftlichen Vorgang.
Bildschirmmasken werden mit ihrer  Ablauflogik als _dynamisches Programm_ bezeichnet
Aufruf über Transaktionscode oder Easy Access
- Kundenauftrag anlegen
- Zahlungseingang buchen


#### ? - Customizing
Transformation der Standardsoftware aus Auslieferungszustand zu im Anwenderunternehmen gewünschten Soll-Zustand.  
Quellcode wird nicht verändert


#### ? - Nenne 4 SAP-Module + Komponenten
1. Vertrieb (SB)
  - Kundenauftrag, Terminauftrag, Bestandsübersicht
2. Finanzwesen (FI)
  - Belegübersicht, Kontenprinzip
3. Materialwirtschaft (MM)
  - Einkauf, Material, Orderbuch
4. Produktionsplanung und -steuerung (PP)
  - Stückliste, Arbeitspläne, Erzeugniskalkulation

#### ? - Hilfefunktion
F1 - Bedeutung von Feldern und technischen Informationen  
F4 - Eingabemöglichkeiten Anzeigen

------
## SD --- Vertrieb

### SD - Funktionalität
- Vertriebsunterstützung
- Verkauf
- Versand und Transport
- Fakturierung
- Kreditmanagement
- Außenhandel

### SD - Organisationsstruktur
- **Mandant**
  - betriebwirtschftl. größte verbindlichkeit
  - Global Bike Group
- **Buchungskreis**
  - betriebwirtschftl. kleinste Einheit
  - Global Bike Germany; Global Bike Inc.
- **Kreditkontrollbereich**
 - OE gewährt und überwacht Kreditlinien
- **Verkaufsorganisation**
  - OE verantwortlich für Verkauf von Produkten und DL
  - Verantwortung für verkaufte Produkte (rückgriffsrechte des Kunden)
  - DE Nord; DE Süd
- **Vertriebsweg**
  - Wie gelangen Produkte zum Kunden
  - Großhandel oder Endkundenverkauf
- **Sparte**
  - Gruppierung von Materialien / DL
- **Vertriebsbereich**
  - Kombiniert Verkaufsorganisation, Vertriebsweg und Sparte
- **Werk**
  - von wo werden güter geliefert
- **Andere**
 - Ladestelle, Verkaufsbüro... (Leipzig)

### SD - Stammdaten


1. **Kundenstammsatz**
  - Alle Infos zu Aufträgen, Lieferungen, Rechnungen, Zahlungen
  - anlegbar durch Verkaufsorga., Vertriebsweg, Sparte
     - Allg Name Adresse
     - Buchungskreisspezifisch = Konten
     - Vertriebsbereichspez. = Verkaufsbüro


2. **Materialstammsatz**
 - siehe MM


3. **Konditionsstammsatz**
 - Preise, Zuschläge, Rabatte
 - mögliche Abhängikeiten von Material oder Kunden


### SD - Prozesse


1. **Vorverkaufsaktivitäten**
  - CRM-Light (Unterstützt beim Verkauf, Versand und Marketing)
  - Funktionalitäten:
     - Kundenkontakt - Herstellung und Aufrechterhalten (Aufzeichnen Telefon, Briefe, Treffen)
     - Durchführung und Verfolgen von FachmesseKampagnen
  - Verkaufsdokumente = Anfragen(nicht beindend) und Angebote (bindend)
  - Benötigt Infos über: *Vergangene Verkäufe*, *vergangene Kommunikation*, *Kontaktinfos*


2. **Kundenauftrag**
  - erstelltes Dokument enthält alle Infortmationen um Kundenanfrage bearbeiten zu können:
    - Kundeninfos
    - Material/DL und Menge
    - Lieferinfos
    - Preise
  - Kopfbereich -> relevante Kopfdaten
  - Positionen
  - Lieferplaneinteilung
    - bestimmung von Lieferterminen, Availability to Promise Datum ermitteln
  -  Zwei Wege:   
**Rückwärtsterminierung**
  - Ausgehen von Wunschlieferdatum
**Vorwärtsterminierung**
 - Ausgehen von Materialbereitstellung

  + Versand und Routenfindung

3. **Verfügbarkeit prüfen**
  - Bestimmen des Materialverfügbarkeitsdatums
  - Berücksichtigen von Lagerbewegungen
    - Einmallieferung
    - Komplettlieferung
    - Liefervorschlag

**Beginn des Auslieferungsprozesses ist die Erstellung des Lieferscheins**

4. **Materialbereitstellung**
 - **Prozess** "Erstellung der Lieferung"

5. **Verpacken / Verladen**


6. **Warenausgang**
  - Ergeignis - gesetzliche Änderung der besitzverhältnisse
  - Reduziert Bestand und schreibt Selbstkosten
  - Aktualisiert Kontendaten
  - Beendet Versandvorgang


7. **Rechnung (Fakturierung)**
  - Daten aus Kundenauftrag / Lieferschein kopieren
  - aktualisieren kreditstatus


8. **Zahlungsbestätigung**
  - Buchen der Zahlung gegen die Rechnung
  - Buchhaltung


XX. **Belegfluss und Auftragsstatusfunktion:**  
Erlaubt mir den Status eines Auftrags zu jedem beliebigen Zeitpunkt zu finden. SAP aktualisiert den Auftragsstatus sobald eine Änderung in einem Dokument im Kundenauftragszyklus vorgenommen wurde (Order to Cash).

-------
## MM --- Materialwirtschaft

### Funktionalität
- Bestandsführung
- Einkaufsabwicklung
- Materialbedarfsplanung
- Materialbewertung
- Rechnungsprüfung

### Organisationsstruktur
**Materialwirtschaft**

-   **Mandant**
  - Betriebswirtschaftlich größte Einheit
- **Buchungskreis**
  - betriebswirtschftl. kleinste Einheit für die eine in sich geschlossene Buchhaltung abgebildet werden kann
- **Werk**
  - Betriebsstätte oder Tätigkeitsbereich zur *Produktion, Distribution, Beschaffung und/oder Instandhaltung*
- **Lagerort**
  - Organisatorische Einheit - Unterscheidung von Beständen innerhalb eines Werkes

**Beschaffung**
- **Einkaufsorganisation**
  - Einkaufsaktivitäten eines Werkes
  - verantwortlich für Beschaffung
- **Einkäufergruppe**
  - Schlüssel für Einkäufer die für bestimmte Einkäufe zuständig sind - kommunikationskanal

### MM - Stammdaten
1. **Lieferantenstammsatz**
  - Infos über externe Zulieferer
  - Allg. Daten = Adresse...
  - Buchungskreisdaten     = Kontendaten
  - Einkaufsorganisationsdaten      = Ansprechpartner


2. **Materialstammsatz**
  - Quelle für Materialbezogene Stammdaten (gespeichert in Sichten)
  - wird von den meisten Komponenten verwendet
  - Grunddaten, Bestand, Qualitätsmanagement,..
    - Allg. Daten = Bezeichnung, Gewichte   
    - Vertriebsspezifisch = Auslieferungswerk
    - Lagerortspezifische Infos = Bestand


3. **Einkaufsinfosatz**
 - Rahmenbedingungen für Bestellungen
 - Infos über Beziehung zwsichen Lieferanten und Material
 - kann automatisch erzeugt werden


4. **Konditionsstammsatz**
 - siehe SD

### MM - Prozesse

1. Bestellanforderung
 - kann automatisch aus Materialbedarfsplanung/ Fertigungsauftrag/ Kundenauftrag entstehen
  - Bezugsquelle ermitteln (Orderbuch, Ausschreibung, Interne Beschaffungsanforderungen)

2. Lieferantenauswahl
3. Bestellung
 - formale Anforderung (Kopfdaten, Übersicht, Belegpositionen)
 - Zwecke einer Bestellung (Standard (Lager oder Verbrauch); Dienstleistungen; Lohnbearbeitung)
4. Benachrichtigung Lieferant
5. Versand der Waren
6. Wareneingang
 - verbuchung des Erhalts
 - Effekte:
    - Materialbeleg
    - Buchhaltungsbeleg
    - aktualisierunge Bestandsmengen
    - Bestandswerte aktualisiert
    - Bestellung aktualisiert
    - Output (Begleitschein)
7. Rechnungsprüfung
 - Inhalt Preis Berechnung etc
 - sicherung erzeugt verbindlichkeit
8. Zahlungsabwicklung
 - erzeugt Finanzbuchhaltungsbeleg der Transaktion dokumentiert


## FI -- Finanzen

_Das FI-Modul ist komplett mit anderen FI Modulen integriert_

### Ziele
1. Sammeln von _Transaktionsdaten_ => Basis für Standardberichte (häufig gerichtet an Externe)
2. Standardberichte enthalten
  - Bilanz
  - GuV
  - Kapitalflussrechnung
 Adressaten:
   - Intern
     - Führung
     - MA
     - Verwaltung
  - Externe
    - Banken
    - Aktionäre
    - Medien

3. Bildet Rahmen für Finanzentscheidungen
4. Erlaubt Sammlung von geschäftlichen Infos
5. Unterstützt Darstellung der Infos


### Organisationsstruktur


1. Mandant
2. Buchungskreis
3. **Kontenplan**
  - _Global Bike Kontenplan_
  - Systematik aus Hauptbuch-Konten
     - verwendet durch 1 oder mehr Buchungskreise  
  - Bietet Rahmen für Aufzechnung von Werten um geordnete Darstellung zu gewährleisten
4. **Geschäftsbereich**
  - _Fahrräder_
  - OE die einen seperaten Bereich der Geschäftstätigkeiten/Verantwortlichkeiten innerhalb der Orga darstellt und dem **Wertänderungen zugeordnet** werden können
5. **Kreditkontrollbereich**
  - _Globale Kreditkontrolle_
  - OE die Kreditlinien gewährt und überwacht
  -  1 oder mehr Buchungskreise


### FI - Stammdaten

- **Hauptbuchkonten** (General Ledger)
  - Jede eindeutige Kombination von Buchungskreis und Kostenplan - in diesen werden Finanztransaktionen gespeichert
- Alle Buchunungen die die Konten im Kontenplan beeinflussen
-  vorbereitung der Bilanzerstellung


- **Debitoren- und Kreditorenkonten**
  - Konten von Kunden und Lieferanten
  - Debitorenbuchhaltung:
    - Umsätze und Zahlungen
    - **Integration** zwischen Vertrieb (SD) und FI
    - Ausgelößt durch Rechnung in SD
  - Kreditorenbuchhaltung
    - Infos zu Lieferanten
    - **integration** zur Materialwirtschsft
    - Einkaufs und Wareneingangsaktivitäten im **MM** generieren Hauptbuchbeleg


### FI - Prozesse
Buchung eines Sachkontenbelegs

#### FI - Reporting
- Sachkontensoldenanzeige
- Bilanz
  - Vermögen
  - Verb.
  - EK
- GuV
  - Darstellung Aufwendungen / Erträge über Periode
- Kapitalflussrechnung
 - Zu- und Abflüsse in bar über Periode


#### Buchungskontrolle und Historie
 - _Audit Trails_

### Das SAP Belegprinzip

Bei jedem Geschäftsvorfall der Auswirkung auf FI hat werden Daten eindeutig in der SAP Datenbank fortgeschrieben.  
- Belegnummer ermöglicht später Geschäftsvorfall zu finden
- Beleg enthält:
   - Verantwortliche Person
   - Datum / Uhrzeit
   - Betriebswirtschaftliche Datenbank
- Kann nicht gelöscht werden   

**bietet Rahmen für internes Kontrollsystem (gesetzlich gefordert)**


## PP -- Produktionsplanung und Steuerung

### Funktionalität
SAP teil Produktion in verschiedene Prozesse ein:
1. Produktionsplanung
2. Produktionsdurchführung (diskrete- / Serienfertigung)
3. Produktion in der Prozessindustrie


### Organisationsstruktur

1. Mandant
2. Buchungskreis
3. Werk
  - Betriebsstätte oder Tätigkeitsereich zur Produktion, Disposition, Beschaffung und / oder Instandhaltung
  - _z.B. Dallas_
4. Lagerort
  - OE die eine Unterscheidung von Beständen innerhalb eines Werkes ermöglicht
  - z.B. _Rohstoff_ , _Fertigerzeugnis_
5. Arbeitsplatz (zählt im SAP zu Stammdaten)
  - OE die definiert wo und wann ein Arbeitsablauf durchgefürt wird.
  - hat gegebene Kapazität
  - durchgeführte Aktivitäten werden mit Verrechnungssätzen bewertet die durch Kostenstellen und Leistungsarten bestimmt werden.
  - können Maschinen, Personen, Produktionslinien oder Mitarbeitergruppen sein.
 - z.B. _Montage, Verpacken, Prüfen_


### Stammdaten

- Materialstammdaten
- **Stückliste**
  - Liste aller Komponenten aus denen ein Produkt oder eine Baugruppe besteht
  - einstufig oder mehrstufig
    - Bsp. Einstufig: Fertiges Fahrrad <- Komplettrad, Pedale, Rahmen, Garantie, Verpackung, Bremsen, Sitz...
    - Bsp. Mehrstufig: Fertiges Fahrrad <- Rad (Reifen, Schlauch, Felge), Lenker (griffe, Bremsgriff, Vorbau), ...
  - es gibt verschiedene **Positionstypen**:
    - Lagerposition, Dokumentposition, Rohmaßposition - Stahlblech
- **Arbeitsplan**
  - Nutzen:
    - Planung von Herstellung von Materialien (Produkten)
    - verwendung als Vorlage für Produktionsaufträge und Terminierung.
    - dienen auch als Grundlage für Erzeugniskalkulation
  - Serie von aufeinander folgenden Schritten ( Vorgängen ) die durchgeführt werden _müssen_ um ein bestimmtes Produkt zu produzieren.
  - Was, Wann, Wo, Wie, Zeit
- **Arbeitsplatz**
  - Ort in einem Werk an dem ein Mehrwert (Vorgänge oder Aktivitäten) erbracht wird
  - Definiert kapazitäten von:
    - Manuelle Arbeit
    - Maschine
    - Leistungsausbringung
    - Emissionen
  - Kapazitäten werden verwendet bei:
    - Kapazitätsplanung
    - Feinplanung  
    - Kalkulation
  - Folgende **ressourcen-bezogene Daten** werden erfasst:
    - Grunddaten (Verantwortliche, Ort)
    - Terminierungsdaten (Liege und Transportzeiten, Formelschlüssel)
    - Kalkulationsdaten (Kostenstelle)
    - Personaldaten
    - Kapazitätsdaten
- **Produktgruppe**
  - Gesamtplanung / Fasst Material- und andere Produktgruppen zusammen
  - ein oder mehrstufig (letzte Stufe immer Material)


### PP - Prozesse

##### 1. **Materialplanung**


- **Prognose**
  - Grundlage für Absatz und Produktionsgrobplanung
  - Wichtig um Über oder Unterbestände im Lager zu vermeiden
  - immer falsch
  - Trend, Saison, Trend + Saison, Konstant
- **SOP  Absatz und Produktionsgrobplanung**
  - Flexibles Planungs- und Prognosewerkzeug
  - Informationen aus Vertrieb, Marketing, Produktion, Rechnungswesen, Personalwirtschaft
  - i.d.R. drei schritte:
    1. **Absatzplan**
    2. **Produtionsplan**
    3. **Kapazitätsgrobplanung**

- **Programmplanung**
  - Verbindet SOP und Feinplanung (MPS, MRP)
  - Ergebnisse der Programmplanung werden als **Produktionsprogramm** bezeichnet und basierend auf unabhängigen Anforderungen generiert
    - Primärbedarf (aus Prognose) und Kundenbestandsabgleich (Absatz) ?!

    - Es gibt verschiedene Planungsstrategien (setzen Produktionsmenge und Termine) zum Beispiel:
      - Lagerfertigung (Make-to-Stock MTS) - unabhängiger Bedarf
      - Kundeneinzelfertigung (Make-to-Order MTO) - Planung durch Kundenaufträge

  - **Leitteileplanung (MPS)**
    - ermöglicht bei den Planungsmethoden zwischen Materialisen die starken Einfluss auf Gewinn haben / kritische Ressourcen verwenden zu unterscheiden.
- **Materialbedarfsplanung (MRP)**
  - plangesteuerte Ditribution - System berechnet Nettobedrf unter Berücksichtigung des Lagerbestands und terminiert Zugänge aus EInkauf und Produktion
  - plant alle Ebenen der Stückliste
  - sichert die Verfügbarkeit von Materialien basierend auf dem durch die MPS oder Programmplanung ermittelten Primärbedarf
    1. Nettobedarfsrechnung
    2. Losgrößenberechnung
      - statisch, periodisch, optimum
    3. Beschaffungsart
     - fremd (Bestellung), intern ((Plan- Fertigungs-, Prozess- Auftrag)  

     **Plan- oder verbrauchsgesteuerte Disposition**  
      hängt von MRP-Typ ab

|  Plangesteuert | verbrauchsgesteuert |
| ------------- | ------------------- |
| MRP | Meldebestand |
| Saisonales MRP | Prognosebasiert |
|  | Wiederbeschaffung |


  - Planauftrag (Planung) wird zu Fertigungsauftrag (Steuerung) oder Bestellung (Steuerung)

  - Fertigungsauftrag
       - Eine interne Anforderung ein bestimmtes Produkt zu Termin zu produzieren
      - Definiert:
        - Material, Menge, Werk, Rahmenzeiten, Kosten  
     --> lößt Fertigungsprozess aus   
     - Bestellung
       - Eine Anforderung an einen Lieferanten ein Material oder DL zu Zeitpunkt zu liefern

        4. Terminierung
          - Berechnet Produktionstermine und Kapazitätsanforderungen für alle Vorgänge eines Auftrags
          -  Bestimmt Arbeitsplan
          - Nach freigabe Erstellung von:
            - Vorgangsbasierte Listen (Lohnschein, Rückmeldeschein)
            - Komponentenbasierte Listen (Materialentnahmeschein)
            - Fertigungshilfsmittellisten
            - Sonstiges (Steuerkarte)
        5. Stücklistenauflösung



##### 2. **Produktionsplanung**

##### 3. **Produktionsdurchführung**

Verfügbarkeitsprüfung
  - Automatisch: stehen Komponenten, Ressourcen, Kapazitäten zur verfügung
  - Erzeugt Verfügbarkeitsprotokoll mit Fehlteileliste

**Rückmeldung**  
Werden verwendet, um den Verlauf eines Auftrages im Produkionszyklus zu überwachen und zu verfolgen.
- eine korrekte Rückmeldung kurz nach Abschluss eines Vorgangs ist für eine realistsische Produktionsplanung und -steuerung unerlässlich.
- Enthalten sein müssen:
    - Mengen
    - Kontrolldaten zur Leistungsarten
    - Termine
    - Personaldaten

**Wareneingang**:
Empfang der bestätigten Fertigungsmenge aus der Produktion in den Bestand.  
Auswirkungen:
-  Aktualisiert Bestandsmenge
- Aktualisiert Bestandswert
- Speichert Preis
- Aktualisiert Fertigungsauftrag   

**Drei** Dokumente werden erstellt:
 - Materialbeleg
 - Finanzbeleg
 - Kostenrechnungsbeleg


**Auftragsabrechnung**
Abrechnung der tatsächlichen Kosten im Auftrag für einen oder mehrere Empfänger ( ein Material, eine Kostenstelle, ein Innenauftrag, ein Kundenauftrag, ein Project, you name it)
Parameter:
 - Abrechnungsprofil (Empfänger, aufteilungsregeln)
 - Abrechnungsstruktur (zuordnung der Kosten)
 - Abrechnungsvorschrift
