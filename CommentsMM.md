# Comments MM 22 Mei

_Dit ziet er al heel goed uit. Ga zo door, en maak er echt wat moois van. De grote lijn staat goed. Je vragen geven je steun bij het schrijven en de lezer bij het lezen.
Zorg nu vooral dat je dingen precies opschrijft, en niet half-half. Dat laatste lijkt me je valkuil._

 
## Intro
* zet een spatie voor je \cite commando, en zet het in de zin (dus niet na de punt)
* ~_een andere politiek stelsel _ ander stelsel~
* 43-48 Je blijft wel heel erg abstract. Zo zegt dit maar weinig. Dus maak het concreet waar je kunt. Laat eens zien welke  verschillende stelsels en hoe dat van invloed is op de resultaten. Twee keer _daarnaast_ is best leleijk. l47, vreemd, je zegt sommige onderzoeken, maar refereert dan maar naar 1. Wat is het nou (1 of meerdere)?
* 37-42 Mooi, maar te abstract. Leg maar uit hoe dat dan werkt. Dus dat je een classifier leert die op basis van de woorden in een tekst voorspelt wat de ideologische positie van het stuk is.  Dus besteed wat zinnen aan _tekst-classificatie_. En dat je dat dus kunt leren op basis van Handelingen, met daarbij natuurlijk wel de sterke aanname dat de ideologisch epositie van een spreker van een partij in al zijn toespraken doorschemert en dat je blijkbaar op basis van al die toespraken een profiel van een partij of ideologie kunt opbouwen.
* de _dus_ in 53 zie ik nog niet. Deze vraag behoeft echt een veel uitgebreidere intro, namelijk dat werk van Hirst waarin hij laat zien hoe vertekenend dingen kunnen zijn.
* RQ 4: wat bedoel je met "afhankelijk"? Ik lees dit bijvoorbeeld dat de precision/recall voor een partij varieert met het links/rechts spectrum. Kan je concreet maken wat je bedoelt? Bijvoorbeeld, zijn (teksten van) linkse partijen makkelijker te herkenenn dan die van rechtse? 
* Ik stel voor dat je per deelvraag in 4-5 zinnen vertelt wat je gata doen, en hem dus ook wat meer concreet maakt. Voor vraag 1 kan je dan de methoden noemen die je gaat bekijken, waar op je evalueert (precisie/recall/F1), en wat de hoofdresultaten zijn (iets als _de beste classifier is Methode X met een F1 score van YYY, en F1 scores per partij varierend van AAA (voor partij a) tot BBB (partij b)_ ) Voor de overige vragen ook. **Maak het dus allemaal wat inzichtelijker, en geef de lezer alvast een idee wat zij te lezen krijgt**
* ~"Overzhct" Dit hoeft niet allemaal in de toekomende tijd. Je kunt ook iets zeggen als "Sectie 5 bevat dede evaluatie van ...."~


## Methodologie

### Data

1. ~Kijk eens op <https://nl.wikipedia.org/wiki/Spreekbeurt> Ik denk dat _debatbijdrage_ een betere term is. ~
2. 165-166 maak het concreet, wat voor soorten _spreekbeureten_ heb je dan? Heoveel waardes zijn er van elke kolom? Hoeveel rijen zijn er. Nu kan je meteen wat leuke weetje geven. 
3. ~In de volgende zinnen geef je die wel, maar op een rare manier met steeds _zoals_ wat voor mij lijkt dat je een paar voorbeelden geeft maar dat er nog meer is (wat volgensmij niet zo is, maar wees dus heel concreet en volledig).~
4. ~Die _speeches, interrupties en antwoorden_ zijn niet helder (en mede door jou gedefinieerd), dus die moet je hier heel precies definieren.~
5. l171 ~Nu heeft iemand dus meerdere _spreekbeurten_, want jij hebt het over de eerste. Maar wat is dan een _speech_? Het is een warboel van termen.~
6. ~l172 _vaak langer zijn_ Laat maar zien met een leuk grafiekje. En geef wat cijfers.~
7. ~Zoals besproken geeft Tabel 1 aanleiding tot vragen. Vooral snap ik niet hoe de aantallen zo kunnen verschillen. Dus bespreek dit.  Ik zou ook aangeven hoeveel debatten/topics/files je hebt waarin ook echt wordt gesproken door minstens 1 iemand van een partij. Dat is dan de bovengrens lijkt het.  Misschien is dit ook een leuke (pandas ) query en plot: Voor elk aantal partijen aanwezig bij een debat, geef aan hoeveel debatten er van dat type zijn. ~
8. ~Ik zou Table 1 omgekeerd op aantal ordenen.~


### Methoden 

1. ~l192 gooi er maar uit, ik hou niet van die "tijd" argumenten~
2. ~l198 `\w+` moet dit zijn, maar die houdt veel meer over dan alleen de letters.~
3. ~l214 leg uit wat n-grammen zijn, en hoe dat dan werkt in je classifier. En waarom je eigenlijk bigrammen erbij zou nemen (je hebt de delen waaruit een bigram bestaat toch al?)~
4. ~l219 _duurt 219 dit te lang met een gridsearch_ Huh,wat is _dit_? Leg uit wat je hier bedoelt.~
5. ~l232 Bernoulli distributie betekent toch gewoon dat je de "set of words" interopretatie neemt, en multinomial dat je bag of words gebruikt? Ik zou dit weglaten.~
6. l240 Excuus, maar ik geloof dat ik niet weet wat een correct positief waarde is in jouw geval. Dat is toch helemaal niet evident? Je moet het echt beter uitleggen.
7. l245/246, _gewogen bij_ ??? Dit is erg induidelijk. Behandel macro en micro precisie en reccall, etc, en beschrijf precies wat wat is. Je kunt hier rsutig wat meer de tijd voor nemen. Het is echt leuk als dit deel ook begrijpelijk is voor een niet-expert. Nu is het geen vlees noch vis, voor niemand waardevol eigenlijk. Hfd 8 van <https://nlp.stanford.edu/IR-book/information-retrieval-book.html> legt het heel goed uit. Kijk ook naar tabel 13.8 en het stukje over macro en micro averaging. 
8. **3.2.2** Goed, maar je zou toch ook het contrapositief doen, met juist alleen de namen van de partijen en partijleden. 
9. ~Je moet hier ook wel even vertellen _hoe_ je die namen op het spoor bent gekomen, en hoe goed dit werkte (doe dus een kleine steekproef met de hand).~
10. ~l269 _dit_ experiment~
11. **3.2.3** ~Ik zou _zittingsperiode_ gebruiken in plaats van _parlement_ in dit stukje. ~
12. ~Ik zou eerst de 2 experimenten behandlen en daarna jouw precieze data vertellen.~
13. ~Voor dit experiment is het volgens mij van belang dat je de partijnamen weglaat. Hoe doe je dit? Kan je ook aangeven waarom dit belangrijk is? En doet Hirst dat ook?~
14. l292 _beste model_
15. **3.2.4** ~Leuk! De ordening in de tabel is raar: ik denk dat je die van de rechtste partijen wilt omdraaien, zodat ht toch ongeveer linear is op links-rechts.~
16. Het is niet toegestaan een paragraaf te eindigen met een tabel of vergelijking. Dus plaatstabel 2 dan bovenaan de pagina, of doe iets anders.

## Algemeen

* Zorg dat je referenties tiptop in orde zijn.
