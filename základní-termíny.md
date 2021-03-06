# Základní kameny \(= slovníček\)

Poznámka dopředu: bookování = rezervování. Kdysi jsem se tomu smál, ale už mi to připadá úplně normální.

## IBE

Sice tvrdím, že letenky jsou eshop. Ale obvykle se tomu, co vyvíjíme říká IBE - Internet Booking Engine.

## IATA kódy destinací

Destinací může být letiště nebo i město, ale také heliporty a železniční nebo autobusové zastávky. Na raritní místa toho pochopitelně mnoho nelétá \(nebo nejezdí, systém občas nabídne i autobus nebo vlak\). Letiště mohou být sdružena pod kód města.

* PRG - kód Letiště Václava Havla v Praze
* NYC - kód města New York
* JFK - kód Letiště J.F. Kennedyho v New Yorku, lety vyhledat i pod kódem NYC
* EWR - kód letiště v Newarku, lze jej najít i pod kód NYC, přestože technicky Newark je jiné město než New York... dokonce je i v jiném státě
* PFL - kód autobusového nádraží Praha Florenc

[http://www.iata.org/publications/Pages/code-search.aspx](http://www.iata.org/publications/Pages/code-search.aspx)

## City pairy a routing

City pair je dvojice IATA kódů odkud kam se letí. Například PRG a FRA \(Frankfurt\), často se uvádí dohromady PRGFRA. Routing už bývá složitější. Například PRG-FRA/AMS-NYC, jde o cestu z Prahy do New Yorku přes Frankfurt nebo Amsterodam.

## Letecké společnosti, číslo letu, marketingová a operující společnost

Číslo letu se obvykle skládá z kódu letecké společnosti:

* OK - Czech Airlines
* BA - British Airways
* AA - American Airlines

... a čísla letu:

* BA853 - let společnosti British Airways z Prahy do Londýna na letiště Heathrow \(kód LHR\), nemusí létat pravidelně ani ve stejný čas, ale bude vždy na trase PRGLHR

Někdy ale může být let takzvaně "operován", což znamená, že jej ve skutečnosti letí jiná letecká společnost. Vám ji ale prodá tzv. marketingová letecká společnost pod svým kódem, se kterým let eviduje u sebe a který na letišti všude vidíte.

* BA1511 - let na trase JFKLHR prodávaný společností British Airways pod číslem 1511. Ve skutečnosti ale poletíte s American Airlines, která jej operuje.

Není výjimkou, že let je operován pro několik marketingových dopravců, takže můžete na letišti vidět na tabuli různé lety se stejným časem odletu ze stejného terminálu. Je to stejné letadlo.

## Frequent flyer programy a letecké aliance

Je běžné, že letecké společnosti provozují věrnostní programy. Anglicky zvané Frequent flyer.

Kromě toho se některé letecké společnosti spojily do aliancí. Jsou tři:

* Oneworld
* Sky team
* Star alliance

GDSům se v rámci těchto aliancí dobře kombinují lety, ale to vám může být jedno. Pro vaše zákazníky naopak může mít význam, že společnosti si v rámci aliance často uznávají věrností body.

Další informace: [https://en.wikipedia.org/wiki/Airline\_alliance](https://en.wikipedia.org/wiki/Airline_alliance "https://en.wikipedia.org/wiki/Airline_alliance")

## Letový řád

Sice existuje, ale nebude vás až tolik zajímat. Jednak může být i velmi nepravidelný a druhak si lidé mnohem více než podle letového řádu vybírají podle dostupné ceny.

## Segmenty a itinerář

Segment je konkrétní úsek cesty, obsahující číslo letu, datum a čas odletu. Zpáteční cesta PRGNYC s přestupem se tak skládá ze čtyř segmentů:

* BA853 PRGLHR 12.5.2017 6:50
* BA157 LHRJFK 12.5.2017 9:40
* BA1511 JFKLHR 28.5.2015 18:05
* BA854 LHRPRG 29.5.2017 10:35

Seznamu segmentů se také říká itinerář.

## Kabiny a bookovací třídy

V zásadě se kvalita cestování dělí do skupin Economy, Premium Economy, Business a First Class. Ve velkých letadlech to bude znamenat oddělené prostory. V malých bude Business část oddělená závěsem a obsazeno bude například jedno sedadlo ze dvou. First class tam nebude. Někdy se tomuto říká kabina někdy třída.

Letenky se ovšem neprodávají na kabiny, ale na bookovací třídy, což jsou písmenka, například Y, K, M nebo T. Jejich obecné dělení do kabin sice existuje, ale letecké společnosti je příliš nedodržují.

## Ceny letenek

Koncová cena letenky, kterou zákazník zaplatí se skládá z celé řady komponent, které je třeba nasčítat.

* Cena tarifu - základní část ceny za letenku. Tuto cenu dost často vidíte v reklamách, ačkoliv zdaleka nemusí být nejvyšší složkou.
* Taxy - skládájí se z celé řady poplatků.
  * Letištní taxy - poplatky za pobyt na letištích, kterými cestujete.
  * Palivové poplatky - cena za palivo.
  * Hrst dalších - např. různé daně, které si určují země průletu.
* Servisní poplatek - částka, kterou si účtuje cestovní agentury \(vy\) za zprostředkování rezervace.
* Poplatek za způsob platby - částka, kterou si účtuje například platební brána, za zprostředkování platby kartou.

## Tarify a fare basis kód

Tarifů vypisují letecké společnosti opravdu hodně, toto je například výpis části tarifů pro let PRGJFK.

![](/assets/ukázka-tarifů.png)

Vidíte z něj:

* Tarifů vidíte 18. Dalších 32 jsem si nechal pro sebe.
* Všechny tarify patří společnosti Lufthansa \(LH\)
* Cena tarifu \(tedy bez  se pohybuje od 959CZK do 13384CZK.
* Všechny tarify jsou zpáteční \(bílé R\).
* Tarify jsou označeny "tajemnými" kódy \(KLNCQ0B\).
* Tarify jsou určeny pro několik bookovacích tříd: K, L, T, S.
* Tarify mají omezenou minimální a maximální dobu pobytu \(6/12M\).
* Tarify mají omezené období, kdy podle nich lze letět \(01OCT-14MAY\).

Co z něj nevidíte:

* ... že podle těchto tarifů lze části cesty \(nebo i celou\) letět i s jinou leteckou společností než je LH.
* ... že některé tarify je možné prodávat pouze v nějakém období před odletem \(například nejméně 14 dní před\).
* ... že tarify mají dané routingy, na které je možné je použít. Takže ve skutečnosti můžete cestu urazit 2-6 segmenty.
* ... že některé tarify mají omezení a lze je použít pouze v týdnu nebo naopak o víkendu.
* ... že některé tarify umožňují více zavazadel než ostatní.
* ... že některé letenky lze levně zrušit a jiné nikoliv.
* ... že některé letenky lze levně změnit a jiné nikoliv.
* ... že některé typy pasažérů mohou mít při použití těchto tarifů slevu.

A co už vůbec netušíte:

* Jestli lze letenky podle těchto tarifů koupit. Protože:
  * Za prvé v letadlech, kterými podle daného tarifu můžete letět, nemusí být v daných třídách \(K\) volné místo.
  * Za druhé žádná taková letadla pro vámi vybrané datumy ani nemusí letět.

Poznámka na závěr:

* "Tajemným" kódům se říká \(KLNCQ0B\) Fare basis a obvykle začínají kódem bookovací třídy, kterých se týká.

## Availabilita \(a cache\)

Dostupnost. Tím se myslí dostupnost bookovacích tříd v letadle. Mluvíme o ní hlavně v souvislosti s GDSy. V nich ji vidíme například takto:

![](/assets/import.png)

Vidíme například, že:

* systém eviduje 9 volných míst v bookovacích třídách J, R, Y, B, H, K, M, L, V, N, Q, S a G na letu BA855
* systém eviduje 4 volná místa v bookovací třídě D na stejném letu
* let AA6634 prodáva AA jako operovaný \(před číslem letu je @\) a neprodává úplně všechny třídy stejně
* na letu QS1096 systém neumí říct počet volných míst, takže pro dostupné třídy vypisuje pouze A
* třídy U a J mají speciální význam, ale nevím jaký, písmeno C ovšem znamená, že třída je již zavřená.

Co je ještě dobré vědět:

* neplatí, že všichni lidé na celém světě vidí tytéž dostupnosti. Roli může hrát strategie aerolinky vůči trhu nebo to jestli letíte pouze uvedený úsek nebo delší cestu.
* údaje, které vidíte mohou být různě cachované.
* i když by dostupnost byla brána přímo z inventárního systému letecké společnosti, pořád to neznamená, že se vám uvedená místa podaří zarezervovat. Klidně vám je totiž může někdo vyfouknout pod nosem.
* pokud se některé bookovací třídy už nenabízí, neznamená to, že nemohou zase začít. Letecké společnosti místa průběžně doplňují \(a odstraňují\) v souladu s tím, jak si myslí, že nejlépe využijí dané letadlo.

## BSP - zúčtování

Jak to vlastně funguje s placením? Jestliže statisíce cestovních agentur z celého světa prodává letenky stovek leteckých společností znamená to, že si zběsile vystavují faktury každý každému? Ne.

Alespoň v rámci GDS systémů funguje konsolidátor plateb jménem BSP, který pro agentury a letecké společnosti zajišťuje následující:

* všechny agentury platí všechno jemu
* všem leteckým společnostem platí on

I tento vztah stojí za tím, že vystavovat letenky přes rezervační systém nemůže jen tak někdo, ale právě ony výše zmíněné IATA agentury. Vystavením letenky vzniká závazek agentury vůči BSP a závazek BSP vůči letecké společnosti.

Zároveň existuje celá řada pravidel, podle kterých musí agentury s rezervacemi zacházet, jinak se vystavují riziku takzvaného ADM. A to je prostě pokuta, kterou BSP také vybírá.

## Ocenění a plating carrier

Jak je to ovšem v situaci, že cestujeme s několika leteckými společnostmi. Zopakujme si itinerář uvedený výše:

* BA853 PRGLHR 12.5.2017 6:50
* BA157 LHRJFK 12.5.2017 9:40
* BA1511 JFKLHR 28.5.2015 18:05
* BA854 LHRPRG 29.5.2017 10:35

Z toho zatím vůbec není vidět kolik to bude stát a komu se bude platit. K tomu je potřeba najít dle dostupnosti konkrétní bookovací třídy a potom je ocenit konkrétním tarifem nebo dokonce více tarify.

Výsledek může být třeba takovýto:

* BA853 PRGLHR 12.5.2017 6:50 - třída K, fare basis KLNCQ0B
* BA157 LHRJFK 12.5.2017 9:40 - třída Q, fare basis QLX4S4T1
* BA1511 JFKLHR 28.5.2015 18:05- třída Q, fare basis QLX4S4T1
* BA854 LHRPRG 29.5.2017 10:35- třída K, fare basis KLNCQ0B

Tarify mají základní cenu, ale už víme, že se musí napočítat spoustu dalších složek. Nebudu předstírat, že rozumím, jak se tarify kombinují a taxy vypočítají. Protože je to složité, tak to necháme vypočítat GDS a předpokládejme, že vyšlo 12587CZK.

Nyní může být důležité, komu bude ve finále tato částka přisouzena. Z části o letech víme, že v itineráře může být zahrnuto vícero marktingových leteckých společností a vícero operujících společností. Takzvaný plating carrier je jedna letecká společnost přisouzená ocenění a světe div se, ze jistých okolností to nemusí být ani jedna z nich. Typicky to bude ale ta marketingová společnost, která působí na našem trhu a poletíte s ní delší část cesty. Ani o toto se ale v praxi nebudete moc starat. GDS plating cariera přiřadí spolu s výpočtem ceny.

Cena 12587CZK je ovšem bez service fee a poplatku za platbu. O těchto složkách GDS nic neví a vy si je budete muset připočítat sami, pokud nepoužijete nadstavbu na GDS, která to udělá za vás.

## Pasažéři, jejich typy a údaje o nich

Základní typy jsou:

* Adult - Tedy dospělí. Normální cestující.
* Infant - Kojenci, obvykle od 0-1 let. Nemá nárok na sedačku, cestuje na klíně jiné osoby. Obvyklá cena je 10% ceny tarifu, ale není to pravidlem.
* Child - Dítě, obvykle 2-11 let. Má nárok na sedačku, tarify pro něj někdy obsahují slevu. Někdy ne.

Někdy se setkáte i s:

* Youth - česky obvykle Mládežník. Věk obvykle 12-24.
* Senior - česky taky Senior. Věk obvykle od 60 let.

Kdybyste chtěli být velcí fajnešmekři, tak se můžete pokusit vyhledávat tarify například pro Poutníky, Novináře Evropského parlamentu nebo Vojenské rekruty. Ale nebudete to dělat.

O každém cestujícím potřebujete vědět:

* oslovení, jméno a příjmení, podle zvyklostí trhu někdy i prostřední jméno
* pro typy cestujících s věkovým omezením: datum narození
* nepovinně, pro lety do některých zemí: čísla pasů a související údaje
* nepovinně, typ a číslo frekvent flyer programů \(= věrnostní karty\)

Celkově vzato je tato sekce obrovsky zjednodušená a vyhnul jsem se celé řadě témat, například jak dostat do letadla dvě osoby se stejným jménem. Ale pro začátek to stačí.

## Lokátor, bookování a bookabilita \(a cache\)

To že jsme se od destinací dostali až k bookování \(tedy vytvoření rezervace v inventárním systému letecké společnosti\) není ještě výhra. Shrňme si, co k rezervaci potřebujeme a co známe:

* Itinerář cesty
* Pasažéry a jejich informace
* Ocenění \(zahrnuje i bookovací třídy, farebasis kódy a plating carriera\)

Z těchto věcí budete potřebovat vytvořit rezervaci a zajímat vás budou dvě věci:

* do kdy je třeba letenku vystavit - teoreticky to může být dřív i později, ale prakticky to bude do půlnoci.
* že vám letecké segmenty potvrdí letecké společnosti, které je letí - a zde přichází ke slovu bookabilita.

Bookabilita je míra toho, jak často se vám rezervace podaří. Nedělejte si iluze, 100% případů to nebude. Na cestě od vyhledání letů k jejich zarezervování se utkáváte s všelijakými cachemi a také s ostatními cestujícími. Proto se vám může stát, že se rezervace nezdaří a vy budete muset zákazníkovi vysvětlit, že to má zkusit jinak.

Úspěšně vystavená rezervace má přiřazený lokátor, což v prostředí GDS šestimístný řetězec s písmeny a číslicemi, např. ABC123.

## Look2book \(a cache\)

K bookování se ale váže ještě jeden zádrhel.

Pokud dejme tomu chcete za půl roku cestovat dovolenou na měsíc do jihovýchodní Asie. Tak vás napadne políčit na nejlevnější letenku. Protože jste cestovatel pohodář nesejde vám ani tolik na místě, kam přesně poletíte a odkud se budete vracet a máte třeba 4 destinace, které zvažujete. V úvahu ta pro vás také připadá dejme tomu 20 různých dní pro odlet a klidně tam budete 20-30 dní, když se dost ušetří. Také víte, že ceny se hodně mění, takže to budete hlídat třeba třikrát denně po celý měsíc než se rozhoupete k rezervací.

Ano?

Ne!

Pokud totiž na konci uděláte jednu rezervaci docílíte takzvaného look \(dívat se/vyhledávat\) to book \(rezervovat poměru\) 316000:1 \(pokud správně počítám\). A věřte mi. To je moc. Agentura, která je za váš přístup odpovědná \(vy\), bude muset za nerozumný poměr zaplatit.

Stejného můžete také docílit:

* pokud budete mít hodně navštěvované stránky bez reálných rezervací. 
* pokud se rozhodnete v rámci zrychlování odpovědi cachovat výsledky dopředu \(pro strýčka příhodu\).
* pokud se domluvíte s nějakým integrátorem \(momondo, kayak...\).
* pokud na vaše jinak zcela rozumné stránky někdo zaútočí.

Look2book poměru se není třeba obávat zbytečně moc. Pokud odpovídá jedno vyhledávání reálného zákazníka jednomu dotazu na API, obvykle se do potíží nedostane. Jakmile začnete vymýšlet něco jiného, je třeba se svým plánem svěřit poskytovali API.

## Platba, platební brány a za kolik

Pokud máte zarezervovanou letenku začíná souboj s časem. Potřebujete ji vystavit. Typicky ještě dnes. Pokud počkáte do druhého dne, o místo v letadle nepřijdete \(v drtivé většině případů\). Nepřijdete ani o své bookovací třídy, ale můžete přijít o tarify, které jste si zarezervovali. Pravděpodobně se také hne převodní kurz, kterým se na vaši měnu převádí tarify a taxy pokud nejsou vypsány ve vaší měně.

Druhý den tak bude vaše letenka pravděpodobně stát trochu jinak. Peníze ovšem od zákazníka chcete obvykle před tím než ji vystavíte. Takže si probereme jaké máme možnosti, jak z něj peníze dostat.

* **Hotově** - předpokládá, že máte místo, kam vám zákazník přinese peníze fyzicky. Poplatky za tento způsob si stanovíte sami.
* **Převodem** - zákazník vám pošle převodem, což se v aktuální den obvykle nestihne. Poplatky za tento způsob si vyberou vaše banky, ale obvykle se jedná o drobné částky, které se v cenách letenky neuvádějí.
* **Kartou přes obecnou platební bránu**, například Global payments - jako agentura si budete muset s Global payments domluvit podmínky, za kterých budou pro vás od vašich zákazníků vybírat peníze z platebních karet. Pro ilustraci, řekněme, že tyto podmínky budou 2% z placené částky. O provedené platbě se dozvíte v řádu sekund.
* **Kartou nebo převodem bránou banky** - některé banky nabízí platební brány, které usnadňují platbu jejím klientům a také zkracují dobu, za kterou se o platbě dozvíte. Platí o nich zhruba totéž, co o předchozích branách. Může se to však i lišit :-\).
* **Integrátoři platebních metod**, například PayU - také zde platí zhruba totéž, co u obecné platební brány, podmínky se ale mohou lišit ještě podle jednotlivých integrovaných platebních metod.
* **PayPal a spol** - pro tyto typy plateb je třeba kromě poplatků za transakci, zvážit i způsoby \(a jejich cenu\), kterými dostanene peníze ze svého "účtu" do své kapsy. To může být zatíženo dalšími poplatky.
* **Ostatní** - nevím o tom, že by se pro platbu za letenky používaly - dobírka, smsky, platby mobilem. Ale mohu s plést. Rád informace doplním, pokud mi je poskytnete.

Pokud použijete některou z online platebních metod, budete muset pravděpodobně svoji aplikaci naučit několik nových kousků:

* **přesměrování na platební bránu** - někdy bývá opepřeno výpočtem různých podpisů nebo dodatečnými inicializačními dotazy.
* **příjem zákazníka z platební brány zpátky** \(a ověření stavu platby\) - někdy je třeba ověřovat důvěryhodnost dotazů, někdy se výsledek platby předává "bokem" dodatečnými dotazy.
* **ověření stavu platby, pokud se zákazník z brány nevrátí** - důvodů proč se zákazník nevrátí může být celá hrstka a zdaleka to neznamená, že nezaplatil. Takže ideálně se potřebujete pravidelně dotazovat na výsledek platebních pokusů, o kterých nevíte, jak dopadli. Tedy pokud to brána umožňuje.
* **navýšení ceny letenky o náklady na platební transakci** - pokud si platební brána strhává dejme tomu výše zmíněná 2% a vaše service fee je dejme tomu 300 Kč, znamená to, že od ceny letenky 15000 korun zákazníka dotujete, místo, abyste z něj měli příjem. Jediný způsob, jak tomu zabránit je zahrnout transakční náklady do struktury ceny letenky.

Problematiku EET jsem zatím ponechal stranou a doplním ji hned, jak budu mít jasněji.

## \(E\)ticketing a číslo \(e\)ticketu

Eticketingem je myšleno vystavení elektronické letenky z existující rezervace. Dokud nebylo vystavování elektronických letenek běžné, říkalo se ticketing. Nyní jsou situace, kdy eticket vystavit nelze vzácné, a tak se oba termíny míchají dohromady.

Vystavení eticketu je série dotazů, na jejímž konci přibude k vaší rezervaci několik dlouhých čísel, například 01234567789012. Počet čísel závisí například na počtu cestujících nebo počtu segmentů.

Zákazníkům můžete čísla ticketů zabudovat do krásného PDFka spolu se všemi údaji o jejich rezervaci, které jen dokážete nashromáždit, a doporučit jim ho ať si ho pro všechny případy raději vytisknou. Nebo jim můžete napsat, že na letišti bude stejně každého zajímat jen jejich pas. První varianta bude většinou zbytečná, ve druhé se můžete sem tam zmýlit.

## Voidování

Voidováním se myslí zrušení vystavené letenky. Letenky, které jsou vystavené alespoň den dopředu, jde obvykle do půlnoci daného dne beztrestně zrušit. Poté už je letenka zaúčtovaná a vám nezbude než se při jejím rušení řídit poplatky určenými použitými tarify.

