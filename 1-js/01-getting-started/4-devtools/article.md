# Developer console

Kode lengva palikti errorų. Ko gero, tau teks sukelti errorų... Juokauju, tau *tikrai* teks sukelti errorų, nebent esi [robotas](https://en.wikipedia.org/wiki/Bender_(Futurama)).

Tačiau naršyklėje, useriai by default nemato errorų. Todėl jeigu skripte kažkas veikia ne taip, kaip turėtų, mes to nepamatysim ir negalėsim pataisyt.

Tam, kad pamatyti errorus ir gauti daug kitos naudingos informacijos apie skriptus, "developer tools" yra integruoti pačiose naršyklėse.

Dauguma programuotojų naudojasi Chrome arba Firefox, nes šios naršyklės turi geriausius developer tools'us. Kitos naršklės taip pat turi developer tools'us, kartais su įdomiais feature'sais, tačiau dažniausiai bando "pasivyti" Chrome arba Firefox. Todėl dauguma programuotojų turi "mėgstamiausią" naršyklę ir įsijungią kitą naršyklę, jeigu problema yra specifinė kažkokiai konkrečiai naršyklei.

Developer tools'ai turi daug feature'sų. Pradžiai, mes išmoksim kaip juos atidaryti, pažvelgti į error'us ir paleisti JavaScript komandas.

## Google Chrome

Atidaryk puslapį [bug.html](bug.html).

Šio puslapio JavaScript kode yra error'as. Jis paslėptas nuo "parpastų" žmonių, tad atidarykime developer tools'us.

Spausk `key:F12` arba, jeigu naudoji Mac, `key:Cmd+Opt+J`.

Developer tools'ai standartiškai atidarys Console tab'ą.

Turėtų atrodyt kažkas panašaus į tai:

![chrome](chrome.png)

Konkretus vaizdas priklauso nuo Chrome versijos, kurią naudoji. Kartais atsiranda pakeitimų, bet visgi vaizdas turėtų būti panašus.

- Čia mes galim pamatyt raudoną error message. Šiuo atveju skriptas turi nežinomą "lalala" komandą.
- Dešinėje yra clickable link'as į `bug.html:12` su skaičiumi eilutės, kurioje yra error'as.

Žemiau error message'o yra mėlynas `>` simbolis. Jis parodo "command line", kuriame mes galime rašyti JavaScript komandas. Spausk `key:Enter` kad jas paleisti (`key:Shift+Enter` kad rašyti komandas per daugiau nei vieną eilutę).

Dabar mes galime matyti error'us. Kaip pradžiai, to pakanka. Vėliau mes grįšim į developer tools'us ir kalbėsim apie debugginimą chapteryje <info:debugging-chrome>.


## Firefox, Edge ir kiti

Dauguma kitų naršyklių naudoja `key:F12` developer tools'ų atidarymui.

Jų išvaizda gan panaši. Kai išmoksti vieną (gali pradėti nuo Chrome), gali greitai pradėti naudotis kita.

## Safari

Safari (Mac naršyklė, neveikia Windows/Linux) yra šiek tiek unikali. Iš pradžių mums reikia enablinti "Developer menu".

Atidaryk Preferences ir eik į "Advanced". Apačioj bus checkbox'as:

![safari](safari.png)

Dabar `key:Cmd+Opt+C` įjungs konsolę. Taip pat turėk omeny, kad naujas item'as "Develop" atsirado viršutiniam meniu. Jame yra daug komandų ir nustatymų.

```smart header="Kelių eilučių komandos"
Dažniausiai, jeigu konsolėje parašome vieną eilutę kodo ir paspaudžiame `key:Enter`, ji suveikia.

Tam, kad parašyti kelias eilutes, spausk `key:Shift+Enter`. Tokiu būdu mes galime parašyti ilgesnius fragmentus JavaScript kodo.
```

## Reziumė

- Developer tools'ai leidžia mum pamatyti errorus, paleisti komandas, analizuoti kintamuosiuos ir daugiau.
- Juos paleisti galime su `key:F12` dauguma naršklių Windows'uose. Chrome, jeigu naudojame Mac, reikaluaja `key:Cmd+Opt+J`, Safari: `key:Cmd+Opt+C` (iš pradžių reikia aktyvuoti).

Dabar mes turime paruoštą aplinką. Kitoj pamokoj paragausim JavaScript'o.
