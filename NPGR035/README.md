# Poznámky k NPGR035
1. ## Popíšte SVM a postup jeho trénovania. Čo je to kernel a na čo slúži pri SVM?


Support Vector Machine (SVM) je algoritmus strojového učenia, ktorý používa matematické metódy na vytváranie modelov diskrétnych ľudí alebo objektov, ktoré sa líšia vo svojich vlastnostiach alebo atribútoch.

Postup tréningu SVM je nasledujúci: 

1. Voľba modelu: Identifikujte typ SVM, ktorý bude použitý pre trénovanie. Typom SVM sú lineárny, nonlineárny a polynomický SVM.

2. Príprava údajov: Uistite sa, že všetky vstupné údaje sú vhodne upravené pre učenie SVM. 

3. Zvolte hodnotu zmrazenia: Najprv je potrebné zvoliť hodnotu zmrazenia pre SVM. 

4. Volba parametra jadra: Toto je nastavenie v SVM, ktoré určuje typ častice jadra použitého pre trénovanie modelu. 

5. Trénovanie modelu: Použite vybratý SVM a vybrané parametre jadra na trénovanie modelu. 

Kernel je algoritmus, ktorý SVM používa na analyzovanie a klasifikovanie údajov. Kernel je funkcia, ktorá transformuje údaje do druhého priestoru prostredníctvom výpočtu rozdielov medzi údajmi. Tento proces je zvonka zameraný na zlepšenie kvalitatívnych výsledkov klasifikácie. Kernel transformuje údaje do lepšie defined priestoru, v ktorom sú ľahšie odhadnuté hranice medzi rôznymi skupinami údajov, trénovanie a výpočet týchto štrukturálnych hraníc je potom oveľa jednoduchší.

2. ## Popíšte dopredné neurónové siete so spätným šírením chyby a postup ich trénovania. 


Dopredné neurónové siete (FNN) so spätným šírením chyby (backpropagation) sú počítačové algoritmy, ktoré používajú naštruktúrovanú sieť neurónov na odhadovanie funkcie. FNN so spätným šírením chyby sa skladá z vstupnej vrstvy, n-skrytých vrstiev a výstupnej vrstvy. Každá vrstva neurónov obsahuje určité množstvo neurónov, a každý neurón je spojený s vstupmi a výstupmi. 

Postup trénovania FNN s backpropagation zahŕňa niekoľko krokov, ako je napríklad inicializovanie váh pre sieť, forvardové šírenie signálu, kalkulácia chyby a spätné šírenie chyby. 

Na začiatku inicializácie váh by sa mohli inicializovať na náhodné hodnoty v určitom rozsahu. 

Potom sa signál pošle forvard, čo znamená, že signál prechádza cez každú vrstvu a užívateľom definujú výpočet ako polohu a váhu použitu na výpočet výstupu z jednotlivých neurónov. 

Kalkulácia chyby bude vykonaná tak, že rôzne vstupné dáta budú mať správne vystupy a výstup siete bude porovnávaný s oprávnenými výstupmi. Chyba je potom vypočítaná ako rozdiel medzi očakávanými výstupmi a výstupmi vykázanými sieťou. 

Spätné šírenie chyby sa potom vykoná tak, že na základe učiacej stratégie bude chyba prekladaná späť cez sieť na každú vrstvu a váhy budú upravované v súlade s cyklom učenia. Tento postup bude opakovaný dovtedy, kým celková chyba v sieti nebude dostatočne nízka alebo dosiahne minimálny stav. 

Takže, to sú hlavné kroky trénovania FNN s backpropagation.

3. ## Popíšte samoorganizujúce sa mapy a postup ich trénovania.


Samoorganizujúce sa mapy sú veľmi flexibilnými neurónovými sieťami, ktoré dokážu naučiť sa samostatne utriediť neskončný počet vzájomne prepojených neurónov do topológie, ktorá najlepšie vyhovuje spracovávanej úlohe.  Ich trénovanie sa uskutočňuje pomocou učenia sietí bez supervízie, čo znamená, že vstupné údaje a výstupné údaje v zásade neobsahujú žiadne cieľové štruktúry.  Učenie sa prebieha tým, že sa neurón mapuje na vzájomne prepojené vrstvy, takže sa výstupné neuróny v jednej vrstve stanú vstupnými neurónmi pre druhú vrstvu. Učenie sa môže vykonávať buď interaktívnym alebo adaptívnym spôsobom.  Prvý z nich zahŕňa ručné upravovanie topológie medzi vrstvami v procese trénovania, zatiaľ čo druhé zahŕňa automatické upravovanie prepojení medzi vrstvami na základe odpovedí neuronovej siete.  V oboch prípadoch sú doplnkové funkcie učenia, ako napríklad váha a Reinforcement learning, potrebné, aby sa mapa dosiahla čo najlepší výsledok.

4. ## Popíšte lineárny klasifikátor a postup jeho trénovania.


Lineárny klasifikátor je strojové učenie algoritmus, ktorý sa používa na klasifikáciu vstupných údajov do dvoch alebo viacerých tried. Je postavený na lineárnej úlohe triedenia, v ktorej je hlavnou myšlienkou nájsť ideálny rozdelovací bod pre dáta. Lineárny klasifikátor sa často používa na vypočítanie binary weighted values pre každú vstupnú premennu a potom odhadnúť, či je vstup skôr triedou 1, alebo triedou 0.

Kroky pre trénovanie lineárneho klasifikátora: 


1. Načítanie trénovacích dát: Na začiatok je potrebné načítať dáta, ktoré chceme použiť na trénovanie.

2. Inicializujte váhu: Zvolením hodnôt váh pomáha algoritmu efektívne pracovať.

3. Vypočítajte lineárny predikčný model: Vypočítajte lineárny predikčný model pomocou predvolených váh.

4. Vypočítajte pravděpodobnosti predikcie: Na základe lineárneho predikčného modelu vypočítajte pravdepodobnosť predikcie pre konkrétny vstup.

5. Aktualizujte váhu a opravte chyby: Ak je chyba medzi skutočným výsledkom a lineárnym predikčným modelom, aktualizujte váhu a opravte chybu.

6. Opakujte kroky 3 až 5, kým nedočkáte optimálnych váh pre algoritmus: Data nie sú nikdy dokonale izolované pre trénovanie algoritmu. Preto je potrebné opakovane trénovať algoritmus s novou sadou vstupných dát a váh, až kým sa nedosiahne optimálne riešenie.


