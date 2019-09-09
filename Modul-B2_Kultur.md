\--------------------------

1
=

tc:

vn: hschabv; hschabm

qt: Einfachauswahl im Spaltenformat/Comparison

hl:

in:

q: Welches ist der höchste allgemeinbildende Schulabschluss Ihres Vaters/Ihrer
Mutter?

is:

it1: (hschabv) Vater

it2: (hschabm) Mutter

st:

ao1: 1: keinen Schulabschluss

ao2: 2: anderer Schulabschluss

ao3: 3: Haupt-, Volksschulabschluss (mind. 8. Klasse)

ao4: 4: mittlere Reife, Realschulabschluss (10. Klasse)

ao5: 5: Fachhochschulreife

ao6: 6: allgemeine/fachgebundene Hochschulreife (Abitur)

mv: -12: weiß ich nicht

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

>   GOTO 2a if h_split2==1

>   GOTO 2b if h_split2==2

hi: Hilfsvariable muss an vorheriger Stelle generiert werden

h_split2 = 50/50-Split; values (1;2) zufällig aufgeteilt, 1=2a; 2=2b

\--------------------------

2a
==

tc: 50 Prozent der Befragten

vn: deltposv1; deltposm1

qt: Einfachauswahl im Spaltenformat/Comparison

hl:

in:

q: Welche berufliche Stellung hat Ihr Vater/Ihre Mutter?

is: Falls Ihr Vater oder Ihre Mutter zurzeit nicht erwerbstätig sind (z. B.
Rentner(in), Pensionär(in), Hausfrau/-mann oder arbeitssuchend), beziehen Sie
sich bitte auf die jeweils zuletzt ausgeübte Tätigkeit.

it1: (deltposv1): Vater

It2 (deltposm1): Mutter

ao1: 1: ungelernt

ao2: 2: angelernt

ao3: 3: Facharbeiter(in)

ao4: 4: Vorarbeiter(in), Kolonnenführer(in)

ao5: 5: Meister(in), Polier(in), Brigadier(in)

ao6: 6: mit ausführender Tätigkeit z. B. Verkäufer(in), Datentypist(in),
Sekretariatsassistent(in), Pflegehelfer(in)

ao7: 7: mit qualifizierter Tätigkeit z. B. Sachbearbeiter(in), Buchhalter(in),
technische(r) Zeichner(in)

ao8: 8: mit Fachverantwortung für Personal z. B. wissenschaftliche(r)
Mitarbeiter(in), Prokurist(in), Abteilungsleiter(in) bzw. Meister(in) im
Angestelltenverhältnis

ao9: 9: mit umfassenden Führungsaufgaben und Entscheidungsbefugnissen z. B.
Direktor(in), Geschäftsführer(in), Mitglied des Vorstandes

ao10: 10: im einfachen Dienst z. B. Amtsgehilfe/-gehilfin, Schaffner(in),
Betriebsassistent(in), ab (Ober)Gefreiter

ao11: 11: im mittleren Dienst z. B. Polizei(haupt)meister(in), Sekretär(in),
Gerichtsvollzieher(in), ab Unteroffizier(in)

ao12: 12: im gehobenen Dienst z. B. Inspektor(in), Lehrer(in), Amtsrat/-rätin,
Kriminalkommissar(in), ab Leutnant(in)

ao13: 13: im höheren Dienst z. B. Regierungsrat/-rätin, Studienrat/-rätin,
Hochschullehrer(in), Rektor(in), Richter(in), ab Major(in)

ao14: 14: keine weiteren Mitarbeiter(innen)

ao15: 15: 1 bis 4 Mitarbeiter(innen)

ao16: 16: 5 und mehr Mitarbeiter(innen)

ao17: 17: keine weiteren Mitarbeiter(innen)

ao18: 18: 1 bis 4 Mitarbeiter(innen)

ao19: 19: 5 und mehr Mitarbeiter(innen)

ao20: 20: PGH-Mitglied

ao21: 21: mit einer landwirtschaftlich genutzten Fläche bis unter 10 ha

ao22: 22: mit einer landwirtschaftlich genutzten Fläche von 10 ha und mehr

ao23: 23: Genossenschaftsbauer/-bäuerin (ehemals LPG)

ao24: 24: !!Mithelfende(r) Familienangehörige(r)!!

ao25: -11: !!nie berufstätig gewesen!!

mv: -12: !!weiß ich nicht!!

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO 3b

hi: Zwischenüberschriften zwischen den ao’s möglich?

>   st1: !!Arbeiter(in), und zwar...!! (ao1, ao2, ao3, ao4, ao5)

>   st2: !!Angestellte(r), und zwar...!! (ao6, ao7, ao8, ao9)

>   st3: !!Beamter/Beamtin, Richter(in), Berufssoldat(in), und zwar...!! (ao10,
>   ao11, ao12, ao13)

>   st4: !!Akademiker(in) in freiem Beruf (z. B. Rechtsanwalt/-anwältin,
>   niedergelassene/r Arzt/Ärztin, Steuerberater(in), Künstler(in)!! (ao14,
>   ao15, ao16)

>   st5: !!Selbstständige im Handel, im Gastgewerbe, im Handwerk, in der
>   Industrie, der Dienstleistung, auch Ich-AG oder PGH-Mitglied und
>   hat/hatte...!! (ao17, ao18, ao19, ao20)

>   st6: !!Selbstständige(r) Landwirt(in) bzw. Genossenschaftsbauer/-bäuerin!!
>   (ao21, ao22, ao23)

\--------------------------

2b
==

tc: 50 Prozent der Befragten

vn: deltposv2; deltposm2

qt: Einfachauswahl im Spaltenformat/Comparison

hl:

in:

q: Welche berufliche Stellung hat Ihr Vater/Ihre Mutter?

is: Falls Ihr Vater oder Ihre Mutter zurzeit nicht erwerbstätig sind (z. B.
Rentner(in), Pensionär(in), Hausfrau/-mann oder arbeitssuchend), beziehen Sie
sich bitte auf die jeweils zuletzt ausgeübte Tätigkeit.

it1: (deltposv2): Vater

It2 (deltposm2): Mutter

st1: !!Arbeiter!! (ao1, ao2, ao3, ao4)

st2: !!Angestellte!! (ao5, ao6, ao7, ao8)

st3: !!Beamte!! (ao9, ao10, ao11, ao12)

st4: !!Selbstständige!1 (ao13, ao14, ao15)

st5: !!Akademiker(in) in freiem Beruf!! (ao16, ao17, ao18)

st6: !!Selbstständige(r) Landwirt(in) bzw. Genossenschaftsbauer/-bäuerin!!
(ao21, ao22, ao23)

ao1: 1: ungelernt/angelernt

ao2: 2: Facharbeiter(in)

ao3: 3: Vorarbeiter(in), Kolonnenführer(in)

ao4: 4: Meister(in), Polier(in), Brigadier(in)

ao5: 5: mit ausführender Tätigkeit z. B. Verkäufer(in),
Sekretariatsassistent(in), Pflegehelfer(in)

ao6: 6: mit qualifizierter Tätigkeit z. B. Sachbearbeiter(in), Buchhalter(in),
technische(r) Zeichner(in)

ao7: 7: mit gehobener Position z. B. wiss. Mitarbeiter(in), Prokurist(in),
Abteilungsleiter(in) bzw. Meister(in) im Angestelltenverhältnis

ao8: 8: mit umfassenden Führungsaufgaben und Entscheidungsbefugnissen z. B.
Direktor(in), Geschäftsführer(in), Mitglied des Vorstandes

ao9: 9: im einfachen Dienst z. B. Amtsgehilfe/-gehilfin, Schaffner(in),
Betriebsassistent(in)

ao10: 10: im mittleren Dienst z. B. Polizei(haupt)meister(in), Sekretär(in),
Gerichtsvollzieher(in)

ao11: 11: im gehobenen Dienst z. B. Inspektor(in), Lehrer(in), Amtsrat/-rätin,
Kriminalkommisar(in)

ao12: 12: im höheren Dienst z. B. Regierungsrat/-rätin, Studienrat/-rätin,
Rektor(in), Richter(in)

ao13: 13: kleinere Selbstständige z. B. Einzelhändler(in) mit kleinem Geschäft,
Hauptvertreter(in), mittlere Landwirtschaft

ao14: 14: mittlere Selbstständige z. B. Einzelhändler(in) mit großem Geschäft,
Handwerker(in, größere Landwirtschaft

ao15: 15: größere Selbstständige z. B. Unternehmer(in) mit großem Betrieb

ao16: 16: keine weiteren Mitarbeiter(innen)

ao17: 17: 1 bis 4 Mitarbeiter(innen)

ao18: 18: 5 und mehr Mitarbeiter(innen)

ao19: 19: !!Mithelfende(r) Familienangehörige(r)!!

ao20: -11: !!nie berufstätig gewesen!!

mv: -12: !!weiß ich nicht!!

ka:

vc:

av:

kh:

fv:

hv:

fo: siehe mitgeliefertes Template

tr: GOTO 3a

\--------------------------

3a
==

tc: 50 Prozent der Befragten

vn: buchanzi1, buchanze1

qt: Einfachauswahl im Spaltenformat/Comparison

hl:

in:

q: Was schätzen Sie, wie viele Bücher besitzen Sie heute und wie viele Bücher
besaßen Ihre Eltern zu Ihrer Kindheit?

is: Als Hilfestellung: Auf einen Meter Regalbrett passen ungefähr 40 Bücher.
Zählen Sie bitte keine E-Books, Zeitungen und Zeitschriften mit.

is: Anzahl Bücher

it1: (buchanzi1): Sie

it2: (buchanze1): Elternhaus

ao1: 1: 0 bis 10

ao2: 2: 11 bis 25

ao3: 3: 26 bis 50

ao4: 4: 51 bis 100

ao5: 5: 101 bis 150

ao6: 6: 151 bis 200

ao7: 7: 201 bis 249

ao8: 8: 250 bis 300

ao9: 9: 300 bis 400

ao10: 10: 400 bis 500

ao11: 11: mehr als 500

mv: -12: : weiß ich nicht

ka:

vc:

av:

kh:

fv:

hv:

fo: ao12 absetzen

tr: GOTO 4

hi:

\--------------------------

3b
==

tc: 50 Prozent der Befragten

vn: buchanzi2; buchanze2

qt: Einfachauswahl im Spaltenformat/Comparison

hl:

in:

q: Wie viele Bücher besitzen Sie bzw. Ihre Eltern?

is: Als Hilfestellung: Auf einen Meter Regalbrett passen ungefähr 40 Bücher.
Zählen Sie bitte keine E-Books, Zeitungen und Zeitschriften mit.

is: Anzahl Bücher

it1: (buchanzi2): Sie

it2: (buchanze2): Eltern

ao1: 1: 0 bis 10

ao2: 2: 11 bis 25

ao3: 3: 26 bis 50

ao4: 4: 51 bis 100

ao5: 5: 101 bis 150

ao6: 6: 151 bis 200

ao7: 7: 201 bis 249

ao8: 8: 250 bis 300

ao9: 9: 300 bis 400

ao10: 10: 400 bis 500

ao11: 11: mehr als 500

mv: -12: weiß ich nicht

ka:

vc:

av:

kh:

fv:

hv:

fo: ao12 absetzen

tr: GOTO 4

hi:

\--------------------------

4
=

tc:

vn: diskpol / disklit / diskkun / diskmus / diskspo / disktv / diskwiss

qt: Einfachauswahlmatrix

hl:

in:

q: Wie oft diskutieren Sie mit anderen in Ihrer Freizeit über folgende Aspekte?

is:

it1: (diskpol) politische oder soziale Fragen

it2: (disklit) Literatur

it3: (diskkun) Kunst

it4: (diskmus) Musik  
it5: (diskspo) Sport

it6: (disktv) Fernsehserien/TV

it7: (diskwiss) wissenschaftliche Themen und Fragestellungen

st:

ao1: 1: 1: täglich

ao2: 2: 2: mehrmals in der Woche

ao3: 3: 3: einmal in der Woche

ao4: 4: 4: mehrmals im Monat

ao5: 5: 5: nie oder selten

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: Items bitte zufällig rotieren.

tr: GOTO 5

hi:

\--------------------------

5
=

tc:

vn: freimus / freikunst / freikult / freiaba / freifreu / freikonz / freinet /
freispor / freiehr / freipc

qt: Einfachauswahlmatrix

hl:

in:

q: Wie häufig gehen Sie in Ihrer Freizeit folgenden Tätigkeiten nach?

is:

it1: (freimus) musizieren

it2: (freikunst) künstlerisch betätigen

it3: (freikult) kulturelle Veranstaltungen besuchen

it4: (freiaba) Abends Ausgehen

it5: (freifreu) mit Freunden treffen

it6: (freikonz) auf Konzerte gehen

it7: (freinet) soziale Netzwerke nutzen

it8: (freispor) sportlich betätigen

it9: (freiehr) ehrenamtlich engagieren

it10: (freipc) Computer spielen

st:

ao1: 1: 1: nie

ao2: 2: 2: selten

ao3: 3: 3: manchmal

ao4: 4: 4: häufig

ao5: 5: 5: sehr häufig

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: Items bitte zufällig rotieren.

tr: GOTO 6

hi:

\--------------------------

6
=

tc:

vn: bezgew / bezmein / bezprob / bezsit / beztip / bezunth / bezfrag / bezfunt /
bezmis / bezwohl / bezuntp / bezint / bezplan

qt: Einfachauswahlmatrix

hl:

in:

q: Wenn Sie an die Beziehung zu Ihren Eltern denken, inwiefern treffen die
folgenden Aussagen zu?

is:

it1: (bezgew) Ich habe meinen Eltern gegenüber manchmal ein schlechtes Gewissen,
weil ich studiere.

it2: (bezmein) Die Meinung meiner Eltern ist mir sehr wichtig.  
it3: (bezprob) Wenn ich Probleme im Studium habe, dann spreche ich mit meinen
Eltern darüber.

it4: (bezsit) Meine Eltern können meine Lebenssituation gut nachvollziehen

it5: (beztip) Meine Eltern geben mir Tipps, wenn es um mein Studium geht.

it6: (bezunth) Ich fahre oft nach Hause, um meine Eltern zu unterstützen.

it7: (bezfrag) Meine Eltern fragen regelmäßig nach, wie es im Studium läuft.

it8: (bezfunt) Nach meinem Studium möchte ich meine Eltern finanziell
unterstützen.

it9: (bezmis) Ich fühle mich von meinen Eltern oft unverstanden.

it10: (bezwohl) Bei meinen Eltern fühle ich mich richtig wohl.

it11: (bezuntp) In Prüfungsphasen kann ich mich auf die Unterstützung meiner
Eltern verlassen.

it12: (bezint) Meine Eltern interessieren sich für das, was ich studiere.

it13: (bezplan) Meine Eltern fänden es besser, wenn ich arbeite anstatt zu
studieren.

st:

ao1: 1: 1: trifft gar nicht zu

ao2: 2: 2

ao3: 3: 3

ao4: 4: 4

ao5: 5: 5: trifft voll und ganz zu

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: Items bitte zufällig rotieren.

tr: GOTO 7

hi:

\--------------------------

7
=

tc:

vn: skkarr / skeuro / skwiss / skjobs / skantr / skausl

qt: Einfachauswahlmatrix

hl:

in:

q: Wie wahrscheinlich ist es, dass jemand aus Ihrem persönlichen Umfeld…

is:

it1: (skkarr) … Ihnen hilfreiche Ratschläge für den weiteren Berufs- und
Karriereweg gibt?

it2: (skeuro) … Ihnen spontan 1000 € leiht?

it3: (skwiss) … Ihre wissenschaftlichen Arbeiten gegenliest?

it4: (skjobs) … Ihnen einen Job oder ein Praktikum vermittelt?

it5: (skantr) … Ihnen beim Ausfüllen von amtlichen Anträgen (z.B. Bafög,
Steuererklärung) hilft?

it6: (skausl) … Ihnen nahelegt im Ausland zu studieren?

st:

ao1: 1: 1: sehr unwahrscheinlich

ao2: 2: 2

ao3: 3: 3

ao4: 4: 4

ao5: 5: 5: sehr wahrscheinlich

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: Items bitte zufällig rotieren.

tr:

>   GOTO 8a IF sabsan = 1 \| sabsan = 2

>   ELSE GOTO 8b

hi:

\--------------------------

8a
==

tc: sabsan = 1 \| sabsan = 2

vn: bilaspab / bilaspma / bilaspdr / bilaspber

qt: Einfachauswahlmatrix

hl:

in:

q: Was denken Sie: Wie wichtig ist es Ihren Eltern, dass Sie…

is:

it1: (bilaspab) … einen Hochschulabschluss erreichen?

it2: (bilaspma) … einen Masterabschluss erreichen?

it3: (bilaspdr) … einen Doktortitel erreichen?

it4: (bilaspber) … beruflich ganz weit nach vorne kommen?

st:

ao1: 1: 1: sehr unwichtig

ao2: 2: 2

ao3: 3: 3

ao4: 4: 4

ao5: 5: 5: sehr wichtig

mv: -12: weiß ich nicht

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

>   GOTO 9a if h_split2==1

>   GOTO 9b if h_split2==2

hi:

\--------------------------

8b
==

tc: IF sabsan \<\> 1 OR sabsan \<\> 2

vn: bilas (bilaspab / bilaspdr / bilaspber)

qt: Einfachauswahlmatrix

hl:

in:

q: Was denken Sie: Wie wichtig ist es Ihren Eltern, dass Sie…

is:

it1: (bilaspab) … einen Hochschulabschluss erreichen?

It2: (bilaspdr) … einen Doktortitel erreichen?

It3: (bilaspber) … beruflich ganz weit nach vorne kommen?

st:

ao1: 1: 1: sehr unwichtig

ao2: 2: 2

ao3: 3: 3

ao4: 4: 4

ao5: 5: 5: sehr wichtig

mv: -12: weiß ich nicht

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

>   GOTO 9a if h_split2==1

>   GOTO 9b if h_split2==2

hi:

\--------------------------

9a
==

tc: 50 Prozent der Befragten

vn: einkein1; einkerf1

qt: Einfachauswahl im Spaltenformat/Comparison

hl:

in:

q: Was denken Sie: Welches Monatseinkommen werden Sie nach dem Studium bekommen?

is: Beziehen Sie Ihre Angaben auf das Netto-Gehalt, d.h. Einkommen abzüglich
Steuer.

it1: (einkein1) Berufseinstieg

it2: (einkerf1) 10 Jahre im Beruf

st:

ao1: 1: unter 1.000 €

ao2: 2: 1.000 € bis unter 1.500 €

ao3: 3: 1.500 € bis unter 2.000 €

ao4: 4: 2.000 € bis unter 2.500 €

ao5: 5: 2.500 € bis unter 3.000 €

ao6: 6: 3.000 € bis unter 4.000 €

ao7: 7: 4.000 € bis unter 5.000 €

ao8: 8: 5.000 € bis unter 10.000 €

ao9: 9: 10.000 € und mehr

mv: -12: : weiß ich nicht

ka:

vc:

av:

kh:

fv:

hv:

fo: ao10 absetzen

tr: GOTO 10

hi:

\--------------------------

9b
==

tc: 50 Prozent der Befragten

vn: einkein2, einkerf2

qt: Offene Angabe

hl:

in:

q: Was denken Sie: Welches Monatseinkommen werden Sie nach dem Studium bekommen?

is: Beziehen Sie Ihre Angaben auf das Netto-Gehalt, d.h. Einkommen abzüglich
Steuer.

it:

st: Netto-Monatseinkommen bei…

ao1 (einkein2): 5, Präfix: … Berufseinstieg: , Suffix: €/Monat

ao2 (einkerf2): 5, Präfix: … 10 Jahre im Beruf: , Suffix: €/Monat

mv: -12: weiß ich nicht

ka:

vc:

av:

kh:

fv:

hv:

fo: ao3 absetzen

tr: GOTO 10

hi:

\--------------------------

10
==

tc:

vn: promno / promges / promelt / promgroß / promver

qt: Mehrfachauswahl mit vertikalen ao

hl:

in:

q: Hat in Ihrer Familie bereits jemand eine Promotion begonnen oder erfolgreich
abgeschlossen?

is:

it:

st:

ao1 (promno): nein

ao2 (promges): ja, Geschwister

ao3 (promelt): ja, Eltern

ao4 (promgroß): ja, Großeltern

ao5 (promver): ja, andere Verwandte

mv: -12: weiß ich nicht

ka:

vc:

av:

kh:

fv:

hv:

fo: ao6 absetzen

tr:

hi: [ao1 (promno): nein] soll exklusiv sein
