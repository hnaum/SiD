\--------------------------------

D3_1
====

tc:

vn: wohnort

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Wo wohnen Sie während der Vorlesungszeit des Sommersemesters 2020)

is:

it:

st: Ich wohne ...

ao1: 1: ... ausschließlich am Hochschulort.

ao2: 2: ... ausschließlich außerhalb des Hochschulortes.

ao3: 3: ... am Hochschulort und außerhalb des Hochschulortes.

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO 2 (D3_2)

hi:

\--------------------------------

D3_2
====

tc:

vn: wohnami, wohnamio

qt: Offene Frage

hl:

in:

q: Mit wie vielen Personen wohnen Sie insgesamt – also Sie selbst mit
eingeschlossen – zusammen?

is:

it:

st:

ao1: 2 Stellen, Präfix [wohnami]: Suffix: Anzahl [number] Person(en)

ao2: -12 (wohnamio)

mv:

ka:

vc:

av: number: 2 stellig : 1 TO 15

kh: Bitte geben Sie die Anzahl an Personen an, mit denen Sie zusammenwohnen.

fv:

hv:

fo:

tr: GOTO 3 (D3_3)

hi: Variable wohnamio bitte erst einblenden, wenn Wert bei wohnami nicht
definiert ist

\--------------------------------

D3_3
====

tc:

vn: wohnplz; wohnplzo; wohnplzort; wohnplzorto

qt: offene Angabe

hl:

in:

q: Bitte geben Sie die fünfstellige Postleitzahl Ihres derzeitigen Wohnortes am
Hochschulort an.

is:

it:

st:

ao1: 5 Stellen, Präfix [wohnplz] Suffix: Postleitzahl:[number]

ao2: 50 Stellen, Präfix [wohnplzort] Suffix: Falls Sie die Postleitzahl nicht
kennen, geben Sie bitten den Ort an: [50 Zeichen]

ao3: -12 (wohnplzo)

ao4: -12 (wohnplzorto)

mv:

ka:

vc:

av1: ao1 (wohnplz) number: 10000 : 1 TO 99999

av2: ao2 (wohnplzort) 50 Zeichen

kh1: (wohnplzo): Bitte geben Sie Ihre Postleitzahl an (01000 bis 99999).

kh2: (wohnplzorto): Bitte geben Sie Ihren Wohnort an (50 Zeichen).

fv:

hv:

fo:

tr: GOTO 4 (D3_4)

hi: Variablen wohnplzo und wohnplzorto bitte erst einblenden, wenn Werte bei
wohnplz bzw. wohnpolzort nicht definiert sind

\--------------------------------

D3_4
====

tc:

vn: wohnqmw; wohnqmwo; wohnqmz; wohnqmzo

qt: offene Angabe

hl:

in:

q: Wie groß ...

is:

it:

st:

ao1: 3 Stellen, Präfix (wohnqmw) Suffix: ist (Individualisierung: “Ihr Haus” bei
Elternwohnern, sonst “Ihre Wohnung”)

ao2: -12 (wohnqmwo): weiß ich nicht (Exklusivkategorie)

ao3: 2 Stellen, Präfix (wohnqmz) Suffix: ist das von Ihnen genutzte Zimmer:
[number] m²

ao4: -12 (wohnqmzo): weiß ich nicht (Exklusivkategorie)

mv:

ka:

vc1: SHOW ao3 IF wenn Elternwohner\*innen oder WG-Wohnende

vc2: SHOW ao4 IF wenn Elternwohner\*innen oder WG-Wohnende

av1: number: 3 stellig : 1 TO 999

av2: number: 2 stellig : 1 TO 99

kh:

fv:

hv:

fo:

tr: GOTO 5 (D3_5)

hi:

\--------------------------------

D3_5
====

tc:

vn: wohnzust

qt: Einfachauswahlmatrix

hl:

in:

q: Wie würden Sie den allgemeinen Zustand Ihrer Wohnung insgesamt einschätzen?

is:

it:

st:

ao1: 1: sehr schlecht

ao2: 2

ao3: 3

ao4: 4

ao5: 5: sehr gut

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO 6 (D3_6)

hi:

\--------------------------------

D3_6
====

tc:

vn: feinelto; feinkino; feinparo; feinjobdso; feinjobo; feinspao; feinbafo;
feinkredo; feinstio; feinekio; feinbest1; feinbest2; feinbest3; feinbest4;
feinbest5; feinbest6; feinbest7; feinbest8; feinbest9; feinandqo

qt: Akkordeon, Einfachauswahl, offene Angabe

hl:

in:

q: Auf Ihre Person bezogen: Wie viel Geld steht Ihnen durchschnittlich pro Monat
während des Sommersemesters 2020 zur Verfügung?