5. ## Popíšte K-means algoritmus, voľbu K a možné alternatívy.


K-means algoritmus je populárny algoritmus pre clusterovanie, ktorý sa používa na nájdenie skupín položiek s podobnými atribútmi a ktorý patrí medzi najpoužívanejšie metódy pre skupinovanie. Ide o iteratívny algoritmus, ktorý spočíva v často opakovanom hľadaní najvhodnejších centrálnych (stredových) bodov pre každú skupinu dát. Každý bod z dát je potom zaradený do skupiny s centrálnym bodom, ktorý je najbližšie.
Voľba K je počet skupín, ktoré algoritmus vytvorí. K je parameter definovaný užívateľom avšak ideálna hodnota K nie je jednoznačne určiteľná prekaždý dátový set a musí sa nájsť testovaním a experimentovaním s rôznymi hodnotami K.
Alternatívou ku K-means algoritmu je napríklad algoritmus hierarchickej clusteringovej analýzy. Tento algoritmus vytvára clustery tvorbou hierarchie clustrov s použitím porovnávania blízkych objektov v rôznych clusteroch.

6. ## Popíšte detailne metódu FLDA.


FLDA (Fisher Linear Discriminant Analysis) je metóda klasifikácie predstavujúca jeden z implicitných lineárnych techník. Hlavnou myšlienkou FLDA je nájsť rovnicu, ktorá bude dokonale oddeľovať vyšetrované triedy, používajúc zároveň čo najlepšie ohraničené meteria.

Princíp FLDA je v skutočnosti ľahko vyjadriteľný. Ide o to, aby sa našla funkcia, ktorá bude maximálne rozlíšiť údajové triedy pri dosiahnutí najlepšej možnej ohraničenosti v priestore. Ak je v skutočnosti FLDA implementovaná s viac klasami ako dvoma, potom tu existuje obmedzenie, ktoré vyžaduje, aby bola imaginárna hranica počas uprednostnenia funkčnosti rovnomerne distribuovaná medzi klasami.

Na začiatku FLDA je potrebné nájsť modellineárneho delenia priestoru. Jednoducho povedané, lineárna funkcia je f (x)= ax, kde a je vektor pozície, ktorý môže byť zvolený na základe vlastností dátovej množiny.

Po nájdení lineárnej rovnice, je potrebné určiť, ako to môže byť vhodne premietnuté do a charakterizovať vonkajší priestor. Toto je dosiahnuté tým, že sa analyzuje schopnosť každej premenu spaľovať rozdiely medzi rôznymi triedami, vyhodnocuje odchýlka každej transformácie od miery dôvery schopnej použiť jednotlivé transformačné vývoje.

Na záver je potrebné určiť, či je modelová transformácia úplne prijateľná. Prístup je uskutočnený funkciou F-stupňa, ktorá uvažuje premenu klasifikačného priestoru, koeficienta korelácie medzi rôznymi triedami atď. Ak sa modelová funkcia vyčísli ako úplne uspokojivá, znamená to, že bola nájdená najlepšia možná transformácia tried z núdzového priestoru do priestoru izolovaného. Tím sa dosiahne najlepší lineárny klasifikačný model produkovaný FLDA.

7. ## Popíšte detailne metódu ICA.


ICA (independent component analysis) je neparametrický analytický nástroj používaný na analýzu a extrakci čistých signálov z viacnásobných pozorovaní. Idea pozadu tkvie v tom, že mocnosti signálov súdobých v nezávislých komponentoch sú niečím iným než známe zložky systému. Napríklad ak máme mnoho ľudí sledujúcich rôzne signály, ktoré sú nesúvislé a nezávislé na sebe, môžeme z nich extrahovať čisté signály ICA. 

ICA je postavená na viacerých prístupoch počítačovej technológie a matematických techník porovnávania signálov. Všeobecne platí, že ICA spočíva v hľadaní nezávislých komponentov v dátach súčasne tým, že porovnáva vstupné signály. 

Čistenie dát pre ICA sa realizuje ako transformácia korelácie, ktorá prevedie maticu konštantných (zrazených) čísel na maticu nulovej korelácie (nezrazenú). Ideálna korelačná matrica má všetky jednotlivé vstupné signály s nulovou koreláciou, čo znamená, že sú úplne nezávislé. Toto korelačné čistenie je dôležitou prípravou pred samotnou analýzou ICA. 

Keď sú dáta pripravené, môžu byť rozdelené na zhluky nesúvislých signálov, matica rozložená a vizualizovaná. ICA používa postupné skenovanie na odstránenie nepotrebných častí signálu a extrakciu čistého signálu, ktorý sa potom môže transformovať na príjemnejšiu formu a lepšie pochopenie výsledkov.

8. ## Popíšte detailne metódu k najbližších susedov.


Metóda k najbližších susedov (angl. k-nearest neighbor, KNN) je veľmi jednoduchá klasifikačná metóda, ktorá sa často používa ako vstup pre viacročné systémy umelej inteligencie. Je to klasifikátor, ktorý sa rozhoduje na základe najbližších susedov, ktorí boli predtým pozorovaní.

Je to triedenie založené na princípu "Ľudia, ktorí sú si podobní, majú podobné vlastnosti". V ideálnom prípade metóda k najbližších susedov založená na euklidovskej vzdialenosti (angl. Euclidean distance) somarizuje podobnosti medzi vstupom a predviďanými výstupmi. Teraz, aby sa predikcia mohla vykonať, vytvárajú sa tzv. najbližší susedia. 

Najbližší susedia (angl. nearest neighbor) sú datové body v danom priestore, ktoré majú najbližšiu euklidovskú vzdialenosť voči testovaciemu bodu. Na základe týchto najbližších susedov potom modely určia predikciu. 

KNN je relatívne jednoduchá metóda, ktorá sa používa pre klasifikáciu objektov do základných tried alebo umožňuje vytváranie regresných analýz, čo umožňuje modelom určiť najbližšie susedov. Sú to úzko používané metriky pre strojové učenie a sú používané na extrapoláciu informácií z ich pôvodného datasetu. 

Metóda KNN odhaduje klasifikáciu nových objektov na základe klasifikácie predtým uvedených. Vyžaduje si určité počítanie, ktoré je vykonané na začiatku, keď sa účastník zaregistruje do databázy. Metóda KNN používa euklidovskú vzdialenosť ako metriku predikcie, čo je vzdialenosť medzi najbližšími susedmi. 

