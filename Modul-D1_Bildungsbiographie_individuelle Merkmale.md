1
=

tc1: NO IF vsbstyp=5 \| 6

tc2: NO IF vsbstyp1-15= 10 \| 11 \| 12 \| 13 \| 14

vn: vtrae; vtraeo

qt: Einfachauswahl, offene Angabe

hl:

in:

q: An welcher Schule haben Sie Ihre Studienberechtigung erworben?

is:

it:

st:

ao1: 1: : An einer staatlichen Schule

ao2: 2: : An einer privaten Schule

ao3: 3: : An einer kirchlichen Schule

ao4: 4: : An einer anderen Schule, und zwar: (offene Angabe: Präfix [vtraeo], 50
Zeichen)

ao5: 12: : weiß ich nicht

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO 2

hi:

\--------------------------------

2 
==

tc1: NO IF vsbstyp=5 \| 6

tc2: NO IF vsbstyp1-15= 10 \| 11 \| 12 \| 13 \| 14

tc3: NO IF …………. (beruflich Qualifizierte 3. BW)

vn: prffach1; prffach2; prffach3; prffach4; prffach5; stdfach1, stdfach2,
stdfach3, stdfach4, stdfach5; notefach1, notefach2, notefach3, notefach4,
notefach5, gesfach1, gesfach2, gesfach3, gesfach4, gesfach5

qt: offene Angabe / Einfachauswahl mit Dropdown-Menü

hl:

in:

q: Bitte nennen Sie uns Ihre schulischen Prüfungsfächer, die wöchentliche
Stundenzahl, Ihre jeweilige Abschlussnote und das Geschlecht Ihrer jeweiligen
Leher\*in?

is: Beziehen Sie Ihre Angaben bitte auf Ihr Abschlussjahr.

it:

st:

ao1: offene Angabe (Präfix [prffach1], 50 Zeichen

ao2: offene Angabe (Präfix [prffach2], 50 Zeichen

ao3: offene Angabe (Präfix [prffach3], 50 Zeichen

ao4: offene Angabe (Präfix [prffach4], 50 Zeichen

ao5: offene Angabe (Präfix [prffach5], 50 Zeichen

ao6: stdfach1: : 1 Std.\|2 Std.\|3 Std.\|4 Std.\|5 Std.\|6 Std.\|7 Std.\|8
Std.\|9 Std.\|10 Std. (Dropdown)

ao7: stdfach2: : 1 Std.\|2 Std.\|3 Std.\|4 Std.\|5 Std.\|6 Std.\|7 Std.\|8
Std.\|9 Std.\|10 Std. (Dropdown)

ao8: stdfach3: : 1 Std.\|2 Std.\|3 Std.\|4 Std.\|5 Std.\|6 Std.\|7 Std.\|8
Std.\|9 Std.\|10 Std. (Dropdown)

ao9: stdfach4: : 1 Std.\|2 Std.\|3 Std.\|4 Std.\|5 Std.\|6 Std.\|7 Std.\|8
Std.\|9 Std.\|10 Std. (Dropdown)

ao10: stdfach5: : 1 Std.\|2 Std.\|3 Std.\|4 Std.\|5 Std.\|6 Std.\|7 Std.\|8
Std.\|9 Std.\|10 Std. (Dropdown)

ao11: notefach1: : sehr
gut\|gut\|befriedigend\|ausreichend\|mangelhaft\|ungenügend (Dropdown)

ao12: notefach2: : sehr
gut\|gut\|befriedigend\|ausreichend\|mangelhaft\|ungenügend (Dropdown)

ao13: notefach3: : sehr
gut\|gut\|befriedigend\|ausreichend\|mangelhaft\|ungenügend (Dropdown)

ao14: notefach4: : sehr
gut\|gut\|befriedigend\|ausreichend\|mangelhaft\|ungenügend (Dropdown)

ao15: notefach5: : sehr
gut\|gut\|befriedigend\|ausreichend\|mangelhaft\|ungenügend (Dropdown)

ao16: gesfach1: : männlich \| weiblich (Dropdown)

ao17: gesfach2: : männlich \| weiblich (Dropdown)

ao18: gesfach3: : männlich \| weiblich (Dropdown)

ao19: gesfach4: : männlich \| weiblich (Dropdown)

ao20: gesfach5: : männlich \| weiblich (Dropdown)

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO 3

hi:

Stundenzahl, Note und Geschlecht sollen zeilenweise, also für jedes Prüfungsfach
angegeben werden können. Wünschenswert ist folgendes Format:

Stunden

je Woche Note: Geschlecht

Prüfungsfach: \___________\_ [Drop Down1] [Drop Down2] [Drop Down3]

Prüfungsfach: \___________\_ [Drop Down1] [Drop Down2] [Drop Down3]

\--------------------------------

3 
==

tc:

vn: inklnein; inklja; inklschu

qt: Mehrfachauswahl

hl:

in:

q: Wurden sie jemals in einer integrative arbeitenden Klasse/Inklusionsklasse
unterrichtet oder haben Sie eine Förderschule besucht?

is:

it: Kennzeichnend für eine integrative arbeitende Klasse/Inklusionsklasse ist
der gemeinsame Unterricht von Schüler\*innen mit und ohne sonderpädagogischen
Förderbedarf.

st:

ao1: inklnein: : nein, weder noch [Exklusivkategorie]

ao2: inklja: : Ja, ich wurde in einer integrative arbeitenden
Klasse/Inklusionsklasse unterrichtet.

ao3: inklschu: : Ja, ich war auf einer Förderschule.

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO 4 \| 7 \| 9 (vausbja=3 weiter mit 4; ssemhs= 1 \| 2 \| 01 \| 02 weiter mit
7; alle anderen weiter mit 9)

hi:

\--------------------------------

4 
==

tc1: NO IF vsbstyp=5 \| 6

tc2: NO IF vsbstyp1-15= 10 \| 11 \| 12 \| 13 \| 14

tc3: IF vausbja=3

vn: vausbzpjo; vausbzpmo; vausbzpka

qt: Einfachauswahl /offene Angabe / Dropdown

hl:

in:

q: Bitte geben Sie an, wann Sie Ihre (letzte) Berufsausbildung abgeschlossen
haben (Zeitpunkt der Zeugnisübergabe):

is:

it:

st:

ao1: (vausbzpjo) 4 Stellen; 1950-2020; Präfix: [number]; Suffix: Jahr des
Abschlusses der Berufsausbildung

ao2: (vausbzpmo): : Januar\|Februar\|…\|November\|Dezember (Dropdown)

ao3: (vausbzpka): : weiß ich nicht (Exklusivkategorie)

mv:

ka:

vc:

av: number: vierstellig : 1950 TO 2020

kh: (vausbzpjo) Bitte geben Sie das Jahr des Abschlusses ein.

fv:

hv:

fo:

tr:

GOTO 5

hi:

\--------------------------------

5 
==

tc1: NO IF vsbstyp=5 \| 6

tc2: NO IF vsbstyp1-15= 10 \| 11 \| 12 \| 13 \| 14

tc3: IF vausbja=3

vn: vausberuf, vausberufo

qt: Einfachauswahl / offene Angabe

hl:

in:

q: Welche Berufsausbildung haben Sie (zuletzt) abgeschlossen? Bitte nennen Sie
den gelernten Beruf.

is:

it:

st:

ao1: (vausberuf): 75 Zeichen; Präfix: [vausberufo]; Suffix: Beruf:
(Exklusivkategorie)

ao2: (vausbzpka): -12: : weiß ich nicht

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO 6

hi:

\--------------------------------

6
=

tc1: NO IF vsbstyp=5 \| 6

tc2: NO IF vsbstyp1-15= 10 \| 11 \| 12 \| 13 \| 14

tc3: IF vausbja=3

vn: vausbnote; vausbnoteo

qt: Einfachauswahl / offene Angabe

hl:

in:

q: Mit welcher Note haben Sie Ihre (letzte) Berufsausbildung abgeschlossen?

is:

it:

st:

ao1: xxx-Format; 3 Stellen; Präfix: [number]; Suffix: Abschlussnote (z. B. 2,5):
(Exklusivkategorie)

ao2: -11: : Ich habe keine Note erhalten.

ao3: -12: : weiß ich nicht

mv:

ka:

vc:

av: number: dreistellig : 1,0 TO 4,0

kh: Bitte geben Sie Ihren Notendurchschnitt an (0,1 bis 4,0).

fv:

hv:

fo:

tr:

GOTO 7 \| 9 (ssemhs=1 \| 2 \| 01 \| 02 weiter mit 7; alle anderen weiter mit 9)

hi:

\--------------------------------

1 
==

tc: IF ssemhs=1 \| 2 \| 01 \| 02 (nur Studierende im 1. + 2. Fachsemester)

vn: stfwint; stfwent; stfwein; stfwber; stfwsoz; stfwarb; stfwalt; stfwwiss;
stfwfam; stfwzeit; stfwzul; stfwhelf; stfwver; stfwand; stfwando

qt: Einfachauswahlmatrix / offene Angabe

hl:

in:

q: Wie wichtig waren Ihnen die folgenden Gründe bei der Wahl Ihres derzeitigen
Studienfaches?

is:

it1: (stfwint): spezielles Fachinteresse

it2: (stfwent): persönliche Entfaltung

it3: (stfwein): Einkommenschancen im späteren Beruf

it4: (stfwber): fester Berufswunsch

it5: (stfwsoz): eine hohe soziale Position zu erreichen

it6: (stfwart): gute Aussichten auf sicheren Arbeitsplatz

it7: (stfwalt): Ausweichlösung, da keine Zulassung im gewünschten Studienfach

it8: (stfwwiss): eine gute wissenschaftliche Ausbildung zu erhalten

it9: (stfwfam): weil meine Eltern/Familie mir dazu greaten haben

it10: (stfwzeit): wegen der kurzen Studienzeiten

it11: (stfwzul): geringe Hürden bei der Zulassung (z. B. keine
Zulassungsbeschränkung)

it12: (stfwhelf): anderen Menschen helfen zu können

it13: (stfwver): Vereinbarkeit meiner Beeinträchtigung mit späteren
Beschäftigungsmöglichkeiten

it14: (stfwand): anderes, und zwar:

it15: (offene Angabe) 120 Zeichen; Präfix: [stfwando]; Suffix: weiterer Grund:

st:

ao1: 1: : gar nicht wichtig

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: : sehr wichtig

mv:

ka:

vc: SHOW stfwver IF gartmob – gartka=1

av:

kh: Bitte geben Sie einen weiteren Grund an.

fv:

hv:

fo:

tr:

GOTO 8

hi: Items zufällig rotieren

\--------------------------------

8 
==

tc: IF ssemhs=1 \| 2 \| 01 \| 02 (nur Studierende im 1. + 2. Fachsemester)

vn: hswzul; hswtrad; hswkont; hswatt, hswreg; hswbed; hswruf; hswfach; hswrank;
hswint; hsweng; hswsupp; hswbarr; hswtz, hswand; hswando

qt: Einfachauswahlmatrix / offene Angabe

hl:

in:

q: Wie wichtig waren Ihnen die folgenden Gründe bei der Wahl Ihrer derzeitigen
Hochschule?

is:

it1: (hswzul): keine Zulassung an Wunschhochschule

it2: (hswtrad): Tradition und Ruf der Hochschule

it3: (hswkont): persönlicher Kontakt zu Freunden und/oder Familie vor Ort

it4: (hswatt): Attraktivität von Stadt und Umgebung

it5: (hswreg): regionale Nähe zum Heimatort

it6: (hswbed): günstige Lebensbedingungen am Hochschulort (Wohnen,
Lebenshaltung)

it7: (hswruf): gutter Ruf der Lehrenden in meinem Fachgebiet

it8: (hswfach): gewünschte Fachrichtung

it9: (hswrank): gute Platzierung meines Fachs in Rankings

it10: (hswint): international Ausrichtung des Studienangebotes

it11: (hsweng): Wunschstudiengang wird auf Englisch angeboten

it12: (hswsupp): hochschulspezifische Unterstützungsangebote (Beratung,
psychologische Betreuung, Vorsorge, “Brückenkurse”)

it13: (hswbarr): gute Ausstattung/Barrierefreiheit

it14: (hswtz): Möglichkeit, in Teilzeit studieren zu können

it15: (hswand): anderes, und zwar:

it16: (offene Angabe) 100 Zeichen; Präfix: [hswando]; Suffix: weiterer Grund:

st:

ao1: 1: : gar nicht wichtig

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: : sehr wichtig

mv:

ka:

vc:

av:

kh: Bitte geben Sie einen weiteren Grund an.

fv:

hv:

fo:

tr:

GOTO 9

hi: Items zufällig rotieren

\--------------------------------

9 
==

tc:

vn: sartzeit

qt: Einfachauswahl

hl:

in:

q: Betreiben Sie Ihr Studium in Vollzeit oder Teilzeit?

is:

it:

st:

ao1: 1: : Ich studiere in Vollzeit.

ao2: 2: : Ich studiere in Teilzeit.

ao3: 3: : Ich studiere in einem Vollzeitstudiengang mit einer individuellen
Teilzeitregelung.

ao4: 4: : Ich studiere in einem Vollzeitstudiengang, betreibe mein Studium
jedoch ohne offizielle Regelung als Teilzeitstudium.

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO 10 \| 13 (ssabsja=2 weiter mit 10; alle anderen weiter mit 13)

hi:

\--------------------------------

10 
===

tc: IF sabsja=2 (nur Studierende mit vorherigem Hochschulabschluss)

vn: sabserbl1; sabserbl

qt: Einfachauswahl

hl:

in:

q: In welchem Bundesland liegt die Hochschule, an der Sie Ihren letzten
Hochschulabschluss erworben haben?

is:

it1: (sabserbl1): Ich habe meinen letzten Hochschulabschluss an meiner
derzeitigen Hochschule erworben.

it2: (sabserbl): Bundesland:

st:

ao1 (sabserbl1): 0: : nein

ao2 (sabserbl1) 1: : ja

ao3 (sabserbl): 2: : Baden-Württemberg

ao4 (sabserbl): 3: : Bayern

ao5 (sabserbl): 4: : Berlin

ao6 (sabserbl): 5: : Brandenburg

ao7 (sabserbl): 6: : Bremen

ao8 (sabserbl): 7: : Hamburg

ao9 (sabserbl): 8: : Hessen

ao10 (sabserbl): 9: : Mecklenburg-Vorpommern

ao11 (sabserbl): 10: : Niedersachsen

ao12 (sabserbl): 11: : Nordrhein-Westfalen

ao13 (sabserbl): 12: : Rheinland-Pfalz

ao14 (sabserbl): 13: : Saarland

ao15 (sabserbl): 14: : Sachsen

ao16 (sabserbl): 15: : Sachsen-Anhalt

ao17 (sabserbl): 16: : Schleswig-Holstein

ao18 (sabserbl): 17: : Thüringen

ao19 (sabserbl): 18: : Im Ausland

mv:

ka:

vc: SHOW sabserbl1=0 IF sabserbl=2 \| 3 \| … \| 18

av:

kh:

fv:

hv:

fo:

tr:

GOTO 11 \| 12 (sabserbl= 2 \| 3 \| … \| 18 weiter mit 11; alle anderen weiter
mit 12)

hi: Bitte auf zwei Seiten programmieren (Filter“ nein/ja“ (an der derzeitigen
Hochschule), bei „nein“ erscheinen die Bundesländer 2-18

\--------------------------------

11a 
====

tc: IF sabserbl = 2 – 17 (nur für Studierende, die das Bundesland Ihrer
vorherigen Hochschule angegeben haben)

vn: sabserhs

qt: Dropdown-Menü

hl:

in:

q: An welcher Hochschule haben Sie Ihren Abschluss erworben?

is:

it:

st:

ao (sabserhs): Hochschulliste als Dropdown-Menü

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO 13

hi: Bitte mit nachfolgender Frage auf einer Seite programmieren.

\--------------------------------

11b 
====

tc1: IF sabserbl= 2 – 17

tc2: IF sabserbl= 18

vn: sabserhs2

qt: Offene Nennung

hl:

in:

q1: Sollte die Hochschule nicht aufgeführt sein, tragen Sie diese bitte in das
dafür vorgesehene Feld ein.

q2: An welcher Hochschule haben Sie Ihren Abschluss erworben?

is:

it:

st:

ao1: (offene Nennung): 100 Stellen; Präfix: [sabserhs2]; Suffix: … (muss hier
was eingetragen werden, wenn bereits das offene Feld in der Frage “erklärt”
wird?)

mv:

ka:

vc1: SHOW q1 IF sabserbl= 2 - 17

vc2: SHOW q2 IF sabserbl=18

av:

kh:

fv:

hv:

fo:

tr:

GOTO 12

hi:

\--------------------------------

12 
===

tc: IF sabsja=1 (nur für Studierende mit vorherigem Hochschulabschluss)

vn: sabserfacho

qt: Offene Nennung

hl:

in:

q: In welchem Fach haben Sie diesen Abschluss erworben?

is:

it:

st:

ao1: (offene Nennung): 60 Stellen; Präfix: [sabserfacho]; Suffix: … (muss hier
was eingetragen werden, wenn bereits das offene Feld in der Frage “erklärt”
wird?)

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO

hi:

\--------------------------------

13 
===

tc:

vn: absterm

qt: Einfachauswahl / Dropdown-Menü

hl:

in:

q: Wann werden Sie voraussichtlich Ihr derzeitiges Studium abschließen?

is:

it:

st:

ao1: Dropdown: Sommersemester 2020 \| Wintersemester 2020/21 \| Sommersemester
2021 \|Wintersemester 2021/22 \| Sommersemester 2022 \| … \| Sommersemester 2030

ao2: -12: : weiß ich noch nicht

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO 14 \| 17 (ssweije=1 und/oder saweija=1 und/oder shwija=1 und/oder ssuja=1
weiter mit 14; alle anderen weiter mit 17)

hi:

\--------------------------------

14 
===

tc: IF ssweija=1 und/oder saweija=1 und/oder shwija=1 und/oder ssuja=1 (nur
Studierende mit vorherigem Studienfachwechsel, Abschlusswechsel,
Hochschulwechsel und/oder Studienunterbrechung)

vn: ssweijaaz; saweijaaz, sshwjaaz; ssujaaz

qt: Dropdown-Menü

hl:

in:

q: Wie häufig haben Sie seit Ihrer Erstimmatrikulation…

is: Nicht gemeint sind Wechsel oder Unterbrechungen beim Übergang vom Bachelor-
ins Masterstudium.

it1: (ssweijaaz): … das Studienfach gewechselt?

it2: (sawejaaz): ... den Abschluss gewechselt?

it3: (shwjaaz): … die Hochschule gewechselt?

it4: (ssujaaz): … das Studium zwischenzeitlich unterbrochen?

st:

ao1: 1: : einmal

ao2: 2: : zweimal

ao3: 3: : dreimal

ao4: 4: : viermal

ao5: 5: : fünfmal und mehr

(ao1 bis ao5 Dropdown)

mv:

ka:

vc1: SHOW ssweijaaz IF ssweija=1

vc2: SHOW sawejaaz IF saweija=1

vc3: SHOW shwjaaz IF shwja=1

vc4: SHOW ssujaaz IF ssuja=1

av:

kh:

fv:

hv:

fo:

tr:

GOTO 15 \| 16 (bei Angabe bei ssujaaz weiter mit 16; alle anderen weiter mit 15)

hi:

\--------------------------------

15 
===

tc:

vn: beginn01 – beginn05; ende01 – ende05; hs01 – hs05; fach01 – fach05; abs01 –
abs05; stand01 – stand05; techepi

qt: Dropdown-Menü / offene Angaben

hl:

in:

q: Bitte tragen Sie die wesentlichen Stationen Ihres Studienverlaufs in das
nachfolgende Tableau ein.

is: Vermerken Sie bitte alle Fach-, Hochschul- und Abschlusswechsel seit
Studienbeginn. Sollten die vorgegebenen 5 Episoden nicht ausreichen, so können
Sie weitere Episoden aktivieren.

it1 (beginn01 – beginn05, ende01 – ende05): Beginn und Ende (Semester)

it2 (hs01 – hs05): Hochschule

it3 (fach01 – fach05): Studienfach

it4 (abs01 – abs05): angestrebter Abschluss

it5 (stand01 – stand05): letzter Stand

it6: techepi): Benötigen Sie weitere Episoden?

st:

ao1: (Dropdown bitte absteigend - beginn01 – beginn05): Sommersemester 2020 \|
Wintersemester 2019/2020 \| Sommersemester 2019 \| Wintersemester 2018/2019 \| …
\| Wintersemester 2020

ao2: -12: : weiß ich noch nicht

ao3: (offene Angabe): 100 Stellen; Präfix: [hs01 – hs05]; Suffix: Hochschule

ao4: (offene Angabe) 60 Stellen; Präfix: [fach01 – fach05]; Suffix: Studienfach

ao5: (Dropdown abs01 – abs05): Bachelor \| Bachelor (Lehramt) \| Master \|
Master (Lehramt) \| Staatsexamen \| Staatsexamen (Lehramt) \| Diplom, Promotion
\| kirchliche Abschlussprüfung \| künstlerische Abschlussprüfung \| anderer
Abschluss (bspw. Ausländischer Abschluss \| Magister) \| kein Studienabschluss

ao6: (Dropdown stand01 – stand05): begonnen \| abgeschlossen \| abgebrochen \|
unterbrochen

ao7: (techepi): 0: : nein

ao8: (techepi): 1: : ja

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO 16 \| 17 (ssuja=1 weiter mit 16; alle anderen weiter mit 17)

hi: Wenn techepi=1, bitte zwei weitere Zeilen einblenden.

Das Tableau passt nicht in die gängige Template-Vorlage!

\--------------------------------

16 
===

tc: IF ssuja=1 (nur Studierende, die mindestens eine Studienunterbrechung
hatten)

vn: suzeitp01; suzeitp02; suzeit03; sudau01; sudau02; sudau03; subeur01;
subeur02; subeur03

qt: Tableau-Abfrage (Dropdown-Menü, offene Angabe, Einfachauswahl)

hl:

in:

Individualisierung:

q1: Bitte beschreiben Sie Ihre Studienunterbrechung näher.

q2: Bitte beschreiben Sie Ihre Studienunterbrechung näher.

q3: Bitte beschreiben Sie Ihre letzten drei Studienunterbrechungen nächer.

is1 (nur für q2): Bitte beginnen Sie mit Ihrer letzten Studienunterbrechung.

is2 (nur für q3): Bitte beginnen Si emit Ihrer letzten Studienunterbrechung.
Sollten Sie mehr als dreimal unterbrochen haben, beginnen Sie bitte mit Ihrer
drittletzten Unterbrechung.

it1: (suzeitp01 – sozeitp03): Zeitpunkt der Unterbrechung:

it2: (sudau01 – sudau03): Dauer der Unterbrechung

it3: (subeur01 – subeur03): mit Beurlaubung?

st:

ao1: (Dropdown suzeitp01 – suzeitp03): : Sommersemester 2020 \| Wintersemester
2019/2020 \| Sommersemester 2019 \| … \| Wintersemester 2004/2005

ao2: (offene Angabe): 2 Stellen (00-99); Präfix: [sudau01 – sudau03]; Suffix:
Monate

ao3: (subeur01 – subeur03) 1: : nein

ao4: (subeur01 – subeur03) 2: : ja

mv:

ka:

vc1: SHOW q1 AND suzeitp01 \| sudau01 \| subeur01 IF ssujaaz=1 \| kA

vc2: SHOW q2 AND suzeitp01 \| sudau01 \| subeur01 \| suzeitß02 \| sudau02 \|
subeur02 IF ssujaaz=2

vc3: SHOW q3 AND suzeitp01 \| sudau01 \| subeur01 \| suzeitp01 \| sudau01 \|
subeur01 \| suzeitp02 \| sudau02 \| subeur02 \| suzeitp03 \| sudau03 \| subeur03
IF ssujaaz= 3 \| 4 \| 5

av:

kh:

fv:

hv:

fo:

tr:

GOTO 17

hi: In Abhängigkeit der Antworten auf Seite D1_14 erfolgt eine Einblendung von
bis zu drei Unterbrechungen, für die je Zeile anhand verschiedener
Antwortformate Informationen erhoben werden.

\--------------------------------

17 
===

tc:

vn: sintaner; sintzur; sintfair; sinternst; sintkont; sintfach; sintsem

qt: Einfachauswahlmatrix

hl:

in:

q: Wie sehr treffen die folgenden Aussagen auf Sie und Ihr Studium zu?

is:

it1 (sintaner): Ich fühle mich von den Lehrenden anerkannt.

it2 (sintzur): Mit den Lehrenden meines Studiengangs komme ich gut zurecht.

it3 (sintfair): Die meisten Lehrenden behandeln mich fair.

it4 (sinternst): Die Lehrenden interessieren sich für das, was ich zu sagen
habe.

it5 (sintkont): Mir ist es während meines bisherigen Studiums gut gelungen,
Kontakte zu anderen Studierenden aufzubauen.

it6 (sintfach): Ich kenne viele Kommiliton\*innen, mit denen ich mich über
fachspezifische Fragen austauschen kann.

it7 (sintsem): Ich habe viele KOntakte zu Studierenden aus meinem Semester.

st:

ao1: 1: : trifft gar nicht zu

ao2: 2

ao3: 3

ao4: 4

ao5: 5: : trifft voll und ganz zu

ao6: -12: : kann ich nicht beurteilen

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO 18

hi:

\--------------------------------

18 
===

tc:

vn: pakagern; pakafrem; pakaort; pakalost

qt: Einfachauswahlmatrix

hl:

in:

q: Inwieweit treffen die folgenden Aussagen auf Sie zu?

is:

it1 (pakagern): Alles in allem bin ich gerne Student(in).

it2 (pakafrem): Die studentische Welt ist mir fremd.

it3 (pakaort): Die Hochschule ist genau der richtige Platz für mich.

it4 (pakalost): An der Hochschule fühle ich mich verloren.

st:

ao1: 1: : trifft gar nicht zu

ao2: 2

ao3: 3

ao4: 4

ao5: 5: : trifft voll und ganz zu

ao6: -12: : kann ich nicht beurteilen

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO 19

hi:

\--------------------------------

19 
===

tc:

vn: sask1; sask2; sask3; sask4; sask5

qt: 5er Skala mit Bezeichnung der Endpunkte

hl:

in:

q:

is:

it1 (sask1): Ich halte meine Begabung für das Studium für …

it2 (sask2): Neues zu lernen im Studium fällt mir …

it3 (sask3): Meiner Meinung nach bin ich …

it4 (sask4): Meine studienbezogenen Fähigkeiten sind …

it5 (sask5): Aufgaben im Rahmen des Studiums fallen mir …

st:

ao1 (sask1) 1 : : niedrig

ao2 (sask1) 2

ao3 (sask1) 3

ao4 (sask1) 4

ao5 (sask1) 5: : hoch

ao6 (sask2) 1 : : schwer

ao7 (sask2) 2

ao8 (sask2) 3

ao9 (sask2) 4

ao10 (sask2) 5: : leicht

ao11 (sask3) 1 : : nicht intelligent

ao12 (sask3) 2

ao13 (sask3) 3

ao14 (sask3) 4

ao15 (sask3) 5: : sehr intelligent

ao16 (sask4) 1 : : niedrig

ao17 (sask4) 2

ao18 (sask4) 3

ao19 (sask4) 4

ao20 (sask4) 5: : hoch

ao21 (sask5) 1 : : schwer

ao22 (sask5) 2

ao23 (sask5) 3

ao24 (sask5) 4

ao25 (sask5) 5: : leicht

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO 20

hi:

\--------------------------------

20 
===

tc:

vn: kominter; kommeth; komwiss; komtext; komkrit; komsch; kommuen; komteam;
komvera; komkomm; komplan

qt: Einfachauswahlmatrix

hl:

in:

q: Bitte schätzen Sie ein, inwieweit Sie aktuell über die folgenden Fähigkeiten
und Kenntnisse verfügen.

is:

it1 (kominter): fachübergreifendes Wissen und Denken/Interdisziplinarität

it2 (kommeth): Anwendung fachbezogener Methoden

it3 (komwiss): Erarbeitung einer wissenschaftlichen Fragestellung

it4 (komtext): Verstehen von wissenschaftlichen Texten.

it5 (komkrit): kritisches Denken (eigene Ideen/Ideen anderer in Frage stellen)

it6 (komsch): schriftlicher Ausdruck

it7 (kommuen): mündlicher Ausdruck

it8 (komteam): Teamfähigkeit / Zusammenarbeit in einer Gruppe

it9 (komvera): Übernahme von Verantwortung in einer Gruppe

it10 (komkomm): Kommunikation mit Professor\*innen

it11 (komplan): Planungs- und Organisationsfähigkeit

st:

ao1: 1: : gar nicht

ao2: 2

ao3: 3

ao4: 4

ao5: 5: : sehr stark

ao6: -11: : trifft nicht zu

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO 21

hi:

\--------------------------------

21 
===

tc:

vn: ksprdeu; kspreng; ksprfra; ksprspa; ksprand; ksprando

qt: Einfachauswahlmatrix

hl:

in:

q: Wie gut beherrschen Sie die folgenden Sprachen?

is:

it1 (ksprdeu): Deutsch

it2 (kspreng): Englisch

it3 (ksprfra): Französisch

it4 (krprspa): Spanisch

it5 (ksprand): Andere Sprache, und zwar:

it6 (offene Angabe): 50 Stellen; Präfix: [ksprando]; Suffix: Andere Sprache:

st:

ao1: 1: : Grundkenntnisse

ao2: 2

ao3: 3

ao4: 4

ao5: 5: : sehr gute Kenntnisse

ao6: 6: : ich beherrsche diese Sprache nicht

ao7: 7: : Muttersprache

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO 50% 22 / 50% 23

hi:

\--------------------------------

22 
===

tc:

vn: dpzufr; dpinter; dpfrag; dsmein; dswiss; dsfreiz; staufw; sfober; sfklaus;
ssverl; sswied; sszeit

qt: Einfachauswahlmatrix

hl:

in:

q: Wie sehr treffen die folgenden Aussagen auf Sie und Ihr Studium zu?

is:

it1 (dpzufr): Studieren gibt mir manchmal das Gefühl von tiefer persönlicher
Zufriedenheit.

it2 (dpinter): Ich habe das Gefühl, dass praktisch jedes Thema hochinteressant
sein kann, wenn ich mich erst einmal damit befasse.

it3 (dpfrag): In die meisten meiner Lehrveranstaltungen gehe ich mit Fragen, auf
die ich nach einer Antwort suche.

it4 (dsmein): Ich bin erst zufrieden, wenn ich mich intensiv genug in ein Thema
eingearbeitet habe, um mir eine eigene Meinung bilden zu können.

it5 (dswiss): Ich überprüfe mein Wissen zu wichtigen Themen bis ich es wirklich
verstanden habe.

it6 (dsfreiz): Ich nutze meine Freizeit häufig dafür, mehr über interessante
Themen zu erfahren, die wir in Lehrveranstaltungen diskutiert haben.

it7 (sfaufw): Mein Ziel ist es, Lehrveranstaltungen mit so wenig Aufwand wie
möglich zu bestehen.

it8 (sfober): Ich finde es nicht hilfreich, Themen zu vertiefen. Es verwirrt nur
und ist verschwendete Zeit, wenn man nur oberflächliches Wissen benötigt.

it9 (sfklaus): Ich sehe keinen Grund darin Stoff zu lernen, der wahrscheinlich
nicht klausurrelevant ist.

it10 (ssverl): Ich lerne nur das ernsthaft, was in meinem Studium verlangt wird.

it11 (sswied): Manche Dinge wiederhole ich so lange bis ich sie auswendig kann,
selbst wenn ich sie nicht verstehe.

it12 (sszeit): Lehrende sollten nicht erwarten, dass Studierende viel Zeit damit
verbringen Stoff zu lernen, von dem jeder weiß, dass es nicht geprüft wird.

st:

ao1: 1: : trifft gar nicht zu

ao2: 2

ao3: 3

ao4: 4

ao5: 5: : trifft voll und ganz zu

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO 24

hi: Items zufällig rotieren

\--------------------------------

23 
===

tc:

vn: kogorga; kogkrit1; kogkrit2; kogzus; kogwied; mkogplan1; mkogplan2;
mkogwach1; mkogwach2; mkogreg; ressanst1; ressanst2; sesskonz1; resskonz2;
resszeit; lernumg1; lernumg2; resskomm; lit

qt: Einfachauswahlmatrix

hl:

in:

q: Wie sehr treffen die folgenden Aussagen auf Sie und Ihr Studium zu?

is:

it1 (kogorga): Ich stelle mir aus Mitschrift, Skript oder Literatur kurze
Zusammenfassungen mit den wichtigsten Punkten zusammen.

it2 (kogkrit1): Beim Lernen hinterfrage ich die meisten Schlussfolgerungen
kritisch.

it3 (kogkrit2): Ich denke über Alternativen zu den Behauptungen oder
Schlussfolgerungen in den Lerntexten nach.

it4 (kogzus): Zu neuen Lerninhalten stelle ich mir praktische Anwendungen vor.

it5 (kogwied): Ich lerne den Lernstoff anhand von Skripten oder anderen
Aufzeichnungen möglichst auswendig.

it6 (mkogplan1): Ich überlege mir vorher, in welcher Reihenfolge ich den Stoff
durcharbeite.

it7 (mkogplan2): Ich versuche, mir vorher genau zu überlegen, welche Teile eines
bestimmten Themengebiets ich lernen muss und welche nicht.

it8 (mkogwach1): Ich bearbeite zusätzliche Aufgaben, um festzustellen, ob ich
den Stoff wirklich verstanden habe.

it9 (mkogwach2): Um Wissenslücken festzustellen, rekapituliere ich die
wichtigsten Inhalte, ohne meine Unterlagen zu Hilfe zu nehmen,

it10 (mkogreg): Wenn ich Lerninhalte nicht direkt verstehe, gehe ich den Text
noch einmal langsam durch.

it11 (ressanst1): Ich arbeite so lange, bis ich mir sicher bin, die Prüfung gut
bestehen zu können.

it12 (ressanst2): Ich lerne auch spätabends und am Wochenende, wenn es sein
muss.

it13 (resskonz1): Ich ertappe mich dabei, dass ich mit meinen Gedanken ganz
woanders bin.

it14 (resskonz2): Beim Lernen fällt es mir schwer, bei der Sache zu bleiben.

it15 (resszeit): Beim Lernen stelle ich einen Zeitplan auf, an den ich mich auch
halte.\#

it16 (lernumg1): Mein Arbeitsplatz ist so gestaltet, dass ich alles schnell
finden kann.

it17 (lernumg2): Wenn ich lerne, sorge ich dafür, dass ich in Ruhe arbeiten
kann.

it18 (resskomm): Ich lerne zusammen mit meinen Studienkolleg\*innen.

it19 (lit): Ich suche nach weiterführender Literatur, wenn mir bestimmte Inhalte
noch nicht ganz klar sind.

st:

ao1: 1: : trifft gar nicht zu

ao2: 2

ao3: 3

ao4: 4

ao5: 5: : trifft voll und ganz zu

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO 24

hi: Die Items bitte zufällig rotieren.

\--------------------------------

24 
===

tc:

vn: pbigintro; pbigextro; pbigtrau; pbigkrit; pbiggenau; pbigfaul; pbigruh;
pbignerv; pbigkrea; pbignoku

qt: Einfachauswahlmatrix

hl:

in:

q: Inwieweit treffen die folgenden Aussagen auf Sie zu?

is:

it1 (pbigintro): Ich bin eher zurückhaltend, reserviert.

it2 (pbigextro): Ich gehe aus mir raus, bin gesellig.

it3 (pbigtrau): Ich schenke anderen leicht Vertrauen, glaube an das Gute im
Menschen.

it4 (pbigkrit): Ich neige dazu, andere zu kritisiereen.

it5 (pbiggenau): Ich erledige Aufgaben gründlich.

it6 (pbigfaul): Ich bin bequem, neige zur Faulheit.

it7 (pbigruh): Ich bin entspannt, lasse mich durch Stress nicht aus der Ruhe
bringen.

it8 (pbignerv): Ich werde leicht nervös und unsicher.

it9 (pbigkrea): Ich habe eine aktive Vorstellungskraft, bin phantasievoll.

it10 (pbignoku): Ich habe nur wenig künstlerisches Interesse.

st:

ao1: 1: : trifft gar nicht zu

ao2: 2

ao3: 3

ao4: 4

ao5: 5: : trifft voll und ganz zu

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO 25

hi: Items bitte zufällig rotieren

\--------------------------------

25 
===

tc:

vn: pswskill; pswkraft; pswaufg

qt: Einfachauswahlmatrix

hl:

in:

q: Inwieweit treffen die folgenden Aussagen auf Sie zu?

is:

it1 (pswskill): In schwierigen Situationen kann ich mich auf meine Fähigkeiten
verlassen.

it2 (pswkraft): Die meisten Probleme kann ich aus eigener Kraft gut meistern.

it3 (pswaufg): Auch anstrengende und komplizierte Aufgaben kann ich in der Regel
gut lösen.

st:

ao1: 1: : trifft gar nicht zu

ao2: 2

ao3: 3

ao4: 4

ao5: 5: : trifft voll und ganz zu

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO 26

hi: Items bitte zufällig rotieren

\--------------------------------

26 
===

tc:

vn: risk

qt: Einfachauswahlmatrix

hl:

in:

q: Wie schätzen Sie sich persönlich ein: Wie risikobereit sind Sie im
Allgemeinen?

is:

it:

st:

ao1 (risk) 1: : gar nicht risikobereit

ao2 (risk) 2

ao3 (risk) 3

ao4 (risk) 4

ao5 (risk) 5: : sehr risikobereit

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO 27

hi:

\--------------------------------

27 
===

tc:

vn: feelstress; feellast; feeldruck

qt: Einfachauswahlmatrix

hl:

in:

q: Wie haben Sie sich in den letzten vier Wochen übeerwiegend gefühlt?

is:

it1 (feelstress): gestresst

it2 (feellast): überlastet

it3 (feeldruck): unter Druck

st:

ao1: 1: : gar nicht

ao2: 2

ao3: 3

ao4: 4

ao5: 5: : sehr stark

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO 28

hi:

\--------------------------------

28 
===

tc: IF NOT partpsy=1

vn: depschw; depglue; depdep; deptrau; depverz; depgedr; depgut; depsich;
depruhe; depspass

qt: Einfachauswahlmatrix

hl:

in:

q: Wie fühlen Sie sic him Allgemeinen?

is:

it1 (depschw): Meine Stimmung ist schwermütig.

it2 (depglue): Ich bin glücklich.

it3 (depdep): Ich bin deprimiert.

it4 (deptrau): Ich bin traurig.

it5 (depverz): Ich bin verzweifelt.

it6 (depgedr): Ich bin in gedrückter Stimmung

it7 (depgut): Ich fühle mich gut.

it8 (depsich): Ich fühle mich sicher.

it9 (depruhe): Ich ruhig und gelassen.

it10 (depspass): Das Leben macht mir Spass.

st:

ao1: 1: : nie

ao2: 2: : selten

ao3: 3: : manchmal

ao4: 4: : häufig

ao5: 5: : sehr häufig

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO nächstes Modul

hi: Items bitte rotieren
