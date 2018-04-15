# Simon Says

## &lt;flókin verkefni />

Þegar búa þarf til flókin verkefni í foritun er best að skipta þau upp í mörgu minni, auðveldari verkefni. Þannig áður en við byrjun að forritta minnisleikinn okkar skulum við hugsa út í hvað við þurfum. Við þurfum að búa til runu fyrir spilarann til að muna. Við þurfum að sýna rununa einhvern veginn. Við þurfum að vita hvað spilarinn ýtti á og við þurfum að bera saman. Byrjum því á að fá þessi föll sem við þurfum. Við þurfum föll fyrir takkanna ( A, B og AB). Við þurfum líka föll fyrir að setja upp runu, spilarunu og bera saman. Byrjum að búa þau föll til tóm.

## &lt;Föllin />

Til að búa til föll fyrir takkanna er ýtt á Input og valið ‘on Button A pressed’ og dregið á ritborðið.

![](img/image1.png?raw=true)

Gerðu þetta þrisvar sinnum og breyttu button þannig þú ert með fyrir A, B og A+B

![](img/image2.png?raw=true)

Til að búa til föll þá þarf að ýta fyrst á advanced svo functions og velja þar ‘Make a Function’. Gerðu þetta þrisvar og skírðu föllin SpilaRunu, BeraSaman og Byrjun.

![](img/image3.png?raw=true)

![](img/image4.png?raw=true)

![](img/image5.png?raw=true)

## &lt;Byrjun />

Núna erum við búin að skipta leiknum upp í nokkur minni verkefni en hvar eigum við að byrja? BeraSaman fallið sér um að bera runurnar saman þannig við getum ekki gert það fyrir en báðar runurnar eru komnar. Við geymum það því aðeins. Til þess að spila runu þurfum við að vera kominn með einhverja runu. Þannig við þurfum líka að bíða aðeins með SpilaRunu fallið. Fallið Byrjun á að sjá um að búa til rununa sem á að herma eftir. Það er góður staður til að byrja á.
Þar sem Byrjun fallið þarf að búa til runu og við þurfum að muna rununa. Þannig getum við skipt Byrjun í tvö enn minni verkefni. Byrjum á að búa til eitthvað til að muna rununa. Besta leiðin til að muna runua er að búa til fylki (array). Byrjum á að velja Variables->Make a Variable og skírum það Runa. Þá ef þið ýtið aftur á Variables ætti þetta að líta svona út:

![](img/image6.png?raw=true)

Við viljum að Byrjun stilli Runu sem tómt fylki. Ýtið aftur á Variables og veljið set item to 0 blockina og dragið hana í Byrjun fallið. Ýtið svo á örina við hliðin á item og veljið Runa.

![](img/image7.png?raw=true)

Núna stillir hann Runa sem talan 0. Það er ekki alveg það sem við viljum en þetta er  í áttinna að því. Við viljum að þetta sé fylki (array). Ýtið á Advanced-> Arrays og dragið ‘create array with 0’ kubbinn og látið hann þar sem 0 er hjá ‘Runa’ kubbnum.

![](img/image8.png?raw=true)

![](img/image9.png?raw=true)

Hvað er fylki? Auðveldast er að hugsa um fylki sem lista af einhverju. Fylki með tölunum 1,2,3,4 væri skráð svona [1,2,3,4] við getum valið bara eitt stak í fylki ef við segjum bara hvar það er í fylkinu. T.d væri fylki[0] = 1 (fylki byrja að telja í 0). Þannig að fylki[3] væri sama sem 4


Núna er Runa fylki en það er með töluna 0 inn í sér. Við viljum að það sé tómt í byrjun. Ýtið á tannhjólið við hliðin á create.
![](img/image10.png?raw=true)

 Dragið þar value úr kubbnum. Núna ætti að standa create empty array.

![](img/image11.png?raw=true)

![](img/image12.png?raw=true)

