---
title: Pflichtenheft
date: 16.11.2016
subtitle: MoneyTime
author: MoneyTime Projektgruppe 
maketitle: yes
toc: yes
numbersections: yes
papersize: a4
fontsize: 12pt
lang: de-DE
documentclass: scrartcl 
classoption: oneside
header-includes:
    - \usepackage{fourier}

abstract: Die Web-Applikation "MoneyTime" wird im Rahmen der Vorlesung "Webbasierte Applikationen" entwickelt. Das Ziel des Projektes soll es sein eine Web-Applikation zu entwickeln, welche es einem Unternehmen ermöglicht Leistungen der Mitarbeiter zu Dokumentieren und im späteren Verlauf dem Kunden gegenüber abzurechnen. Bei der Entwicklung soll eine responsive Webseite erstellt werden, die auf allen mobilen Endgeräten darstellbar ist.
---

# Zielsetzung

## Musskriterien

In der WebApplikation MoneyTime müssen folgende Funktionen umgesetzt werden:

* Anlegen von Kunden und dazugehörige Projekte
* Anlegen von unterschiedlichen Leistungen
* Zeiterfassung einer Leistung auf einen Kunden bzw. auf ein Projekt 
* Auswertungsübersichten darüber:
* welcher Benutzer hat welche Leistungen erbracht
    * für welchen Kunden bzw. welches Projekt wurden welche Leistungen erbracht
    * welche Leistungen sind noch nicht abgeschlossen
* Jeder Benutzer besitzt ein eigenes Benutzerkonto
* Es existieren unterschiedliche Benutzerrollen
    * Geschäftsführer
    * Mitarbeiter

## Wunschkriterien

* Visualisieren der erbrachten Leistungen mittels Diagramme 
* Abrechnung von Leistungen und Aufträgen gegenüber dem Kunden
* Lokalisierung des Mitarbeiters via GPS
* Angebotserstellung sowie eine Funktion zur Übergabe der Daten an ein Programm zur Rechnungslegung

## Abgrenzungskriterien

MoneyTime soll nicht eingesetzt werden um die Effizienz der Mitarbeiter zu ermitteln, da für diese Erhebung weitaus mehr Daten zur Verfügung stehen müssen als MoneyTime erfassen kann.

# Produkteinsatz

## Anwendungsbereiche

MoneyTime soll in einer Desktop-Version, für den Einsatz im Büro, sowie mobile Versionen für Smartphones und Tablets, für die mobile Nutzung, zur Verfügung stehen. Diese beiden Versionen ermöglichen den Einsatz von MoneyTime in sehr vielen Bereichen.

## Zielgruppe

MoneyTime richtet sich hauptsächlich an Unternehmen im Dienstleistungssektor, z.B. Mitarbeiter im Außendienst, Servicetechniker, häusliche Pflege.
Durch die Freiheit unterschiedliche Leistungen zu definieren, kann MoneyTime jedoch in weiteren Bereichen eingesetzt werden.

# Produktumgebung

## IST-Zustand

Da es sich um ein Entwicklungsprojekt handelt gibt es kein Produkt, welches von der Applikation "MoneyTime" abgelöst werden soll.

## Software

MoneyTime benötigt für den Betrieb einen der gängigen Webserver sowie ein Datenbanksystem auf welchem die erzeugten Daten abgespeichert werden.

## Hardware

Da es sich bei MoneyTime um eine Webapplikation handelt, ist keine bestimmte Systemarchitektur notwendig. Welche Ressourcen auf der eingesetzten Hardware zur Verfügung stehen muss, wird sich in der Testphase zeigen.

## Schnittstellen

Derzeit sind keine Schnittstellen zu weiteren Produkten notwendig.


# Produkt-Funktionen

Die Hauptfunktion von MT ist, dass ein Mitarbeiter seine erbrachten Dienstleistungen, in Form von Zeiten, dokumentieren kann. Dabei soll eine Zuordnung zu unterschiedlichen Kunden, sowie gegebenenfalls auch zu einzelnen Projekten erfolgen. 

Die Applikation verfolgt einen benutzerorientierten Ansatz, sodass einem Benutzer eindeutig eine Aktion zugeordnet werden kann. 

## Benutzerfunktionen

### Benutzerkennung

Jeder Benutzer erhält in MoneyTime einen persönlichen Benutzeraccount. Dieser ergibt sich aus der E-Mail-Adresse des Benutzers.

### Persönliche Daten

Von Namen und E-Mail-Adressen der Benutzern abgesehen werden keine persönlichen Daten gespeichert.

### Persönliche Konfiguration

Dem Benutzer steht keine Funktion zur Verfügung um das Layout der Webapplikation zu verändern.

### Persönliches Profil

Der Benutzer kann die für ihn hinterlegten Daten in der Datenbank nicht verändern. Davon ausgenommen ist sein persönliches Passwort. Dieses kann er über eine Funktion ändern.


## Administratorfunktionen

Die verfügbaren Funktionen für den Administrator sind folgende:

* Anlegen, Bearbeiten und Löschen von Benutzer
* Anlegen, Bearbeiten und Löschen von Leistungen
* Anlegen, Bearbeiten und Löschen von Kunden 
* Anlegen, Bearbeiten und Löschen von Projekte


# Produktdaten

Die Software trägt den Namen MoneyTime und ist eine Webapplikation.

# Produktleistungen

Mit MoneyTime soll erreicht werden, dass der nicht dokumentierte Anteil der von Mitarbeitern erbrachten Dienstleistungen auf ein Minimum gesenkt wird. Weiterhin soll MoneyTime als Werkzeug zur Dokumentation von Vorgängen dienen. Damit soll sichergestellt werden, dass bei Ausfall eines Mitarbeiters ein anderer Mitarbeiter nachvollziehen kann welche Arbeiten bei einem Kunden verrichtet wurden.

# Benutzeroberfläche

## Startseite

Auf der Startseite wird der Benutzer aufgefordert sich mit seinem persönlichen Benutzernamen und Kennwort anzumelden. Eine Funktion um das Passwort automatisiert zurückzusetzen wird nicht implementiert.

## Hauptseite

Auf der Hauptseite von MoneyTime wird dem Benutzer direkt das Benutzermenü mit den Hauptnavigationspunkten angezeigt. Wenn ein Benutzer eine nicht beendete Leistung hat, wird ihm diese angezeigt.

## Benutzermenü

### Leistung erfassen

Auswahl des Kunden, eines Projektes sowie der zu erbringenden Leistung. Weiterhin ist ein Button zum Beginnen der Leistung vorhanden.

### offene Leistungen

In diesem Bereich kann sich der Benutzer seine offenen, noch nicht abgeschlossenen Leistungen anzeigen lassen und bearbeiten.
Lediglich die Bearbeitung des Feldes Bemerkung ist noch möglich. 
Eine Änderung der Felder Kunde, Benutzer, Leistung sowie der aufgezeichneten Zeit ist nicht mehr möglich. 
Weiterhin ist eine Checkbox vorhanden, bei deren Aktivierung die offene Leistung als abgeschlossen gekennzeichnet wird.

### abgeschlossene Leistungen

Hier kann sich der Benutzer seine erbrachten Leistungen anzeigen lassen. Eine Filterung ist über das Datum, den Kunden, ein Projekt als auch über die Art der erbrachten Leistung möglich. Die Ausgabe der Datensätze erfolgt in Tabellenform. Durch das Anklicken des Datensatzes werden dem Benutzer auch die Bemerkungen angezeigt.

# Qualitätsbestimmungen

* Einfache Bedienung (Usability)
* Modularer Aufbau, wenig Coderedundanz (DRY-Prinzip)
* Einfache Installation / Wartung
* IT-Sicherheit

# Testszenarien 

Die Webapplikation wird im Rahmen einer Beta-Testphase durch die Entwickler getestet. Während der Tests soll jede Funktion von MoneyTime durch unterschiedliche Entwickler getestet werden.

# Entwicklungsumgebung

## Software

Serverseitig ist ein Tomcat Webserver sowie eine Oracle SQL Datenbank vorhanden. 
Clientseitig ist die Wahl der IDE frei. Bevorzugt wird jedoch IntelliJ von Jetbrains. Die Entwicklungsdaten werden auf einem privaten GitHub-Repository abgelegt.

## Hardware

Der Backendserver ist eine virtuelle Maschine. Welches OS mit welchen Erweiterungen installiert ist, ist bis zum Zeitpunkt der Erstellung des Pflichtenheftes nicht bekannt.

# Ergänzungen

## Fachliche Anforderungen

Die Projektmitglieder müssen wenigstens Erfahrungen in einem der unten aufgeführten Punkte mitbringen:

* Design
* CSS
* Planung von Projekten
* JavaScript
* HTML
* SQL
