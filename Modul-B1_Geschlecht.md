\--------------------------------

1
=

tc:

vn: sexorient; sexoriento

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Was beschreibt Ihre sexuelle Orientierung am ehesten?

is:

it:

st:

ao1: 1: heterosexuell

ao2: 2: schwul

ao3: 3: lesbisch

ao4: 4: bisexuell

ao5: 5: offene Angabe: 25, Prefix: eine andere, und zwar:

ao6: 6: unklar



mv: -12: Ich möchte diese Frage nicht beantworten.

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
=

tc:

vn: genidsach / genidloes / genidrat / genidueb / genidmach / genidrue /
genidlieb / genideinf / genidemo / genidang / genidempf / genidvor

qt: Einfachauswahlmatrix

hl:

in:

q: Wenn Sie sich selbst beschreiben müssten: Welche Eigenschaften treffen am
ehesten auf Sie zu?

is:

it1: (genidsach): sachlich

it2: (genidloes): lösungsorientiert

it3: (genidrat): rational

it4: (genidueb): überheblich

it5: (genidmach): machtbesessen

it6: (genidrue): rücksichtslos

it7: (genidlieb): liebevoll

it8: (genideinf): einfühlsam

it9: (genidemo): emotional

it10: (genidang): ängstlich

it11: (genidempf): empfindlich

it12: (genidvor): vorsichtig

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

fo: Items bitte zufällig rotieren.

tr:

GOTO 4 IF demosex=3

ELSE GOTO 3 (Aufteilung 3a und 3b)

hi:

\--------------------------------

3a
==

tc: IF demosex\<\>3

vn: besex01 / besex02 / besex03 / besex04 / besex05 / besex06 / besex07 /
besex08 / besex09 / besex10 / besex11,

hosex01 / hosex02 / hosex03 / hosex04 / hosex05 / hosex06 / hosex07 / hosex08 /
hosex09 / hosex10 / hosex11

qt: Einfachauswahlmatrix

hl:

in:

q: Nachfolgend finden Sie eine Reihe von Aussagen über Frauen und Männer und
ihre Beziehungen in der heutigen Gesellschaft. Bitte geben Sie an, in welchem
Ausmaß Sie der jeweiligen Aussage zustimmen oder nicht zustimmen. Benutzen Sie
dazu die folgende Skala:

is:

it1: (besex01): Egal wie erfolgreich ein Mann auch sein mag, ohne die Liebe
einer Frau fehlt ihm etwas ganz Wichtiges.

it2: (hosex01): Viele Frauen versuchen unter dem Deckmantel der
Gleichberechtigung, besondere Vergünstigungen zu erlangen, wie z.B. eine
Bevorzugung bei der Besetzung von Arbeitsstellen.

it3: (besex02): Bei einer Katastrophe sollten Frauen vor Männern gerettet
werden.

it4: (hosex02): Die meisten Frauen interpretieren harmlose Äußerungen oder
Handlungen als frauenfeindlich.

it5: (hosex03): Frauen sind zu schnell beleidigt.

it6: (besex03): Man kann im Leben erst richtig glücklich sein, wenn man einen
Partner hat, den man liebt.

it7: (hosex04): Feministinnen wollen, dass Frauen mehr Macht bekommen als
Männer.

it8: (besex04): Viele Frauen haben eine Art von Ehrlichkeit, die nur wenige
Männer besitzen.

it9: (besex05): Frauen sollten von Männern umsorgt und beschützt werden.

it10: (hosex05): Die meisten Frauen sehen gar nicht, was Männer alles für sie
tun.

it11: (hosex06): Frauen versuchen, Macht zu erlangen, indem sie Männer immer
mehr beherrschen.

it12: (besex06): Jeder Mann sollte eine Frau haben, die er über alles liebt.

it13: (besex07): Männer sind ohne Frauen unvollkommen.

it14: (hosex07): Frauen übertreiben Probleme, die sie am Arbeitsplatz haben.

it15: (hosex08): Hat eine Frau erst mal einen Mann „rumgekriegt“, dann versucht
sie, ihn an die kurze Leine zu legen.

it16: (hosex09): Wenn Frauen in einem fairen Wettbewerb gegenüber Männern den
Kürzeren ziehen, behaupten sie gerne, sie seien diskriminiert worden.

it17: (besex08): Eine Frau sollte von ihrem Mann auf Händen getragen werden.

it18: (hosex10): Viele Frauen haben Spaß daran, mit Männern zu „spielen“, indem
sie sich zuerst verführerisch geben, dann aber die Annäherungsversuche der
Männer zurückweisen.

it19: (besex09): Verglichen mit Männern haben Frauen ein besseres moralisches
Empfinden.

it20: (besex10): Ein Mann sollte bereit sein, sein eigenes Wohl zu opfern, um
für seine Frau sorgen zu können.

it21: (hosex11): Feministinnen stellen an Männer unberechtigte Forderungen.

it22: (besex11): Verglichen mit Männern haben Frauen einen feineren Sinn für
Kultur und einen besseren Geschmack.

st:

ao1: 1: stimme überhaupt nicht zu

ao2: 2: stimme nicht zu

ao3: 3: stimme eher nicht zu

ao4: 4: stimme eher zu

ao5: 5: stimme zu

ao6: 6: stimme voll und ganz zu

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo: Items bitte zufällig rotieren.

tr:

GOTO 4

hi:

\--------------------------------

3b
==

tc: IF demosex\<\>3

vn: trad01 / trad02 / trad03 / trad04 / trad05 / trad06 / trad07 / trad08 /
trad09 / trad010 / trad11 / trad12 / trad13 / trad14 / trad15 / trad16 / trad17
/ trad18 / trad19 / trad20 / trad21,

ntrad ntrad01 / ntrad02 / ntrad03 / ntrad04 / ntrad05 / ntrad06 / ntrad07 /
ntrad08 / ntrad09 / ntrad10 / ntrad11 / ntrad12 / ntrad13 / ntrad14 / ntrad15

qt: Einfachauswahlmatrix

hl:

in:

q: Geben Sie bitte bei den folgenden Aussagen an, inwieweit sie sich mit Ihrer
persönlichen Meinung decken. Tun Sie dies bitte, indem Sie jeweils den
entsprechenden Zahlenwert für „sehr falsch“, „falsch“, „eher falsch“, „eher
richtig“, „richtig“, „sehr richtig“ ankreuzen.

is:

it1: (trad01): Es ist für eine Frau wichtiger, den Ehemann bei seiner Karriere
zu unterstützen, als selbst Karriere zu machen.

it2: (trad02): Die Idee, dass junge Frauen und Mädchen in der Fußball-Bundesliga
spielen, ist einfach lächerlich.

it3: (ntrad01): Der Anteil an Zeit und Energie, den jemand seiner Karriere
einerseits und der Familie andererseits zukommen lässt, sollte von den
persönlichen Wünschen und Interessen und nicht vom Geschlecht bestimmt werden.

it4: (trad03): Es ist für eine Frau wichtiger, eine gute Figur zu haben und gut
gekleidet zu sein, als für einen Mann.

it5: (trad04): Der alte Ausspruch "die Frau gehört ins Haus und zur Familie" ist
im Grund richtig, und es sollte auch so bleiben.

it6: (trad05): Eine Frau sollte gegenüber Männern nicht zu strebsam sein

it7: (trad06): Eine Frau, die in der Öffentlichkeit arbeitet (z.B. eine
Verkäuferin), sollte nicht mehr arbeiten, wenn zu sehen ist, dass sie schwanger
ist.

it8: (trad07): Der Mann sollte in einer Familie für alle größeren Entscheidungen
verantwortlich und zuständig sein.

it9: (trad08): In einer Gruppe mit weiblichen und männlichen Mitgliedern sollte
ein Mann die Führungsposition innehaben.

it10: (trad09): Verheiratete Frauen, die Kinder im Schulalter haben, sollten
nicht arbeiten, es sei denn, es ist für die Familie finanziell unbedingt
notwendig.

it11: (trad010): Wenn sich ein gut qualifizierter Mann und eine etwas besser
qualifizierte Frau um eine Arbeitsstelle bewerben, so sollte der Mann die Stelle
erhalten, da er eine Familie ernähren muss.

it12: (ntrad02): Die Ehe ist eine Partnerschaft, in der Frau und Mann
gleichermaßen für die Finanzen verantwortlich sein sollten.

it13: (trad11): Eine Frau sollte lieber auf ihre Karriere verzichten, als darauf
bestehen, dass ihr Mann wegen einem für sie notwendigen Ortswechsel eine neue
Arbeitsstelle suchen muss.

it14: (ntrad03): Eine verheiratete Frau, die lieber im Beruf weiterkommen möchte
und keine Kinder haben will, sollte deswegen kein schlechtes Gewissen haben.

it15: (trad12): Verheiratete Frauen, die Kinder im Vorschulalter haben, sollten
nicht arbeiten, es sei denn, dass es für die Familie finanziell notwendig ist.

it16: (trad13): Im allgemeinen ist es besser, wenn ein Mann der Leiter einer
Abteilung ist, in der Frauen und Männer arbeiten.

it17: (ntrad04): Im allgemeinen ist es besser, wenn ein Mann der Leiter einer
Abteilung ist, in der Frauen und Männer arbeiten.

it18: (ntrad05): Es ist gut, wenn Frauen lokalpolitische Ämter innehaben.

it19: (trad14): Wenn sich ein Student und eine Studentin um ein Stipendium
bewerben, so sollte es der Student erhalten, da er größere berufliche Chancen
hat.

it20: (ntrad06): Wenn eine Frau eine obszöne Sprache gebraucht, so ist das nicht
anstößiger, als wenn ein Mann dies tut.

it21: (ntrad07): Auch Jungen sollten mit Puppen spielen.

it22: (trad15): Man sollte Mädchen raten, einen weiblichen Beruf wie
Krankenschwester, Schneiderin oder Grundschullehrerin zu wählen.

it23: (ntrad08): Frauen sollten alle athletischen Sportarten betreiben.

it24: (ntrad09): Eltern sollten bei Töchtern ebenso wie bei Söhnen unabhängiges
und selbständiges Verhalten ermuntern und fördern.

it25: (ntrad10): Frauen sollten auch traditionell männliche Berufe wie Maurer
oder Pilot ergreifen.

it26: (ntrad11): Wenn eine Frau ihren Mädchennamen nach der Hochzeit behalten
will, so ist nichts dagegen einzuwenden.

it27: (ntrad12): Es wäre nichts dagegen zu sagen, wenn einmal eine Frau
Bundeskanzler würde.

it28: (trad16): Die berufliche Ausbildung von Jungen sollte für Eltern und
Lehrer wichtiger sein als die von Mädchen.

it29: (trad17): Auch wenn eine Frau arbeitet, sollte der Mann der
"Haupt-Brotverdiener" sein, und die Frau sollte die Verantwortung für den
Haushalt tragen.

it30: (trad18): In der Grundschule sollten Mädchen Kleider und keine langen
Hosen tragen.

it31: (ntrad13): Wenn eine Frau Pfarrer oder Priester wird, so ist nichts
dagegen einzuwenden.

it32: (ntrad14): Frauen sollten vermehrt wichtige landes- und bundespolitische
Ämter innehaben.

it33: (trad19): Es ist nicht gut, wenn ein Mann zu Hause bleibt und die Kinder
versorgt und seine Frau arbeitet.

it34: (trad20): Der einzige Grund, warum Mädchen einen Beruf erlernen sollten,
besteht darin, dass sie eventuell nicht heiraten oder geschieden werden können.

it35: (trad21): Es gibt keine richtige Begründung dafür, dass Männer im vollen
Bus ihren Sitzplatz einer Frau anbieten sollten.

it36: (ntrad15): Männer sollten ruhig auch Berufe ergreifen, die traditionell
Frauen vorbehalten sind (z.B. Kindergärtner, Telefon-Vermittler).

st:

ao1: 1: sehr falsch

ao2: 2: falsch

ao3: 3: eher falsch

ao4: 4: eher richtig

ao5: 5: richtig

ao6: 6: sehr richtig

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO 4

hi:

\--------------------------------

4
=

tc:

vn1: athhm / athhv / athhi / athha

vn2: ateem / ateev / ateei / ateea

vn3: atwem / atwev / atwei / atwea

vn4: atkbm / atkbv / atkbi / atkba

vn5: atkam / atkav / atkai / atkaa

qt: Mehrfachauswahlmatrix mit horizontalen ao mit offener Nennung

hl:

in:

q: Wenn Sie an Ihre Kindheit denken: Wer hat in Ihrer Familie in welchem Ausmaß
zu den folgenden Bereichen im Haushalt beigetragen?

is: \*\*Bitte summieren Sie jeweils die ++Spaltenprozente++ auf 100 Prozent.
Sollten Sie keine (Stief-)Mutter und/oder keinen (Stief-)Vater haben, kreuzen
Sie bitte entsprechend „trifft nicht zu“ an.\*\*

it1: (Stamm-m): (Stief-)Mutter

it2: (Stamm-v): (Stief-)Vater

it3: (Stamm-i): ich selbst

it4: (Stamm-a): andere Personen

st:

ao1 (athh): Hausarbeit: 3, Suffix: %

ao2 (ate): Erwerbseinkommen: 3, Suffix: %

ao3 (atwe): Treffen wichtiger Entscheidungen: 3, Suffix: %

ao4 (atkb): Kinderbetreuung: 3, Suffix: %

ao5 (atka): trifft nicht zu

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO 5a

hi:

\--------------------------------

5a
==

tc:

vn: antfemst

qt: Regler

hl:

in:

q: Bitte denken Sie an die Lehrenden in Ihrem aktuellen Semester: Wie hoch ist
der Anteil an weiblichem Lehrpersonal?

is:

it:

st:

ao1: 0 : 0%

ao50: 50 : \|

ao100: 100 : 100%

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO 5b

hi:

\--------------------------------

5b
==

tc:

vn: antfemsb

qt: Regler

hl:

in:

q: Bitte denken Sie an die Lehrkörper an der Schule, an der Sie Ihre
Studienberechtigung erhalten haben: Wie hoch war der Anteil an für Sie
zuständigem weiblichen Lehrpersonal?

is:

it:

st:

ao1: 0 : 0%

ao50: 50 : \|

ao100: 100 : 100%

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

tc:

vn: promgroßv / promgroßm / promvat / prommut / prombrud / promschw / promtan /
promonk / promcoin / promcoine

qt: Einfachauswahl

hl:

in:

q: Gibt es in ihrem familiären Umfeld jemanden der/die studiert bzw. promoviert
(hat)?

is:

it1: (promgroßv): Großvater

it2: (promgroßm): Großmutter

it3: (promvat): Vater

it4: (prommut): Mutter

it5: (prombrud): Bruder

it6: (promschw): Schwester

it7: (promtan): Tante

it8: (promonk): Onkel

it9: (promcoin): Cousin

it10: (promcoine): Cousine

st:

ao1: 1: nein

ao2: 2: studiert

ao3: 3: promoviert



mv: -12: weiß ich nicht

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
