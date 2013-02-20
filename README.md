Hallo zusammen,

da die Infektionswelle ordentlich zugeschlagen hat und das Interesse an dem Thema groß war, hier für alle Interessierten eine Übersicht des gestrigen Treffens.

# JSF 2.2 Workshop - Adopt a JSR #

Das Log fasst die von uns besprochenen Themen und Punkte zusammen und gibt einen Ausblick, was unsere Arbeit an Adopt JSR 344 bewirken soll - und soll an dieser Stelle als draft unserer Gruppenarbeit dienen. 


## Ziel ##

Im Rahmen eines Reviews der JSR 344 Spezifikation soll eine Beispiel Application (Java EE 6) um eine Auswahl an neuen Features sowie fixes entstehen. 
Die Entstehung der Application soll im Tutorial-Style dokumentiert werden und ggf. das aktuelle offizielle Oracle Tutorial zu JSF ablösen.


## Motivation ##
 * aktives Testen der Referenzimplementierung
 * Bewertung des API / evtl Änderungsvorschläge
 * Bewertung des Aspekts "ease of development" (aus Sicht von Frontend- sowie Backend-Entwicklern)
 * viele schlechte Tutorials zu JSF (speziell Oracle) + outdated

----------

# Beispiel Application / Tutorial #

Das Tutorial soll einen soliden Einstieg in JSF 2.2 geben - schrittweise: vom Setup bis zu einer vollstängien Application.


## Die Idee ##
Ein bestehendes Tutorial verbessern und mit JSF 2.2 Features erweitern. Dazu wurden zwei Tutorials genannt: das Oracle EE Tutorial zu JSF [1] sowie JSF @work irian [2], weitere Vorschläge sind gerne willkommen. 


## Einstieg / Setup ##
Zwei mögliche Ausgangslagen an Infrastruktur sollen thematisiert werden:

* Quick Start mit einem JEE Container (GlassFish, JBoss...)
 ...weil dieser Container alle notwendigen (EE) Komponenten für den Soforteinstieg mitbringt.

* Einstieg mit Servlet Container (Jetty, Tomcat)
 ...weil es in der freien Wildbahn administrative und infrastrukturelle Handicaps gibt, z.B. Admins, die nur den Tomcat kennen oder mangelnde EE Unterstützung bei Cloud-Anbieter (wie etwa Heroku). Somit wäre unser Tutorial auch "cloud-ready" (buzzword alarm).


## JSF 2.2 Features ##
Das Project soll folgende Bestandteile des JSR 344 integrieren / evaluieren:

 * Bookmarkability 
 * HTML5
 ** Flow Management
 ** Ajax
 * Neue Komponenten wie z.B. file upload
 * Multi-field validation
 * WindowID

sowie

 * verbesserter CDI support (@ViewScoped, injection in Konvertern, Validatoren und anderen Artefakten) [hier die von Michael erwähnte Brücke zu JSR 346]
 * programmatische Konfiguration (wir alle mögen keine XML Konfigurationen - und stehen auf compiler Unterstützung)

Je nach Gruppen-Größe / Kapazität können Teile gestrichen oder hinzugefügt werden.


## Abschließend ##
Als abschließendes Feedback sollen folgende Punkte bewertet werden:

* Ease of development
* Security enhancements


[1] @Rafel Israels: könntest du diese Lücke schließen und den Link zum besagten Tutorial posten?
[2] http://jsfatwork.irian.at


----------

## TODO ##

Organisatorisch stehen aktuell folgende Sachen aus:

* Nächste(s) Treffen planen
 - nächstes Treffen noch allgemein / organisatorisch 
 (Ergänzungen / Änderungen / Aufteilen der Teil-Themen / Arbeitsgruppen (?))

 - bis dahin Einarbeitung & Vorbereitung der Interessierten
   
* Welche Application genau / welches "Referenz-Tutorial"? 
 - Oracle EE / JSF, JSF @work irian
 - weitere Vorschläge

* Entscheiden: Project Lead
  
* JUGC @ java.net mehr involvieren (speziell für den Adopt a JSR Prozess)


----------

Ich hoffe, das gibt allen einen groben Überblick - und ich hoffe, ich habe nichts vergessen oder durcheinander gebracht :-)