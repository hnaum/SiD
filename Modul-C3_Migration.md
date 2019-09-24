\--------------------------------

1
=

tc: IF dkinja = 2

vn: daltein

qt: offene Frage

hl:

in:

q: Wie alt waren Sie als Sie nach Deutschland gekommen sind?

is:

it:

st:

ao: 2; 1-99; Präfix: Alter:; Suffix: Jahre

mv:

ka:

vc:

av: number: \<= zweistellig : 1 TO 99

kh:

fv:

hv:

fo:

tr: GOTO 2

hi:

\--------------------------------

2
=

tc: Die vorliegende Frage wird ausschließlich dt./BI-Studierenden gestellt, die
im Ausland geboren sind. Internationale Studierende bekommen diese Frage nicht.

vn: dnat (dnatm/ dnatv)

qt: Einfachauswahl, Comparison

hl:

in:

q: Welche Staatsangehörigkeit hat Ihre Mutter bzw. Ihr Vater?

is:

it1: (dnatm): Mutter

it2: (dnatv): Vater

st:

ao1: 1: : die deutsche Staatsangehörigkeit

ao2: 2: : die deutsche und eine andere Staatsangehörigkeit

ao3: 3: : eine andere Staatsangehörigkeit

ao4: -12: : weiß ich nicht

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO 2

hi:

\--------------------------------

3
=

tc: Die vorliegende Frage wird ausschließlich dt./BI-Studierenden gestellt, die
im Ausland geboren sind. Internationale Studierende bekommen diese Frage nicht.

vn: dsprelt

qt: Einfachauswahl

hl:

in:

q: Welche Sprache wird in Ihrem Elternhaus normalerweise gesprochen?

is:

it:

st:

ao1: 1: : Deutsch

ao2: 2: : Deutsch und eine andere Sprache

ao3: 3: : eine andere Sprache

mv:

ka:

vc:

av:

kh:

fv:

hv:

fo:

tr: GOTO nächstes Modul

hi:
