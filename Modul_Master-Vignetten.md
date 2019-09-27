Master-Vignetten

\--------------------------------

mvig[deck][vignr]
=================

tc: 

vn: mabew

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl: Attraktivität eines Masterstudiums

in: Nachfolgend bitten wir Sie, für vier hypothetische Masterstudiengänge mit
unterschiedlichen Eigenschaften einzuschätzen, wie wahrscheinlich Sie sich
bewerben würden. Die Merkmale der Studiengänge sind jeweils in kurzen Texten
dargestellt.

Es handelt sich um einen Studiengang an einer staatlichen oder privaten
Hochschule, der auf Ihrem angestrebten Bachelorabschluss fachlich aufbaut.
Wohnkosten und Freizeitmöglichkeiten entsprechen in etwa Ihrem jetzigen
Studienort.

in1: [vigA]

in2: [vigB]

in3: [vigC]

q4: Wie wahrscheinlich würden Sie sich auf diesen Masterstudiengang bewerben?

is:

it:

st:

ao1: 0: sehr wahrscheinlich

ao2: 1:

ao3: 2:

ao4: 3:

ao5: 4:

ao6: 5:

ao7: 6:

ao8: 7:

ao9: 8:

ao10: 9:

ao11: 10: sehr wahrscheinlich

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-ma02

hi: Filter am Anfang des Moduls als Einblendbedingung (nur Bachelorstudierende ab dem 4 Semester IF sabsan = 1 AND ssemhs>=4) nötig, oder wird die Zuweisung in das Modul anderweitig gesteuert? Und wenn hier gefiltert wird, muss die Einblendbedingung dann auf jede Seite im Modul?
vig1, vig2 und vig3 sind Absätze der Vignette, die Zuordnung und Auswahl der
Vignetten wird in einer Excel-Liste geliefert: [Master-Vignetten](https://github.com/dzhw/SiD/blob/master/Vignetten_Master.xls)

\--------------------------------

KSM-ma02
========

tc:

vn: maber

qt: Einfachauswahl mit vertikalen Antwortoptionen

hl:

in:

q: Wissen Sie schon, welchen Beruf Sie ergreifen möchten?

is:

it:

st:

ao1: 1: nein, noch offen

ao2: 2: ja, mit einiger Sicherheit

ao3: 3: ja, mit großer Sicherheit

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-ma03 if maber==2 OR maber==3

GOTO KSM-ma04 if maber==1

hi:

\--------------------------------

KSM-ma03
========

tc:

vn: berufswahl

qt: offene Frage

hl:

in:

q: Bitte nennen Sie die genaue Berufsbezeichnung:

is:

it:

st:

ao: (berufswahl): [90 pt, einzeilig, 255 Zeichen]

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-ma04

hi:

\--------------------------------

KSM-ma04
========

tc:  (alle)

vn: bervorb

qt: Einfachauswahl mit horizontalen Antwortoptionen

hl:

in:

q: Wie gut fühlen Sie sich durch das Studium für die Ausübung eines Berufs
vorbereitet?

is:

it:

st:

ao1: 1: überhaupt nicht vorbereitet

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr gut vorbereitet

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-ma05

hi:

\--------------------------------

KSM-ma05
========

tc:

vn: jobfach; jobabsch; joblohn; joberfü

qt: Einfachauswahlmatrix

hl:

in:

q: Inwiefern erwarten Sie Schwierigkeiten nach Ihrem Bachelorabschluss, eine
Stelle zu finden, die...?

is:

it1: (jobfach): ... Ihren fachlichen Fähigkeiten entspricht

it2: (jobabsch): ... Ihrem Hochschulabschluss entspricht

it3: (joblohn): ... Ihren Lohnansprüchen genügt

it4: (joberfü): ... Sie wirklich erfüllt

st:

ao1: 1: überhaupt nicht vorbereitet

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: sehr gut vorbereitet

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-ma06

hi:

\--------------------------------

KSM-ma06
========

tc:  

vn: balohn, baloho

qt: Einfachauswahl mit offener Angabe

hl:

in:

q: Wie schätzen Sie Ihr künftiges monatliches Nettogehalt mit einem
!!Bachelorabschluss!! ein?

is:

it:

st:

ao1: 1: (balohno) [number, 20pt, 5Zeichen]

ao2: 2: weiß nicht

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

\--------------------------------

KSM-ma06
========

tc: 

vn: malohn, malohno

qt: Einfachauswahl mit offener Angabe

hl:

in:

q: Wie schätzen Sie Ihr künftiges monatliches Nettogehalt mit einem
!!Masterabschluss!! ein?

is:

it:

st:

ao1: 1: (malohno): [number, 20pt, 5 Zeichen]

ao2: 2: weiß nicht

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: 
GOTO KSM-ma07 IF mastplan = 4 OR mastplan = 5
GOTO KSM-ma08 IF mastplan = 1 OR mastplan = 2
GOTO KSM-ma09 IF mastplan = 3

hi: Hier in Abhängigkeit von der Absicht ein Masterstudium aufzunehmen auf die folgenden Fragen weiterleiten

\--------------------------------

KSM-ma07
========

tc: 

vn: mastergrund1- mastergrund15; mastergrund15o

qt: Einfachauswahlmatrix

hl:

in:

q: Im Laufe dieser Befragung haben Sie angegeben, dass Sie ein Masterstudium
planen. Aus welchem Grund möchten Sie ein Masterstudium aufnehmen?

is:

it1: (mastergrund1): um meinen Berufswunsch zu erfüllen

it2: (mastergrund2): um meine Berufsaussichten zu verbessern

it3: (mastergrund3): um meine beruflichen Möglichkeiten zu erweitern

it4: (mastergrund4): um mir ein höheres Einkommen zu sichern

it5: (mastergrund5): weil der Master ein höheres soziales Ansehen besitzt

it6: (mastergrund6): um eine gute wissenschaftliche Ausbildung zu erhalten

it7: (mastergrund7): um mich persönlich zu entfalten

it8: (mastergrund8): weil es in meinem angestrebten Berufsfeld üblich ist

it9: (mastergrund9): um mich fachlich zu spezialisieren

it10: (mastergrund10): um länger an der Hochschule bleiben zu können

it11: (mastergrund11): um die Erwerbstätigkeit aufzuschieben

it12: (mastergrund12): um später in der Wissenschaft zu arbeiten

it13: (mastergrund13): weil ich noch nicht weiß, was ich sonst machen soll

it14: (mastergrund14): weil mein\*e Professor\*in mich dazu ermutigt hat

it15: (mastergrund15): anderes, und zwar... [mastergrund15o]

st:

ao1: 1: trifft überhaupt nicht zu

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: trifft voll und ganz zu

mv:

ka:

vc: 

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-ma09

hi: Wo und mit welcher Variable „Masterintention“ erhoben wird, ist mir nicht
klar Variablenbezug zur Einblendbedingung fehlt noch --> Antwort:  IF mastplan = 4 OR mastplan = 5, wird beim Seitenübergang von KSM-ma06 nach KSM-07/08 definiert.

\--------------------------------

KSM-ma08
========

tc:

vn: mastercontra1- mastercontra12; mastercontra12o

qt: Einfachauswahlmatrix

hl:

in:

q: Im Laufe dieser Befragung haben Sie angegeben, dass Sie eher kein
Masterstudium planen. Aus welchen Gründen möchten Sie kein Masterstudium
aufnehmen?

is:

it1: (mastercontra1): weil die Studiendauer zu lang wird

it2: (mastercontra2): weil ich es mir finanziell nicht leisten kann

it3: (mastercontra3): weil ich dann überqualifiziert bin

it4: (mastercontra4): weil der Master zu theoretisch ist und zu wenig
Anwendungsbezug hat

it5: (mastercontra5): weil ich das Bedürfnis habe, außerhalb der Hochschule zu
arbeiten

it6: (mastercontra6): weil der Master für den Berufseinstieg nötig ist

it7: (mastercontra7): weil ich schnellstmöglich finanziell unabhängig sein will

it8: (mastercontra8): weil mir das Anforderungsniveau des Masterstudiums zu hoch
ist

it9: (mastercontra9): weil ich kein Interesse an einer wissenschaftlichen
Tätigkeit habe

it10: (mastercontra10): weil der Master eine zu große Spezialisierung bedeutet

it11: (mastercontra11): weil die Chance auf mein Wunschstudium zu gering ist

it12: (mastercontra12): anderes, und zwar: [mastercontra12o]

st:

ao1: 1: trifft überhaupt nicht zu

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: trifft voll und ganz zu

mv:

ka:

vc: 

av:

kh:

fv:

hv:

fo:

tr: GOTO KSM-ma09

hi: Wo und mit welcher Variable „Masterintention“ erhoben wird, ist mir nicht
klar Variablenbezug zur Einblendbedingung fehlt noch --> Antwort:  IF mastplan = 4 OR mastplan = 5, wird beim Seitenübergang von KSM-ma06 nach KSM-07/08 definiert.

\--------------------------------

KSM-ma09
========

tc:

vn: bawert1; bawert2; bawert3

qt: Einfachauswahlmatrix

hl:

in:

q: Wie stehen Sie zu den folgenden Aussagen bezüglich des Bachelorabschlusses?
Ein Bachelorabschluss ist…

is:

it1: (bawert1): …kein vollwertiger Hochschulabschluss, vielmehr vergleichbar mit
der beruflichen Ausbildung

it2: (bawert2): …wird von Arbeitgebern kaum angesehen

it3: (bawert3): …nur ein Zwischenschritt zu einem Masterstudium

st:

ao1: 1: stimme überhaupt nicht zu

ao2: 2:

ao3: 3:

ao4: 4:

ao5: 5: stimme voll und ganz zu

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
