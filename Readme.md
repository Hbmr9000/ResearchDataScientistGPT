# Sprachmodellbasierter Service für die Auswertung wissenschaftlicher Veröffentlichungen

## Einleitung
Dieses Projekt zielt darauf ab, einen Service zu entwickeln, der wissenschaftliche Veröffentlichungen mittels Sprachmodellen analysiert. Das Ziel ist es, die extrahierten Daten in ein einheitliches Datenbankformat zu überführen und darauf basierend Auswertungen durchzuführen. Dies soll durch den Einsatz von Sprachmodellen wie Langchain oder anderen Sprachmodell Agents realisiert werden.

## Ziele des Projekts
1. Automatisierte Auswertung wissenschaftlicher Veröffentlichungen.
2. Vereinheitlichung der extrahierten Daten in einem gemeinsamen Datenbankformat.
3. Durchführung von Datenanalysen auf Basis der strukturierten Datenbank.

## Schritte zur Umsetzung

### 1. Datenextraktion aus wissenschaftlichen Veröffentlichungen
- Nutzung von Sprachmodellen zur Identifikation relevanter Datenpunkte in den Texten.
- Extraktion und Kategorisierung dieser Datenpunkte.

### 2. Datenaufbereitung und -transformation
- Konvertierung der extrahierten Daten in ein einheitliches Format.
- Validierung und Bereinigung der Daten.

### 3. Datenbankerstellung und -verwaltung
- Entwicklung einer strukturierten Datenbank, die die aufbereiteten Daten aufnimmt.
- Implementierung von Schnittstellen für den Datenzugriff und die Datenmanipulation.

### 4. Datenanalyse
- Einsatz von Sprachmodellen zur Durchführung komplexer Datenanalysen.
- Generierung von Berichten und Visualisierungen basierend auf den Analyseergebnissen.

## Technologien und Tools
- **Sprachmodelle**: Einsatz von Langchain oder anderen Sprachmodell Agents für die Datenextraktion und -analyse.
- **Datenbankmanagement**: Auswahl eines geeigneten Datenbanksystems zur Speicherung der strukturierten Daten.
- **Datenaufbereitung**: Nutzung von Tools zur Datenbereinigung und -transformation.

## Erwartete Ergebnisse
- Ein funktionsfähiger Service, der die automatisierte Auswertung und Analyse wissenschaftlicher Veröffentlichungen ermöglicht.
- Eine einheitliche Datenbank, die alle relevanten Daten strukturiert speichert.
- Umfassende Auswertungen und Berichte, die dem Biologen wertvolle Einblicke in die Forschungsdaten bieten.

## Use Cases und Verhaltensmodelle

### 1. Use Case: Extraktion von Daten aus Veröffentlichungen
- **Verhalten**: Das Sprachmodell identifiziert und extrahiert relevante Datenpunkte (z.B. experimentelle Ergebnisse, Methodendetails, Autoreninformationen) aus den Texten wissenschaftlicher Veröffentlichungen.
- **Interaktion**: Nutzer lädt Dokumente hoch → Sprachmodell verarbeitet Dokumente → Relevante Daten werden extrahiert und kategorisiert.

### 2. Use Case: Datenaufbereitung und -transformation
- **Verhalten**: Die extrahierten Daten werden in ein einheitliches Format konvertiert, bereinigt und validiert.
- **Interaktion**: Extrahierte Daten werden in das Aufbereitungssystem eingespeist → Daten werden transformiert und bereinigt → Bereinigte Daten werden für die Speicherung vorbereitet.

### 3. Use Case: Erstellung und Verwaltung der Datenbank
- **Verhalten**: Die bereinigten Daten werden in eine strukturierte Datenbank überführt, die lokal aufgesetzt wird und bei jeder Instanz neu initialisiert wird.
- **Interaktion**: Bereinigte Daten werden in die Datenbank importiert → Datenbank wird initialisiert und bereitgestellt → Schnittstellen zur Datenbank werden für den Datenzugriff eingerichtet.

### 4. Use Case: Datenanalyse und Berichtserstellung
- **Verhalten**: Das Sprachmodell führt komplexe Datenanalysen durch und generiert Berichte sowie Visualisierungen basierend auf den Daten in der Datenbank.
- **Interaktion**: Nutzer startet Analysen über das Interface → Sprachmodell führt Analysen durch → Berichte und Visualisierungen werden generiert und präsentiert.

## Datenbankarchitektur

- **Datenbanktyp**: Lokale relationale Datenbank (z.B. SQLite, PostgreSQL)
- **Struktur**:
  - Tabellen für: Veröffentlichungen, Autoren, experimentelle Daten, Methoden, Ergebnisse
  - Beziehungen: Zwischen Veröffentlichungen und Autoren, Methoden und Ergebnissen

## Umsetzung der Datenbankarchitektur und Interaktionen mittels Flowwise

### 1. Flowwise Setup
- Integration von Langchain zur Steuerung der Datenextraktions- und Analyseschritte.
- Definition der Flows zur Verarbeitung der Daten in der Datenbank.

### 2. Implementierungsschritte
- Konfiguration von Langchain-Modellen für die spezifischen Aufgaben.
- Aufbau der Flows für Datenextraktion, -aufbereitung und -analyse.
- Entwicklung der Schnittstellen zur lokalen Datenbank.

### 3. Datenbankverwaltung
- Initialisierung der Datenbank bei jeder Instanz.
- Sicherstellung, dass keine Konsistenz über verschiedene Instanzen hinweg erforderlich ist.

---


further resource of github repos regarding the dataanalysis pipeline to be used: https://github.com/hbctraining/scRNA-seq_online