V procese KNN sa v skutočnosti vykoná nasledujúci postup: Najprv je potrebné vybrať si konkrétny počet susedov, ktorých sa chcete pozrieť (modelová parameter nazývaný "K"). Vybraní susedia sa skontrolujú a spoznajú sa s nimi. Všetky údaje o najlepších susedoch sú potom sčítavané a na základe toho sa vykoná predikcia.

9. ## Aký je rozdiel medzi dvomi základnými prístupmi k znižovaniu dimenzie (wrapper a filter), aké hodnotiace miery sa pri nich používajú?


Rozdiel medzi dvoma základnými prístupmi k znižovaniu dimenzie je v tom, ako sa vykonáva samotný proces selekcie atribútov. Filter používa rôzne stupne hodnotenia (ako je vzdialenosť alebo nezávislé testovanie) na identifikáciu atribútov, ktoré majú najvyššiu koreláciu alebo najväčší vplyv na predikčné výsledky. Na druhej strane wrapper sa používa na funkčné usporiadanie k kombinácii atribútov, ktoré preukážu najlepšie predikčné výsledky pre dáta. Hodnotiace miery sa pri oboch prístupoch používajú na nameranie úspešnosti procesu. Pri filtre sa využíva váha výstupu, podobnosť, informačná entropia alebo hodnota odstránenia nezávislých atribútov. Pri wrappe sa skôr využíva krížová validácia alebo kritérium šikmých stien.

10. ## Aký je rozdiel medzi dvomi základnými prístupmi k znižovaniu dimenzie (wrapper a filter), aké postupy sa používajú pri výbere príznakov?


Rozdiel medzi dvoma základnými prístupmi k znižovaniu dimenzie (wrapper a filter) spočíva v tom, že pri wrap-metóde sa využíva výstup modelu predikcie ako kritérium pre výber príznakov, zatiaľ čo pri filtrovacej metóde je výstup predikcie vynechaný zo vzorky a preskúmavané je len štatistické skóre. 

Metóda filteru zahŕňa zhromažďovanie štatistických údajov o príznakoch a ich závislosti od cieľovej premenné, čo sa uskutočňuje pomocou rôznych vyhodnotení ako napríklad meranie korelácie alebo čiastkové prekrývania. Po hodnotení všetkých príznakov sa pri výbere príznakov používajú štatistické a matematické postupy, ako napríklad hodnotenie informácií alebo vytváranie hodnotení vnútorných modelov, ktoré určia, ktoré z pôvodných príznakov by mohli byť odstránené.

Na druhú stranu, metóda wrapperu sa zameriava na dosiahnutie optimálneho výkonu modelu predikcie. Namiesto zhromažďovania štatistických údajov o príznakoch sa využíva algoritmus vyhľadávania, ktorý je najvhodnejší nielen na definovanie kritérií vyhľadávania príznakov, ale tiež na špecifikovanie nejakej vhodnej oblasti vyhľadávania. Tento proces sa nelineárnym spôsobom opakuje, kým sa nedosiahne optimálne riešenie a výstupom sú príznaky, ktoré majú najlepší vplyv na predikčné výsledky.

11. ## Popíšte detailne metódu PCA. Aký je rozdiel medzi PCA a ICA?


Princípnej analytická predstavuje činnosť, ktorá je zameraná na identifikáciu dôležitých vzťahov v dátach a transformáciu ich do pozorovaní, ktoré sú lineárne nezávislé.

PCA sa snaží nájsť nezávislé významné rysové vlastnosti v dátach. Jej cieľom je redukovať dimenzionalitu dát. Ak chcete odstrániť redundancie v dátach, dátový prístup sa často vyžaduje. PCA to okrem toho robí aj analýzou korelácie a závislosti medzi pozorovaniami v komplexnom dátovom priestore.

PCA transformuje dáta na množinu vektorov, ktoré majú najväčšiu vzájomnú variabilitu a minimálnu koreláciu. Musíte mať na pamäti, že lepšie výsledky sa dajú dosiahnuť iba vtedy, ak skutočne uvedieme pripravené dáta. Tento proces sa môže robiť iba na dátach jednej úrovne, pretože lineárny model ani jeho extrapolácie spoločne decimujú hybridné dáta, čo môže narušiť jeho účinnosť.

PCA sa používa na zoskupovanie dát, ktoré sa líšia v reprezentácii, merania alebo dimenzie. Dve hlavné vlastnosti PCA sú redukcia dimenzionality a interpretácia dát.

Rozdiel medzi PCA a ICA je v tom, že PCA hľadá vzájomne nezávislé pozorovania (nehybridné pozorovania), ktoré majú najväčšiu variabilitu, zatiaľ čo ICA hľadá skupinu pozorovania (hybridné pozorovania), ktoré sú vzájomne subsystémové. PCA je nástroj na zníženie rozmernosti zameraný na zníženie rozmernosti. Zatiaľ čo ICA je nástroj, ktorý sa používa na detekciu distinctiveness pozorovaní.

12. ## Popíšte detailne metódu PCA. Akým spôsobom ju používame pri znížení dimenzie?


Princíp komponentovej analýzy (PCA) je založený na transformovaní zvoleného množstva premenlivých do novej multidimenzionálnej sústavy premenlivých. Cieľom tohto transformovania je identifikácia nových dimenzií s maximálnou variabilitou daných dát a jeho zjednodušenie na menej počet dimenzií. PCA pozostáva z linearnej transformácie dát do nového priestoru pre samé premenlivé. V novom priestore nájdeme nové premenlivé (zväčša kombinácie jednotlivých premenlivých). Tieto nové premenlivé sa nazývajú komponenty.

V každom komponentovi sa nachádzajú informácie o variancii dát. Táto variancia sa môže posudzovať použitím metriky ako je napríklad zrýchlenie. Cieľom PCA je dostať sa k setu komponentov, ktoré zahrňujú čo najviac informácií o variancii v dátach.

PCA sa často používa na zníženie dimenzie. V tomto prípade je cieľom dosiahnuť najväčšiu možnú variabilitu v dátach, pričom sa pri tom zachováva čo najmenší počet premenných. PCA teda vytvára nové komponenty s najvyššou variabilitou v priestore maticovej prevodovky prvkov obrazu. Po izolovaní komponentov sa potom vyberajú tie s najvyššou variabilitou a zvyšné sa odstránia. Tento proces zvyčajne prispieva k zníženiu počtu zložiek dátového priestoru a môže pomôcť zjednodušiť analýzu dát.

