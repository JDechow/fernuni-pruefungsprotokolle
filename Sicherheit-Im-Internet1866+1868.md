# Gedaechtnisprotokoll der Klausur vom 9. Februar 2019


## Aufgabe 1

Wahr-Falsch-Fragen

## Aufgabe 2

[War genau die gleiche Aufgabe wie SS16 Aufgabe 1](https://vu.fernuni-hagen.de/lvuweb/lvuauth/file/FeU/Informatik/2018WS/01868/material/ungetaktet/PK+635021+SS16.pdf)

Nenne 3 Angriffsziele.

> Loesungsvorschlag:
> * Uebertragungsweg
> * Daten
> * System / Rechner

Nenne Unterscheidungskriterien fuer Bedrohungen

> Loesungsvorschlag:
> * aktiv/passiv
> * technisch/nicht technisch
> * absichtlich/nicht absichtlich

Nenne schuetzenswerte Eigenschaften eines Systems

> Loesungsvorschlag:
> * Integritaet
> * Vertraulichkeit
> * Zuverlaessigkeit
> * Authentizitaet

Ein Dokument wird von einem FernUni-Mitarbeiter in Büro A zu einem Mitarbeiter in Büro B desselben Gebäudes per E-Mail geschickt. Auch der Mail-Server befindet sich in diesem Gebäude. Ist die Vertraulichkeit des Dokuments beim Transport hiermit bereits sichergestellt, d.h. kann auf eine Verschlüsselung verzichtet werden? Begründen Sie Ihre Antwort.

> Loesungsvorschlag: 
> Nicht sichergestellt. Email Server ist ja mit dem Internet verbunden. Und auch in der Firma darf nicht jeder alles Wissen (z.B. HR vs. normaler MA)


## Aufgabe 3
## Aufgabe 4
## Aufgabe 5

### Paketfiltergedoens

Tabelle mit Regeln und Ja/Nein Ankreuzfragen.

Neue Regeln dazu um neue Routen zu definieren.

## Aufgabe 6
## Aufgabe 7
## Aufgabe 8
## Aufgabe 9


## Aufgabe 10

### WEP (eigentlich ja eine Matheaufgabe)
WEP Verschluesselung IV 11bit lang bekannt, 7bit vom WEP Schluessel auch bekannt.
Angreifer kann in 45 Minuten den WEP Schluessel knacken.
Der Angreifer schafft pro Minute 4^(3x+2) Schluessel zu testen.
Ein Tag ist der Einfachheit halber 2^16 Sekunden (korr. JD Minuten) lang.
Welcher Wert ist x?

> Loesungsvorschlag JD:
45 Minuten sind 1/24 * 3/4 * 2^16 Sekunden = 1/32 * 2^16 Sekunden = 2^(-5) * 2^16 Sekunden = 2^11 Sekunden.

Unbekannt sind: beim IV: 24-11=13 Bit; beim Schlüssel: 48-7=41 Bit.
Im Mittel müssen also 13+41-1 Bit = 53 Bit oder 2^53 Schlüssel ausgetestet werden.

2^53  /  4^(3x+2)  = 2^11 <=> 2^53 / 2^(2*(3x+2)) = 2^11 => 53 - 2*(3x+2) = 11

=> 21 = 3x+2 => x = 19/3


## Unsortierte Fragen, Aufgabenzuordnung vergessen

### Kerberos
Kerberossystem mit 123 Schluesseln, 3x Clients und y Servern. 1 Ticket is ausgestellt, 60 = x + y.
Wieviele Clients und wieviele Server gibt es.
> Loesungsvorschlag:
> Daraus kann man 2 Gleichungen herleiten:
> * 60 = x + y
> * 123 = 1 + 3x + y
>
> x=31
> y=29
> 
> Das heisst 93 Clients und 29 Server.

### Voip
Was ist re-keying?
> Loesungsvorschlag: 
> Vom Masterkey einen neuen Session-Key generieren bei SRTP.

Was ist ein Media Gateway?
> Loesungsvorschlag: 
> Uebergang vom klassischen Telefonnetz zum VoIP-Netz

Telefonnummern-Umsetzung von +49123456789 zu...
> Loesungsvorschlag: 
> ... 9.8.7.6.5.4.3.2.1.9.4.e164.arpa

### PGP
Warum hybrides Verfahren und wie wird der Schluessel und die Nachricht uebermittelt?

Wie funktioniert signieren bei PGP?

Was ist der Vorteil an hybriden Verfahren, wenn man eine Nachricht an mehrere Empfänger schicken möchte?

### Zugriffskontrolle Nutzerauth

Vor- und Nachteile von ACLs und Capabilities

Welches Schutzziel Biba Modell?
> Loesungsvorschlag: Integritaet

Was bedeutet no read down bzw. no write up?

Wie ist eine Sicherheitsstufe bei Bell-La-Padula definiert?

### Anonym

Nenne 3 einfache Anonymisierungstechnicken.

> * Proxy
> * Tor
> * Mixes

Nachteile der oben genannten und was ein Mix besser/anders macht. Und mithilfe welcher Methoden.

> Loesungsvorschlag:

Drei Unterschiede zwischen Mix-Kaskade und Tor-Circuit.

> Loesungsvorschlag:


### RSA

p = 11 und q = 3, e = 7 ... finde d durch probieren
> e * d mod (q-1)(p-1) = 1
> d = 3

Warum darf e nicht 5 sein?
> muss teilerfremd zu (q-1)(p-1) sein.

welche Probleme gibt es, wenn e = 19 (Hinweis: 19 mod 20 = -1)
> ?

### Wahr-Falsch Fragen

Befehl: ps -elf  Gibt das Infos über Festplatte, Partitionierung...?

Bei Anruf aus klassischem Telefonnetz: ist DNS-Spoofing möglich?



