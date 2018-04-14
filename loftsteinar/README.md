# Loftsteina-leikur

![](imgs/asteroids.gif?raw=true)

> Leikur: Stjórna geimskipi og forðast loftsteina sem koma á móti.

## &lt;Flokkar />

Fyrir þetta verkefni þarf eftirfarandi flokka:

![](imgs/basic.png?raw=true)

![](imgs/led.png?raw=true)

![](imgs/logic.png?raw=true)

![](imgs/input.png?raw=true)

![](imgs/loops.png?raw=true)

![](imgs/math.png?raw=true)

![](imgs/variables.png?raw=true)

## &lt;Geimskip />

Byrjum á að gera breytur fyrir geimskipið okkar:

![](imgs/1-1.png?raw=true)

> Þessar breytur eru fyrir staðsetninguna á skipinu okkar á tölvuskjánum. gx er staðsetningin á x-ásnum og gy er staðsetningin á y-ásnum

Setjum svo geimskipið okkar í forerver-lykkjuna:

![](imgs/1-2.png?raw=true)

Svona birtist það í microbit:

![](imgs/1-3.png?raw=true)

## &lt;Takkar />

Núna viljum við hreyfa skipið okkar

Bætum við clear screen í forever-lykkjuna okkar

![](imgs/1-4.png?raw=true)

og kóðum svo takkana:

![](imgs/1-5.png?raw=true)

> Þegar við ýtum á A og B þá lækkar og hækkar x-gildið á geimskipinu, eða: geimskipið fer til hægri og vinstri.

If else setningarnar fyrir ofan láta skipið hreyfa sig í kringum skjáinn

![](imgs/1-6.gif?raw=true)

> Til umhugsunar: Hvað eru clear screen og if-else blokkirnar að gera hér?

## &lt;Loftsteinn />

Bætum við loftstein efst á borðið, undir Math(Stærðfræði) er hægt að velja random tölu:

![](imgs/1-7.png?raw=true)

> Breyturnar y1 og x1 eru fyrir staðsetningu loftsteinsins, munið að 0 í y-gildi er efsta röðin á skjánum.

Teiknum svo loftsteininn:

![](imgs/1-8.png?raw=true)

Loftsteinninn birtist á einhverri röð, ýtið á &#128259; til að prófa.

![](imgs/1-9.png?raw=true)

## &lt;Hreyfum loftsteinana />

Bætum við í forever-lykkjuna, færum loftsteininn um 1 á y. Bætum líka við hraða á leikinn:

![](imgs/10.png?raw=true)

> Við pásum í hverju skrefi því annars vinnur talvan of hratt. Prófið að taka pásu-blokkina út til að prófa.

![](imgs/11.png?raw=true)

![](imgs/12.gif?raw=true)

> Tilraun: Hvað gerist þegar hraðatalan (speed) er minnkuð? En hækkuð?

Núna ætlum við að láta loftsteininn koma til baka á nýjum stað ef hann fer útaf skjánum.

![](imgs/13.png?raw=true)

![](imgs/14.gif?raw=true)

## &lt;Gerum árekstra! />

Nú viljum við láta eitthvað gerast þegar loftsteinninn klessir á skipið.

Förum í logic og bætum þessu við í forever-lykkjuna okkar.

![](imgs/15.png?raw=true)

Ef loftsteinninn og geimskipið eru á sama stað á bæði x og y þá er árekstur. Gerum sprengingu á skjáinn. 
> Aukadæmi: Gerið ykkar eigin útgáfu af sprengingunni!

![](imgs/16.gif?raw=true)

## &lt;Líf og leik lokið/>

Gerum breytu fyrir líf í on start:

![](imgs/17.png?raw=true)

Bætum við virkni í áreksturinn þannig við missum líf, bætum svo við neðst í forever-lykkjuna að leikurinn klárist:

![](imgs/18.png?raw=true)

Núna, ef við klessum þrisvar á loftsteina þá er leik lokið.

## &lt;Stig />

Bætum við stigum. Segjum að við fáum eitt stig fyrir hvern loftstein sem hittir okkur ekki.

![](imgs/19.png?raw=true)

![](imgs/20.png?raw=true)

![](imgs/21.png?raw=true)

## Til hamingju þú hefur klárað leikinn!

## &lt;Aukadæmi - annar loftsteinn />

Til að gera leikinn skemmtilegri getum við bætt við öðrum loftstein. Köllum breyturnar hans y2 og x2.

![](imgs/22.png?raw=true)

Hérna notum við einfalt bragð. Við viljum ekki að loftsteinarnir séu hlið við hlið. Við setjum y2 sem -3, þannig byrjar hann útaf skjánum og dettur svo inn á hann.

Gerum plot fyrir nýja loftsteininn.

![](imgs/24.png?raw=true)

Bætum núna alveg eins árekstrarkóða fyrir loftstein 2 eins og við gerðum fyrir lofstein 1.

![](imgs/23.png?raw=true)

Svo sameinum við áreksturskynjarana

Gerum alveg eins logic fyrir loftstein 2.

![](imgs/25.png?raw=true)

Til að sameina if-setninguna þurfum við or-kubb úr logic.

![](imgs/26.png?raw=true)

Setjum or-kubbinn í if-kubbinn

![](imgs/27.png?raw=true)

Setjum svo kubbana inn sitt hvoru megin:

![](imgs/28.png?raw=true)