Núna erum við komin með leið til að geyma rununa okkar. Þegar bætist við runan þurfum við bara að bæta við staki í ‘Runa’ fylkið. En hvernig ætlum við að gera það? Það er hitt verkefnið sem ‘Byrjun’ þarf að sjá um. Við erum með 3 takka: A, B eða báða í einu (A+B).  Við þurfum því að velja af handahófi einn af þessum tökkum hverju sinni.

## &lt;AfHandahófi />

Skulum búa til nýtt fall ( alveg eins og áður) og skíra það AfHandahófi. Við viljum að það fall velji 1 af tökkunum og láti ‘Byrjun’ vita hvað það valdi svo hægt sé að bæta það við ‘Runa’. Ef við ýtum á Math sjáum við kubb sem stendur á ‘pick random 0 to 4’.

![](img/image13.png?raw=true)

Sá kubbur velur tölu af handahófi getum við nýtt okkur það? Tölur eru ekki takkar en við getum samt notað það. Við skulum bara ákveða að 0 = A, 1= B og 2 = AB. Drögum þennan kubb að AfHandahófi. Bíddu þeir passa ekki saman.


![](img/image14.png?raw=true)

Við þurfum að búa til eitthvað stak sem tekur á móti þessari tölu. Veljum Variables og ýtum á ‘Make a Variable’ og skírum hana næstaStak. Færum ‘set item to 0’ inn í AfHandahófi og festum ‘pick random 0 to 4’ kubbunninn okkar við hann.

![](img/image15.png?raw=true)
![](img/image16.png?raw=true)

 Núna í hvert skipti sem við köllum á þetta fall mun næsta stak fá nýja tölu af handahófi frá 0 upp í 4. Við viljum samt bara fá frá 0 upp í 2 þannig breytið 4 í 2.

![](img/image17.png?raw=true)

Ýtið svo á örina við hliðin á item og veljið NæstaStak.

![](img/image18.png?raw=true)

Núna viljum við bæta það sem kemur úr AfHandahófi fallið í ‘Runa’. Í fyrstu umferð skulum við byrja á fjórum táknum, þannig við þurfum að kalla á AfHandahófi 4 sinnum og láta inn í ‘Runa’ jafn oft. Byrjum samt á því að gera þetta bara einu sinni til að sjá hvernig þetta virkar. Við viljum því byrja á að kalla á ‘AfHandahófi’ fallið og svo bæta NæstaStak við í ‘Runa’. Til að kalla á fallið ýtum við á advanced->Functions og veljum call function ‘AfHandahófi’.

 ![](img/image19.png?raw=true)

 Drögum þann kubb út og festum hann neðst í ‘Byrjun’ fallið. Þetta kallar á ‘AfHandahófi’ og breytir gildinu á ‘NæstaStak´.

 ![](img/image20.png?raw=true)

 Við viljum núna bæta ‘NæstaStak’ við ‘Runa’. Við gerum það með því að velja Advanced->Arrays-> og velja ‘list add value to end’.

 ![](img/image21.png?raw=true)

 Drögum hann út og látum hann neðst í ‘Byrjun’ fallið.

 ![](img/image22.png?raw=true)

 Veljið örina við hliðin á list og veljið ‘Runa’.

  ![](img/image23.png?raw=true)

  Næst skuluð þið ýta á Vairables-> og draga ‘NæstaStak’ kubbinn út og láta hann í tómarúmið á milli ‘value’ og ‘end’.

  ![](img/image24.png?raw=true)
  ![](img/image25.png?raw=true)

  Núna erum við búin að bæta við einu staki við ‘Runa’ fylkið. Við viljum gera þetta þrisvar sinnum í viðbót. Við gætum gert seinasta skref aftur 3 sinnum og það mundi virka fínt fyrir þetta. En hvað ef við viljum svo breyta? Kanski viljum við 60,600 eða 6000 stök í byrjun. Við nennum ekki alveg að gera þetta svo oft aftur. Sem betur fer er til betri leið. Við getum sagt fallinnu að gera þetta eins oft og við viljum. Til þessum þurfum við að láta þessa tvo kubba inn í lykkju. TIl þess að búa til lykkju veljum við Loops og drögum ‘repeat 4 times do’ kubbinn út.

   ![](img/image26.png?raw=true)

  Látum kubbinn undir ‘set Runa to create empty array’.

  ![](img/image27.png?raw=true)

  Drögum svo ‘call function AfHandahófi’ kubbinn inn í lykju kubbinn. Báðir kubbarnir ættu þá að enda inn í nýja græna lykkju kubbinn okkar.

  ![](img/image28.png?raw=true)

Núna ef við t.d vildum byrja á 600 stökum gætum við breyt 4 í 600. Við viljum samt bara 4 þannig ekki breyta tölunni. Loks skuluð þið bæta við call function spilaRunu neðst.

![](img/image29.png?raw=true)

Núna gerir ‘Byrjun’ það sem við viljum að það geri. Við þurfum kanski að bæta einhverju við seinna þegar við förum að vinna í hin verkefnin en eins og er virkar þetta fínt. Byrjun er fyrsta functionið sem við viljum kalla á. Við skulum því líka láta eitt call function inn í start. Velum Byrjun í þeim kubb.  Svo skulum við því færa okkur yfir í ‘SpilaRunu’ fallið.

![](img/image30.png?raw=true)

## &lt;SpilaRunu />

Núna þurfum við að ákveða hvernig við ætlum að sýna hvaða takka á að ýta á. Best væri að nota led ljósin til þess. Það eru einmitt ljós við hliðin á tökkunum svo við getum notað þau. Við þurfum að vita hnitin á þessum ljósum. Í venjulegu hnitakerfi væri þetta 1,3 og 5,3 en í forritun er byrjað að telja frá núlli. Þannig hnitin eru 0,2 og 4,2. Ef við erum ekki viss með hnitin þá getum við farið með músina yfir eitt af ljósunum í smá stund og þá birtast hnitin. Skulum byrja á að láta ljós birtast ef leikmaður á að ýta á A takkann. Þá viljum við að ljós [0,2] blikki. Til þess notum við toggle. Toggle kveikir á ljósinu ef það er slökkt á því og slekkur ef það er kveikt. Farið í Led->og dragið toggle x 0 y 0 blokkina í spilarunu.

![](img/image31.png?raw=true)

Breytið svo núllið við hliðin á y í 2.

![](img/image32.png?raw=true)

Við viljum svo slökkva á ljósinu líka þannig endurtakið þetta og látið þann kubb fyrir neðan þennan.

![](img/image33.png?raw=true)

Núna blikkar ljósið við hliðin á A takkanum. Þetta blikkar samt rosalega hratt og það er erfitt að sjá hvað er að gerast. Við þurfum að gera eitthvað þannig að það blikki hægar. VIð getum notað pause (ms) blokkina til þess. Pause blokkinn lætur forritið bíða í þann tíma sem við segjum. Þið finnið pause í Basic-> pause (ms) 100.

![](img/image36.png?raw=true)

 Dragið þá blokk út og látið á milli toogle blokkirnar. Núna er komin smá pása þangað til að slekst á ljósinu.

 ![](img/image34.png?raw=true)

 Þetta er samt ennþá aðeins of hratt. Við þurfum að hækka töluna sem þetta býður. Ég mæli með 600 en þið getið prófað ykkur áfram og fundið einhverja tölu sem ykkur finnst virka vel.

![](img/image35.png?raw=true)

Þessar þrjár blokkir eru að sjá um að birta ljósið fyrir A takkann. Þetta er í raun minna verkefni sem SpilaRuna fallið þarf að sjá um. Við getum því fært þetta í sér fall. Búum til nýtt fall og skírum það SýnaA. Til að búa til nýtt fall er ýtt á Advanced->Functions->Make a function (alveg eins og áður).
Skulum líka búa til function sem sýnir fyrir B takkann og báða takkanna. Skírum það SýnaB og SýnaAB. Dragið ‘SýnaA’ functionið út og færið blokkirnar sem eru í ‘SpilaRunu’ yfir í það fall.

![](img/image40.png?raw=true)

Núna skulum við gera ‘SýnaB’ fallið. Það er alveg eins og ‘SýnaA’ nema við breytum x í 4. Y er ennþá 2.

![](img/image37.png?raw=true)

Þá er bara ‘SýnaAB’ fallið eftir, þar viljum við að bæði ljósin blikki. Við þurfum þá fyrst að toggla bæði ljósin, svo bíða og svo slökkva á bæði með því að toggla. Þetta verður því mjög svipað og hin tvö föllin. Dragið tvær toggle blokkir og látið í ‘SýnaAB’. Breytið hnitin í 0,2 og 4,2.

![](img/image38.png?raw=true)

SVo dragið þið pause kubb á milli, alveg eins og áður. Svo loks gerið þið aftur tvær toggle blokkir eins og áður og breytið hnitin í 0,2 og 4,2.

![](img/image39.png?raw=true)

Núna erum við komin með föll sem geta birt ljósin sem sýna hvaða takka á að ýta á. HVernig getum við samt vitað hvaða ljós við iegum að birta? Í ‘Runa’ fylkið erum við með tölur: 0,1 eða 2. VIð getum nýtt okkur það. Ef talan er 0 þá viljum við kalla á ‘sýnaA’, ef talan er 1 þá viljum við kalla á ‘sýnaB’ og ef talan er 2 þa´viljum við kalla á ‘sýnaAB’. Sem betur fer er til blokk sem getur gert þetta. Ef við veljum Logic-> og veljum ‘if true then else’ blokkinna.

![](img/image41.png?raw=true)

Þessi blokk athugar eitthvað hjá if, ef if stenst þá gerir kubburinn það sem er í then. Ef það stenst ekki þá gerir það það sem er í else. Þetta er næstum því það sem við viljum.

![](img/image42.png?raw=true)

Við erum með 3 möguleika svo við viljum eitthvað sem mundi lesast einhvern veginn svona: ef 0 þá sýnaA annars ef 1 þá sýnaB annars þá sýnaAB. Við þurfum ekki að athuga hvort að það sé 2 því að við erum búin að útiloka 0 og 1 þannig það hlítur að vera 2.  Á ensku er þetta if->then->else if->then->else if-> then. Við þurfum þvi að breyta blokkinna okkar. Ýtið á tannjólið við hliðin á if og bætið við else if fyrir neðan if.

![](img/image43.png?raw=true)

Núna þurfum við að bæta inn skilyrðunum og hvað gerist þegar skilyðurunum eru mætt. Byrjum á að bæta inn skilyrðunum. Runa heldur utan um allar tölurnar sem eru komnar þannig við viljum nota það. Við viljum skoða eitt stak í fylkinu Runa í einu en við viljum samt skoða öll. Við getum ekki notað repeat eins og seinast því Runa mun ekki alltaf vera af sömu lengd. Til er lykkja sem getur farið yfir öll stökin í Runa ( munið að Runa er eiginlega eins og listi af tölum) sama hversu margar tölur eru inn í Runa. Við þurfum lykkju ( á ensku kallast það loop) sem skoðar allar tölurnar í Runa. Í loops er til kubbur sem á stendur “for element value of list do” veljið hann og dragið hann efst í spilaRunu kubbinn.

![](img/image44.png?raw=true)

Látið síðan if-the-elseif kubbinn sem var fyrir inn í lykkju kubbinn.

![](img/image45.png?raw=true)

Næst skulum við stilla hvernig lykkjan okkar virkar. Byrjum á að breyta list í runa.

![](img/image46.png?raw=true)

Næst þurfum við eitthað gildi sem við getum skoðað. Búum til nýtt variable og skírum að bara i og látum það í staðinn fyrir value.

![](img/image47.png?raw=true)

Það sem for lykkjan gerir er að athuga fyrsta stakið í fylkinu Runa. Þannig ef Runa mundi líta svona út: [2,0,1,0] þá væri frysta stakið 2. Þá verður i = 2 á meðan við gerum það sem er inn í lykkju(græna) kubbnum okkar. Þegar það er lokið athugar lykkjan næsta stakið í Runa og þá mundi i verða 0 í þessu tilviki. Þetta gerir kubburinn sjálfkrafa þangað til að hann er búinn að fara yfir allar tölurnar í Runa.

