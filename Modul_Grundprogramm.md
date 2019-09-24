\------------------------------------------------------------

SDK-scr01
=========

tc:

vn: vsbdeba

qt: Einfachauswahl

hl:

in:

q: Um die Befragung passend für Ihre Situation gestalten zu können und
insbesondere auf die Situation internationaler Studierender eingehen zu können,
müssen wir Ihnen zu Beginn zwei zentrale Eingangsfragen stellen.

Die erste Frage lautet: Wo haben Sie Ihre Hochschulreife erworben?

is:

it:

st:

ao1: 1: in Deutschland

ao2: 2: in einem anderen Land

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

hi:

\------------------------------------------------------------

SDK-scr01
=========

tc:

vn: dnatdeu, dnatausl

qt: Mehrfachauswahl

hl:

in:

q: Die zweite Frage lautet: Welche Staatsangehörigkeit haben Sie?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: 1: die deutsche Staatsangehörigkeit

ao2: 2: eine oder mehrere andere Staatsangehörigkeit(en)

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO CMI1

hi:

kh:

fv:

hv:

fo:

tr:

hi:

\------------------------------------------------------------

CMI1
====

tc:

vn: dnatderw

qt: Einfachauswahl

hl:

in:

q: Besitzen Sie die deutsche Staatsangehörigkeit …

is:

it:

st:

ao1: 1: von Geburt an?

ao2: 2: als Spätaussielder(in)?

ao3: 3: durch Einbürgerung?

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

hi:

\------------------------------------------------------------

CMI2
====

tc:

vn: dnatko

qt: Einfachauswahl

hl:

in:

q1: Welche nicht-deutsche Staatsangehörigkeit besaßen Sie vor Ihrem Zuzug nach
Deutschland?

q2: Welche Staatsangehörigkeit besaßen Sie vor Ihrer Einbürgerung?

q3: Sie haben zu Beginn der Befragung angegeben, die deutsche und eine oder
mehrere ausländische Staatsangehörigkeit(en) zu haben.

Welche Staatsangehörigkeit besitzen Sie neben der deutschen?

q4: Sie haben zu Beginn der Befragung angegeben, eine oder mehrere ausländische
Staatsangehörigkeit(en) zu haben.

Welche ausländische Staatsangehörigkeit besitzen Sie?

is: Bitte wählen Sie hier zunächst den Kontinent aus.

it:

st:

ao1: 100: Europa

ao2: 200: Afrika

ao3: 300: Amerika

ao4: 400: Asien

ao5: 500: Australien und Ozeanien

mv:

ka:

vc:

SHOW q1 if dnatderw=2

SHOW q2 if dnatderw=3

SHOW q3 if dnatdeu=1 AND dnatausl=1

SHOW q4 if dnatdeu=0 AND dnatausl=1

av:

kh:

fv:

hv:

fo:

tr: GOTO CMI3

hi:

\------------------------------------------------------------

CMI3
====

tc:

vn: dnatsta, dnatstao

qt: Einfachauswahl mit Dropdown

hl:

in:

q1: Bitte geben Sie nun die Staatsangehörigkeit an, die Sie vor Ihrem Zuzug nach
Deutschland hatten.

q2: Bitte geben Sie nun Ihre Staatsangehörigkeit vor Ihrer Einbürgerung an.

q3: Bitte geben Sie nun Ihre Staatsangehörigkeit an, die Sie neben der deutschen
besitzen.

q4: Bitte geben Sie nun Ihre ausländische Staatsangehörigkeit an.

is:

it:

st:

ao: Einfachauswahl: Dropdown Staatenliste_DBI

mv:

ka:

vc: SHOW Einfachauswahl if dnatko\>0

SHOW q1 if dnatderw=2

SHOW q2 if dnatderw=3

SHOW q3 if dnatdeu=1 AND dnatausl=1

SHOW q4 if dnatdeu=0 AND dnatausl=1

av:

kh:

fv:

hv:

fo:

tr: GOTO CMI4

hi:

\------------------------------------------------------------

CMI3
====

tc:

vn: dnatstao

qt: offene Frage

hl:

in:

q1: Bitte geben Sie nun die Staatsangehörigkeit an, die Sie vor Ihrem Zuzug nach
Deutschland hatten.

q2: Bitte geben Sie nun Ihre Staatsangehörigkeit vor Ihrer Einbürgerung an.

q3: Bitte geben Sie nun Ihre Staatsangehörigkeit an, die Sie neben der deutschen
besitzen.

q4: Bitte geben Sie nun Ihre ausländische Staatsangehörigkeit an.

is:

it:

st:

ao1: offene Angabe: 30, Prefix: Staatsangehörigkeit:

mv:

ka:

vc: SHOW offene Angabe if dnatko=SYSMISS

SHOW q1 if dnatderw=2

SHOW q2 if dnatderw=3

SHOW q3 if dnatdeu=1 AND dnatausl=1

SHOW q4 if dnatdeu=0 AND dnatausl=1

av:

kh:

fv:

hv:

fo:

tr: GOTO CMI4

hi:

\------------------------------------------------------------

CMI4
====

tc:

vn: dgebort

qt: Einfachauswahl

hl:

in:

q: Wo wurden Sie geboren?

is:

it:

st:

ao1: 1: in Deutschland

ao2: 2: in einem anderen Land

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO CMI5 if dgebort=2

GOTO SDK-scr03 if dgebort=1

hi:

\------------------------------------------------------------

CMI5
====

tc:

vn: dgebko

qt: Einfachauswahl

hl:

in:

q: In welchem Land wurden Sie geboren?

is: Bitte wählen Sie hier zunächst den Kontinent aus.

it:

st:

ao1: 100: Europa

ao2: 200: Afrika

ao3: 300: Amerika

ao4: 400: Asien

ao5: 500: Australien und Ozeanien

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: CMI6

hi:

\------------------------------------------------------------

CMI6
====

tc:

vn: dgebsta

qt: Einfachauswahl mit Dropdown

hl:

in:

q: Bitte geben Sie nun das Land an, in dem Sie geboren sind.

is:

it:

st:

ao: Einfachauswahl: Dropdown Staatenliste_DBI

mv:

ka:

vc: SHOW Einfachauswahl if dgebko\>0

av:

kh:

fv:

hv:

fo:

tr: GOTO B16

hi:

\------------------------------------------------------------

CMI6
====

tc:

vn: dgebstao

qt: offene Frage

hl:

in:

q: Bitte geben Sie nun das Land an, in dem Sie geboren sind.

is:

it:

st:

ao1: offene Angabe: 30, Prefix: Staatsangehörigkeit:

mv:

ka:

vc: SHOW offene Angabe if dgebko=SYSMISS

av:

kh:

fv:

hv:

fo:

tr: GOTO B16

hi:

\------------------------------------------------------------

B16
===

tc:

vn: baufgrueuba; baufgruausba; baufgruasylba; baufgrufamba; baufgrutouba; baufgrustuba; baufgruandba; baufgruandba_open; baufgruwnba

qt: Mehrfachauswahl mit offener Angabe

hl:

in:

q: Für den Zuzug nach Deutschland gibt es unterschiedliche rechtliche Grundlagen. Wie war das bei Ihnen, welchen Status haben Sie damals bei Ihrer Einreise nach Deutschland gehabt?

is:

it:

st:

ao1: 1: (baufgrueuba): Bürger/ Bürgerin eines EU Mitgliedstaates/ Staates im EWR (Europäischer Wirtschaftsraum)

ao2: 2: (baufgruausba): Aussiedler/ Aussiedlerin, das heißt deutschstämmige Person aus osteuropäischen Staaten

ao3: 3: (baufgruasylba): Asylbewerber/ Asylbewerberin oder Flüchtling

ao4: 4: (baufgrufamba): Familiennachzug, z. B. als Ehegatte/ Ehegattin oder Kind eines/ einer Aufenthaltsberechtigten

ao5: 5: (baufgrutouba): mit einem Touristenvisum

ao6: 6: (baufgrustuba): Studierender/ Studierende, Schüler/ Schülerin oder Auszubildender/ Auszubildende (einschließlich Aufenthaltserlaubnis zur Studienvorbereitung)

ao7: 7: (baufgruandba): anderen, und zwar: (baufgruandba_open)

ato:

ao8: 8: (baufgruwnba): weiß ich nicht [EK]

mv:

ka:

vc:

av:

kh:

fv:

hv: Bildungsausländer\*Innen = 1 auf Grundlage von SDK-scr01 – SDK-scr03

fo:

tr: GOTO SDK-scr03

hi:

\------------------------------------------------------------

SDK-scr03
=========

tc:

vn: imausl

qt: Einfachauswahl

hl:

in:

q: Befinden Sie sich zurzeit studienbezogen außerhalb Deutschlands?

is:

it:

st:

ao1: 1: nein

ao2: 2: ja

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: SDK-NEU

hi:

\------------------------------------------------------------

SDK-NEU
=======

tc:

vn: NEU

qt: Einfachauswahl mit Dropdown und offener Angabe

hl:

in:

q: Sie wurden von der Hochschule HS-Name aus [PRELOAD_??] eingeladen, sind Sie hier aktuell immatrikuliert?

is: Falls Sie an mehreren Hochschulen eingeschrieben sind, beziehen Sie Ihre Antwort auf diese und alle weiteren Fragen bitte auf die Hochschule, an der Sie den für Sie gegenwärtig wichtigeren Studiengang studieren.

it:

st:

ao1: 1: Ja, und zwar am Standort: Dropdown

ato: Nein, ich bin an folgender Hochschule immatrikuliert:

mv:

ka:

vc: SHOW (Individualisierung) if token=xxx

av:

kh:

fv:

hv:

fo:

tr: GOTO SDK-erf02

hi:

\------------------------------------------------------------

SDK-erf02
=========

tc:

vn: sperleiszufr

qt: Einfachauswahl

hl:

in:

q: Alles in allem: Wie zufrieden sind Sie insgesamt mit den Bedingungen im Studium?

is:

it:

st:

ao: 1: 1: sehr unzufrieden

ao: 2: 2:

ao: 3: 3:

ao: 4: 4:

ao: 5: 5: sehr zufrieden

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO SDK-stu04

hi:

\------------------------------------------------------------

SDK-stu04
=========

tc:

vn: sabslaja

qt: Einfachauswahl

hl:

in:

q: Sind Sie in einem Lehramtsstudiengang eingeschrieben?

is:

it:

st:

ao1: 1: nein

ao2: 2: ja, und zwar Lehramt an Grundschulen (Primarstufe)

ao3: 3: ja, und zwar Lehramt an Haupt-, Real- und Mittelschulen (Sekundarstufe I)

ao4: 4: ja, und zwar Lehramt an Gymnasien (Sekundarstufe II)

ao5: 5: ja, Lehramt an beruflichen/berufsbildenden Schulen, Berufskollegs

ao6: 6: ja, Lehramt an Förderschulen/Sonderpädagogik

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO SDK-stu06

hi:

\------------------------------------------------------------

SDK-stu06
=========

tc:

vn: sfach1; sfach1o; sfach1ka

qt: Einfachauswahl mit Dropdown

hl:

in:

q1: Bitte wählen Sie Ihr (erstes) Studienfach/Hauptfach aus der unten angegebenen Liste aus.

q2: Bitte wählen Sie Ihr erstes Unterrichtsfach/Hauptfach aus der unten angegebenen Liste aus.

is:

it:

st:

ao: 1: Dropdown Fächerliste (DDM StaBu-Liste)

mv:

ka:

vc: SHOW q1 if sabslaja=1 OR sabslaja=SYSMISS

SHOW q2 if sabslaja=2

av:

kh:

fv:

hv:

fo: Sie haben Ihr Studienfach nicht angegeben. Die Angabe Ihres Studienfachs ist für diese Befragung sehr wichtig. Sollte Ihr Studienfach in der Liste nicht aufgeführt sein, tragen Sie es bitte in dem dafür vorgesehenen Textfeld ein.

(1) offene Abfrage: 50, Anderes Studienfach:

(2) Checkbox: Ich möchte mein Studienfach nicht angeben.

tr: GOTO SDK-stu07

hi:

\------------------------------------------------------------

SDK-stu07
=========

tc:

vn: sfach1o2

qt: Offene Frage

hl:

in:

q1: Bitte tragen Sie Ihr (erstes) Studienfach in das dafür vorgesehene Feld ein.

q2: Bitte tragen Sie Ihr erstes Unterrichtsfach in das dafür vorgesehene Feld ein.

is:

it:

st:

ao1: 1: 60, Prefix: (erstes) Studienfach

ao2: 2: 60, Prefix: erstes Unterrichtsfach

mv:

ka:

vc: SHOW q1 if sabslaja=1 OR sabslaja=SYSMISS

SHOW q2 if sabslaja=2

SHOW ao1 Prefix if sabslaja=1 OR sabslaja=SYSMISS

SHOW ao2 Prefix if sabslaja=2

av:

kh:

fv:

hv:

fo:

tr: GOTO SDK-stu06

hi:

\------------------------------------------------------------

SDK-stu06
=========

tc:

vn: sfazweit1

qt: Einfachauswahl

hl:

in:

q: Studieren Sie noch ein weiteres Fach?

is:

it:

st:

ao1: 1: Nein

ao2: 2: Ja, ein Fach

ao3: 3: Ja, zwei oder mehr Fächer

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO SDK-stu05

hi:

\------------------------------------------------------------

SDK-stu05
=========

tc:

vn: sabsan

qt: Einfachauswahl

hl:

in:

q: Und welchen Abschluss streben Sie in ihrem aktuellen Studiengang an?

is: Bei mehreren Abschlüssen bitte den zeitlich nächsten nennen.

it:

st:

ao1: 1: Bachelor

ao2: 2: Master

ao3: 3: Staatsexamen

ao4: 4: Diplom

ao5: 5: Promotion

ao6: 6: kirchliche Abschlussprüfung

ao7: 7: künstlerische Abschlussprüfung

ao8: 8: anderen Abschluss (bspw. Ausländischer Abschluss, Magister)

ao9: 9: keinen Studienabschluss

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO SDK-stu if sabsan=9

GOTO SDK-stu12

hi:

\------------------------------------------------------------

SDK-stu
=======

tc:

vn: sabsweit; sabsweito

qt: Mehrfachauswahl

hl:

in:

q: Sie haben angegeben in Ihrem aktuellen Studium keinen Studienabschluss anzustreben. Nutzen Sie aktuell hochschulische Weiterbildungsangebote?

is: Bitte alles zutreffende auswählen.

it:

st:

ao1: 1: Nein

ao2: 2: Ja, Zertifikatskurs(e)

ao3: 3: Ja, Seminar(reihe)

ao4: 4: Ja, Workshop(s)

ao5: 5: Ja, Modul/Kurs

ao6: 6: Ja, anderes

ato: Prefix: und zwar:

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO SDK-stu12

hi:

\------------------------------------------------------------

SDK-stu12
=========

tc:

vn: sformpraes; sformdua; sformberu; sformfern; sformsons; sformsonso

qt: Mehrfachauswahl mit offener Angabe

hl:

in:

q: Um welche Form des Studiums handelt es sich bei Ihrem Studiengang?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: 1: Präsenzstudiengang (in Gegensatz zu Fernstudium)

ao2: 2: Dualer Studiengang

ao3: 3: Berufsbegleitender Studiengang

ao4: 4: Fernstudiengang

ao5: 5: anderes,

ato: 30, Prefix: und zwar:

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO SDK-stu14

hi:

\------------------------------------------------------------

SDK-stu14
=========

tc:

vn: ssemhs

qt: offene Frage

hl:

in:

q1: Im wievielten Fachsemester befinden Sie sich zurzeit?

is1: Fachsemester sind die Semester, die sie in Ihrem derzeitigen Bachelor-Studiengang eingeschrieben sind.

is2: Fachsemester sind die Semester, die sie in Ihrem derzeitigen Master-Studiengang eingeschrieben sind.

it:

st:

ao1: 2, Prefix: Zahl der Fachsemester:

mv:

ka:

vc: SHOW is1 if sabsan=1

SHOW is2 if sabsan=2

av: number, 1-2 stellig

kh:

fv:

hv:

fo:

tr: GOTO SDK-stu15

hi:

\------------------------------------------------------------

SDK-stu15
=========

tc:

vn: ssemhs

qt: offene Frage

hl:

in:

q1: Im wievielten Hochschulsemester befinden Sie sich zurzeit?

is: Hochschulsemester sind alle Semester, die Sie seit Ihrer Erstimmatrikulation insgesamt studiert haben (also auch die Zeiten eines möglichen Bachelorstudiums), einschließlich Urlaubs-, Auslands- und Praxissemester.

it:

st:

ao1: 2, Prefix: Zahl der Hochschulsemester:

mv:

ka:

vc:

av: number, 1-2 stellig

kh:

fv:

hv:

fo:

tr: GOTO SDK-erf01

hi:

\------------------------------------------------------------

SDK-erf01
=========

tc:

vn: spernot; spernoto

qt: offene Frage, Einfachauswahl

hl:

in:

q: Wie wurden Ihre bisherigen Studienleistungen in Ihrem aktuellen Studium im Durchschnitt bewertet?

is: Für den Fall, dass Sie keine Noten erhalten, sondern Ihre Studienleistungen mit Punkten, Prozentangaben o. Ä. bewertet werden, rechnen Sie diese bitte in Noten um.

it:

st:

ao1: 3, Prefix: Durchschnittsnote (z.B. 2,5):

ao2: 11: Ich habe bisher keine Noten erhalten / In meinem Studium gibt es keine Noten.

ao3: -12: weiß ich nicht

mv: -11: Ich habe bisher keine Noten erhalten / In meinem Studium gibt es keine Noten.

\-12: weiß ich nicht

ka:

vc:

av: number: \<= dreistellig: 1,0 TO 4,0

kh: Bitte geben Sie Ihren Notendurchschnitt an (1,0 bis 4,0).

fv:

hv:

fo: Bitte die beiden geschlossenen Antwortoptionen/-items neben der Notenabfrage in einer Zeile positionieren.

tr: GOTO SDK-erf03

hi:

\------------------------------------------------------------

SDK-erf03
=========

tc:

vn: sperleisrel

qt: Einfachauswahl

hl:

in:

q: Wie schätzen Sie Ihre bisherigen Studienleistungen in Ihrem aktuellen Studium im Vergleich zu den Leistungen Ihrer Kommiliton(inn)en ein?

is:

it:

st:

ao: 1: 1:unterdurchschnittlich

ao: 2: 2:

ao: 3: 3: durchschnittlich

ao: 4: 4:

ao: 5: 5: überdurchschnittlich

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO SDK-sde01

hi:

\------------------------------------------------------------

SDK-erf03
=========

tc:

vn: sperleiszufr

qt: Einfachauswahl

hl:

in:

q: Wie zufrieden sind Sie insgesamt mit den bisher von Ihnen erbrachten Studienleistungen in Ihrem aktuellen Studium?

is:

it:

st:

ao: 1: 1:sehr unzufrieden

ao: 2: 2:

ao: 3: 3:

ao: 4: 4:

ao: 5: 5: sehr zufrieden

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO SDK-sde01

hi:

\------------------------------------------------------------

SDK-erf03
=========

tc:

vn: studerfolg; masterfolg; promoerfolg

qt: Mehrfachauswahlmatrix

hl:

in:

q: Inwieweit trauen Sie sich zu, …?

is:

it1: studerfolg: … ein Studium erfolgreich abzuschließen?

it2: masterfolg: … ein Masterstudium erfolgreich abzuschließen?

it3: promoerfolg: … eine Promotion erfolgreich abzuschließen?

st:

ao: 1: 1: sehr unwahrscheinlich

ao: 2: 2:

ao: 3: 3:

ao: 4: 4:

ao: 5: 5: sehr wahrscheinlich

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO SDK-sde01

hi:

\------------------------------------------------------------

SDK-sde01
=========

tc:

vn: demosex; demosexo

qt: Einfachauswahl mit offener Angabe

hl:

in:

q: Welches Geschlecht haben Sie?

is:

it:

st:

ao1: 1: männlich

ao2: 2: weiblich

ao3: 3: anderes,

ato: Prefix: und zwar:

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO SDK-sde02

hi:

\------------------------------------------------------------

SDK-sde01
=========

tc:

vn: demosex; demosexo

qt: Einfachauswahl mit offener Angabe

hl:

in:

q: Welches Geschlecht haben Sie?

is:

it:

st:

ao1: 1: männlich

ao2: 2: weiblich

ao3: 3: divers

ao4: 4: keine der genannten Kategorien,

ato: Prefix: sondern:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO SDK-sde02

hi:

\------------------------------------------------------------

SDK-sde02
=========

tc:

vn: demoage

qt: offene Frage

hl:

in:

q: Wie alt sind Sie?

is:

it:

st:

ao1: 2: Prefix: Alter: : Postfix: Jahre

mv:

ka:

vc:

av: number: zweistellig: 16 TO 99

kh: Bitte geben Sie Ihr Lebensalter an (16 bis 99).

fv:

hv:

fo:

tr: SDK-sde03

hi:

\------------------------------------------------------------

SDK-sde03
=========

tc:

vn: demofam

qt: Einfachauswahl

hl:

in:

q: Welchen Familienstand haben Sie?

is:

it:

st:

ao1: 1: nicht verheiratet, ohne feste Partnerbeziehung

ao2: 2: nicht verheiratet, mit fester Partnerbeziehung

ao3: 3: verheiratet/eingetragene Lebenspartnerschaft

mv: -13: Keine Angabe

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

hi:

\------------------------------------------------------------

SDK-sde04
=========

tc:

vn: dkinja

qt: Einfachauswahl

hl:

in:

q: Haben Sie Kinder?

is:

it:

st:

ao1: 1: nein

ao2: 2: ja

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

hi:

\------------------------------------------------------------

SDK-gub01
=========

tc:

vn: gbeges; gartmob; gartseh; gartohr; gartspr; gartpsy; gartsom; garttls; gartson; gartka

qt: Mehrfachauswahl

hl:

in: Im Folgenden stellen wir Ihnen einige kurze Fragen zu möglichen Beeinträchtigungen. Wie für alle Fragen gilt: Die Beantwortung dieser Fragen ist selbstverständlich freiwillig und wir sichern Ihnen Anonymität und den Schutz Ihrer Daten zu.

q: Haben Sie eine oder mehrere der nachfolgend aufgeführten gesundheitlichen Beeinträchtigungen?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: 1: (gbeges): nein (EK)

ao2: 2: (gartmob): Bewegungsbeeinträchtigung (z. B. beim Gehen, Stehen, Greifen)

ao3: 3: (gartseh): Sehbeeinträchtigung/Blindheit

ao4: 4: (gartohr): Hörbeeinträchtigung/Gehörlosigkeit

ao5: 5: (gartspr): Sprechbeeinträchtigung (z. B. Stottern)

ao6: 6: (gartpsy): psychische Erkrankung (z. B. Depression, Essstörung)

ao7: 7: (gartsom): länger dauernde Krankheit/chronische Krankheit (z. B. Rheuma, MS, Darmerkrankung)

ao8: 8: (garttls): Teilleistungsstörung (z. B. Legasthenie, Dyskalkulie)

ao9: 9: (gartson): andere Beeinträchtigung/schwere Erkrankung (z. B. Tumorerkrankung, Autismus-Spektrum-Störung)

ao10: 10: (gartka): Ich möchte die Form meiner Beeinträchtigung nicht nennen. (EK)

mv:

ka: ka1 (ao2 TO ao10): ja, und zwar:

vc:

av:

kh:

fv:

hv:

fo:

tr:

hi:

\------------------------------------------------------------

SDK-sde08
=========

tc:

vn: deltberuv; deltberum

qt: Comparison

hl:

in:

q: Welches ist der höchste berufliche Abschluss Ihres Vaters/Ihrer Mutter?

is:

it1 (deltberuv): Vater

it2 (deltberum): Mutter

st:

ao1: 7: Promotion (Doktortitel)

ao2: 6: Universitätsabschluss

ao3: 5: Fachhochschulabschluss

ao4: 4: Abschluss an einer Meister-, Techniker-/ Fachschule

ao5: 3: Lehre bzw. Facharbeiterabschluss, Abschluss an einer Berufsfach-, Handels-, Berufsaufbauschule

ao6: 2: anderer beruflicher Abschluss

ao7: 1: hat keinen beruflichen Abschluss


mv: -12: weiß ich nicht

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO SDK-sde10

hi:

\------------------------------------------------------------

SDK-sde10
=========

tc:

vn: deltjobv [deltjobvo1] [deltjobvo2]; deltjobm [deltjobmo1] [deltjobmo2]

qt: Comparison

hl:

in:

q: Und welchen Beruf übt Ihr Vater/Ihre Mutter hauptberuflich aus? Bitte erläutern Sie die Tätigkeit Ihres Vaters/Ihrer Mutter kurz.

is: Falls Ihr Vater oder Ihre Mutter zurzeit nicht erwerbstätig sind (z. B. Rentner(in), Pensionär(in), Hausfrau/-mann oder arbeitssuchend), geben Sie bitte die jeweils zuletzt ausgeübte Tätigkeit an.

Bitte tragen Sie die genaue Bezeichnung und Tätigkeit inklusive Führungsaufgaben ein. 
Zum Beispiel:

\- Bankkaufmann/-frau (nicht: Angestellte/r) 

Beratung, Verkauf von Finanzprodukten, Abteilungsleitung

\- Zollbeamte(r) im gehobenen Dienst (nicht: Beamter/in)

Zollfahndung, Einsatzplanung

\- Maschinenbauingenieur(in) (nicht: Ingenieur/in)

Konstruktion, Optimierungsprozesse, Produktionsleitung

It1: Vater

It2: Mutter

st:

ao1: 1: 50: Prefix: Berufsbezeichnung:

ao2: 2: 50: Prefix: Tätigkeitsbeschreibung:

ao3: -11: nie berufstätig gewesen

ao4: -12: weiß ich nicht

mv: -11: nie berufstätig gewesen

\-12: weiß ich nicht

ka:

vc:

av:

kh:

fv:

hv:

fo: Vater“ und „Mutter“ bitte in einer extra Zeile positionieren, die mittig über den jeweils darunterliegenden Antwortzeilen liegt (siehe Darstellung hierunter):

Vater Mutter

Berufsbezeichnung: Eingabefeld Eingabefeld

Tätigkeitsbeschreibung: Eingabefeld Eingabefeld

weiß ich nicht Kästchen Kästchen

o Bei Angabe von „weiß ich nicht“, sollen die Textfelder in der jeweiligen
Spalte bitte nicht ausgefüllt werden können und umgekehrt (Exklusivkategorie).

tr: GOTO SDK-sde21

hi:

\------------------------------------------------------------

SDK-sde21
=========

tc:

vn: deltgebv; deltgebm

qt: Comparison

hl:

in:

q: Wo wurden Ihre Eltern geboren?

is:

it1 (deltgebv): Vater

it2 (deltgebm): Mutter

st:

ao1: 1: in Deutschland

ao2: 2: in einem anderen Land


mv: -12 weiß ich nicht

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO CMI13 if deltgebv=2 OR deltgebm=2

GOTO SDK-vbi2

hi:

\------------------------------------------------------------

CMI13
=====

tc:

vn: deltgkov

qt: Einfachauswahl

hl:

in:

q: In welchem Land wurde Ihr Vater geboren?

is: Bitte wählen Sie zunächst den Kontinent aus.

it:

st:

ao1: 100: Europa

ao2: 200: Afrika

ao3: 300: Amerika

ao4: 400: Asien

ao5: 500: Australien und Ozeanien

mv:

ka:

vc: SHOW Einfachauswahl if deltgebv=2

av:

kh:

fv:

hv:

fo:

tr:

hi:

\------------------------------------------------------------

CMI13
=====

tc:

vn: deltgkom

qt: Einfachauswahl

hl:

in:

q: In welchem Land wurde Ihre Mutter geboren?

is: Bitte wählen Sie zunächst den Kontinent aus.

it:

st:

ao1: 100: Europa

ao2: 200: Afrika

ao3: 300: Amerika

ao4: 400: Asien

ao5: 500: Australien und Ozeanien

mv:

ka:

vc: SHOW Einfachauswahl if deltgebm=2

av:

kh:

fv:

hv:

fo:

tr: GOTO CMI14

hi:

\------------------------------------------------------------

CMI14
=====

tc:

vn: deltgstav

qt: Einfachauswahl mit Dropdown

hl:

in:

q: Bitte geben Sie hier das Geburtsland Ihres Vaters an.

is:

it:

st:

ao: Dropdown Staatenliste_DBI_Eltern

mv:

ka:

vc: SHOW Einfachauswahl if deltgkov\>0

av:

kh:

fv:

hv:

fo:

tr:

hi:

\------------------------------------------------------------

CMI14
=====

tc:

vn: deltgstavo

qt: offene Frage

hl:

in:

q: Bitte geben Sie hier das Geburtsland Ihres Vaters an.

is:

it:

st:

ao1: 30: Prefix: Geburtsland des Vaters:

mv:

ka:

vc: SHOW Einfachauswahl if deltgkov=SYSMISS AND deltgebv=2

av:

kh:

fv:

hv:

fo:

tr:

hi:

\------------------------------------------------------------

CMI14
=====

tc:

vn: deltgstam

qt: Einfachauswahl mit Dropdown

hl:

in:

q: Bitte geben Sie hier das Geburtsland Ihrer Mutter an.

is:

it:

st:

ao: Dropdown Staatenliste_DBI_Eltern

mv:

ka:

vc: SHOW Einfachauswahl if deltgkom\>0

av:

kh:

fv:

hv:

fo:

tr:

hi:

\------------------------------------------------------------

CMI14
=====

tc:

vn: deltgstamo

qt: offene Frage

hl:

in:

q: Bitte geben Sie hier das Geburtsland Ihrer Mutter an.

is:

it:

st:

ao1: 30: Prefix: Geburtsland der Mutter:

mv:

ka:

vc: SHOW Einfachauswahl if deltgkom=SYSMISS AND deltgebm=2

av:

kh:

fv:

hv:

fo:

tr: GOTO SDK-vbi2

hi:

\------------------------------------------------------------

SDK-vbi2
========

tc:

vn: vsbplz; [vsbplzo]; vsbort

qt: offene Frage

hl:

in:

q: Bitte geben Sie die fünfstellige Postleitzahl des Ortes an, in dem Sie bei Erhalt Ihrer Studienberechtigung gewohnt haben.

is:

it:

st:

ao1: 5, Prefix: Postleitzahl:

mv:

ka:

vc:

av: number, 5-stellig: 01000 TO 99999

kh:

fv: sf_ao: Falls Sie die Postleitzahl nicht kennen, geben Sie bitte den Ort an:
: 12 Stellen

hv:

fo: Softreminder: Bitte den Text „[Textfeld; 12 Stellen]“ erst dann einblenden,
wenn die PLZ nicht angegeben wurde.

tr: GOTO SDK-vbi2_1

hi:

\------------------------------------------------------------

SDK-vbi2_1
==========

tc:

vn: vsbplz; [vsbplzo]; vsbort

qt: offene Frage

hl:

in:

q: Bitte geben Sie die fünfstellige Postleitzahl des Ortes an, in dem Sie bei Erhalt Ihrer Studienberechtigung gewohnt haben.

is:

it:

st:

ao1: 5, Prefix: Postleitzahl:

ao2: 25, Prefix: Falls Sie die Postleitzahl nicht kennen, geben Sie bitte den Ort an:

mv:

ka:

vc:

av: number, 5-stellig: 00000 TO 99999

kh:

fv:

hv:

fo:

tr:

hi:

\------------------------------------------------------------

SDK-vbi3
========

tc:

vn: vsbart

qt: Einfachauswahl

hl:

in:

q: Welche Studienberechtigung hatten Sie bei Ihrer Erstimmatrikulation?

is:

it:

st:

ao1: 1: allgemeine Hochschulreife

ao2: 2: fachgebundene Hochschulreife

ao3: 3: Fachhochschulreife

ao4: 4: andere Studienberechtigung

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO SDK-vbi3_1

hi:

\------------------------------------------------------------

SDK-vbi3_1
==========

tc:

vn: vsbart

qt: Einfachauswahl

hl:

in:

q: Die Berechtigung zum Studium kann in Deutschland auf verschiedenen Wegen erfolgen: Zum einen (klassisch) über ein Schulzeugnis, zum anderen aber auch über die Anerkennung beruflicher Qualifikationen oder besonderer Eignungen.

Auf welchem Weg erfolgte Ihre Zulassung zu Ihrem ersten Studium?

is:

it:

st:

ao1: 1: Schulzeugnis (Abitur, Fachhochschulreife, fachgebundene Hochschulreife, auch Abendgymnasium/Kolleg )

ao2: 2: Berufliche Qualifikation (Fortbildungsabschluss als Meister o.ä.; Ausbildungsabschluss und Berufspraxis)

ao3: 3: Eignungs- bzw. Begabtenprüfung

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

hi:

\------------------------------------------------------------

SDK-vbi3_2
==========

tc:

vn: vsbart

qt: Einfachauswahl

hl:

in:

q: Welchen höchsten Schulabschluss haben Sie vor dem Studium erworben?

is:

it:

st:

ao1: 1: allgemeine Hochschulreife

ao2: 2: fachgebundene Hochschulreife

ao3: 3: Fachhochschulreife

ao4: 4: Mittlere Reife

ao5: 5: Hauptschulabschluss

ao6: 6: Anderer Abschluss

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO SDK-vbi5

hi:

\------------------------------------------------------------

SDK-vbi5
========

tc:

vn: vsbstyp; vsbtypo

qt: Einfachauswahl mit offener Abfrage

hl:

in:

q: Auf welchem Schultyp bzw. auf welchem Weg haben Sie Ihre Studienberechtigung erworben?

is:

it:

st:

ao1: 1: gymnasiale Oberstufe (Gymnasium, Gesamtschule, berufliches Gymnasium, Fachgymnasium, Oberstufenzentrum u.a.)

ao2: 2: Berufsoberschule, Fachoberschule, andere berufsbildende Schulen (Berufsfachschule, Berufskolleg u.a.)

ao3: 3: Abendgymnasium, Kolleg (nicht Berufskolleg) 

ao4: 4: berufliche Aufstiegsfortbildung (Meister(in), Fachwirt(in), Erzieher(in), Techniker(in) u. a.)

ao5: 5: abgeschlossene Berufsausbildung mit mindestens dreijähriger Berufserfahrung und Eignungsfeststellung, Begabtenprüfung oder Probestudium

ao6: 6: auf einem anderen Weg,

ato: 50: Prefix: und zwar:

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: Bitte die Beispiele in Klammern in etwas kleinerer Schriftgröße (2pt kleiner) umsetzen.

tr: GOTO SDK-vbi5

hi:

\------------------------------------------------------------

SDK-vbi5_1
==========

tc:

vn: vsbstyp1-15; vsbtypob

qt: Mehrfachauswahl mit offener Abfrage

hl:

in:

q: Auf welchem Schultyp bzw. auf welchem Weg haben Sie Ihre Studienberechtigung erworben?

is: Mehrfachnennungen möglich

it:

st:

ao1: (vsbtyp1): Gymnasium

ao2: (vsbtyp2): Gesamtschule mit gymnasialer Oberstufe

ao3: (vsbtyp3): Schule in freier Trägerschaft (z.B. Waldorfschule)

ao4: (vsbtyp4): Abendgymnasium, Kolleg (nicht Berufskolleg)

ao5: (vsbtyp5): Fachgymnasium, berufliches Gymnasium

ao6: (vsbtyp6): Berufsfachschule

ao7: (vsbtyp7): Berufsoberschule

ao8: (vsbtyp8): Fachoberschule

ao9: (vsbtyp9): andere berufsbildende Schule (Fachschule, Fachakademie, Berufskolleg u. a.)

ao10: (vsbtyp10): berufliche Aufstiegsfortbildung als Meister, Techniker, Fachwirt, Erzieher o.ä.

ao11: (vsbtyp11): abgeschlossene Berufsausbildung mit anschließender Berufspraxis

ao12: (vsbtyp12): Eignungsprüfung für Kunst- und Musikhochschulen

ao13: (vsbtyp13): Begabtenprüfung

ao14: (vsbtyp14): Mediziner\*innen-Test (TMS)

ao15: (vsbtyp15): auf einem anderen Weg,

ato: (vsbtypob): Prefix: und zwar:

mv:

ka: ka1 (ao1 TO ao9) Schulischer Weg: : ka2(ao10 TO ao11) Berufliche Qualifikation: :ka3(ao12 TO ao15) Eignungsprüfungen:

vc:

av:

kh:

fv:

hv:

fo: Bitte die Beispiele in Klammern in etwas kleinerer Schriftgröße (2pt kleiner) umsetzen.

tr: GOTO SDK-vbi7

hi:

\------------------------------------------------------------

SDK-vbi7
========

tc:

vn: vsbnoteo; vsbnote

qt: offene Frage

hl:

in:

q: Welche Abschlussnote hatten Sie in dem Zeugnis, das Sie zur Aufnahme eines Studiums berechtigt?

is: (bitte Punktzahl ggf. in Note umrechnen)

it:

st:

ao1: 3: Prefix: Durchschnittsnote (z. B. 2,5):

ao2: -11: Ich habe keine Note erhalten. (EK)

ao3: -12: weiß ich nicht (EK)

mv: -11: Ich habe keine Note erhalten

\-12: weiß ich nicht

ka:

vc:

av: number: zweistellig: 1,0 TO 4,0

kh: Bitte geben Sie Ihren Notendurchschnitt an (1,0 bis 4,0).

fv:

hv:

fo: Die Antwortoptionen bitte als Exklusivkategorien programmieren.

tr:

hi:

\------------------------------------------------------------

SDK-vbi8
========

tc:

vn: vsbzpj

qt: Einfachauswahl mit Dropdown

hl:

in:

q: In welchem Jahr haben Sie die Hochschulzugangsberechtigung erlangt

(Zeitpunkt der Zeugnisübergabe)?

is:

it:

st:

ao1: 1: Jahr:

ao2: -12: weiß ich nicht

mv: -12: weiß ich nicht

ka: Jahr: alle ao

vc:

av:

kh:

fv:

hv:

fo:

tr:

hi:

\------------------------------------------------------------

SDK-vbi8_1
==========

tc:

vn: vsbzpj

qt: offene Frage, Mehrfachauswahl

hl:

in:

q: In welchem Jahr haben Sie die Hochschulzugangsberechtigung erlangt (Zeitpunkt der Zeugnisübergabe)?

is:

it:

st:

ao1: 4: Prefix: Jahr:

ao2: -12: weiß ich nicht (EK)

mv: -12: weiß ich nicht

ka:

vc:

av: number: vierstellig

kh:

fv:

hv:

fo:

tr: GOTO SDK-vbi1001 if

hi:

\------------------------------------------------------------

SDK-vbi1001
===========

tc: SDK-vbi5 oder SDK-vbi5_1

vn: vausbja

qt: Einfachauswahl

hl:

in:

q: Haben Sie vor Ihrer Erstimmatrikulation bereits eine Berufsausbildung begonnen bzw. abgeschlossen?

is:

it:

st:

ao1: 1: nein

ao2: 2: ja, begonnen und nicht abgeschlossen

ao3: 3: ja, begonnen und abgeschlossen

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO SDK-stu16

hi:

\------------------------------------------------------------

SDK-stu16
=========

tc:

vn: sabsja

qt: Einfachauswahl

hl:

in:

q: Haben Sie bereits einen Hochschulabschluss erworben?

is:

it:

st:

ao1: 1: Nein

ao2: 2: Ja

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

hi:

\------------------------------------------------------------

SDK-stu16_1
===========

tc: sabsja==2

vn: sabszp

qt: Einfachauswahl mit Dropdown x2

hl:

in:

q: Wann haben Sie diesen Abschluss erworben?

is:

it:

st:

ao: Dropdown Monat

ao1: 1: Januar

ao2: 2: Februar

ao3: 3: März

ao4: 4: April

ao5: 5: Mai

ao6: 6: Juni

ao7: 7: Juli

ao8: 8: August

ao9: 9: September

ao10: 10: Oktober

ao11: 11: November

ao12: 12: Dezember

ao: Dropdown Jahr

mv:

ka: ka1(Dropdown Monat): Monat

ka2(Dropdown Jahr): Jahr

vc:

av:

kh:

fv:

hv:

fo:

tr:

hi:

\------------------------------------------------------------

SDK-stu17
=========

tc: sabsja==2

vn: sabser

qt: Einfachauswahl

hl:

in:

q: Welchen Abschluss haben Sie bereits erworben?

is:

it:

st:

ao1: 1: Bachelor

ao2: 2: Master

ao3: 3: Staatsexamen

ao4: 4: Diplom

ao5: 5: Promotion

ao6: 6: kirchliche Abschlussprüfung

ao7: 7: künstlerische Abschlussprüfung

ao8: 8: anderen Abschluss (bspw. ausländischer Abschluss)

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO SDK-stu0

hi:

\------------------------------------------------------------

SDK-stu0
========

tc: sabsja==2

vn: sabsla

qt: Einfachauswahl

hl:

in:

q: Handelt es sich hierbei um ein Lehramtsstudium?

is: Bei mehreren Hochschulabschlüssen bitte den letzten angeben.

it:

st:

ao1: 1: Nein

ao2: 2: Ja

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO SDK-stu21

hi:

\------------------------------------------------------------

SDK-stu21
=========

tc: sabsja==2

vn: sabsernot

qt: Einfachauswahl mit offene Angabe

hl:

in:

q: Welche Abschlussnote haben sie in ihrem vorhergien Studium erhalten?

is: Für den Fall, dass Sie keine Noten erhalten haben, sondern Ihre Studienleistungen mit Punkten, Prozentangaben o. Ä. bewertet werden, rechnen Sie diese bitte in eine Abschlussnote um.

it:

st:

ao1: 1: offene Angabe: 3, Prefix: Abschlussnote (z. B. 2,5):

ao2: -11: Ich habe keine Note erhalten. / In meinem vorigen Studium gab es keine Noten.

ao3: -12: Weiß ich nicht

mv:

ka:

vc:

av: 3-stellig: 1,0 TO 4,0

kh:

fv:

hv:

fo:

tr:

GOTO SDK-stu17 IF sabser=1

GOTO SDK-stu17 IF sabser\>1

hi:

\------------------------------------------------------------

SDK-stu17
=========

tc:

vn: mastplan; promoplan

qt: Einfachauswahl matrix

hl:

in:

q: Planen Sie nach dem Studium…

is:

it1: … ein Masterstudium aufnehmen?

It2: … eine Promotion aufnehmen?

st:

ao1:1: 1: sehr unwahrscheinlich

ao2: 2: 2:

ao3: 3: 3:

ao4: 4: 4:

ao5: 5: 5: sehr wahrscheinlich

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO SDK-pla02

hi:

\------------------------------------------------------------

SDK-stu17
=========

tc:

vn: promoplan

qt: Einfachauswahl mit Horizontalen ao

hl:

in:

q: Planen Sie nach dem Studium…

is:

it:

st: … eine Promotion aufnehmen?

ao1:1: 1: sehr unwahrscheinlich

ao2: 2: 2:

ao3: 3: 3:

ao4: 4: 4:

ao5: 5: 5: sehr wahrscheinlich

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO SDK-pla02

hi:

\------------------------------------------------------------

SDK-pla02
=========

tc:

vn: ssweja; saweja; shwja; ssuja

qt: Einfachauswahl matrix

hl:

in:

q: Haben Sie seit Ihrer Erstimmatrikulation…

is: (Nicht gemeint sind Veränderungen bzw. Unterbrechungen beim Übergang vom Bachelor- ins Masterstudium)

it1: ssweja: … das Studienfach gewechselt?

it2: saweja: … den Abschluss gewechselt?

it3: shwja: … die Hochschule gewechselt?

it4: ssuja: … das Studium zwischenzeitlich unterbrochen?

st:

ao1: 1: ja

ao2: 2: nein

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

hi:

\------------------------------------------------------------

SDK-stu17
=========

tc:

vn: promoplan

qt: Einfachauswahl mit Horizontalen ao

hl:

in:

q: Planen Sie nach dem Studium…

is:

it:

st: … eine Promotion aufnehmen?

ao1: 1: 1: sehr unwahrscheinlich

ao2: 2: 2:

ao3: 3: 3:

ao4: 4: 4:

ao5: 5: 5: sehr wahrscheinlich

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO SDK-pla02

hi:

\------------------------------------------------------------

SDK-pla02
=========

tc:

vn: ssahswe; ssafawe; ssaunt; ssaaja

qt: Einfachauswahl matrix

hl:

in:

q: Wie ernsthaft denken Sie zur Zeit daran …

is:

it1: (ssahswe): … die Hochschule zu wechseln?

it2: (ssafawe): … Ihr Studienfach zu wechseln?

it3: (ssaunt): … Ihr aktuelles Studium zu unterbrechen?

it4: (ssaaja): … das Studium ganz aufzugeben?

st:

ao1: 1: 1: gar nicht

ao2: 2: 2:

ao3: 3: 3:

ao4: 4: 4:

ao5: 5: 5: sehr ernsthaft

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO SEK-woh01

hi:

\------------------------------------------------------------

SEK-woh01
=========

tc:

vn: wohnfo

qt: Einfachauswahl

hl:

in:

q1: Wie wohnen Sie während der Vorlesungszeit des aktuellen Semesters [Individualisierung]?

q2: Wie wohnen Sie während der Vorlesungszeit des aktuellen Semesters?

is: Wenn Sie bei Ihren Eltern oder anderen Verwandten/Bekannten wohnen, geben Sie bitte die Wohnform Ihrer Eltern bzw. der Verwandten/Bekannten an.

it:

st:

ao1: 1: zur Miete (auch Wohngemeinschaft)

ao2: 2: zur Untermiete

ao3: 3: als (Mit-)Eigentümer(in)

ao4: 4: im Einzelzimmer (Flurgemeinschaft)

ao5: 5: im Einzelzimmer (in einer Wohngruppe)

ao6: 6: im Einzelappartement

ao7: 7: in einer Mehrzimmerwohnung (für Paare oder Studierende mit Kind)

mv:

ka: ka1: ao1 TO ao3: in einer Wohnung, einem Zimmer oder einem Haus:

ka2: ao4TO ao7: im Studierendenwohnheim:

vc: SHOW (Individualisierung) if wohnort=3

SHOW q1 if sformfern!=1 AND sformdual!=0

SHOW q2 if sformfern=1 AND sformdual=0

av:

kh:

fv:

hv:

fo:

tr: GOTO SDK-woh02

hi:

\------------------------------------------------------------

SDK-woh02
=========

tc:

vn: wohnal; wohnwg; wohnel; wohnpar; wohnkin; wohnfam; wohnsons

qt: Mehrfachauswahl

hl:

in:

q1: Mit wem wohnen Sie während der Vorlesungszeit des aktuellen Semesters [Individualisierung] zusammen?

q2: Mit wem wohnen Sie zusammen?

is: Bitte alles Zutreffende auswählen.

it:

st: Ich wohne …

ao1: 1: allein [EK]

ao2: 2: mit Mitbewohner(inne)n in einer Wohngemeinschaft.

ao3: 3: bei/mit meinen Eltern (bzw. Elternteil)

ao4: 4: mit meinem/meiner (Ehe-) Partner(in).

ao5: 5: mit meinem Kind/meinen Kindern.

ao6: 6: mit anderen Familienangehörigen.

ao7: 7: mit anderen Personen.

mv:

ka:

vc: SHOW Individualisierung if wohnort=3

SHOW q1 if sformfern!=1 AND sformdual!=0

SHOW q2 if sformfern=1 AND sformdual=0

av:

kh:

fv:

hv:

fo:

tr: GOTO SDK-fin01

hi:

\------------------------------------------------------------

 SDK-fin01
==========

tc:

vn: eaktsens

qt: Einfachauswahl

hl:

in:

q: Sind Sie während der Vorlesungszeit [Individualisierung] erwerbstätig?

is: Mit \*\*„*Erwerbstätigkeit(en)*“\*\* sind sämtliche Tätigkeiten gemeint, mit denen Sie im aktuellen Semester Geld verdienen (z. B. Nebenjob, Berufstätigkeit, freiberufliche/selbständige Tätigkeit).

it:

st:

ao1: 1: Nein

ao2: 2: Ja, mit einer Tätigkeit

ao3: 3: Ja, mit zwei verschiedenen Tätigkeiten

ao4: 4: Ja, mit drei oder mehreren Tätigkeiten

mv:

ka:

vc: SHOW Individualisierung if sformdua==1 : neben Ihrer Tätigkeit in der Ausbildungsstätte

av:

kh:

fv:

hv:

fo:

tr: GOTO SDK-fin04 if eaktsens=2 OR eaktsens=3 OR eaktsens=4

hi:

\------------------------------------------------------------

SDK-fin04
=========

tc: if eaktsens=2 OR eaktsens=3 OR eaktsens=4

vn:

qt: Einfachauswahlmatrix

hl:

in:

q: In welchem Maße [Individualisierung] einen fachlichen Bezug zu Ihrem aktuellen Studium?

is:

it: 1: Tätigkeit A [Individualisierung]

it: 2: Tätigkeit B [Individualisierung]

it: 3: Tätigkeit C [Individualisierung]

st:

ao1: 1: 1: in gar keinem Maße

ao2: 2: 2:

ao3: 3: 3:

ao4: 4: 4:

ao5: 5: : in sehr hohem Maße

mv:

ka:

vc: SHOW Individualisierung if eaktsens=2 : hat ihre Erwerbstätigkeit

SHOW Individualisierung if eaktsens=2 AND sformdua=1 : hat Ihre Erwerbstätigkeit, die Sie neben Ihrer Tätigkeit im Ausbildungsbetrieb ausüben,

SHOW Individualisierung if eaktsens=3 : haben Ihre Erwerbstätigkeiten 

SHOW Individualisierung if eaktsens=3 AND sformdua=1 : haben Ihre Erwerbstätigkeiten, die Sie neben Ihrer Tätigkeit im Ausbildungsbetrieb ausüben,

SHOW Individualisierung if eaktsens=4 : haben Ihre Erwerbstätigkeiten

SHOW Individualisierung if eaktsens=4 AND sformdua=1 : haben Ihre Erwerbstätigkeiten, die Sie neben Ihrer Tätigkeit im Ausbildungsbetrieb ausüben,

SHOW it1 if eaktsens=2

SHOW it1 if eaktsens=2 AND sformdua=1

SHOW it1 & it2 if eaktsens=3

SHOW it1 & it2 if eaktsens=3 AND sformdua=1 :

SHOW it1 & it2 & it3 if eaktsens=4 :

SHOW it1 & it2 & it3 if eaktsens=4 AND sformdua=1 :

av:

kh:

fv:

hv:

fo: It1 den Text “Tätigkeit A” nicht anzeigen

tr: ?

hi:

\------------------------------------------------------------

SEK-aer01
=========

tc:

vn: ainfaus

qt: Einfachauswahl

hl:

in:

q: Haben Sie sich während Ihres Studiums studienbezogen im Ausland aufgehalten?

is: (z. B. Auslandsstudium/-semester, Auslandspraktikum, Sprachkurs im Ausland, Studienreise im Ausland, Projektarbeit im Ausland, Summerschool im Ausland)

it:

st:

ao1: 1: Nein

ao2: 2: Ja, ein Aufenthalt

ao3: 3: Ja, zwei Aufenthalte

ao4: 4: Ja, drei oder mehr Aufenthalte

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO ?

hi:

\------------------------------------------------------------

SEK-aer01
=========

tc:

vn:

qt: Einfachauswahl

hl:

in:

q1: Beabsichtigen Sie künftig einen studienbezogenen Auslandsaufenthalt durchzuführen?

q2: Beabsichtigen Sie einen weiteren studienbezogenen Auslandsaufenthalt durchzuführen?

is:

it:

st:

ao1: 1: Nein, kein Interesse

ao2: 2: Nein, sehe keine Realisierungschance

ao3: 3: Weiß ich noch nicht

ao4: 4: Ja

mv:

ka:

vc: SHOW q1 if ainfaus=1

SHOW q2 if ainfaus=2 OR ainfaus=3 OR ainfaus=4

av:

kh:

fv:

hv:

fo:

tr: GOTO SDK-zei01

hi:

\------------------------------------------------------------

SDK-zei01
=========

tc:

vn: zlvwo; zseswo; zerwo; zcarwo; zlvwo2; zseswo2; zerwo2; zcarwo2

qt: offene Frage Matrix

hl:

in:

q: Wie viele Stunden wenden Sie in einer für Sie typischen Woche für folgende Aktivitäten auf?

is: Bitte runden Sie Ihre Zeitangaben jeweils auf volle Zeitstunden.

it: (zlvwo): Während der Vorlesungszeit / Studienphase

it: 2: Während der vorlesungsfreien Zeit / Praxisphase

st:

ao1: 1: Lehrveranstaltungen (Vorlesungen, Seminare, Übungen, Tutorien usw.)

ao2: 2: Selbststudium (Vor‐/Nachbereitung, Referate, Fachlektüre, Studien-/Haus-/Abschlussarbeiten, stud. Lerngruppen, Prüfungsvorbereitung usw.)

ao3: 3: Erwerbstätigkeit (Nebenjob, Beruf, freiberufliche/selbstständige Tätigkeit usw.)

ao4: 4: Pflege- und Betreuungsarbeiten (Familienleben, Kinderbetreuung, Pflege Angehöriger usw.)

mv:

ka:

vc: offene Frage Matrix if sformdua=0 AND sformfern=0 AND sformberu=0

av: number: \<= zweistellig, 0 TO 99

kh: Bitte geben Sie volle Zeitstunden an (0 bis 99).

fv:

hv:

fo:

tr:

hi:

\------------------------------------------------------------

SDK-zei01
=========

tc:

vn:

qt: Einfachauswahlmatrix

hl:

in:

q: Wie wichtig sind Ihnen die folgenden Aspekte des weiteren Berufs- und
Lebensweges?

is:.

it: 1: hohes Einkommen

it: 2: prestigeträchtige Berufsposition

it: 3: sicherer Arbeitsplatz

it: 4: gute Aufstiegsmöglichkeiten

it: 5: flexible Arbeitszeiten

it: 6: die Erwartungen meiner Vorgesetzten erfüllen

it: 7: verantwortungsvolle Aufgaben übernehmen

it: 8: eigene Ideen verwirklichen zu können

it: 9: selbstständig Entscheidungen treffen zu können

it: 10: eine Arbeit, die mir immer wieder neue Aufgaben stellt

it: 11: Möglichkeit zu wissenschaftlicher Tätigkeit

it: 12: anderen Menschen helfen zu können

it: 13: ein Beruf, in dem man Nützliches für die Allgemeinheit tun kann

it: 14: Vereinbarkeit von Privatleben (Familie) und Beruf

it: 15: eine glückliche Beziehung zu führen

it: 16: eine Familie zu gründen

st:

ao1: 1: 1: unbedeutend

ao2: 2: 2:

ao3: 3: 3:

ao4: 4: 4:

ao5: 5: 5: sehr bedeutend

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

hi:
