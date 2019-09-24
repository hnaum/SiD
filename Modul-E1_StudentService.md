\--------------------------------

E1_1
====

tc:

vn: moftfrue; moftvorm; moftmitt; moftnach; moftaben

qt: Einfachauswahlmatrix

hl:

in:

q: Wie häufig gehen Sie im Laufe einer für Sie typischen Woche zum Essen in eine
Mensa oder Cafeteria Ihrer Hochschule?

is:

it1: (moftfrue): zum Frühstück

it2: (moftvorm): zu einer Zwischenmahlzeit am Vormittag

it3: (moftmitt): zum MIttagessen

it4: (moftnach): zu einer Zwischenmahlzeit am Nachmittag

it5: (moftaben): zum Abendessen

st:

ao1: 0: 0-mal

ao2: 1: 1-mal

ao3: 2: 2-mal

ao4: 3: 3-mal

ao5: 4: 4-mal

ao6: 5: 5-mal

ao7: 6: 6-mal

ao8: 7: 7-mal

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO E1_2

hi:

\--------------------------------

E1_2
====

tc:

vn: mzufges; mzufqual; mzufausw; mzufatmo; mzufprl; mzufpraes; mzufatmo;
mzuflage; mzufwart; mzufserv; mzufverl; mzuföff; mzufkomm

qt: Einfachauswahlmatrix

hl:

in:

q: Wie zufrieden sind Sie mit Ihrer Mensa/Cafeteria hinsichtlich der folgenden
Aspekte?

is:

it1: (mzufges): Geschmack

it2: (mzufqual): Ernährungsqualität und Gesundheitswert

it3: (mzufausw): Auswahl- und Kombinationsmöglichkeiten

it4: (mzufatmo): Atmosphäre und Raumgestaltung

it5: (mzufprl): Preis-Leistungs-Verhältnis

it6: (mzufpraes): Präsentation und Darbietung des Essensangebots

it1: (mzufatmo): Atmosphäre und Raumgestaltung

it1: (mzuflage): Lage und Erreichbarkeit

it1: (mzufwart): Wartezeiten

it1: (mzufserv): Service

it1: (mzufverl): Zeitliche Vereinbarkeit mit Lehr-/Veranstaltungsplan

it1: (mzuföff): Öffnungszeiten

it1: (mzufkomm): Ort der Kommunikation

st:

ao1: 1: überhaupt nicht zufrieden

ao2: 2

ao3: 3

ao4: 4

ao5: 5: sehr zufrieden

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO E1_3

hi:

\--------------------------------

E1_3
====

tc:

vn: indergenu; indervega; inderprei; inderprob; inderoeko; inderschn; inderfair;
indersatt; indervege; inderunwe; inderregi; inderzuha; inderzuck; inderkoch;
inderfris; indergese; inderwich, inderkalo, inderplan

qt: Einfachauswahlmatrix

hl:

in:

q: Nun geht es um Ihr allgemeines Ernährungsverhalten: Inwieweit treffen die
folgenden Aussagen auf Ihre persönliche Ernährung zu?

is:

it1: (indergenu): Essen hat für mich vor allem mit Genuss zu tun.

it2: (indersatt): Essen muss vor allem satt machen.

it3: (inderprei): Mein Essen muss preiswert sein.

it4: (inderwich): Meine Ernährung ist mir nicht so wichtig.

it5: (indervege): Ich ernähre mich vegetarisch.

It6: (indervega): Ich ernähre mich vegan.

It7: (inderoeko): Ich achte bei Lebensmitteln darauf, dass sie
EU-Öko/Bio-zertifiziert sind.

It8: (inderfair): Ich achte darauf, dass Lebensmittel fair gehandelt sind.

It9: (inderregi): Ich konsumiere vor allem regionale Lebensmittel.

It10: (inderzuck): Ich versuche den Konsum von Zucker zu vermeiden.

it11: (inderkalo): Beim Essen achte ich darauf, wie viele Kalorien ich zu mir
nehme.

it12: (inderplan): Ich orientiere mich an einem Ernährungsplan.

it13: (inderzuha): Ich ernähre mich so, wie ich es von zuhause gewöhnt bin.

it14: (inderprob): Ich probiere gerne Speisen aus anderen Kulturkreisen aus.

it15: (inderschn): Mein Essen muss schnell zubereitet sein.

it16: (inderunwe): Ich esse häufig unterwegs, z. B. zwischen
Lehrveranstaltungen.

it17: (inderkoch): Meistens koche ich mein Essen selbst.

it18: (indergese): Ich esse am liebsten in geselliger Runde.

it19: (inderfris): Ich koche vor allem mit frischen Lebensmitteln.

st:

ao1:1: trifft gar nicht zu

ao2: 2

ao3: 3

ao4: 4

ao5: 5: trifft voll und ganz zu

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO E1_4

hi:

\--------------------------------

E1_4
====

tc:

vn: sver (sverkin; sverbeein; svererwerb; svercare)

qt: Einfachauswahlmatrix

hl:

in:

q: Ein Studium erfordert oftmals etwas Zeit: Inwieweit ist ein Studium aus Ihrer
Perspektive überhaupt vereinbar mit folgenden Aspekten?

is:

it1: (sverkin): Studium mit Kind

it1: (sverbeein): Studium mit Beeinträchtigung

it1: (svererwerb): Studium und Erwerbstätigkeit

it1: (svercare): Studium und die Pflege von Angehörigen

st:

ao1: 1: überhaupt nicht vereinbar

ao2: 2

ao3: 3

ao4: 4

ao5: 5: sehr gut vereinbar

ao6: 6: weiß ich nicht

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: IF (Kind = ja OR IF Beeinträchtigung = ja OR IF Erwerbstätigkeit = ja OR
Pflege von Angehörigen = ja) GOTO E1_5

ELSE GOTO E1_6

hi:

\--------------------------------

E1_5
====

tc: Frage geht an Studierende mit Kind, mit Beeinträchtigung, erwerbstätige
Studierende, Studierende mit Pflegetätigkeit

vn: szufver (szufverkin; szufverbeein; szufvererwerb; szufvercare)

qt: Einfachauswahlmatrix

hl:

in:

q: Und wie zufrieden sind Sie mit der Vereinbarkeit von Studium und…

is:

it1: (szufverkin): … Kinderbetreuung?

It2: (szufverbeein): … Beeinträchtigung?

It3: (szufvererwerb): … Erwerbstätigkeit?

It4: (szufvercare): … Pflege von Angehörigen?

st:

ao1: 1: gar nicht zufrieden

ao2: 2

ao3: 3

ao4: 4

ao5: 5: sehr zufrieden

mv:

ka:

vc: SHOW it1 IF Kind = ja

SHOW it2 IF Beeinträchtigung = ja

SHOW it3 IF Erwerbstätigkeit = ja

SHOW it4 IF Pflege von Angehörigen = ja

av:

kh:

fv:

hv:

fo:

tr: GOTO E1_6

hi:

\--------------------------------

E1_6
====

tc: Hier fehlt Filter für it16 bis it22 – nur für Studierende mit
Beeinträchtigung!

vn: ibedsfin; ibedkv; ibedafin; ibedpart; ibedfamu; ibeddep; ibedaldr; ibedvbew;
ibedvbki; ibedvbhc; ibedllpran; ibedaoz; ibedabersw; ibedaorg; ibedabs; ibebsln;
ibebssu; ibebsth; ibebspa; ibebsbh; ibebsat; ibebsrb; ibedno

qt: Einfachauswahlmatrix

hl:

in:

q: Wir möchten nun gerne noch etwas mehr über Ihre Situation erfahren:

Inwieweit hatten Sie in den letzten zwölf Monaten Fragen bis hin zu
Schwierigkeiten hinsichtlich folgender Themen?

is:

it1: (ibedsfin): Finanzierung des Studiums

it2: (ibedkv): Krankenversicherung

it3: (ibedafin): Finanzierung eines studienbezogenen Auslandsaufenthalts

it4: (ibedpart): Partnerschaftsprobleme

it5: (ibedfamu): Probleme im familiären Umfeld

it6: (ibeddep): depressive Verstimmungen

it7: (ibedaldr): Probleme mit Alkohol oder anderen Drogen

it8: (ibedvbew): Vereinbarkeit von Studium und Erwerbstätigkeit

it9: (ibedvbki): Vereinbarkeit von Studium und Kind(ern)

it10: (ibedvbhc): Vereinbarkeit von Studium und Behinderung/chronischer
Krankheit

it11: (ibedllpran): Lern-/Leistungsprobleme, Prüfungsangst

it12: (ibedaoz): Arbeitsorganisation, Zeitmanagement

it13: (ibedabersw): Studienorganisation, Studienganggestaltung/-wechsel

it14: (ibedaorg): Organisation eines studienbezogenen Auslandsaufenthalts

it15: (ibedabs): Studienabschlussprobleme

it16: (ibebsln): Nachteilsausgleiche bei Leistungsnachweisen

it17: (ibebssu): Umgang mit längeren beeinträchtigungsbedingten
Studienunterbrechungen

it18: (ibebsth): Organisation und Nutzung von technischen Hilfsmitteln

it19: (ibebspa): Organisation und Nutzung von personellen Assistenzen

it20: (ibebsbh): Umgang mit baulichen Hürden, Raumverlegungen und Umbauten

it21: (ibebsat): Aneignung bedarfsgerechter Arbeitstechniken

it22: (ibebsrb): Durchsetzung von Ansprüchen, Rechtsberatung

it23: (ibedno): Ich hatte zu keinem der genannten Themenbereiche Fragen bis hin
zu Schwierigkeiten oder Belastungen. (Exklusivkategorie)

st:

ao1: 1: gar nicht

ao2: 2

ao3: 3

ao4: 4

ao5: 5: in hohem Maße

ao6: 0: nicht ausgewählt (nur ibedno)

ao7: 1: ausgewählt (nur ibedno)

mv:

ka1: (it1, it2, it3): Finanzierungsbezogene Themen

ka2: (it4, it5, it6, it7): Persönliche Themen

ka3: (it8, it9, it10, it11, it12, it13, it14, it15): Studienbezogene Themen

ka4: (it16, it17, it18, it19, it20, it21, it22): Beeinträchtigungsbezogene
Themen

vc: Wenn **gartmob-gartka** auf [SDK-gub\#01] (Grundprogramm) mindestens einmal
=1 [Identifikation Studierende mit Beeinträchtigung]; dann **Einblendung**
zusätzlicher Items Themenbereich **Beeinträchtigungsbezogene Themen** ibebsln;
ibebssu; ibebsth; ibebspa; ibebsbh; ibebsat; ibebsrb

av:

kh:

fv:

hv:

fo:

tr:

IF ((ibedsfin \| … \| ibedabs bzw. ibebsrb \> 1) & ibedno =0) GOTO E1_7

ELSE E1_9

hi: Skalierung bitte bei der Teilüberschrift „Studienbezogene Themen“ nochmals
einblenden; Items des letzten Themenbereichs (Beeinträchtigungsbezogene Themen)
bitte nur für Studierende mit Beeinträchtigung einblenden (siehe unten).;

Bitte die Teilüberschriften nach oben optisch absetzen

\--------------------------------

E1_7
====

tc1: IF (ibedsfi \| ... \| ibedabs) \> 1

tc2: IF ibedno = 0

vn: iinasfin; iinakv; iinaafin; iinapart; iinafamu; iinadep; iinaaldr; iinavbew;
iianvbki; iinavbhs; iinallpran; iinaaoz; iinaabersw; iinaaorg; iinaabs;
iinabsln; iinabssu; iinabsth; iinabspa; iinabsbh, iinabsat, iinabsrb; iinano

qt: Einfachauswahlmatrix

hl:

in:

q: Haben Sie zu den zuvor genannten Themen/Problembereichen in den letzten zwölf
Monaten Beratung in Anspruch genommen?

is:

it1: (iinasfin): Finanzierung des Studiums

it2: (iinakv): Krankenversicherung

it3: (iinaafin): Finanzierung eines studienbezogenen Auslandsaufenthalts

it4: (iinapart): Partnerschaftsprobleme

it5: (iinafamu): Probleme im familiären Umfeld

it6: (iinadep): depressive Verstimmungen

it7: (iinaaldr): Probleme mit Alkohol oder anderen Drogen

it8: (iinavbew): Vereinbarkeit von Studium und Erwerbstätigkeit

it9: (iinavbki): Vereinbarkeit von Studium und Kind(ern)

it10: (iinavbhc): Vereinbarkeit von Studium und Behinderung/chronischer
Krankheit

it11: (iinallpran): Lern-/Leistungsprobleme, Prüfungsangst

it12: (iinaaoz): Arbeitsorganisation, Zeitmanagement

it13: (iinaabersw): Studienorganisation, Studienganggestaltung/-wechsel

it14: (iinaaorg): Organisation eines studienbezogenen Auslandsaufenthalts

it15: (iinaabs): Studienabschlussprobleme

it16: (innabsln): Nachteilsausgleiche bei Leistungsnachweisen

it17: (iinabssu): Umgang mit längeren beeinträchtigungsbedingten
Studienunterbrechungen

it18: (iinabsth): Organisation und Nutzung von technischen Hilfsmitteln

it19: (iinabspa): Organisation und Nutzung von personellen Assistenten

it20: (iinabsbh): Umgang mit baulichen Hürden, Raumverlegungen und Umbauten

it21: (iinabsat): Aneignung bedarfsberechter Arbeitstechniken

it22: (iinabsrb): Durchsetzung von Ansprüchen, Rechtsberatung

Leerzeile

it23: (iinano): Ich habe zu keinem der genannten Themenbereiche in den letzten
12 Monaten Beratung in Anspruch genommen (Exklusivkategorie)

st:

ao1: 1: nein

ao2: 2: ja, innerhalb des Hochschulbereichs

ao3: 3: ja, außerhalb des Hochschulbereichs

ao4: 4: ja, innerhalb und außerhalb des Hochschulbereichs

ao6: 0: nicht ausgewählt (nur ibedno)

ao6: 1: ausgewählt (nur ibedno)

mv:

ka1: (it1, it2, it3): Finanzierungsbezogene Themen

ka2: (it4, it5, it6, it7): Persönliche Themen

ka3: (it8, it9, it10, it11, it12, it13, it14, it15): Studienbezogene Themen

ka4: (it16, it17, it18, it19, it20, it21, it22): Beeinträchtigungsbezogene
Themen

vc: SHOW it1 IF ibedsfin \> 1

SHOW it2 IF ibedkv \> 1

SHOW it3 IF ibedafin \> 1

SHOW it4 IF ibedpart \> 1

SHOW it5 IF ibedfamu \> 1

SHOW it6 IF ibeddep \> 1

SHOW it7 IF ibedaldr \> 1

SHOW it8 IF ibedvbew \> 1

SHOW it9 IF ibedvbki \> 1

SHOW it10 IF ibedvbhc \> 1

SHOW it11 IF ibedllpran \> 1

SHOW it12 IF ibedaoz \> 1

SHOW it13 IF ibedabersw \> 1

SHOW it14 IF ibedaorg \> 1

SHOW it15 IF ibedabs \> 1

SHOW it16 IF ibebsln \> 1

SHOW it17 IF ibebssu \> 1

SHOW it18 IF ibebsth \> 1

SHOW it19 IF ibebspa \> 1

SHOW it20 IF ibebsbh \> 1

SHOW it21 IF ibebsat \> 1

SHOW it22 IF ibebsrb \> 1

av:

kh:

fv:

hv:

fo:

tr: IF iinano=1 GOTO E1_8

ELSE GOTO E1_9

hi:

\--------------------------------

E1_8
====

tc: IF iinano = 1

vn: ihinzeit; ihingel; ihinkan; ihinpre; ihinfreu; ihinhil; ihinhem; ihinnac;
ihinand

qt: Mehrfachauswahl mit vertikalen ao (Mehrfachnennung)

hl:

in:

q: Warum haben Sie kein Beratungsangebot genutzt?

is: Bitte alles Zutreffende auswählen.

it1: (ihinzeit): ... weil ich keine Zeit dafür hatte/der Aufwand zu groß
erschien.

it2: (ihingel): ... weil sich das Problem von allein gelöst hat.

it3: (ihinkan): ... weil ich kein passendes Angebot gefunden habe.

it4: (ihinpre): ... weil ich mein Problem(meine Schwierigkeit nicht preisgeben
wollte.

it5: (ihinfreu): ... weil ich im privaten Umfeld Hilfe/Unterstützung gefunden
habe.

it6: (ihinhil): ...weil ich nicht wusste, wen ich um Beratung hätte bitten
können.

it7: (ihinhem): ...weil ich Hemmungen hatte, Hilfe in Anspruch zu nehmen.

it8: (ihinnac): ... weil ich dadurch Nachteile im weiteren Studium befürchtete.

it9: (ihinand): ... aus anderen Gründen

st: Ich habe kein Beratungsangebot in Anspruch genommen ...

ao:

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO E1_9

hi:

\--------------------------------

E1_9
====

tc:

vn: uekastei; uekastte; uekasfrsp; uekasosk; uekauefa; uekabeei; uekabekr

qt: Einfachauswahlmatrix

hl:

in:

q: Unabhängig von Ihren fachlichen Lehrveranstaltungen, welche zusätzlichen
Kurse werden an Ihrer Hochschule angeboten und welche haben Sie genutzt?

is:

it1: (uekastei): Kurse zum Studieneinstieg (z. B. “Brückenkurse zur Aufarbeitung
von Wissenslücken)

it2: (uekastte): Kurse zur Schulung von Studien- und Lerntechniken (z. B.
Schreibwerkstatt, Präsentationstraining)

it3: (uekafrsp): (Fremd-)Sprachenkurse

it4: (uekasosk): Kurse zur Schulung von “soft skills” (z. B. Rhetorik, soziale
Kompetenzen)

it5: (uekauefa): Kurse zum Erwerb überfachlicher Zusatzqualifikationen (z. B.
Projekt-, Wissensmanagement, spezielle EDV-Software)

it6: (uekabeei): Kurse zum Berufseinstieg (z. B. Bewerbungsstrategien,
Assessment Center-Training, Karrieremessen)

it7: (uekabekr): Kurse zum Umgang mit der eigenen Beeinträchtigung/chronischen
Krankheit

st:

ao1: 1: nicht angeboten

ao2: 2: angeboten, aber nicht genutzt

ao3: 3: angebogen und genutzt

ao4: -12: weiß nicht

mv:

ka:

vc: SHOW uekabekr IF gartmob-gartka = 1 (mindestens einmal angegeben)

av:

kh:

fv:

hv:

fo:

tr: IF uekastei \| […] \| uekabekr = 3 GOTO E1_10

ELSE GOTO E1_11

hi:

\--------------------------------

E1_10
=====

tc: IF uekastei \| ... \| uekabekr = 3 (mindestens ein Kursangebot genutzt)

vn: zuekastei; zuekastte; zuekafrsp; zuekasosk; zuekauefa; zuekabeei; zuekabekr

qt:

hl:

in:

q: Wie zufrieden sind/waren Sie mit den von Ihnen genutzten Kursangeboten?

is:

it1: (zuekastei): Kurse zum Studieneinstieg (z. B. “Brückenkurse zur
Aufarbeitung von Wissenslücken)

it2: (zuekastte): Kurse zur Schulung von Studien- und Lerntechniken (z. B.
Schreibwerkstatt, Präsentationstraining)

it3: (zuekafrsp): (Fremd-)Sprachenkurse

it4: (zuekasosk): Kurse zur Schulung von “soft skills” (z. B. Rhetorik, soziale
Kompetenzen)

it5: (zuekauefa): Kurse zum Erwerb überfachlicher Zusatzqualifikationen (z. B.
Projekt-, Wissensmanagement,

spezielle EDV-Software)

it6: (zuekabeei): Kurse zum Berufseinstieg (z. B. Bewerbungsstrategien,
Assessment Center-Training,

Karrieremessen)

it7: (zuekabekr): Kurse zum Umgang mit der eigenen Beeinträchtigung/chronischen
Krankheit

st:

ao1: 1: überhaupt nicht zufrieden

ao2: 2:

ao3: 3:

ao4: 4

ao5: 5: sehr zufrieden

mv:

ka:

vc1: SHOW zuekastei IF uekastei = 3

vc2: SHOW zuekastte IF uekastte = 3

vc3: SHOW zuekafrsp IF uekafrsp = 3

vc4: SHOW zuekasosk IF uekasosk = 3

vc5: SHOW zuekauefa IF uekauefa = 3

vc6: SHOW zuekabeei IF uekabeei = 3

vc7: SHOW zuekabekr IF uekabekr = 3

av:

kh:

fv:

hv:

fo:

tr: GOTO E1_11

hi:

\--------------------------------

E1_11
=====

tc:

vn: infoauvo; infofopr; infohosp; infostve; infopaho; infohole

qt:

hl:

in:

q: Wie gut informiert sind Sie über die folgenden Bereiche Ihrer Hochschule?

is:

it1: (infoauvo): außercussiculare Vortragsreihen (z. B. Studium generale)

it2: (Infofopr): Forschungsschwerpunkte Ihrer Professor\*innen

it3: (infohosp): Programm des Hochschulsports

it4: (infostve): politische Zusammensetzung der gegenwärtigen
Studierendenvertretung

it5: (infopaho): Partys auf dem Hochschulcampus

if6: (infohole): Aufgaben der Hochschulleitung

st:

ao1: 1: gar nicht informiert

ao2: 2

ao3: 3

ao4: 4

ao5: 5: sehr gut informiert

ao6: -66: interessiert mich nicht (Extrakategorie)

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO E1_12

hi:

\--------------------------------

E1_12
=====

tc:

vn: engemusi; engespor; engefasc; engemedi; engedeba; engestse; engestin;
engehogr; engestve; engesoho; engethta; engelege; engepoli

qt:

hl:

in:

q: Neben Lehrveranstaltungen gibt es weitere Möglichkeiten, sich in der
Hochschule zu engagieren. Wie stark engagieren Sie sich in den folgenden
Bereichen?

is:

it1: (engemusi): Chor/Orchester/Band der Hochschule

it2: (engespor): Hochschulsport

it3: (engefasc): Fachschaft

it4: (engemedi): Campusradio/Campus-TV/Printorgan der Hochschule

it5: (engedeba): Debattierklub

it6: (engestse): studentische Selbstverwaltung (z. B. AStA, AEGEE)

it7: (engestin): studentische Interessenvertretung (z. B. AISEC e. V.)

it8: (engehogr): als studentische\*r Vertreter\*in in einem Hochschulgremium

it9: (engestve): studentische Verbindung

it10: (engesoho): soziale Hochschulgruppe

it11: (engethta): studentische Theater-/Tanzgruppe

it12: (engelege): wissenschaftlicher Lesekreis/Gesprächskreis

it13: (engepoli): Hochschulgruppe einer politischen Partei

st:

ao1: 1: überhaupt nicht

ao2: 2

ao3: 3

ao4: 4

ao5: 5: sehr stark

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
