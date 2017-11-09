---
title: Pflichtenheft
date: 09.11.2017
subtitle: LeihDeinWagen
author: LeihDeinWagen Projektgruppe 
maketitle: yes
toc: yes
numbersections: yes
papersize: a4
fontsize: 12pt
lang: de-DE
documentclass: scrartcl 
classoption: oneside
header-includes:
    -\usepackage{fourier}

abstract: Die Webapplikation "LeihDeinWagen" wird im Rahmen der Vorlesung "Webbasierte Anwendungen" entwickelt. 
Das Ziel des Projekts ist es eine Webseite zu entwickeln, die es Personen ermöglichen soll Autos einfach & sicher zu mieten und vermieten. 
Bei der Entwicklung soll eine responsive Webseite erstellt werden, die auf allen mobilen Endgeräten darstellbar ist.

---


# Zielsetzung

## Musskriterien

In der Webapplikation LeihDeinWagen müssen folgende Funktionen umgesetzt werden:

* Automatische Registrierung auf der Website für Kunden
* Suchfunktion
* Filterfunktion 
* Nachrichtenaustausch
* Angebot(e) einstellen, ändern & löschen
* Vermietung über einen festen, längeren Zeitraum oder an bestimmten Tagen
* Kundenprofil & Bewertungssystem

## Wunschkriterien

* Premium-Funktion für Kunden um das einzustellende Angebot an die Spitze der aktuellen Angebote zu platzieren
* Bereitstellung von min. 1 Fahrzeug jedes Fahrzeugtyps durch eine Firma

## Abgrenzung

LeihDeinWagen soll nicht eingesetzt werden um Autos online zu verkaufen oder zu erwerben.


# Produkteinsatz

## Anwendungsbereiche

LeihDeinWagen soll in einer Desktop-Version sowie einer mobile Versionen für Smartphones und Tablets zur Verfügung stehen. 
Diese beiden Versionen ermöglichen den Einsatz von LeihDeinWagen jederzeit and jedem Ort.

## Zielgruppe

LeihDeinWagen richtet sich in erster Linie an Studenten an Hochschulen und Universitäten in Baden-Württemberg.
Nach erfolgreicher Etablierung könnte das Projekt für jede Hochschule/Universität deutschlandweit erweitert werden.


# Produktumgebung

## IST-Zustand

Da es sich um ein Entwicklungsprojekt handelt gibt es kein Produkt, welches von der Applikation "LeihDeinWagen" abgelöst werden soll.

## Software

LeihDeinWagen benötigt für den Betrieb einen der gängigen Webserver sowie ein Datenbanksystem auf welchem die erzeugten Daten abgespeichert werden.

## Hardware

Da es sich bei LeihDeinWagen um eine Webapplikation handelt, ist keine bestimmte Systemarchitektur notwendig. 
Welche Ressourcen auf der eingesetzten Hardware zur Verfügung stehen müssen, wird sich in der Testphase zeigen.

## Schnittstellen

Derzeit sind keine Schnittstellen zu weiteren Produkten notwendig.


# Produkt-Funktionen

Die Hauptfunktion von LeihDeinWagen ist, diverse Fahrzeuge über die Webseite vermieten und mieten zu können. 

Die Applikation verfolgt einen benutzerorientierten Ansatz, sodass einem Benutzer eindeutig eine Aktion zugeordnet werden kann. 

## Benutzerfunktionen

### Benutzerkennung

Jeder Student kann sich einen Benutzeraccount anlegen. Dieser ergibt sich aus der E-Mail-Adresse des Benutzers.
Desweiteren müssen Name und Vorname angegeben werden, da mit Verträgen gehandelt wird.

### Persönliche Daten

Von Namen und E-Mail-Adressen der Benutzer abgesehen werden keine persönlichen Daten gespeichert.

### Persönliche Konfiguration

Dem Benutzer steht keine Funktion zur Verfügung um das Layout der Webapplikation zu verändern/personalisieren.

### Persönliches Profil

Dem Benutzer steht frei sein eigenes Profil zu bearbeiten, dazu zählt: 
	* Profilbild
	* Name
	* Standort
	* Passwort


# Produktdaten

Die Software trägt den Namen LeihDeinWagen und ist eine Webapplikation.


# Produktleistungen

Mit LeihDeinWagen soll erreicht werden, dass ...


# Benutzeroberfläche

## Startseite

Auf der Startseite wird der Benutzer aufgefordert sich mit seinem persönlichen Benutzernamen und Kennwort anzumelden, 
bzw. zu registrieren falls noch nicht geschehen. Außerdem können bereits eingestellte Angebote angesehen werden, jedoch nicht gemietet werden.

## Hauptseite

Auf der Hauptseite von LeihDeinWagen wird dem Benutzer eine der Startseite ähnlichen Seite angezeigt, allerdings ohne die Login/Registrierung. 
Angebote können nun auch gemietet werden. Über die Hauptnavigation kann der Benutzer alle notwendigen Funktionen nutzen. 

## Hauptnavigation

### Suchen

Über die Suchfunktion können angebotene Fahrzeuge gesucht werden. Es kann nach Ort, Fahrzeugtyp, Datum oder Preis gesucht werden.

### Alle Angebote

Im Bereich 'Alle Angebote' befinden sich alle eingestellten Angebote aller Benutzer. Dabei sind die mit der Premium-Funktion eingestellten Angebote 
an der Spitze und es kann nach verschiedenen Punkten gefiltert werden (bspw. Fahrzeugtyp, Marke, Preis, Verbrauch, Leistung, etc.).

### Meine Angebote

Unter 'Meine Angebote' sind die eingestellten Angebote des Benutzers zu sehen. Diese können bearbeitet oder gelöscht werden. 
Während der Bearbeitung steht das Angebot niemandem zur Auswahl zur Verfügung.

### Vermieten

Im Navigationspunkt 'Vermieten' kann der Benutzer ein neues Angebot einstellen. 
Dabei sollen alle relevanten Informationen (Fahrzeugtyp, Leistung, Verbrauch, Datum, Preis, gewünschte Zahlungsart etc.) angegeben werden. 

### Profil

Im Bereich 'Profil' kann der Benutzer sein eigenes Profil einsehen und bearbeiten. Dazu gehören unter anderem Name, Passwort, Standort & Profilbild.
Desweiteren sollen Benutzerbewertungen im Profil angezeigt werden (Sauberkeit, Umgang, Dauer, Vertrauenswürdig, etc.).


# Qualitätsbestimmungen

* Einfache Bedienung (Usability)
* Modularer Aufbau, wenig Coderedundanz
* IT-Sicherheit


# Testszenarien 

Die Webapplikation wird im Rahmen einer Beta-Testphase durch die Entwickler getestet. 
Während der Tests soll jede Funktion von LeihDeinWagen durch unterschiedliche Entwickler getestet werden.


# Entwicklungsumgebung

## Software

Serverseitig ist ein Tomcat Webserver sowie eine Oracle SQL Datenbank vorhanden. 
Clientseitig ist die Wahl der IDE frei. Die Entwicklungsdaten werden auf einem privaten GitHub-Repository abgelegt.

## Hardware

Der Backendserver ist eine virtuelle Maschine. Welches OS mit welchen Erweiterungen installiert ist, ist bis zum Zeitpunkt der Erstellung des Pflichtenheftes nicht bekannt.

# Ergänzungen

## Fachliche Anforderungen

Die Projektmitglieder müssen wenigstens Erfahrungen in einem der unten aufgeführten Punkte mitbringen:

* Design
* CSS
* Planung von Projekten
* JavaScript
* JQuery
* HTML
* SQL