Núna skulum við klára að stilla skilyrðin. Við viljum athuga hvort að tala sé jöfn 0,1 eða 2. Til þess notum við 0=0 kubbinn sem er í logic.

![](img/image48.png?raw=true)

Drögum þann kubb fyrir aftan if og else if.

![](img/image49.png?raw=true)

 Breytum svo fremri tölunum báðum í i og öftustu tölunni í else if í 1.

![](img/image50.png?raw=true)

Núna eru skilyrðin okkar komin. Núna þurfum við að segja hvað gerist þegar í hverju tiliki fyrir sig. Við vildum að 0 væri A takkinn þannig við drögum SynaA í fyrsta then.
1 átti að vera B þannig við drögum synaB í seinna then. Ef talan er ekki 0 eða 1 þá hlítur hún að vera 2. Þá viljum við sýna báða þannig drögum synaAB þangað.

![](img/image51.png?raw=true)
![](img/image52.png?raw=true)

Það er ennþá ekki alveg nógu skírt hvenær ljósin skiptast. Við skulum því bæta við einu pause fyrir ofan if kubbinn okkar. SKrifum 200 inn í hann.

![](img/image53.png?raw=true)

## &lt;Takkarnir 1 />

Næst skulum við stilla hvað takkarnir gera. Við þurfum að muna hvaða takka notandinn ýtir á þannig við getum svo borið það saman við Runa. Þannig getum við athugað hvort að notandinn gerði rétt. Skulum búa til nýtt variable sem heitir notendaRuna. notendaRuna mun vera fylki eins og Runa. Þegar við ýtum á takkanna viljum við bæta við í tölu í notendaRuna. Þegar ýtt er á A bætum við við 0, þegar við ýtum á B þá 1 og 2 ef við ýtum á AB. Skulum því bætt við “list add value to end” kubbum undir alla takkanna. Þessi kubbur er undir arrays.

![](img/image54.png?raw=true)
![](img/image55.png?raw=true)

 Breytum list í notendaRuna og látum value 0 í A, value 1 í B og value 2 í AB.

![](img/image57.png?raw=true)
![](img/image56.png?raw=true)

Þetta er fínt í bili. Núna skulum við búa til fall sem getur borið saman notendarunu og Runa.

## &lt;Bera Saman 1/>

Við viljum taka fyrsta stakið í Runa og bera það saman við fyrsta stakið í notendaRuna. Skulum gera svipað og við gerðum í spilaRunu. Skulum nota lykkju. Drögum “for index from 0 to 4” kubbinn inn í BeraSaman.

![](img/image58.png?raw=true)

Búum til nýtt value sem heitir j og látum það í staðinn fyrir value og breytum 4 í length of array kubb. Við finn þann kubb í Arrays.

![](img/image59.png?raw=true)

Svo förum við í variables og veljum Runa og látum hann fyrir aftan length of array.

![](img/image61.png?raw=true)

Þetta er næstum því rétt. Munið að runa er list og fyrsta stakið í honum fæst með 0 en ekki 1. Þannig að ef Runa er með 4 stök þá færðu seinasta stakið með því að biðjum um Runa[3]. Lengdin á Runa er samt 4. Við þurfum því að gera -1. Takið length of array kubbinn í burtu í smá stund og látið 0 - 0 kubb inn í staðinn. Sá kubbur er inn í math. Látið svo length of array kubbinn í staðinn fyrir fremsta 0 og breutið seinna núllið í 1

![](img/image60.png?raw=true)

## &lt; Tap/>

Núna þurfum við að bera saman fyrstu stökin í báðum. En áður en við gerum það þurfum við aðeins að pæla í hvað gerist ef við gerum vitlaust. Annað hvort gerði notandinn rétt og þá viljum við láta hann vita og halda áfram, eða hann gerði vitlaust og þá viljum við láta hann vita af því og byrja upp á nýtt. Skulum búa til nýtt function og skíra það tap. Tap er auðveldara þannig byrjum á að gera hann.

Góð leið til að láta vita er að sýna mynd. Skulum því sýna stórt X á skjánum ef notandinn tapar. Við gerum það með því að fara í basic og velja show icon kubbinn.