13. ## Popíšte detailne metódu PCA. Akým spôsobom určujeme počet významých vlastných vektorov?


Princípmi hlavných komponent (PCA) je metóda transformácie dát. Prístup je založený na znížení dimenzionality pre zostavenie vlastných vektorov pre dátový vzorec (dataset). 
Tento prístup je obzvlášť užitočný pre dátové množiny s vysokou dimenziou alebo pre dáta s pozdišťujúcimi atribútmi. 
PCA je realizované tak, že je pripočítaná korelačná matica pre dátový vzorec, ako vstup pre analytický proces založený na nájdení vlastných vektorov a vlastných hodnôt pre daný trojuholníkovitý maticový vstup. 
Vlastné vektory a vlastné hodnoty sú vyčlenené ako produkty z eigenvalue/eigen vector problémového vstupu.
Vlastné hodnoty identifikujú mieru významu danej komponenty (prvku) pre daný súbor údajov.
Vlastné vektory charakterizujú kombináciu vstupných prvkov, ktoré potom môžu byť použité ako nový tvorba nových atribútov pre dátový vzorec. 

Hlavný prístup pre PCA je zahrnutý s odfiltrovaním obeťov pre rozličné počty významných vlastných vektorov. Ak chcete určiť počet významných vektorov, ktoré potrebujete, môžete používať niekoľko metodologických postupov:

• Screening - zahŕňa kroky pre úplné prehliadanie komponentov. Tento prístup rýchlo čistí extrémne malé vlastné hodnoty a bez štatistickej interpretácie odstráni tieto komponenty.
• Posthoc hypothesis testovanie - vychádza zo štatistickej úvahy, ktorej cieľom je odstránenie tých komponentov, ktoré nie sú štatisticky nápadné ako zásadné pre zostavenie dátového vzorca.
• Elbow metóda - používa prístup chamtivosti s cieľom nájdenia optimálneho počtu postaficky komponentov. Uvažovanie sa zameriava na sumu vlastných hodnôt pre dátový vzorec.

14. ## Popíšte detailne trénovanie Bayesovho klasifikátora. Čo vieme o chybe tohto klasifikátora?


Bayesov klasifikátor je jedným z najbežnejších klasifikačných algoritmov, ktorý je založený na teórii Bayesovho vyjadrenia pravdepodobnosti. Algoritmus sa zameriava na nájdenie pravdepodobnosti (pravdepodobnosti) vzhľadom na konkrétny stav.

Ako trénovať Bayesov klasifikátor?

1. Načítajte a analyzujte príklady trénovacích dát. Čím viac príkladov poskytnete klasifikátoru, tým lepšie bude pracovať.

2. Oboznámte sa s dostupnou sadou atribútov. Uistite sa, že klasifikátor je schopný pracovať s dostupnými atribútmi trénovacích príkladov.

3. Vytvorte model na klasifikáciu. Model môže obsahovať rozhodovací strom alebo jednoduché rovnice posudzovania pravdepodobnosti. Model môže byť tiež zložitejší napr. model neuronovej siete.

4. Odhadnite pravdepodobnosti. Po modelovaní je ďalšou úlohou odhadovať pravdepodobnosti pre všetky uvedené stavy.

5. Učte zvyšok tréningových dát. Po určení modelu a predikčných pravdepodobností je ďalšou úlohou optimalizácia parametrov modelu pomocou trénovacích dát. To môže byť dosiahnuté stohovaním alebo kvantifikáciou.

6. Testujte svoj model. Po trénovaní je posledným krokom testovanie modelu a odhadovanie jeho presnosti.

Chyba Bayesovho klasifikátora tiež závisí od predvídania vzťahov medzi príznakmi v príkladoch trénovacích dát. Algoritmus sa často stretáva s problémami s nadvládou príznakov (niekedy nazývaná moc znakov). Stres s nadvládou znamená, že niektoré príznaky sú príliš silné alebo príliš často prítomné v trénovacích dátach, čo môže spôsobiť prehnané predpoklady v modeli. V takýchto prípadoch môže mať algoritmus vyššiu chybu.

15. ## Popíšte ako sa vytvárajú rozhodovacie stromy.


Rozhodovacie stromy sa vytvárajú postupným zhrnutím údajov a analýzou pravdepodobností. Jedným z kľúčových článkov tohto procesu je postupná hodnotenie každého atribútu v datasete - čím kvalitnejší je atribút, tým výraznejší je jeho vplyv na výsledný rozhodovací strom. Štruktúrovanie ako rozhodovací strom potom je pomocou príslušných algoritmov pre vyhľadávanie v datasete pre objavenie tých, ktoré majú zásadný vplyv na výsledok. Akonáhle je vybratá premostená cesta, skúsia sa vybrať dôležité charakteristiky ako špecifíky, ktoré majú mať vplyv na výsledky. Postupne vzťahy medzi zinými charakteristikami sú mapované do logicky usporiadaných stromov, ktoré sú následne využívané na ďalší výskum alebo na účely vytvorenia modelu. Proces je komplexný a náročný, ale môže priniesť stupňujúce sa účinky pre aplikáciu strojového učenia.

16. ## Popíšte metódy krížovej validácie a metódu bootstrap. Aký je medzi nimi hlavný rozdiel? Na čo slúžia? 


Krížová validácia (CV) je technika, ktorá sa používa na validáciu riešení strojového učenia. Ide o spôsob, ako sa starostlivo overiť, že algoritmus je vhodný pre dáta, ktoré potenciálne môžu mať nekonzistentné alebo skreslené výsledky. Súčasťou krížovej validácie je rozdelenie dátového súboru na kombináciu trénovacích a testovacích dát, ktoré sa postupne menia. Trénovacie dáta sa používajú na vytvorenie modelu a testovacie dáta na overovanie jeho presnosti.

Bootstrap je obzvlášť užitočný nástroj, ktorý sa používa na simuláciu vyhodnocovania presnosti stredných odhadov. Princíp bootstrapu pozostáva zo 100 alebo 1000 alebo viac výberov zo vzorky dát, s presne tým istým počtom elementov v každej vzorke. Každý z výberov je vzorka s opakovaním – všetky z nich obsahujú niektoré údaje viac ako raz. Metóda bootstrapu je potom použitá na výpočet stredných odhadov zo všetkých vzoriek.

Hlavný rozdiel medzi krížovou validáciou a bootstrapom je v tom, že krížová validácia sa používa na validáciu a overovanie existujúceho modelu, zatiaľ čo bootstrap sa používa na výpočet stredných odhadov. Obe techniky sú užitočné pre kontrolu kvality statistických a strojovým učením modelov, napriek tomu, že ich prístup k tomu je odlišný.

17. ## Popíšte detailne konvolučné siete.


Konvolučné siete sú neuronové siete, ktoré používajú konvolučné operácie na analýzu obrazov. Je to neuronová sieť, ktorá používa konvolučnú sieťovinu. Konvolučná sieťovina je zostavená z niekoľkých vrstiev konvolučných blokov, pričom každý blok obsahuje jednu alebo viac konvolučných jadier. Konvolučné jadro je malý rámec, ktorý sa používa na prechádzanie obrázka a prepočítanie výsledných údajov vyjadrených v jadre. Každá konvolučná vrstva je navrhnutá tak, aby zachytená rôznych charakteristík vstupu, ako sú hranice, farebné časti alebo textúry. Konvolučná vrstva používa filtre, aby zmenšili vstupnú veľkosť obrazu; Avšak, filtre takisto smerujú do toho, aby identifikovali úplné kovovej obrazové informácie. Na rozdiel od bežných neuronových sietí, ktoré používajú len ploché vrstvy na extrakciu údajov zo vstupnej mriežky, konvolučné siete používajú konvolučnú sieťovinu, ktorá umožňuje prieteč automaticky detecovať rôzne štruktúry, vzory a farby z obrazu. Konvolučné siete používajú viacvrstvové neuronové siete s lineárnou transformáciou a niektoré alternatívne aktyvácie funkcií, aby sa identifikovali podrobné vzory v obrazoch.

18. ## Popíšte detailne metódy hierarchického zhlukovania.


Metóda hierarchického zhlukovania je typ klasifikačnej techniky, ktorá používa agregačný postup na vytvorenie a opis zhlukov (skupín) objektov s podobnými atribútmi. Existujú dve hlavné metódy hierarchického zhlukovania: aglomeratívny zhlukovací prístup a disociatívny zhlukovací prístup.

Aglomeratívny zhlukovací prístup (alebo dolnejší prístup) začína zhlukom jednotlivých objektov, ktoré postupne postúpia cez hierarchiu vytvorením ďalších a ďalších zhlukov, až kým každý objekt nie je v jednom jedinom zhluku. Každá úroveň v hierarchii tiež využíva métriku pre pomer blízkosti objektov smerom vzhľadom k odhadu veľkosti zhluku, na ktorý smerujú.

Disociatívny zhlukovací prístup (alebo horný prístup) začína s jediným zhlukom, v ktorom je každý objekt, a rozdeľuje ho na čoraz menšie a menšie zhluky. Všetky tieto menšie zhluky vytvárajú spolu odbornú hierarchiu. Ako v prípade aglomeratívneho prístupu, métre blízkosti objektov sa tiež využívajú na identifikáciu skupín, ktoré sa majú oddeliť.

Hlavnou výhodou hierarchického zhlukovania je, že poskytuje užívateľovi lepšie zobrazenie vzťahov, ktoré existujú medzi objektmi a vytvára hierarchickú štruktúru, ktorá môže byť užitočná aj pre ďalšie výskumy. Nevýhodou je, že to nedokáže pracovať s veľkým množstvom objektov a je potrebné príliš veľa času na to, aby sa tieto výpočty uskutočnili.

19. ## Čo je matica zámen, ako sa vytvára? Na čo sa používa?


Matica zmen je tabuľka, ktorá zobrazuje zmeny v údajoch alebo informáciách od jednej podoby do inej. Je to užitočný nástroj pre manažment a analýzu zmien. Matica zmen je užitočná pre definíciu cieľov, identifikovanie zdrojov a plánovanie udržiteľnosti v rámci projektu. Umožňuje lepšie rozumeť vplyvu rôznych faktorov a riešení na postupné dosahovanie cieľov. Matica zmien tiež poskytuje prehľad o stave projektu a je užitočná pre sledovanie a hodnotenie úspešnosti procesu zmeny.

20. ## Čo je ROC krivka, ako sa vytvára? Na čo sa používa? Aké hodnoty z nej vieme zistiť?


ROC (Receiver Operating Characteristic) je grafické znázornenie účinnosti binárneho klasifikátora. Je to technika validácie modelov predikčných systémov. Na osi y sa nachádza úroveň výstupu signálu detektoru a na osi x, úroveň falošného poplachu pre určitú čitateľnosť signálu. Vytvára sa vykresľovaním hodnôt True Positive Rate (TPR) a False Positive Rate (FPR) v závislosti od hrany hodnovej stupnice signálu.

TPR (Úspešnosť detekcie) predstavuje počet pozitívnych detekcií v porovnaní s počtom skutočných pozitívnych prípadov. FPR (Falošný poplach) predstavuje počet falošných poplachov v porovnaní s počtom skutočných negatívnych prípadov.

ROC krivka sa využíva na meranie úspešnosti modelu klasifikácie. Ze situácie ROC možno očakávať, že tím, ktorý dosahuje vysokú úroveň TPR a nízku úroveň FPR, je viac úspešný ako tím s nízkou úrovňou TPR a vysokou úrovňou FPR.

21. ## Aké metódy používame pre voľbu trénovacej a testovacej množiny?


1. Rozdeľovanie na trénovacie a testovacie množiny: Jednou z najčastejšie používaných metód je rozdeliť dátovú množinu na trénovacie a testovacie súbory. Trénovací súbor je použitý na naučenie modelu. Potom testovacia množina je použitá na otestovanie, či model dobre funguje so skutočnými dátami.

2. K-násobné krížové ovútie: K-násobné krížové overenie je viacnásobné rozdelenie dátového súboru na trénovací a testovací súbor. V každom kroku sa rozdelenie trochu zmení, aby bol zabezpečený čo najlepší pomer trénovacích a testovacích dát.

3. Bootstrapping: Bootstrapping je metóda, pri ktorej sa iba jeden trénovací a jeden testovací súbor vyberajú z predchádzajúceho dátového súboru. Opakuje sa tak, aby bol dosiahnutý celkový trénovací a testovací súbor.

4. Holdout: Hold-out metóda je podobná predchádzajúcej metóde bootstrappingu. Rovnako ako pri bootstrappingu, dáta sú opakovanými cyklami oddelené na trénovaciu množinu a testovaciu množinu. Rozdiel spočíva v tom, že každá obsahovať tie isté dáta po konkrétny počet cyklov.


22. ## Aký je rozdiel medzi PCA a ICA?


PCA (Principal Component Analysis) je metóda analýzy priestorových údajov, ktorá spočíva vo vyhľadávaní lineárnych závislostí medzi prvkami údajov. Je to technika starostlivého odhadovania usporiadania údajov, ktorá využíva lineárne kombinácie dát. Tento proces je vykonaný na maximálne využite information prináša aby bolo možné vety vlehši vzťah  pochopiť jasnší a špecifckejší vzťah medzi údajmi.

ICA (Independent Component Analysis) je podobný k PCA pri analýze údajov. Meria viaceré systémy z vyššieho počtu zdrojov pre identifikáciu súhlasu a vyhľadáva nezávislé súčasti v údajoch. Spočíva v tom, že hľadá vyššiu úroveň informácií, ktoré nie sú viditeľné v centerline dát. ICA hlboko zvažuje hľadanie informácií, ktoré sú ukryté v údajoch a je menej invariantná voči prechodnému šumu.

23. ## Aký je rozdiel medzi PCA a LDA?


PCA (Principal Component Analysis) je metóda redukcie dimenzionality založená na kovariančnej matrice medzi atribútmi. PCA sa používa na sníženie dimenzionality stávajúcich atribútov, aby sa dosiahla lepšia interpretácia alebo visualizácia dát a nájdenie súvisiacich atribútov.

LDA (Linear Discriminant Analysis) je druh diskriminačnej analýzy, ktorá sa používa na klasifikáciu založenú na rozdelení atribútov do skupín. LDA meria magické vzťahy medzi atribútmi a skupinami, aby určila, aké atribúty majú najvyšší vplyv na odlíšenie skupín.

24. ## Akými spôsobmi normalizujeme príznaky?


1. Zásadným krokom je potláčanie príznakov užívaním liekov na predpis. Liečba môže zahŕňať užívanie analgetík, antidepresív, stabilizátorov nálady a iných liekov.

2. Odstránenie stresorov a príčin, ktoré spôsobujú príznaky. Pacient by sa mal obmedziť v pracovných oblastiach, ktoré majú spôsobiť napätie a stres.

3. Štrukturovanie dňa a dostatočný spánok je dôležité pre kontrolu príznakov, takže je dôležité, aby pacienti usilovne dodržiavali svoj denný režim a starostlivo riadili svoje spánkové návyky.

4. Pravidelná fyzická aktivita. Mala by sa uprednostniť, pretože to môže zmierniť úzkosť a dve vyššie uvedené skutočnosti môžu prispieť k lepšiemu pocitu pohody.

5. Relaxačné stratégie môžu byť prospešné pri normalizácii príznakov a prislúchajúcemu zlepšeniu pohody. Meditácia, autogénny tréning a joga sú príkladmi relaxačných stratégií, ktorými sa dá disponovať počas dňa.

6. Obmedzenie príjmu alkoholu a drog je dôležité, pretože môžu narušiť náladu aj príznaky.


25. ## Čo je to chybová funkcia klasifikátora? Ako sa odhaduje chyba klasifikátora?


Chybová funkcia klasifikátora je matematický vzorec, ktorým sa meria účinnosť klasifikátora. Snaží sa odhadnúť chyby, ktoré klasifikátor vytvorí. Chyba klasifikátora sa odhaduje použitím komerčných metrík alebo metrík voľne dostupných na internete. Jednou z najčastejšie používaných merícich metrík je priemerná absolútna chyba, ktorá sa počíta pomocou týchto krokov:

1. Získajte určitý počet príkladov na testovanie (napríklad 1000 príkladov).

2. Pre každý príklad použite klasifikátor a určite, či tento príklad bol klasifikovaný správne, alebo nie.

3. Spočítajte počet chybných klasifikácií a vypočítajte ich percentuálnu súčasť.

4. Posúdiť celkovú chybovosť klasifikátora ako súčin dvoch čísel. Prvá čísla je percento chybných klasifikácií a druhá je absolútna hodnota chyby pre každý príklad, ktorý bol klasifikovaný nesprávne.

5. Prídete k priemernému absolútnemu chybovému číslu pre klasifikátor.

Týmto postupom môžete vypočítať chybovosť klasifikátora a posúdiť jeho účinnosť. Ak chcete vidieť výsledky iného meracieho metríka, postup je podobný, ak sa zameriavate na iný typ chyby.

26. ## Na čo slúžia filter a wrapper? Aký je medzi nimi rozdiel?


Filter a wrappery sú príslušenstvo pre aplikácie, ktoré vám umožňujú filtrovať dáta alebo upraviť dáta bez toho, aby ste museli upravovať samotnú aplikáciu. 

Filter slúžia na filtrovanie vstupných alebo výstupných dát. Umožňujú odfiltrovať informácie a odstrániť akékoľvek potenciálne nežiaduce dáta skôr, než sú dáta odoslané alebo spracované. 

Wrappery slúžia ako nadstavba a umožňujú iným knižniciam či nástrojom komunikovať s aplikáciou. Wrappery inštalujú rozhrania medzi dvoma aplikáciami, čo umožňuje ich prepojenie a pohodlnú komunikáciu.

Rozdiel medzi filterom a wrapperom je teda zásadný. Filtery sú primárne určené na filtrovanie dát, zatiaľ čo wrappery sú spôsob, ako prepojiť dva aplikačné rozhrania. Taktiež filtery pracujú s už existujúcimi dátami, zatiaľ čo v prípade wrapperov nie je potrebné existujúce dáta.

27. ## Popíšte klasifikáciu pomocou Bayesovho klasifikátora.


Bayesov klasifikátor je supervízny algoritmus, ktorý je založený na Bayesovej teórii pravdepodobnosti. Jedná sa o používanú techniku predikčného modelovania a klasifikácie. Je to iteratívny proces, ktorý sa zakladá na predstave o tom, ako je pozorovaná údajová množina charakterizovaná rôznymi atribútmi. Predchádza to, že sa urobia predpoklady o tom, akého typu sú dáta, a vygeneruje sa predikčný model. V Jednotlivých krocích sa potom vyhľadávajú priklady učením napodobňujúce scenáre, ktoré je možné jednoznačne klasifikovať. To poskytuje lepšiu perspektívu pre klasifikáciu, ktorá je vystavaná a vyhodnotená na zistených prikladoch. Následne je pomocou Bayesovho klasifikátora module generovaná predikčná funkcia, ktorá určuje pravdepodobnosť pre každú skupinu v závislosti od hodnôt získaných z údajov. Napokon, model je použitý na na skladanie predikcií na určitej množine dát.

28. ## Popíšte klasifikáciu pomocou lineárneho klasifikátora.


Lineárny klasifikátor je algoritmus, ktorý sa používa na klasifikovanie objektov na základe ich vzájomných atribútov. Klasifikácia používajúca lineárny klasifikátor založený na rozbinarizácii je proces, ktorý určuje, či je objekt klasifikovaný ako „patrí“ alebo „nepatrí“ do triedy, podľa jeho vlastností. Tento proces vyžaduje, aby boli atribúty objektu ideálne priradené do jediného stavu, ako napríklad "áno/nie" alebo "červená/niečervená". Ako prvé sú potom triedy preskúmané a pripravené. Potom sa konštruuje lineárny klasifikátor, ktorý porovnáva objekty na základe ich vlastností. Zložitejšie objekty sú vyhodnocované viacerými lineárnymi klasifikátormi a ich vzor je usporiadaný v stave „patrí“ alebo „nepatrí“ pre jednotlivé klasifikácie. Potom sa všetky tie výsledky spoja do výslednej klasifikácie pre každý objekt.

29. ## Popíšte klasifikáciu pomocou rozhodovacích stromov. 


Rozhodovací strom je typ účelového modelu, ktorý slúži na klasifikáciu (a regression). Umožňuje riadiť sa pravidlami a usilovať sa o objektívne a presne rozhodnutia. Model sa skladá z častí ako sú uzly, hrany a listy. Každý uzol reprezentuje atribút alebo pojem, hranu reprezentuje hypotézu vezmúcu do úvahy a listy reprezentujú odpovede.

Rozhodovací strom najprv kladení otázky priradiť hodnoty vybranému atribútu. Táto otázka je následne stanovená pre každú ďalšiu úroveň v rozhodovacom strome. Proces končí, keď sa dostane na list, ktorý predstavuje priradenie klasifikácie alebo predikcie.

30. ## Popíšte metódu SVD. Na čo slúži?


Singulárna väčšinová dekompozícia (SVD) je technika matematickej analýzy, ktorá je založená na rozkladaní matíc do troch matíc. SVD sa používa na riadenie rôznych úloh, ako sú napríklad prevedenie analytických úloh na lineárne, optimálne riešenie systémov, extrakciu informácií z veľkej množiny údajov a predikciu ďalších znakov z existujúcich znakov. SVD slúži na prerozdelenie matice. Rozkladá túto maticu na tromi časti - dva štvorčeky matíc a jednu trojuholníkovú maticu. Môže slúžiť na odhalenie vzorcov v údajoch, ako aj na redukciu dimenzie. Srozumiteľnejšie, SVD je minimálny počet počet opatrovaní, ktoré by mal byť uvedený pre výkonný a spoľahlivý vstupný systém.

31. ## Popíšte miery používané na ohodnotenie príznakov.


1. Podiel: Miera podielu je často používaná v medicíne ako metóda hodnotenia, aby sa posúdil všeobecný predpoklad o výskyte alebo prevalencii príznakov. Jedná sa o percentuálne číslo, ktoré meria pomer pacientov s danej príčiny a celkový počet testovaných pacientov.

2. Odds Ratio: Tento koeficient sa používa na to, aby sa posúdila pravdepodobnosť výskytu príznaku u dvoch skupín ľudí. Je to vyjadrené vo forme násobku pravdepodobnosti, že daná skupina osôb bude trpieť symptomom voči druhej skupine.

3. Rizovo-benefičný pomer (RBP): Tento pomer poskytuje lekárom jedinečný spôsob, ako posúdiť, aké veľké riziko a benefit majú liečby. Popisuje, aké veľké riziko prinesie daná liečba a aký je priemerný prínos pre pacienta vo forme minimalizácie príznakov alebo zlepšenia pomeru pozitívnych výsledkov.

4. Podielové veľkosti: Táto metrika vyjadruje rozdiely medzi vlastnosťami dvoch skupín, ktoré sa porovnávajú. Presná číselná závisí na počte vzoriek a poskytuje obraznú predstavu veľkosti rozdielu.


32. ## Zadefinujte pojmy entropia a vzájomná informácia. Na čo sa používajú pri výbere príznakov?


Entropia je číselný popis informačnej nezávislosti uvedenej skupiny; je to keš nástroja, ktorý sa používa na meranie dispozície muriva dát. Entropia sa používa na zistenie toho, ako sa prípady rozdelia do skupín. Entropia je veľmi dôležitá, pretože umožňuje posúdiť, aké početné a zmiešané sú výsledky. Entropia tiež meria úroveň heterogenity dát, ktoré sú dostupné.

Vzájomná informácia je číselná charakteristika informácií, ktoré dva aspekty alebo objekty sdílajú navzájom. Tieto objekty môžu byť slová, atribúty alebo konkrétne skupiny náhodne vybraných objektov. Je to štatistický indikátor, ktorý sa často používa na určenie korelácie medzi dvomi aspektmi alebo objektmi. Vzájomná informácia je veľmi dôležitá na zistenie, aká silná je korelácia medzi dvomi aspektmi.

Entropia a vzájomná informácia sa často používajú na výber príznakov. Tieto ukazovatele sú užitočné na vybranie príznakov, ktoré identifikujú skupiny alebo sa používajú na zobrazovanie zhlukov. Takéto príznaky sú často vhodné na zváženie, pretože zvyšujú entropiu a zvyšujú vzájomnú informáciu o skupinách a ich časťach. Príznaky, ktoré majú vyššiu entitu a vyššiu vzájomnú informáciu, sú pravdepodobne najlepšou voľbou pri výbere príznakov.

33. ## Zadefinujte pojmy štatistická nezávislosť a konzistencia. Na čo sa používajú pri výbere príznakov?


Štatistická nezávislosť je definovaná ako náhodné vzájomné správanie dvoch alebo viacerých príznakov. Pre štatistickú nezávislosť sa predpokladá, že jeden príznak sám osebe neovplyvňuje druhý príznak.

Konzistencia znamená, že príznaky sú v rešeršovaných vzorkách pre celú skúmanú populáciu konzistentné v čase a prostredí.

Tieto dva koncepty sa používajú na určenie relevantných príznakov pre výskum, vývoj a predikcie. Príznaky by mali mať obojstrannú súvislosť (koreláciu), byť štatisticky nezávislé a mať konzistencie. Z hľadiska výskumu je nevyhnutné, aby boli príznaky relevantné a mali silný vplyv na záver alebo na predikciu.

34. ## Aké metódy zhlukovania poznáme? Uveďte základné delenie a príklady metód.


Zhlukovanie je proces agregácie vízualizovaných objektov podľa určitých vlastností. Podľa toho, aké kritériá by mali byť plnené alebo aký je cieľ zhlukovania, existujú rôzne metódy uskutočňovania. Metódy zhlukovania možno rozdeliť do dvoch základných kategórií: úmerné zhlukovanie a neúmerné zhlukovanie.

Úmerné zhlukovanie (tiež známe ako zhlukovanie vedome, alebo jednorazové zhlukovanie) je postup určený na klasifikáciu prediktorov podľa príbuzností medzi sebou. Neúmerné zhlukovanie (alebo nevedomé zhlukovanie) je algoritmus, ktorý sa sústreďuje na odhalenie skrytých skupín v dátovom súbore.

Príklady úmerných metód zhlukovania sú K-means, medená algoritmus, hierskej analýza a hľadanie vlastností. Príklady neúmerných metód zhlukovania sú hierarchický aglomeratívny zhlukovací algoritmus, zhlukovanie pre dáta s veľkým objemom a algoritmus DBSCAN.

35. ## Preveďte dáta z 2D do 1D priestoru pomocou PCA.


PCA (Principal Component Analysis) je technika, ktorá slúži na prevedenie dát zo sústavy dimenzií do jednej dimenzie. Princípom PCA je vyradiť redundancie pri dátach a usporiť informácie do jednej dimenzie, čím sa efektívne prenášajú a ukladajú. PCA sa používa najmä na redukciu dimenzií dát a optimizáciu výpočtov. Táto metóda môže byť tiež použitá na prevedenie dát z 2D do 1D. Postup, ktorým sa to dá dosiahnuť, je nasledovný: 

1. Spracovanie dát. Po prvé, získajte a analyzujte všetky dáta, ktoré sa majú premeniť z 2D do 1D. 

2. Skalovanie dát. Skalovanie dát je potrebné na to, aby sa všetky údaje nachádzajúce sa v 2D priestore pohybovali v rovnako veľkom rozsahu.

3. Súčtová transformácia na výstupné dáta. Primárnym krokom v transformácií 2D do 1D je súčtová transformácia. 

4. Použite PCA na konverziu dát z 2D do 1D. Využite PCA na prevedenie 2D dát do 1D priestoru tým, že zmeria závislosti medzi dátami a odoberie po sebe nasledujúce vlastnosti. 

5. Interpretácia výsledkov. Interpretácia výsledkov PCA by mala zahŕňať porozumenie skóre, ktoré poskytujú transformácie súčtu a vyhodnotenie čiastkových komponentov. 

6. Použite transformované dáta. Akonáhle je transformovanie dát do 1D priestoru hotové, výsledné 1D dáta môžete použiť do ďalších procesov ako napríklad vykonávanie výpočtov alebo vytváranie modelov.


36. ## Pomocou naivného Bayesovho klasifikátora klasifikujte daný objekt.


Naivný Bayesov klasifikátor je typ algoritmu strojového učenia, ktorý používa probabilistický prístup na predpovedanie hodnôt jednej alebo viacerých tried na základe histórie dát. Snaží sa nájsť tú najpravdepodobnejšiu triedu pre daný objekt na základe modelu probabilistických charakteristík. Naivný Bayesov klasifikátor by mohol byť použitý na klasifikáciu objektu na základe požadovaných charakteristík, ako sú vek, pohlavie, pozícia v oblasti, príjem atď. Proces klasifikácie by vyžadoval mapovanie a priradenie objektu do tej správnej triedy, pričom by využil aktuálnu históriu dát a probabilistickú pravdepodobnosť.

37. ## Vytvorte rozhodovací strom.


      Kúpiť auto?
     
                     YES
                      /\
                     /  \
                    NO  Áno 
                   /  \
              Model  Cena
38. ## Spočítajte počet parametrov CNN a velkosti jednotlivých výstupov vo vrstvách.


CNN skladá zo štyroch druhov vrstiev: kaňonicky usporiadané vrstvy (convolutional layers), poolovacie vrstvy (pooling layers), plne prepojené (fully connected layers) a dropout layers. Každý typ vrstvy sa skladá zo sady parametrov, ktoré Morú ovplyvňovať výsledný výsledok CNN.

Convolúcia:
Táto vrstva je zodpovedná za extrahovanie vlastností z digitálnych obrázkov. Konkrétne tie obsahujú filtrovací vektor, počet filtrov, pravidlo divného počtu, veľkosť filtera a veľkosť vstupného obrázka. Počet parametrov, ktoré sú v tejto vrstve, sa odhaduje na násobok počtu filtrov s veľkosťou filtra.

Pooling:
V tejto vrstve sa vektor obrázka líši na niekoľko menších vektorov, ktoré majú oveľa menší počet koeficientov ako vektor vstupného obrazu. Táto vrstva má parametre počtu vektorov a veľkosti.

Plne prepojené:
Táto vrstva je zodpovedná za zhlukovanie vstupných dát do výsledných výstupov. Obsahuje parametre toku neuronov a veľkosti vstupnej/výstupnej vrstvy.

Dropout:
Posledná vrstva je zodpovedná za regularizáciu a úpravu hlboko vyčesania. Táto vrstva obsahuje parametre triedy neurónov a dropoutho faktoru pre reguláciu.

Spolu sa teda počet parametrov CNN pohybuje okolo násobku všetkých typov parametrov v jednotlivých vrstvách súčasne. Velkosť každého výstupu v každej vrstve sa pohybuje okolo veľkosti vstupného obrázka, ktorý je pri nízkej úrovni často mensí ako velkosť vstupného obrázka.
