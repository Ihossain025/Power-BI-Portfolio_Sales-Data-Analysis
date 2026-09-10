# 📊 Superstore Sales Performance Dashboard | Power BI

**Business Intelligence • Data Analytics • Power BI • DAX • Data Modeling**

**English | Deutsch**

An interactive Power BI dashboard for analyzing sales performance, profitability, product category performance, and regional performance using the Superstore sales dataset.

---

![Executive Sales Dashboard](Images/Executive_Overview.png)

## 🇬🇧 Introduction & Project Overview

This Power BI project was developed from the perspective of a **Sales Executive** who needs a clear overview of business performance and the ability to investigate specific areas when required.

The project transforms raw transactional sales data into an interactive dashboard that combines **sales, profitability, product, and geographic analysis** in one centralized view.

The dashboard helps management to:

* 📈 Monitor sales and profit development over time
* 🛍️ Compare product categories and sub-categories
* 🌍 Evaluate regional and city-state-level performance
* 📊 Compare current performance with previous period (Year, Quarter, Month)
* 🔎 Drill into regional details when deeper analysis is required

The goal is not only to visualize data, but to provide a practical BI solution that supports **data-driven sales and business decisions**.

### 🇩🇪 Einführung & Projektüberblick

Dieses Power-BI-Projekt wurde aus der Perspektive eines **Vertriebsleiters** entwickelt, der einen klaren Überblick über die Geschäftsentwicklung benötigt und bei Bedarf einzelne Bereiche detaillierter analysieren möchte.

Das Projekt transformiert rohe Transaktionsdaten in ein interaktives Dashboard, das **Umsatz, Profitabilität, Produkte und regionale Performance** in einer zentralen Übersicht kombiniert.

Das Dashboard unterstützt das Management dabei:

* 📈 Umsatz- und Gewinnentwicklung über die Zeit zu überwachen
* 🛍️ Produktkategorien und Subkategorien zu vergleichen
* 🌍 Regionen, Bundesstaaten und Städten zu analysieren
* 📊 die aktuelle Performance mit Zeitraum zu vergleichen
* 🔎 bei Bedarf regionale Details per Drill-through zu untersuchen

Das Ziel ist nicht nur die Visualisierung von Daten, sondern die Entwicklung einer praxisnahen BI-Lösung zur **datenbasierten Unterstützung von Vertriebs- und Geschäftsentscheidungen**.

---

## 🛠️ Skills Demonstrated

### 🇬🇧

This project demonstrates an end-to-end Power BI workflow covering **data preparation, data modeling, DAX analysis, visualization, and dashboard design**.

**🔄 Data Preparation / ETL – Power Query**

* Extracted and transformed the raw Superstore sales data
* Removed unnecessary columns and handled data quality issues
* Corrected data types and cleaned the dataset
* Created separate dimension tables for customers and products
* Removed duplicates where required to maintain data integrity

**🗂️ Data Modeling**

* Designed a **Star Schema** with a central Sales fact table
* Created separate Order Date and Ship Date tables for time-based analysis
* Established 1-to-many relationships between dimensions and the fact table
* Created a dedicated measure table to organize DAX calculations

**📐 Data Analysis – DAX**

* Created measures for Sales, Profit, Profit Margin, Orders, and growth analysis
* Implemented Year-over-Year calculations using time intelligence functions like 'SamePeriodLastYear'
* Used functions such as 'CALCULATE', 'SUM', 'DIVIDE', 'DISTINCTCOUNT', 'COUNTA', 'MAX', 'MIN ', ', etc.

**📊 Data Visualization & UX**

* Designed KPI cards, trend charts, bar/column charts, and comparison visuals
* Added slicers for interactive filtering
* Implemented drill-down and drill-through analysis
* Added page navigation and reset-filter functionality through bookmark
* Designed the dashboard with an executive-focused layout

### 🇩🇪

Dieses Projekt zeigt einen vollständigen Power-BI-Workflow von der **Datenaufbereitung über Datenmodellierung und DAX bis hin zu Visualisierung und Dashboard-Design**.

**🔄 Datenaufbereitung / ETL – Power Query**

* Rohdaten des Superstore-Datensatzes extrahiert und transformiert
* Nicht benötigte Spalten entfernt und Datenqualitätsprobleme bereinigt
* Datentypen korrigiert und Daten bereinigt
* Separate Dimensionstabellen für Kunden und Produkte erstellt
* Duplikate zur Sicherstellung der Datenintegrität entfernt

**🗂️ Datenmodellierung**

* Ein **Star Schema** mit einer zentralen Sales-Faktentabelle entwickelt
* Separate Tabellen für Order Date und Ship Date erstellt
* 1:n-Beziehungen zwischen Dimensionen und Faktentabelle aufgebaut
* Eine separate Measure-Tabelle zur strukturierten Verwaltung der DAX-Measures erstellt

**📐 Datenanalyse – DAX**

* Measures für Umsatz, Profit, Profit Margin, Orders und Wachstum entwickelt
* Year-over-Year-Berechnungen und Time Intelligence umgesetzt
* Funktionen wie `CALCULATE`, `SUM`, `DIVIDE`, `DISTINCTCOUNT`, 'COUNTA', 'MAX', 'MIN ' verwendet

**📊 Visualisierung & UX**

* KPI-Karten, Trenddiagramme, Balken-/Säulendiagramme und Vergleichsvisualisierungen erstellt
* Interaktive Slicer integriert
* Drill-down und Drill-through umgesetzt
* Seiten-Navigation und Reset-Filter-Funktion unter Verwendung  Bookmark integriert
* Dashboard mit Fokus auf eine übersichtliche Management-Perspektive gestaltet

---

## 🧩 Data & Data Model

![Executive Sales Dashboard](Images/Data_Model.png)

### 🇬🇧

The project is based on the **Superstore sales dataset**, originally provided as a flat transactional table.

The data was transformed into a structured **Star Schema** consisting of:

* **Sales Table** – central fact table containing transactional sales data
* **Customer Table** – customer-related attributes
* **Product Table** – product and category hierarchy
* **Order Date Table** – date dimension for order-based time analysis
* **Ship Date Table** – date dimension for shipping-related analysis
* **_All Measure Table** – dedicated table for organizing DAX measures

The dimensional model allows consistent filtering and supports reliable time-series and business analysis.

### 🇩🇪

Das Projekt basiert auf dem **Superstore Sales Dataset**, das ursprünglich als flache Transaktionstabelle vorlag.

Die Daten wurden in ein strukturiertes **Star Schema** überführt:

* **Sales Table** – zentrale Faktentabelle mit den Transaktionsdaten
* **Customer Table** – kundenbezogene Merkmale
* **Product Table** – Produkt- und Kategoriehierarchie
* **Order Date Table** – Datumstabelle für zeitbezogene Bestellanalysen
* **Ship Date Table** – Datumstabelle für Versandanalysen
* **_All Measure Table** – separate Tabelle zur Organisation der DAX-Measures

Das dimensionale Datenmodell ermöglicht konsistente Filterung und zuverlässige Zeitreihen- und Geschäftsanalyse.

---

## 📊 Dashboard & Key Insights

### 🇬🇧

The final solution combines the main analytical perspectives into **one executive dashboard** instead of separate Product, Customer, and Regional dashboards.

The dashboard provides:

**📈 Sales & Profitability**

* Strong overall sales growth across the analyzed period
* Increasing profit over time, but profit margin growth is very low compared to profit
* Q4 consistently represents the strongest sales quarter

**🛍️ Product Performance**

* Technology is the strongest revenue-generating category
* Sub-category performance varies considerably
* The dashboard allows products and categories to be compared dynamically by year and region

**🌍 Regional Performance**

* Regional sales performance differs significantly across the business
* State-level analysis highlights important markets within each region
* Regional performance can be investigated further through the dedicated Regional Deep Dive page

The interactive design allows users to move from a **high-level executive view to more detailed analysis** without requiring separate dashboards for every business area.

### 🇩🇪

Die finale Lösung kombiniert die wichtigsten Analyseperspektiven in **einem zentralen Executive Dashboard**, anstatt separate Dashboards für Produkte, Kunden und Regionen zu verwenden.

Das Dashboard bietet:

**📈 Umsatz & Profitabilität**

* Deutliches Umsatzwachstum über den betrachteten Zeitraum
* Der Gewinn steigt im Laufe der Zeit an, doch das Wachstum der Gewinnmarge ist im Vergleich zum Gewinn sehr gering
* Q4 ist durchgehend das umsatzstärkste Quartal
* Profitabilität kann über Profit Margin und Year-over-Year-Vergleiche überwacht werden

**🛍️ Produktperformance**

* Technology ist die umsatzstärkste Kategorie
* Die Performance der Subkategorien unterscheidet sich deutlich
* Produkte und Kategorien können dynamisch nach Jahr und Region analysiert werden

**🌍 Regionale Performance**

* Die Regionen unterscheiden sich deutlich hinsichtlich ihrer Umsatzperformance
* Die Analyse auf Bundesstaatsebene zeigt wichtige Märkte innerhalb der Regionen
* Über die separate Regional-Deep-Dive-Seite können Regionen detaillierter untersucht werden

Das interaktive Design ermöglicht den Wechsel von einer **Management-Übersicht zu detaillierteren Analysen**, ohne für jeden Geschäftsbereich ein separates Dashboard zu benötigen.

---

## 🔎 Regional Deep Dive

![Executive Sales Dashboard](Images/Regional_Performance_Deep Dive.png)

### 🇬🇧

A dedicated **Regional Deep Dive** page provides more detailed geographic analysis after selecting a region from the main dashboard.

This drill-through functionality allows users to move from regional performance at the executive level to **state/city-level detail**, while maintaining the selected analytical context.

### 🇩🇪

Eine separate **Regional-Deep-Dive-Seite** ermöglicht eine detailliertere geografische Analyse nach Auswahl einer Region im Hauptdashboard.

Die Drill-through-Funktion ermöglicht den Wechsel von der regionalen Managementübersicht zu **Details auf Bundesstaat-/Stadtebene**, während der ausgewählte Analysekontext beibehalten wird.

---

## 🎛️ Interactivity & User Experience

### 🇬🇧

The dashboard was designed to be interactive and easy to explore.

Key features include:

* Year, Region, Category, and Segment slicers
* Drill-down and drill-through analysis
* Interactive visual filtering
* Navigation between dashboard pages
* Reset Filters functionality
* Consistent dark-theme executive design

### 🇩🇪

Das Dashboard wurde interaktiv und benutzerfreundlich gestaltet.

Wichtige Funktionen sind:

* Slicer für Jahr, Region, Kategorie und Segment
* Drill-down und Drill-through
* Interaktive Filterung der Visualisierungen
* Navigation zwischen den Dashboard-Seiten
* Reset-Filter-Funktion
* Einheitliches Executive Design im Dark Theme

---

## 🎯 Conclusion

### 🇬🇧

This project demonstrates how raw transactional data can be transformed into a structured and interactive **Business Intelligence solution using Power BI**.

The project combines technical Power BI skills with business-oriented analysis by connecting **data preparation, Star Schema modeling, DAX, time intelligence, visualization, and interactive dashboard design**.

The main outcome is a centralized dashboard that helps decision-makers understand **what is happening, where performance differs, and where deeper analysis may be required**.

### 🇩🇪

Dieses Projekt zeigt, wie rohe Transaktionsdaten mit **Power BI** in eine strukturierte und interaktive **Business-Intelligence-Lösung** überführt werden können.

Das Projekt verbindet technische Power-BI-Kenntnisse mit einer geschäftsorientierten Analyse und kombiniert **Datenaufbereitung, Star-Schema-Modellierung, DAX, Time Intelligence, Visualisierung und interaktives Dashboard-Design**.

Das zentrale Ergebnis ist ein Dashboard, das Entscheidungsträger dabei unterstützt zu verstehen, **was passiert, wo sich die Performance unterscheidet und in welchen Bereichen eine detailliertere Analyse erforderlich ist**.

---

## 🛠️ Tools & Technologies

**Power BI · Power Query · DAX · Data Modeling · Star Schema · Time Intelligence · Data Visualization**

---

## 📁 Project Structure


SuperstoreSales-PowerBI-Project/
│
├── README.md
├── PowerBI/
│   └── Superstore_Sales_Analysis.pbix
│
├── Dataset/
│   └── Superstore_Data.xlsx
│
└── Images/
    ├── Executive_Overview.png
    ├── Regional_Deep_Dive.png
    └── Data_Model.jpg
```

---

## 👤 Author

**Md Iqbal Hossain**

Power BI · Data Analytics · Business Intelligence