![](img/image62.png?raw=true)

 Veljum svo icon með því að ýta á örina við hliðin á hjartanu. Ég ætla að velja x en þið megið velja hvað sem er.

 ![](img/image63.png?raw=true)

 Skulum svo láta notandann vita að við séum að fara að byrja aftur. Í basic er kubbur sem heitir show string hello. Dragið hann undir show icon kubbinn og skrifið aftur í staðinn fyrir hello. Svo til að byrja aftur þurfum við að kalla bara aftur á byrjun. Farið í functions og dragið call function byrjun og látið hann neðst.

![](img/image64.png?raw=true)

Núna þurfum við samt aðeins að laga byrjun kubbinn. Því núna þegar við byrum aftur man kubburinn ennþá hvað notandinn ýtti á seinast. Við þurfum því að tæma notendaRuna fylkið. Við gerum það með set item to kubbnum.

![](img/image15.png?raw=true)


Dragið hann efsti í Byrjun og breytið item í notendaRuna

![](img/image65.png?raw=true)

Látið svo create empty array í staðinn fyrir 0.

![](img/image8.png?raw=true)
![](img/image66.png?raw=true)

## &lt; Rétt 1/>

Núna þurfum við að hugsa um hvað við gerum ef notandinn gerir rétt. Við viljum hafa 5 umferðir. Í fyrstu umferð koma 4 tákn. Það er gert í byrjun. Ef notandinn gerir þau rétt þá viljum við spila aftur þessi 4 tákn og bæta tveimur við. Notandinn vinnur svo alveg ef hann kemst upp í fimmtu umferð. Við þurfum því function fyrir það þegar notandinn gerir rétt, function til að bæta við í Runa og loks function ef notandinn nær að vinna alveg. Skulum gera rétt functionið. Búið til nýtt function sem heitir rétt. Skulum líka sýna mynd þegar notandinn gerir rétt. Dragið því show icon og veljið eitthvað merki til að gefa til kynna að hann gerði rétt. Ég ætla að velja check merkið en þið getið valið hvað sem er ( bara ekki velja sama mynd og fyrir rangt). Við ætlum svo að halda áfram þannig við þurfum að taka myndina sem þið völduð í burtu. Bætið við pause kubb og clear screen kubb. Skrifið svo 200 inn í pause kubbinn. Allir þessir 3 kubbar eru í basic. Clear screen er í basic og svo more.

![](img/image67.png?raw=true)

Núna vantar bara að kalla á function sem bætir við en við þurfum að búa það til fyrst.

## &lt; Sigur />

Búið til function sem heitir bætaViðRunu. Í þessu functioni viljum við fyrst athuga hvort að notandinn sé búinn að klára 5 umferðir. Okkur vantar því eitthvað til að fylgjast með umferðunum. Búið til nýtt variable og nefnið það umferð. Skulum stilla umferðina sem 1 í byrjun. Dragið því “set item to 0 “ kubb eftst í byrjun og breytið item í umferð og 0 í 1.

![](img/image68.png?raw=true)

Ef umferð er jafnt og 5 þegar við förum í bæaVið fallið þá er leikmaðurinn búinn að vinna. Þá viljum við kalla á eitthvað fall sem lætur hann vita að hann hafi unnið. Búum því til en eitt fall og nefnum það sigur. Þar skulum við líka birta einhverja mynd. Skulum gera það samt aðeins skemmtilegra og láta sú mynd blikka nokkru sinnum áður en notandinn byrjar aftur. Farið því í Loops og veljið repeat 4 times do kubbinn og látið hann í sigur. Þið megið láta hvaða tölu sem er í staðinn fyrir 4 ( ég mæli með að ekki velja stærri en 10 samt). Næst skulum við draga show icon kubb þangað og velja mynd. Svo clear screen og pause. Skrifið 200 inn í pause. Þið finnið pasue með því að ýta á basic og svo more undir basic.

![](img/image69.png?raw=true)

Látið svo show string undir græna kubbinn og breytið hello í aftur. Síðan köllum við á byrjun. Alveg eins og við gerðum í tap kubbnum.

![](img/image70.png?raw=true)

## &lt; BætaVið />

Núna getum við gert bætaVið functionið okkar. Þar viljum við byrja á að athuga hvort að umferðin sé jafn og 5. Ef svo er köllum við á sigur, annars bætum við 2 stökum í Runa og spilum rununa aftur. Við getum sett þetta upp sem:                 
ef umferð= 5 þá sigur annars eitthvað annað. Þanng byrjum á að draga if then else kubb inn í functionið.

![](img/image41.png?raw=true)

Við viljum athuga hvort að umferð sé jafn og 5. Látum því 0=0 kubb inn í stðainn fyrir true.

![](img/image71.png?raw=true)

Drögum svo variable kubbinn umferð í staðinn fyrir fyrsta 0 og breytum hitt 0 í 5.

![](img/image72.png?raw=true)

Ef umferð er sama sem 5 þá viljum við kalla á sigur functionið. Drögum því call function sigur fyrir aftan then.

![](img/image73.png?raw=true)
![](img/image74.png?raw=true)

Ef umferð er ekki sama sem 5 þá viljum við hækka umferð um einn því við erum að fara að byrja næstu umferð. Drögum “change item by 1” kubb
![](img/image75.png?raw=true)
og látum hann efst í else. Breytum svo item í umferð

![](img/image76.png?raw=true)

Þar sem við viljum að notandinn ýti á alla takkann aftur þurfum við að núllstilla notendaRuna, eins og við gerum í byrjum Gerum því alveg eins og þar og höfum set notendaRuna to create empty array kubb á eftir change umferð kubbnum.

![](img/image77.png?raw=true)

Núna þurfum við bara að bæta við tveim nýjum gildum í Runa. Við búum til nýtt gildi með afHandahófi functioninu okkar þannig við þurfum að kalla á það og svo bæta NæstaStak tölunni okkar aftast við Runa. Við gerum mjög svipað í Byrjun functioninu. Byrjum á að fara í Loops og velja repeat 4 times do kubbinn.

![](img/image26.png?raw=true)

Breytið 4 í 2 og látið call function afHandahófi kubb á eftir do.

![](img/image78.png?raw=true)

Loks förum við í Arrays og veljum list add value to end kubbinn

![](img/image79.png?raw=true)

 og látum hann fyrir neðan call function AfHandahófi. Breytið list í Runa og látið næstaStak variable í tóm reitinn. Þið finnið NæstaStak í variables. Núna þurfum við að spila rununa aftur þannig kallið á SpilaRunu functionið neðst. Þá er þetta function tilbúið.

 ![](img/image80.png?raw=true)

 Við viljum kalla á þetta function ef notandinn gerir rétt þannig bætið við call function bætaVið neðst í rétt kubbnum okkar

![](img/image81.png?raw=true)

## &lt; BeraSaman />

Núna getum við loksins klára BeraSaman functionið. Ef notandinn gerði einhverja villu köllum við á tap annars köllum við á rétt. Skulum því búa til variable sem fylgist með hvort að notandinn sé búinn að gera rétt eða ekki. Skírum þessa breytu gerðirétt. Drögum svo set item to 0 kubb og látum hann efst í bera saman. Breytum item í gerðirétt og 0 í true. Þið finnið true í logic.

![](img/image82.png?raw=true)
![](img/image83.png?raw=true)

Til eru breytur sem kallast boolean. Þær eru annað hvort true eða false ( satt eða ósatt). Þannig er gerðirétt true ef notandinn gerði allt rétt en við breytum henni í false ef hann gerði villu. Inn í græna kubbnum viljum við bera saman og athuga hvort að tölurnar eru eins. Ef þær eru ekki eins þá skulum við breyta gerðirétt í false.  Fyrst skulum við draga eina if then kubb inn í græna kubbinn.

![](img/image84.png?raw=true)

 Förum svo í logic og drögum 0=0 kubbinn og látum hann í staðinn fyrir true.

![](img/image86.png?raw=true)

Ýtið svo á örina við hliðin á = merkinu og veljið = með strik í gegnum sig.

![](img/image85.png?raw=true)

Næst þurfum við að breyta 0 báðu megin. Þar sem við erum að vinna með tvö fylki þurfum við að nota list get value at 0 kubbinn. Hann er í arrays.

![](img/image88.png?raw=true)

Látum þannig kubb í staðinn fyrir bæði núllin. Breytið svo fyrsta list í notendaRuna og seinna list í Runa. Loks breytið þið bæði núllin í j.

![](img/image87.png?raw=true)

Þetta athugar hvort að listarnir eru eins. Ef þeir eru ekki eins þá viljum við breyta geraRétt í false. Dragið því set item to kubb og látið fyrir aftan then. Breytið svo item í gerðirétt og 0 í false. False er á sama stað og true var. Núna þurfum við að gera If then else kubb þar sem við förum annað hvort í rétt eða tap functionið. Byrjið á að draga if then else kubb og láta hann neðst í BeraSaman functionið. Sá kubber er í logic. Næst farið þið í variables og finnið gerðirétt, dragið þann kubb og látið í staðinn fyrir true. Munið að gerðirétt er annað hvort true eða false ( satt eða ósatt) ef hann er satt þá gerum við það sem er í then en annnars það sem er í else. Ef gerðirétt er true þá gerði notandinn alveg rétt. Þá viljum við fara í rétt. Farið í functions og dragið call function rétt og látið fyrir aftan then. Látið svo call function tap í else.

![](img/image89.png?raw=true)

## &lt; Takkar 2 />

Núna erum við næstum búin. Við viljum kalla á beraSaman um leið og notandinn er búinn að ýta nógu oft á takkanna. Sem sagt í fyrstu umferð er það 4 sinnum, í umferð 2 er það sex sinnum o.s.fr. Besti staðurinn til að athuga hvort að notandinn sé búinn að ýta nægilega oft er í tökkunum. Við þurfum því að bæta við if then kubb í öllum tökkunum hjá okkur. Ég ætla að sýna hvernig það gerið það fyrir A takkann. Þið gerið svo alveg eins fyrir B og AB. Byrjið á að draga if then kubb og láta hann neðst í on Button A pressed.

![](img/image90.png?raw=true)

Næst farið þið í logic og dragið 0=0 kubb og látið hann í staðinn fyrir true. Svo farið þið í arrays og dragið length of array og látið í staðinn fyrir bæði núllin. Svo loks farið þið í variables og dragið Runa fyrir aftan fremri length of array og notendaruna fyrir aftan hinn.

![](img/image91.png?raw=true)

Fyrir aftan then dragið þið call function beraSaman.

![](img/image92.png?raw=true)

Gerið alveg eins fyrir hina tvo takkanna.

![](img/image93.png?raw=true)

## &lt; Endir />

Eins og er þá getur notandinn ýtt á takkanna á meðan runnan er ennþá að spilast. Þetta getur valdið vandræðum þannig við skulum laga það. Við skulum gera takkanna óvirka á meðan runnan er að spilast. Við gerum þetta með því að hafa boolean gildi sem fylgist með. Búið til nýtt variable sem heitir spila. Látið einn set item as kubb í byrjun functionið.
Látið "spila" inn í fyrsta reitin og false inn í hinn.  

![](img/image94.png?raw=true)

Bætið svo við if then kubb inn í alla takkanna og látið það sem var fyrir inn í tökkunum fyrir aftan then. Látið svo spila variable í staðinn fyrir true all staðar.

![](img/image95.png?raw=true)

 Loks viljum við breyta spila í true um leið og spilaRuna er búið að klára. Látið því set item to kubb neðst í spila runa og látið svo spila í staðinn fyrir item og true í staðinn fyrir 0.

![](img/image96.png?raw=true)

Til hamingju núna er leikurinn tilbúinn.

Eitt auka sem þú gætir reynt við sjálfur væri að sýna einhvern veginn hvaða umferð er. Ef þú vilt prófa það mæli ég með að nota umferð breytuna og kveikja ljós efst á skjánum til að sýna hvað umferð er í gangi