is: Bitte berücksichtigen Sie hier nur das Geld, über das Sie tatsächlich selbst
verfügen. Berücksichtigen Sie hier bitte !!++nicht++!!, was z. B. Ihre Eltern
oder Ihr(e) Partner\*in für Sie direkt an Dritte zahlen (z. B. direkte
Überweisung der Miete an Ihren Vermieter).

Leerzeile

Sollten Sie Ihren Lebensunterhalt auch mit unregelmäßigen Einnahmen oder durch
früher erworbenes Geld (z. B. Ersparnisse) bestreiten, geben Sie bitte nur den
Betrag an, den Sie davon aktuell monatlich im Durchschnitt einsetzen.

it1: (feinelto): Eltern (bar auf die Hand/per Überweisung auf Ihr Konto)

it2: (feinkino): Kindergeld für Sie selbst (sofern nicht bereits bei
Geldbeträgen von den Eltern angegeben)

it3: ( feinparo): Partner\*in (bar auf die Hand/per Überweisung auf Ihr Konto)

it4: (feinjobdso): Ausbildungsvergütung für Duales Studium

it5: (feinjobo): Erwerbstätigkeit

it6: (feinspao): eigene Mittel (z. B. Ersparnisse, Erbe)

it7: (feinbafo): BAföG

it8: (feinkredo): Kredit(e)

it9: (feinstio): Stipendium

it10: (feinekio): Kindergeld/Unterhalt für Ihr(e) Kind(er)

it11: (feinbest1):Leistungen zum Lebensunterhalt nach SGB II (“Hartz IV”) in
Härtefallsituationen

it12: (feinbest2): Grundsicherung wegen voller Erwerbsminderung

it13: (feinbest3): Eingliederungshilfe zur Finanzierung von technischen
Hilfsmitteln zum Studium, Studienassistenzen, Kommunikationsassistenzen etc.

it14: (feinbest4): Integrationshilfen zum Studium (Beantragung über das
Studentenwerk Berlin)

it15: (feinbest5): Leistungen der Eingliederungshilfe zur Finanzierung eines
behindertengerechten Kfz oder für die Nutzung von Fahrdiensten

it16: (feinbest6): Krankenversicherungsleistungen für technische Hilfsmittel

it17: (feinbest7): Leistungen der Pflegeversicherung

it18: (feinbest8): Landespflegegeld/Landesblindengeld

it19: (feinbest9): Hilfe zur Pflege (im Rahmen der Sozialhilfe)

it20: (feinandqo): weitere Finanzierungsquelle(n), und zwar: (offene Angabe:
präfix [für diese zusätzliche offene Angabe muss in diese Klammer eine neue
Variable eingetragen werden] 50 Zeichen)

st:

ao1: 4 Stellen, Präfix [feinelto] Suffix: [number] € pro Monat

ao2: 4 Stellen, Präfix [feinkino] Suffix: [number]€ pro Monat

ao3: 4 Stellen, Präfix [feinparo] Suffix: [number]€ pro Monat

ao4: 4 Stellen, Präfix [feinjobdso] Suffix: [number]€ pro Monat

ao5: 4 Stellen, Präfix [feinjobo] Suffix: [number]€ pro Monat

ao6: 4 Stellen, Präfix [feinspao] Suffix: [number]€ pro Monat

ao7: 4 Stellen, Präfix [feinbafo] Suffix: [number]€ pro Monat

ao8: 4 Stellen, Präfix [feinkredo] Suffix: [number]€ pro Monat

ao9: 4 Stellen, Präfix [feinstio] Suffix: [number]€ pro Monat

ao10: 4 Stellen, Präfix [feinekio] Suffix: [number]€ pro Monat

ao11: 4 Stellen, Präfix [feinbest1] Suffix: [number]€ pro Monat

ao12: 4 Stellen, Präfix [feinbest2] Suffix: [number]€ pro Monat

ao13: 4 Stellen, Präfix [feinbest3] Suffix: [number]€ pro Monat

ao14: 4 Stellen, Präfix [feinbest4] Suffix: [number]€ pro Monat

ao15: 4 Stellen, Präfix [feinbest5] Suffix: [number]€ pro Monat

ao16: 4 Stellen, Präfix [feinbest6] Suffix: [number]€ pro Monat

ao17: 4 Stellen, Präfix [feinbest7] Suffix: [number]€ pro Monat

ao18: 4 Stellen, Präfix [feinbest8] Suffix: [number]€ pro Monat

ao19: 4 Stellen, Präfix [feinbest9] Suffix: [number]€ pro Monat

ao20: 4 Stellen, Präfix [feinandqo] Suffix: [number]€ pro Monat

mv:

ka:

vc1: SHOW it4 (feinjobdso) if [Variable für Dualstudierende] = [Antwortoption]

vc2: SHOW it5 (feinjobo) if [Variable für Dualstudierende] = [Antwortoption]:
Verdienst aus weiteren Tätigkeiten außerhalb der Ausbildungsinstitution während
des Dualen Studiums

vc3: SHOW it10 (feinekio) if [Variable für Studierende mit Kind] =
[Antwortoption]

vc4: SHOW it11 – it19 (feinbest1 – feinbest9) if [Variablen für
best-Studierende] = [Antwortoptionen]

vc5: SHOW it13 (feinbest3) if NOT [Variable für Studierende aus Berlin] =
[Antwortoption]

vc6: SHOW it14 (feinbest4) if [Variable für Studierende aus Berlin] =
[Antwortoption]

av: number : 1-4 stellig : 1 TO 9999

kh: Bitte geben Sie Ihre jeweiligen monatlichen Einnahmen an (1 bis 9999)

fv:

hv:

fo:

tr:

GOTO 7 (D3_7)

hi: “Finanzierung” und “Betrag” als Spaltenüberschriften; pro Zeile soll
angegeben werden können, ob die jeweilige Einnahme/Finanzierungsquelle vorliegt
(ja/nein) und wenn ja, welcher Betrag eingenommen wird (Wertebereich 1 bis 9999)

\--------------------------------

D3_7
====

tc:

vn: feininsg; feininsgo

qt: offene Angabe

hl:

in:

q: Und wie hoch waren Ihre persönlichen Gesamteinnahmen im letzten Monat?

is:

it:

st:

ao1: 4 Stellen, Präfix [feininsg] Sufix: Gesamteinnahmen: ca. [number] €

ao2: -12: : weiß ich nicht (Exklusivkategorie)

ao3: -13: : keine Angabe (Exklusivkategorie)

mv:

ka:

vc:

av: number : 1-4 stellig : 1 TO 9999

kh: Bitte geben Sie Ihre monatlichen Gesamteinnahmen an (1 bis 9999)

fv:

hv:

fo:

tr: GOTO 8 (D3_8)

hi:

\--------------------------------

D3_8
====

tc: IF feinsti = 1 AND feinstio\>0 (Einnahmen aus Stipendium)

vn: festipart

qt: Mehrfachauswahl

hl:

in:

q: Was für ein Stipendium erhalten Sie?

is: Bitte alles zutreffende auswählen.

it:

st:

ao1: 1: Deutschlandstipendium

ao2: 2: Stipendium der Studienstiftung des deutschen Volkes e. V.

ao3: 3: Stipendium einer parteinahen Stiftung

ao4: 4: Stipendium eines anderen Begabtenförderungswerks

ao5: 5: anderes mit staatlichen Mitteln finanziertes Stipendium (Geldgeber:
Land, Kommune, Hochschule)

ao6: 6: Stipendium eines privaten Geldgebers (Industrie, Firma, privater
Stifter)

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO 9 (D3_9)

hi:

\--------------------------------

D3_9
====

tc:

vn1: „Ich bezahle selbst“ [hier eine neue Stammvariable einfügen]: (fausgmieto;
fausgerno; fausgkomo; fausgkleio; fausglerno; fausgmobo; fausggeso; fausgsemo;
fausgstuo; fausffreio; fausgkitaso; fausgkindso; fausgasso; fausandqo)

vn2: „Dritte (Eltern, Partner\*in etc) bezahlen direkt [hier eine neue
Stammvariable einfügen]: (feindmieto; feinderno, feindkomo; feindkleio;
feindlerno; feindgmobo, feindgeso; feindgsemo; feindgstuo; feindgfreio;
feindkitaso; feindkindso; feindgasso; feinandquo2)

qt: offene Matrix

hl:

in: Kommen wir nun zu Ihren monatlichen Kosten und Ausgaben:

q: Bitte geben Sie an, welche Ausgaben Sie bzw. Dritte für Sie (z. B. Eltern
bezahlen Ihre Miete direkt an den Vermieter) im Sommersemester 2020 monatlich
haben.

is:

it1: (fausgmieto; feindmieto): Miete inkl. Nebenkosten (Strom, Heizung,
(Ab-)Wasser usw.)

it2: (fausgerno; feinderno): Ernährung (Lebensmittel und Getränke, auch außer
Haus)

it3: (fausgkomo; feindkomo): (Mobil)Telefon, Internet, Audio-/Videostreaming

it4: (fausgkleio; feindkleio): Kleidung

it5: (fausglerno; feindlerno): Lernmittel (z. B. Fachliteratur; aber nicht:
einmalige Anschaffungskosten für PC, Instrument o. ä.)

it6: (fausgmobo; feindgmobo): Mobilität (z. B. Semesterticket, laufende Ausgaben
für Kfz, öff. Verkehrsmittel)

it7: (fausggeso; feindgeso): Gesundheitskosten (z. B. Krankenversicherung,
Medikamente, Therapiemaßnahmen)

it8: (fausgsemo; feindgsemo): Semesterbeitrag (ohne Semesterticket)

it9: (faugstuo; feindgstuo): Studiengebühren (z. B. Zweit-, Langzeitgebühren)

it10: (fausgfreio; feindgfreio): Freizeit, Kultur und Sport

it11: (fausgkitaso; feindkitaso): Ausgaben Kinderbetreuung

it12: (fausgkindso; feindkindso): kinderbezogene Ausgaben für Drogerieartikel,
Kleidung, Spielzeug

it13: (fausgasso; feindgasso): Ausgaben für personelle Assistenzen (z. B.
Pflegeassistenz, Mitschreibkraft, Haushaltshilfe

it14: (fausandqo; feinandqo2): weitere Ausgaben, und zwar:

st:

ao1: Präfix [fausgmieto; feindmieto] Suffix: [number] € pro Monat

ao2: Präfix [fausgerno; feinderno] Suffix: [number] € pro Monat

ao3: Präfix [fausgkomo; feindkomo] Suffix: [number] € pro Monat

ao4: Präfix [fausgkleio; feindkleio] Suffix: [number] € pro Monat

ao5: Präfix [fausglerno; feindlerno] Suffix: [number] € pro Monat

ao6: Präfix [fausgmobo; feindgmobo] Suffix: [number] € pro Monat

ao7: Präfix [fausggeso; feindgeso] Suffix: [number] € pro Monat

ao8: Präfix [fausgsemo; feindgsemo] Suffix: [number] € pro Monat

ao9: Präfix [faugstuo; feindgstuo] Suffix: [number] € pro Monat

ao10: Präfix [fausgfreio; feindgfreio] Suffix: [number] € pro Monat

ao11: Präfix [fausgkitaso; feindkitaso] Suffix: [number] € pro Monat

ao12: Präfix [fausgkindso; feindkindso] Suffix: [number] € pro Monat

ao13: Präfix [fausgasso; feindgasso] Suffix: [number] € pro Monat

ao14: Präfix [fausandqo; feinandqo2 hier müssen zwei neue Variable eingetragen
werden] Suffix: [number] (50 Zeichen

ao 14: Präfix [fausandqo; feinandqo2] Suffix: [number] € pro Monat

mv:

ka:

vc1: SHOW fausgsemo; feindgsemo IF NOT [Variable für private Hochschulen] = x
(nicht für private Hochschulen

vc2: SHOW fausgstuo; feindgstuo IF NOT [Variable für private Hochschulen] = x
(nicht für private Hochschulen

vc3: SHOW fausgkitaso; feindkitaso IF [Variable für Studierende mit Kind] = x

vc4: SHOW fausgkindso; feindkindso IF [Variable für Studierende mit Kind] = x

vc5: SHOW fausgasso; feindgasso IF [Variable für beeinträchtigt Studierende] = x

av1: number : 1 bis 4 stellig (1-9999)

av2: number : 50 Zeichen (hier nur für 2 Variablen x müssen noch eingetragen
werden, siehe unter ao14)

kh: Bitte geben Sie Ihre jeweiligen monatlichen Ausgaben an (1 bis 9999)

fv:

hv:

fo:

tr: GOTO 10 (D3_10)

hi: “Ich bezahle selbst” und “Dritte (Eltern, Partner\*in etc.) bezahlen direkt”
als Spaltenüberschriften

\--------------------------------

D3_10
=====

tc:

vn: fausing; fausinsgo

qt: offene Angabe

hl:

in:

q: Und wie hoch waren Ihre persönlichen Gesamtausgaben im letzten Monat?

is:

it:

st:

ao1: 4, Präfix [feininsg] Suffix: Gesamtausgaben: ca. [number] €

ao2: -12: : weiß ich nicht (Exklusivkategorie)

ao3: -13: : keine Angabe (Exklusivkategorie)

mv:

ka:

vc:

av: number : 1-4 stellig : 1 TO 9999

kh: Bitte geben Sie Ihre monatlichen Gesamtausgaben an (1 bis 9999)

fv:

hv:

fo:

tr: GOTO 11 (D3_11)

hi:

\--------------------------------

D3_11
=====

tc:

vn: fmineink; fmineinko

qt: offene Angabe

hl:

in:

q: Was wären Ihrer Meinung nach die absolut niedrigsten Einnahmen pro Monat, die
Sie benötigen, um finanziell zu recht zu kommen?

is:

it:

st:

ao1: 4, Präfix [feininsg] Suffix: Mindesteinnahmen: . [number] €

ao2: -12: : weiß ich nicht (Exklusivkategorie)

mv:

ka:

vc:

av: number : 1-4 stellig : 1 TO 9999

kh: Bitte geben Sie Ihre monatlichen Gesamtausgaben an (1 bis 9999)

fv:

hv:

fo:

tr: GOTO 12 bzw. 13 (D3_12 --\> Studierende an privaten Hochschulen; D3_13 --\>
Else)

hi:

\--------------------------------

D3_12
=====

tc: IF [Variable für Studierende an privaten Hochschulen]

vn: fausgebi; fausgebio; fausgebs; fausgebso; fausgebd; fausgebdo; fausgeba;
fausgebao

qt: offene Angabe

hl:

in:

q: Wie viel Geld geben Sie durchschnittlich pro Monat im Sommersemester 2020 für
Studiengebühren aus?

is: Falls Sie hierbei von anderen bzw. Ihrem Arbeitgeber unterstützt werden,
indem diese die Bezahlung direkt übernehmen, geben Sie die Höhe dieser
Leistungen bitte in der betreffenden Spalte an.

it:

st:

ao1: 5 Stellen; Präfix [fausgebi; fausgebio] Suffix: insgesamt: [number] €

ao2: 5 Stellen; Präfix (fausgebs; fausgebso) Suffix: davon bezahle ich selbst:
[number] €

ao3: Stellen; 5 Präfix (fausgebd; fausgebdo) Suffix: bezahlen Dritte (Eltern,
Partner\*in) für mich direkt: [number] €

ao4: 5 Stellen, Präfix (fausgeba, fausgebao) Suffix: bezahlt mein Arbeitgeber
für mich direkt: [nuimber] €

mv:

ka:

vc:

av: number : 1-5 stellig : 1 TO 99999

kh:

fv:

hv:

fo:

tr: GOTO 13 (3_13)

hi:

\--------------------------------

D3_13
=====

tc:

vn: fsitzum1; fsitzum2; fsitzum3; fsitelt1; fsitelt2; fsitelt3

qt: Einfachauswahlmatrix

hl:

in:

q: Inwieweit treffen die nachfolgenden Aussagen auf Sie und Ihre finanzielle
Situation zu?

is:

it1: (fsitzum1): Ich verfüge zurzeit über ausreichend finanzielle Mittel, um
meine monatlichen Ausgaben zu decken.

it2: (fsitzum2): Ich habe zurzeit finanzielle Schwierigkeiten.

it3: (fsitzum3): Die Finanzierung meines Lebensunterhalts während meines
Studiums ist sichergestellt.

it4: (fsitelt1): Meine Eltern unterstützen mich finanziell so gut sie können.

it5: (fsitelt2): Ich habe den Eindruck, meine Eltern finanziell zu überfordern.

it6: (fsitelt3): Ich will finanziell nicht auf meine Eltern angewiesen sein.

st:

ao1: 1: trifft gar nicht zu

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

tr: GOTO 14 (D3_14)

hi: Items bitte zufällig rotieren

\--------------------------------

D3_14
=====

tc:

vn: feinstf1; feinstf2; feinstf3; feinstf4; feinstf5; feinstf6; feinstf7;
feinstf8

qt: Einfachauswahlmatrix (keine Mehrfachauswahl???)

hl:

in:

q: Der Umgang mit Feld kann unterschiedliche Herausforderungen mit sich bringen:
Inwieweit treffen die nachfolgenden Aussagen auf Sie zu?

is:

it1: (feinstf1): Ich gebe Geld lieber sofort aus als es für einen späteren
Zeitpunkt zu sparen.

it2: (feinstf2): Ich kümmere mich sorgfältig um meine finanziellen
Angelegenheiten.

it3: (feinstf3): Es gelingt mir, mit meinem Geld auszukommen.

it4: (feinstf4): Es belastet mich, mir Gedanken über meine finanzielle Zukunft
zu machen.

it5: (feinstf5): Bevor ich etwas kaufe, vergleiche ich immer die Preise

it6: (feinstf6): Ich achte darauf, dass ich Geld für schlechte Zeiten habe.

it7: (feinstf7): Ich empfinde es als sehr anstrengend, den Überblick über meine
Finanzen zu behalten.

it8: (feinstf8): Ich neige dazu, im Hier und Jetzt zu leben und lasse die
Zukunft auf mich zukommen.

st:

ao1: 1: trifft gar nicht zu

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

tr: GOTO 15 (D3_15)

hi: Items bitte zufällig rotieren

\--------------------------------

D3_15
=====

tc:

vn: fbafja

qt: Einfachauswahl

hl:

in:

q: Werden Sie im Sommersemester 2020 nach dem BAföG gefördert?

is:

it:

st:

ao1: 1: Nein, ich habe keinen Antrag gestellt.

ao2: 2: Nein, mein aktueller Antrag wurde endgültig abgelehnt.

ao3: 3: Über meinen Antrag (bzw. Widerspruch) ist noch nicht entschieden.

ao4: 4: Ja

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO 16 (D3_16) IF fbafja = 1

GOTO 17 (D3_17) IF fbafja = 2

GOTO 19 (D3_19) IF fbafja = 4

GOTO 21 (D3_21) IF fbafja = 3

hi:

\--------------------------------

D3_16
=====

tc: IF fbafja = 1 (kein Bafög-Antrag gestellt)

vn: fbafex

qt: Einfachauswahl

hl:

in:

q: Haben Sie während Ihres Studiums früher einmal einen Antrag auf BAföG
gestellt?

is:

it:

st:

ao1: 1: Nein.

ao2: 2: Ja, ich habe einmal einen Antrag gestellt, der wurde aber abgelehnt.

ao3: 3: Ja, in früheren Semestern wurde ich auch gefördert, ein Antrag auf
Weiterförderung wurde dann aber abgelehnt.

ao4: 4: Ja, in früheren Semestern wurde ich auch gefördert, habe dann aber
keinen Antrag auf Weiterförderung mehr gestellt.

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO 18 (D3_18)

hi:

\--------------------------------

D3_17
=====

tc:IF fbafja = 2 (Bafög-Antrag abgelehnt)

vn: fbafabg

qt: Einfachauswahl

hl:

in:

q: Haben Sie bereits früher schon einmal einen Antrag auf BAföG gestellt?

is:

it:

st:

ao1: 1: Nein.

ao2: 2: Ja, ich habe früher einen Antrag gestellt, der wurde aber abgelehnt.

ao3: 3: Ja, in früheren Semestern wurde ich auch gefördert.

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO 18 (D3_18)

hi:

\--------------------------------

D3_18
=====

tc: IF fbafja = 1 \| 2 (im SS 2020 kein Bafög)

vn: fbafkelt; fbafkein; fbafkfhd; fbafktw; fbafkleis; fbafkalt; fbafkzwei;
fbafkweni; fabfkschu; fbafand; fbafando

qt: Einfachauswahl (Mehrfachnennung) und offene Angabe (ao11)

hl:

in:

q: Aus welchen Gründen Individualisierung:

wenn fbafja = 1 AND fbafex = 1 \| kA: haben Sie bisher keinen BAföG-Antrag
gestellt?

wenn fbafja = 2: wurde Ihr aktueller Antrag abgelehnt?

wenn (fbafja = 1) AND (fbafex = 2 \| 3): wurde Ihr Antrag damals abgelehnt?

wenn fbafja = 2 AND fbafex = 4: haben Sie keinen Antrag auf Weiterförderung mehr
gestellt?

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (fbafkelt): Einkommen der Eltern bzw. des Ehepartners/der Ehepartnerin
ist/war zu hoch

ao2: (fbafkein): eigenes Einkommen/Vermögen ist/war zu noch

ao3: (fbafkfhd): Förderungshöchstdauer wurde überschritten

ao4: (fbafktw): Studienfach wurde gewechselt

ao5: (fbafkleis): notwenige Leistungsbescheinigung konnte nicht erbracht warden

ao6: (fbafkalt): bei Studienbeginn war die maßgebliche Altersgrenze bereits
überschritten

ao7: (fbafkzwei): das jetzige Studium ist eine nicht förderungsfähige weitere
Hochschulausbildung (Zweitstudium, Ergänzungsstudium)

ao8: (fbafkweni): der zu erwartende Förderbeitrag ist/war so gering, dass es
sich nicht lohnt/e

ao9: (fbafkschu): will/wollte keine Schulden Machen

ao10: (fbafand): andere Gründe, und zwar:

ao11: 50 Zeichen, Präfix (fbafando) Suffix: 50 Zeichen

ao2:

ao3:

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO 21 (D3_21)

hi:

\--------------------------------

D3_19
=====

tc: IF fbafja = 4 (Form der Bafög-Förderung I)

vn: fbafunab

qt: Einfachauswahl

hl:

in:

q: Wird das BAföG unabhängig vom Einkommen Ihrer Eltern gewährt?

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

tr: GOTO 20 (D3_20)

hi:

\--------------------------------

D3_20
=====

tc: IF fbafja = 4 (Form der Bafög-Förderung II)

vn: fbafkv; fbafkin

qt: Mehrfachauswahl

hl:

in:

q: Ist in Ihrem Förderungsbetrag ein Zuschlag enthalten für …

is: Bitte alles Zutreffende auswählen.

it:

st:

ao1: (fbafkv): … Ihre Kranken- und Pflegeversicherung?

ao2: (fbafkin): … die Betreuung Ihres Kindes/Ihrer Kinder?

mv:

ka:

vc: SHOW fbafkin IF dkinja = 2

av:

kh:

fv:

hv:

fo:

tr: GOTO 21 (D3_21)

hi:

\--------------------------------

D3_21
=====

tc: IF eaktsens = 2 \| 3 \| 4 (Studierende mit mind. einer Erwerbstätigkeit)

vn: etat (etat1 / etat2 / etat3)

edau (edau1/ edau1o / edau2 / edau2o / edau3 / edau3o)

qt: offene Angaben (Tableau – Drop Down)

hl:

in:

q1: Bitte geben Sie die Art und Dauer Ihrer Erwerbstätigkeit, der Sie im
aktuellen Semester nachgehen, an.

q2: Bitte geben Sie die Art und Dauer Ihrer Erwerbstätigkeit, der Sie neben
Ihrer Tätigkeit im Ausbildungsbetrieb im aktuellen Semester nachgehen, an.

q3: Sie haben angegeben, im aktuellen Semester mehreren Erwerbstätigkeiten
nachzugehen.

Bitte geben Sie die jeweilige Art und Dauer Ihrer Erwerbstätigkeiten an.

q4: Sie haben angegeben, im aktuellen Semester mehreren Erwerbstätigkeiten,
neben Ihrer Tätigkeit im Ausbildungsbetrieb, nachzugehen.

Bitte geben Sie die jeweilige Art und Dauer Ihrer Erwerbstätigkeiten an.

q5: Sie haben angegeben, im aktuellen Semester mehreren Erwerbstätigkeiten
nachzugehen.

Bitte geben Sie die jeweilige Art und Dauer Ihrer Erwerbstätigkeiten, der Sie im
aktuellen Semester nachgehen, an.

q6: Sie haben angegeben, im aktuellen Semester mehreren Erwerbstätigkeiten,
neben Ihrer Tätigkeit im Ausbildungsbetrieb, nachzugehen.

Bitte geben Sie die jeweilige Art und Dauer Ihrer Erwerbstätigkeiten an.

is:

it1: (etat1): Art der Tätigkeit [Dropdown-Menü] (Tätigkeit A)

it2: (edau1): Dauer [edau1o] (Tätigkeit A)

it3: (etat2): Art der Tätigkeit [Dropdown-Menü] (Tätigkeit B)

it4: (edau2): Dauer [edau2o] (Tätigkeit B)

it5: (etat3): Art der Tätigkeit [Dropdown-Menü] (Tätigkeit C)

it6: (edau3): Dauer [edau3o] (Tätigkeit C)

st:

ao1: 1: : Tätigkeit als studentische/ wissenschaftliche Hilfskraft im Bereich
Forschung und Lehre

ao2: 2: : Tätigkeit als studentische/ wissenschaftliche Hilfskraft im Bereich
Verwaltung

ao3: 3: : Jobben (z. B. in einer Fabrik, einem Büro, einer Kneipe, Babysitten,
Nachhilfeunterricht)

ao4: 4: : Tätigkeit, die einen Hochschulabschluss voraussetzt (ohne Hilfskraft)

ao5: 5: : Tätigkeit, die einen beruflichen Ausbildungsabschluss voraussetzt

ao6: 6: : Tätigkeit als Praktikant(in)

ao7 (edau): 3; 1-999; Präfix: Dauer:; Suffix: Monate

mv:

ka1 (it1, it2): Tätigkeit A

ka2 (it3, it4): Tätigkeit B

ka3 (it5, it6): Tätigkeit C

vc:

SHOW q1 IF eaktsens = 2

SHOW q2 IF eaktsens = 2 AND sformdua = 1

SHOW q3 IF eaktsens = 3

SHOW q4 IF eaktsens = 3 AND sformdua = 1

SHOW q5 IF eaktsens = 4

SHOW q6 IF eaktsens = 4 AND sformdua = 1

SHOW it1 AND it2 IF eaktsens = 2 OR eaktsens = 2 AND sformdua = 1

SHOW it1 TO it4 IF eaktsens = 3 OR eaktsens = 3 AND sformdua = 1

SHOW it1 TO it6 IF eaktsens = 4 OR eaktsens = 4 AND sformdua = 1

SHOW ka1 AND ka2 IF eaktsens = 3 OR eaktsens = 3 AND sformdua = 1

SHOW ka1 TO ka3 IF eaktsens = 4 OR eaktsens = 4 AND sformdua = 1

av: number: \<= dreistellig : 1 TO 999

kh: Bitte geben Sie an, wieviel Monate Sie Ihre Erwerbstätigkeit bereits ausüben
(1 bis 999)

fv:

hv:

fo:

tr: GOTO 22 (D3_22) IF (Variable für Dual Studierende + Berufsbegleitend
Studierende) = x (hier entsprechende Ausprägungen)

ELSE GOTO 23 (D3_23)

hi: Als Drop-Down Menü für “Art der Tätigkeit”, Bitte „Art der Tätigkeit“ und
„Dauer“ als Spalten programmieren, die für jede Tätigkeit (sie bilden die
Zeilen) abgefragt werden.

\--------------------------------

D3_22
=====

tc: Frage wird berufsbegleitend oder dual Studierenden gestellt

vn1: deltjobbbs (deltjobbbso1 / deltjobbbso2)

vn2: deltjobds (deltjobdso1 / deltjobdso2)

qt: offene Abfrage im Spaltenformat / Einfachauswahl im Spaltenformat

hl:

in:

q: Welchen Beruf üben Sie aktuell aus? Bitte erläutern Sie die Tätigkeit kurz.

is: Falls Sie zurzeit nicht erwerbstätig sind, geben Sie bitte die Ihre zuletzt
ausgeübte Tätigkeit an.

\*\*++Bitte tragen Sie die genaue Bezeichnung und Tätigkeit inklusive
Führungsaufgaben ein. Zum Beispiel:

-   Bankkaufmann/-frau (nicht: Angestellte/r) Beratung, Verkauf von
    Finanzprodukten, Abteilungsleitung

-   Zollbeamte(r) im gehobenen Dienst (nicht: Beamter/in) Zollfahndung,
    Einsatzplanung

-   Maschinenbauingenieur(in) (nicht: Ingenieur/in) Konstruktion,
    Optimierungsprozesse, Produktionsleitung++\*\*

it:

st:

ao1(-o1): 50; Präfix: \*\*++Berufsbezeichnung:++\*\*

ao2 (-o2): 50; Präfix: \*\*++Tätigkeitsbeschreibung:++\*\*

ao3: -11: : \*\*++nie berufstätig gewesen++\*\*

ao4: -12: : weiß ich nicht [EK]

mv:

ka:

vc:

SHOW vn1 IF sformberu == 1

SHOW vn2 IF sformdua == 1

av:

kh:

fv:

hv:

fo:

tr: GOTO 23 (D3_24)

hi:

\--------------------------------

D3_24
=====

tc: IF eaktsens = 2 \|3 \|4

vn: egr (egrfin1 / egrfin2 / egrfin3 / egrkar1 / egrkar2 / egrper1 / egrper2 /
egrper3 / egrerf1 / egrerf2 / egralt1 / egralt2)

qt: Caroussel

hl:

in:

q1: Inwiefern treffen die folgenden Aussagen auf Sie zu? Ich gehe während des
aktuellen Semesters einer Erwerbstätigkeit nach, …

q2: Inwiefern treffen die folgenden Aussagen auf Sie zu? Ich gehe während des
aktuellen Semesters einer Erwerbstätigkeit, die ich neben meiner Tätigkeit im
Ausbildungsbetrieb ausübe, nach, …

q3: Inwiefern treffen die folgenden Aussagen auf Sie zu? Ich gehe während des
aktuellen Semesters mehreren Erwerbstätigkeiten nach, …

q4: Inwiefern treffen die folgenden Aussagen auf Sie zu? Ich gehe während des
aktuellen Semesters mehreren Erwerbstätigkeiten, die ich neben meiner Tätigkeit
im Ausbildungsbetrieb ausübe, nach, …

is:

it1: (egrfin1): weil es zur Finanzierung meines Lebensunterhalts unbedingt
notwendig ist.

it2: (egrfin2): um mir mein Studium finanzieren zu können.

it3: (egrfin3): damit ich mir (etwas) mehr leisten kann.

it4: (egrkar1): um Kontakte für eine spätere Beschäftigung zu knüpfen.

it5: (egrkar2): um mich neben dem Studium weiter zu qualifizieren.

it6: (egrper1): damit ich meinen Horizont erweitern kann.

it7: (egrper2): um mehr über meine Stärken und Schwächen zu erfahren.

it8: (egrper3): um mich persönlich weiter zu entwickeln.

it9: (egrerf1): um praktische Erfahrungen zu sammeln.

it10: (egrerf2): um etwas Neues zu lernen und mich fortzubilden.

it11: (egralt1): um einen Beitrag zur Gesellschaft zu leisten.

it12: (egralt2): um anderen zu helfen.

st:

ao1: 1: trifft gar nicht zu

ao2: 2

ao3: 3:

ao4: 4

ao5: 5: trifft voll und ganz zu

mv:

ka:

vc:

SHOW q1 IF eaktsens = 2

SHOW q2 IF eaktsens = 2 AND sformdua == 1

SHOW q3 IF eaktsens = [ 3 \| 4]

SHOW q4 IF eaktsens = [3 \| 4] AND sformdua == 1

av:

kh:

fv:

hv:

fo:

tr: GOTO 24 (D3_25)

hi: Items bitte zufällig rotieren.

\--------------------------------

D3_24
=====

tc:

vn: zufrwohn /zufrlstand / zufrfinsit / zufrerw / zufrleb

qt: Einfachauswahlmatrix mit horizontal abgetragenen Antwortoptionen

hl:

in:

q: Wie zufrieden sind Sie mit…

is:

it1: (zufrwohn): Ihrer aktuellen Wohnsituation?

it2: (zufrlstand): Ihrem derzeitigen Lebensstandard?

it3: (zufrfinsit): Ihrer aktuellen finanziellen Situation?

it4: (zufrerw): Ihrer/Ihren aktuellen Erwerbstätigkeit/en?

it5: (zufrleb): mit Ihrem Leben insgesamt?

st:

ao1: 1: gar nicht zufrieden

ao2: 2

ao3: 3

ao4: 4

ao5: 5: sehr zufrieden

mv:

ka:

vc:

SHOW it4 IF eaktsens = 2 \|3 \|4

av:

kh:

fv:

hv:

fo:

tr:

GOTO nächstes Modul

hi:
