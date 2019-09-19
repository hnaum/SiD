\--------------------------------

B1_1
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

GOTO B1_2

hi:

\--------------------------------

B1_2
=

tc:

vn: genidsach; genidloes; genidrat; genidueb; genidmach; genidrue; genidlieb; genideinf; genidemo; genidang; genidempf; genidvor

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

GOTO B1_4 IF demosex=3

ELSE GOTO B1_3 (Aufteilung 3a und 3b)

hi:

\--------------------------------

B1_3a
==

tc: IF demosex\<\>3

vn: besex01; besex02; besex03; besex04; besex05; besex06; besex07; besex08; besex09; besex10; besex11;
hosex01; hosex02; hosex03; hosex04; hosex05; hosex06; hosex07; hosex08; hosex09; hosex10; hosex11

qt: Einfachauswahlmatrix

hl:

in:

q: Nachfolgend finden Sie eine Reihe von Aussagen über Frauen und Männer und
ihre Beziehungen in der heutigen Gesellschaft. Bitte geben Sie an, in welchem
Ausmaß Sie der jeweiligen Aussage zustimmen oder nicht zustimmen.

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

it21: (hosex11): Feministinnen stellen oftmals unberechtigte Forderungen an Männer.

it22: (besex11): Verglichen mit Männern haben Frauen einen feineren Sinn für
Kultur und einen besseren Geschmack.

st:

ao1: 1: stimme gar nicht zu

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

fo: Items bitte zufällig rotieren.

tr:

GOTO B1_4a IF wohnpar=1
ELSE GOTO B1_5

hi:

\--------------------------------

B1_3b
==

tc: IF demosex\<\>3

vn: chldsuffer; malebread; fulldadbad; wrkmumhome; chldben; fullmumtod; bothfull; fulldadtod; rolechange 


qt: Einfachauswahlmatrix

hl:

in:

q: Über die Aufgaben von Müttern und Vätern gibt es verschiedene Meinungen.
Bitte geben Sie an, inwiefern Sie den folgenden Aussagen zustimmen.

is:

it1: (chldsuffer): Ein Kleinkind wird sicherlich darunter leiden, wenn seine Mutter berufstätig ist.

it2: (malebread): Es ist für alle Beteiligten viel besser, wenn der Mann voll im Berufsleben steht und die Frau zu Hause bleibt und sich um den Haushalt und die Kinder kümmert.

it3: (fulldadbad): Ein Vollzeit erwerbstätiger Vater kann sich nicht ausreichend um seine Kinder kümmern.

it4: (wrkmumhome): Auch wenn beide Eltern erwerbstätig sind, ist es besser, wenn die Verantwortung für den Haushalt und die Kinder hauptsächlich bei der Frau liegt.

it5: (chldben): Es ist für ein Kind sogar gut, wenn seine Mutter berufstätig ist und sich nicht nur auf den Haushalt konzentriert.

it6: (fullmumtod): Eine Vollzeiterwerbstätige Mutter kann zu ihrem Kleinkind normalerweise ein genauso inniges Verhältnis haben wie eine Mutter, die nicht berufstätig ist.

it7: (bothfull): Die beste Arbeitsteilung in einer Familie ist die, dass beide Partner Vollzeit arbeiten und sich gleichermaßen um den Haushalt und die Kinder kümmern.

it8: (fulldadtod): Ein Vollzeit erwerbstätiger Vater kann zu seinem Kleinkind normalerweise ein genauso inniges Verhältnis haben wie ein Vater, der nicht berufstätig ist.

it9: (rolechange): In einer Familie kann auch der Mann für den Haushalt und die Kinder verantwortlich sein, während die Frau Vollzeit erwerbstätig ist.

st:

ao1: 1: stimme gar nicht zu

ao2: 2: 2

ao3: 3: 3

ao4: 4: 4

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

GOTO B1_4a IF wohnpar=1
ELSE GOTO B1_5

hi:

\--------------------------------

B1_4a
==

tc: IF wohnpar=1

vn: atakhh_p/_i/_a; atakee_p/_i/_a; atakwe_p/_i/_a; atakkb_p/_i/_a

qt: Mehrfachauswahlmatrix mit horizontalen ao mit offener Nennung

hl:

in:

q: In einem Haushalt fallen täglich eine Reihe von Aufgaben an, die es zu bewältigen gilt. Dabei kann eine Aufgabenteilung ausgesprochen effizient sein. Wenn Sie an Ihre Partnerschaft denken: Wer trägt in welchem Ausmaß zu den folgenden Bereichen im Haushalt bei?

is: \*\*Bitte summieren Sie jeweils die ++Spaltenprozente++ auf 100 Prozent.

it1: (_p): Partner*in

it2: (_i): ich selbst

it3: (_a): andere Personen

st:

ao1 (atakhh): Hausarbeit: 3, Suffix: %

ao2 (atakee): Erwerbseinkommen: 3, Suffix: %

ao3 (atakwe): Treffen wichtiger Entscheidungen: 3, Suffix: %

ao4 (atakkb): Kinderbetreuung: 3, Suffix: %

mv:

ka:

vc:

SHOW vn4 if dkinja=2

av:

kh:

fv:

hv:

fo:

tr:

GOTO B1_4b

hi:

\--------------------------------
B1_4b
==

tc: IF wohnpar=1

vn1: atakzufr

qt: Einfachauswahl

hl:

in: 

q: Alles in allem: Wie zufrieden sind Sie insgesamt mit der derzeitigen Arbeitsteilung zwischen Ihnen und Ihrem/Ihrer Partner*in in Ihrem Haushalt?

is: 

it: 

st:

ao1: 1: gar nicht zufrieden 

ao2: 2: 2

ao3: 3: 3

ao4: 4: 4

ao5: 5: sehr zufrieden

mv: 

ka: 

vc: 

av: 

kh: 

fv: 

hv:  

fo: 

tr: GOTO B1_6

hi:  


\--------------------------------

B1_5
==

tc: IF wohnpar ! 1

vn: atihh; atiee; atiwe; atikb


qt: Einfachauswahlmatrix

hl: 

in: 

q:  In einem Haushalt fallen täglich eine Reihe von Aufgaben an, die es zu bewältigen gilt. Dabei kann eine klare Aufgabenteilung ausgesprochen effizient sein. Unabhängig davon, ob Sie aktuell in einer Partnerschaft leben: Bitte geben Sie an, wer Ihrer Meinung nach für die folgenden Haushaltsbereiche ++idealerweise++  zuständig sein sollte.

is: 

it1: (atihh): Hausarbeit

it2: (atiee): Erwerbseinkommen

it3: (atiwe): Treffen wichtiger Entscheidungen

it4: (atikb): Kinderbetreuung

st:

ao1: 1: ausschließlich mein*e Partner*in

ao2: 2: eher mein*e Partner*in

ao3: 3: wir beide gleichermaßen

ao4: 4: eher ich

ao5: 5: ausschließlich ich

mv: 

ka: 

vc: 

av: 

kh: 

fv: 

hv: 

fo: 

tr: GOTO B1_6

hi: 


\--------------------------------

B1_6
==

tc: IF wohnpar=1

vn: athhm_m/_v/_i/_a; ateem_m/_v/_i/_a; atwem_m/_v/_i/_a; atkbm_m/_v/_i/_a; atkam_m/_v/_i/_a;

qt: Mehrfachauswahlmatrix mit horizontalen ao mit offener Nennung

hl:

in:

q: Wenn Sie nun an Ihre Kindheit denken: Wer hat in Ihrer Familie in welchem Ausmaß
zu unterschiedlichen Bereichen im Haushalt beigetragen?

is: \*\*Bitte summieren Sie jeweils die ++Spaltenprozente++ auf 100 Prozent.
Sollten Sie keine (Stief-)Mutter und/oder keinen (Stief-)Vater haben, kreuzen
Sie bitte entsprechend „trifft nicht zu“ an.\*\*

it1: (_m): (Stief-)Mutter

it2: (_v): (Stief-)Vater

it3: (_i): ich selbst

it4: (_a): andere Personen

st:

ao1 (athh): Hausarbeit: 3, Suffix: %

ao2 (atee): Erwerbseinkommen: 3, Suffix: %

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

GOTO B1_7

hi:

\--------------------------------

B1_7
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

GOTO B1_8

hi:

\--------------------------------

B1_8
==

tc:

vn: promgroßv; promgroßm; promvat; prommut; prombrud; promschw; promtan; promonk; promcoin; promcoine

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

GOTO B1_9

hi:


\--------------------------------

B1_9
==

tc:

vn: pflegang; pflegango

qt: Einfachauswahl mit vertikalen ao

hl:

in:

q: Pflegen Sie regelmäßig pflegebedürftige Verwandte oder Freunde?

is:

it:

st:

ao1: 1: Nein
ao2: 2: Ja, und zwar: ___ Personen

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr:

GOTO B1_10 IF pflegang=2
ELSE nächstes Modul

hi:



\--------------------------------

B1_10
==

tc:

vn: pflegt (pflegt1; pflegt2; pflegt3; pflegt4; pflegt5; pflegt5o)

qt: Einfachauswahlmatrix

hl:

in:

q: Wenn Sie an eine typische Woche denken: Wie häufig führen Sie folgende Pflegetätigkeiten aus?

is:

it1: (pflegt1): Besorgungen und Erledigungen außer Haus

it2: (pflegt2): Haushaltsführung, Versorgung mit Mahlzeiten und Getränken

it3: (pflegt3): Einfachere Pflegetätigkeiten, z.B. Hilfe beim An- und Auskleiden,
Waschen, Kämmen und Rasieren

it4: (pflegt4): schwierigere Pflegetätigkeiten, z.B. Hilfe beim Umbetten,
Stuhlgang usw.

it5: (pflegt5; pflegt5o): Etwas anderes und zwar: ___ [offene Angabe, 50 Zeichen]

st:

ao1: 1: überhaupt nicht

ao2: 2 

ao3: 3 

ao4: 4 

ao5: 5: sehr häufig

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

hi:
