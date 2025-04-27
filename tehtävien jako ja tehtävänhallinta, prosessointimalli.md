# 🔐 Responsible Disclosure -käytäntö

Responsible Disclosure -käytäntö tarkoittaa vastuullista tapaa ilmoittaa tietoturvahaavoittuvuuksista organisaatiolle ennen kuin ne paljastetaan julkisesti. Tämä antaa yrityksille mahdollisuuden korjata ongelmat ennen kuin ne voivat aiheuttaa haittaa.

Yrityksen saattavat ottaa tietoturvan vakavasti, että on olemassa käytäntöjä ja tai ohjeistuksia tämän "responsible disclosure" periaatteiden mukaisesti.

Tämä pätee aina, kun löydetään jotakin, mikä voi vaarantaa tietoturvaa - oli löydön tekijänsä ulkopuolinen henkilö/tutkija tai sisäinen henkilö tai vaikappa satunnainen harrastelija talon sisältä.

Nyt katsotaan seuraavista koskien OWASP (top 10 haavoittuvuudet), OSINT (avoimien lähteiden tiedonhankinta), ja pätee myös Brute Force - testaus (esim. Salasanojen murtautumiset järjestelmän pääsemiset) ja näiden yhteyden noudattamisen koskievia ettistä ja juridista kaavaa.

---

## 🔐 Responsible Disclosure & tietoturvatestaus – mitä pitää tietää?

### 🧪 Mitä testauksia tämä koskee?
Kaikki seuraavat termit/tekniikat voivat paljastaa haavoittuvuuksia tai riskejä, ja siksi niihin liittyy vastuullinen ilmoitusvelvollisuus:

| Termi                                | Mitä se tarkoittaa                         | Vaatii Responsible Disclosure -käytännön      |
|-------------------------------------|-------------------------------------------|----------------------------------------------|
| 🕸️ OSINT (Open Source Intelligence) | Julkisista lähteistä kerätty tieto        | Kyllä – voi paljastaa vahingossa arkaluonteista dataa |
| 🧱 Brute Force / salasanojen murtaminen | Testataan salasanojen vahvuutta           | Kyllä – voi rikkoa järjestelmän tai aiheuttaa lukituksia |
| 🧪 Penetraatiotestaus (pentest)     | Simuloitu hyökkäys testitarkoituksessa    | Ehdottomasti kyllä – oltava lupa ja selkeä prosessi |
| 🧯 Vulnerability scanning           | Automaattinen haavoittuvuuksien etsintä   | Kyllä – vaikka automaattinen, tulokset voivat olla herkkiä |
| 🔎 OWASP Top 10                     | Yleisimmät web-haavoittuvuudet (esim. XSS, SQLi) | Kyllä – jos löydetään, pitää ilmoittaa vastuullisesti |

---

## 📋 Miten tämä kannattaa määrittää yrityksen tasolla?

🔐 Responsible Disclosure -ohjeistuksessa tulisi olla:
1. Selkeä kielto luvattomasta testaamisesta
   - "Kaikki tietoturvatestaus tulee suorittaa etukäteen hyväksytyn suunnitelman tai roolin puitteissa."
2. Miten ja mihin ilmoitetaan (esim. haavoittuvuus löytyi OWASP-tyylisesti)
3. Kenellä on oikeus tehdä mitäkin
   - esim. vain hyväksytyt henkilöt/tiimit saa ajaa automaattista skannausta
4. Miten tulokset käsitellään
   - Luottamuksellisesti, sisäisesti, dokumentoiden
5. Miten epäviralliset havainnot ilmoitetaan
   - Jos "harrastelija" löytää jotain → vastuullinen ilmoitus (ei julkisteta, ei revitellä Slackissa, ei omatoimisia korjauksia)

🔎 Responsible Disclosure pätee myös sisäiseen tietoturvatestaukseen.  
Olitpa pentesteri, kehittäjä, IT-osaaja tai vaikka omatoiminen "hakkeri" firman sisällä – löydös pitää ilmoittaa vastuullisesti, ei kokeilla rajaa.  
**Lupa + dokumentointi + ilmoitus = vastuullinen toiminta.**

---

## 💬 Viestintä on iso osa tätä vastuuta

📲 Useimmat firmat käyttää Teamsiä tai muita viestikanavia (Slack, sähköposti, tiketit, jopa WhatsApp joskus).  
🔄 Jos löytyy haavoittuvuus vaikka:
- kolmannen osapuolen sovelluksessa (esim. ulkoinen HR-työkalu),
- jonkun toisen osaston järjestelmässä (esim. myyntidatassa),
- tai viestintä on mennyt väärälle henkilölle (esim. tiedostoja jaettu väärään tiimiin),  
tästä prosessista ja ilmoittamisesta pitää ilmoittaa välittömästi eteenpäin, ettei vain jätettä ohitse että "ei kuulu minulle/meille."

---

## ✅ Mitä tapahtuu ilmoituksen jälkeen?

Saapuvista tiedoista eli pätee se viesti, mistä se on saatu, niin pitää ottaa välittömästi haltuunsa, eikä vain toimia näistä kuten:
- Ei reagoida / ei ehdi katsoa / sai viestin mutta ei ehtinyt oikeasti avata
- Huomasi, mutta antaa sen toisen/muun henkilön ottaa sen
- Tai oikeasti kävi katsomassa, mutta unohdi jälkikäteen ja jne, että pätee näitä on paljon työtehtäviä käsissä, että vasta viikonloppuna ottaa haltuunsa

### Normaalisti useimmin alkaa toimenpiteensä:
- 📋 Tiketti tai tehtävä (todo) luodaan → tieto viedään eteenpäin oikealle vastuuhenkilölle  
- 🔧 Korjaus aloitetaan – mahdollisimman nopeasti tilanteen vakavuuden mukaan  
- 🗂️ Asia dokumentoidaan – opitaan, estetään toisto, ja varmistetaan jäljitettävyys

---

---

## 🔐 Viestinnän vastuullisuus tietoturvassa

🧠 Tämä on just sitä aluetta, jossa viestinnän vastuullisuus ja avoimuus kohtaa tietoturvan – eli jos tapahtuu jotakin vastuullisen ilmoittamisen (Responsible Disclosure) piiriin kuuluvaa, asiakkaat ja joskus myös media pitää osata huomioida oikealla tavalla, oikeaan aikaan. 📣

---

### 💬 Viestintä asiakkaille tai medialle

#### 🎯 Milloin pitää viestiä asiakkaille tai medialle?

| Tilanne                                     | Pitääkö ilmoittaa?                                          | Kenelle?                                          |
|--------------------------------------------|-------------------------------------------------------------|--------------------------------------------------|
| 🛠️ Haavoittuvuus korjattiin ilman vaikutuksia | Ei aina pakko, mutta hyvä käytäntö                          | Asiakkaat (esim. release notes)                 |
| 🔐 Haavoittuvuus vaikutti asiakastietoihin tai toimintaan | ✅ Kyllä, usein pakko (GDPR/NIS2)                           | Asiakkaat, viranomaiset, joskus media          |
| 🚨 Tietomurto tai merkittävä tietovuoto      | ✅ Ehdottomasti                                              | Asiakkaat, viranomaiset, media                 |
| 🔄 Iso tekninen muutos, jolla parannetaan turvallisuutta | Ei pakko, mutta asiakasarvon vuoksi hyvä kertoa             | Asiakkaat                                       |
| 🧪 Haavoittuvuus ilmoitettiin ja se on tutkinnassa | Riippuu vakavuudesta                                       | Ainakin asiakkaat, jos heihin voi vaikuttaa    |

---

#### 💬 Miten viestitään asiakkaille?

🧾 **Viestin rakenne (esimerkki):**  
🔒 Aihe: Tietoturvapäivitys / ilmoitus haavoittuvuudesta  
Hei,  
Yrityksessämme havaittiin [päivämäärä] tekninen haavoittuvuus, joka liittyi [järjestelmä X / palvelu Y].  
✔️ Haavoittuvuus on nyt korjattu eikä sen kautta ole havaittu asiakastietojen vuotoa.  
🔧 Päivitys on tehty [päivämäärä] ja on osana versiota [1.2.3].  
📞 Jos sinulla on kysyttävää, olethan yhteydessä [tietoturvayhteyshenkilö / asiakaspalvelu].  

Ystävällisin terveisin,  
[Yrityksen nimi / Tietoturvatiimi]

---

#### 📡 Medialle (jos aihe on merkittävä)

Jos haavoittuvuus tai tietovuoto on vakava tai vaikuttaa suureen asiakasmassaan, yrityksen pitää harkita myös:  
- 🔊 Lehdistötiedote  
- 🌐 Tiedote verkkosivuille  
- ❓ UKK (usein kysytyt kysymykset) -sivu asiakkaille  
- 💬 Some-kanavat (jos tieto leviää muutenkin siellä)  

💡 **Tärkeää:** Viestinnän pitää olla faktoihin perustuvaa, läpinäkyvää ja ei syyllistävää. Älä piilota tietoa, mutta älä myöskään levitä paniikkia.

---

## 🔁 Päivitykset, muutokset ja tapahtumat

Kyllä, nämä kuuluvat Responsible Disclosure -ympäristöön, vaikka eivät olisi varsinainen tietomurto:

| Esimerkki                                    | Pitääkö ilmoittaa?                      | Miten?                                   |
|---------------------------------------------|-----------------------------------------|-----------------------------------------|
| 🧩 Turvapäivitys julkaistu                   | Kyllä (release notes tai asiakastiedote) | Sähköposti, portaalit                   |
| 🧪 Haavoittuvuus löydetty, korjattu ja tutkittu | Kyllä, jos vaikutti asiakkaisiin        | Sama kanava kuin missä palvelua käytetään |
| 🧯 Simuloitu testi, ei oikea uhka            | Ei pakollinen, mutta voi mainita "turvatoimia kehitetään jatkuvasti" |    |
| 📈 Muutos SLA-tasoon tai tukiprosessiin      | Kyllä, asiakkaille selvästi ilmoitettuna |                                        |
| 📬 Muutos ilmoituskanaviin (esim. uusi "security@firma.fi") | Kyllä, tärkeä tiedottaa asiakkaille ja yhteistyökumppaneille |  |

---

## 🧠 Miksi tämä on tärkeää?

- 🔐 **Asiakkaat haluavat tietää, miten yritys huolehtii heidän tiedoistaan.**
- 🧾 **Viestiminen lisää luottamusta**, ja ennakoiva viestintä voi estää ison mainekriisin.  
- 📣 **Viestinnän avoimuus voi vahvistaa brändiä** – kun yritys osoittaa, että se osaa reagoida ammattimaisesti.  
- ⚖️ Tietyissä tapauksissa ilmoitus on lainsäädännöllisesti pakollinen (GDPR: ilmoitus 72h sisällä tietomurrosta).  

---

## 👥 Muista nämä roolit viestinnässä:

| Rooli                           | Vastuu viestinnässä                             |
|---------------------------------|------------------------------------------------|
| 🧑‍💼 Tietoturvavastaava          | Faktojen kokoaminen ja arvio                  |
| 📢 Viestintäpäällikkö / markkinointi | Selkeä viestintä asiakkaille ja medialle      |
| ⚖️ Juridiikka                   | Tarkistaa mitä saa/ei saa sanoa ja milloin    |
| 🧑‍💻 IT / DevOps                 | Tekniset tiedot ja korjaustoimenpiteet        |
| 📞 Asiakastuki                  | Vastaa kysymyksiin asiakkaiden suuntaan       |

---

---

## 🛠️ Suunnitelmallinen Responsible Disclosure -prosessi

Monet yritykset kaatuu juuri siihen, että "kyllä joku joskus tekee ohjeen"… mutta ei kukaan tee.

Hyvin suunniteltu ja dokumentoitu Responsible Disclosure -prosessi, etenkin penetraatiotestauksen ja muiden tietoturvatestien yhteydessä, on just se, mikä erottaa reagoinnin kaaoksessa vs. toiminnan hallitusti. 💡📋

---

### 👉 Kuinka rakentaa Responsible Disclosure -prosessi?

#### 🛠️ 1. Suunnittelu – ennen kuin mitään testataan

| Elementti            | Miksi tärkeä?                                                 |
|----------------------|-------------------------------------------------------------|
| 🎯 Tavoite           | Mitä testataan, miksi testataan, mitä halutaan löytää?         |
| 🧾 Lupa & hyväksyntä | Vain luvallisella testauksella on suoja – tämä on ehdoton.     |
| 🧭 Scope & rajat     | Missä järjestelmissä saa testata, mihin ei saa koskea? (esim. tuotantoympäristö?) |
| 🧑‍🤝‍🧑 Vastuuhenkilöt | Kuka vetää, kuka hyväksyy löydökset, kenelle ilmoitetaan?       |
| 📅 Aikataulu          | Testauksen ajankohta, kestot, mahdolliset häiriöikkunat.      |

📝 Tämä kaikki kannattaa kirjata testauksen aloitusdokumenttiin → jää jälki, että kaikki oli suunniteltua.

---

#### 🔧 2. Toteutus – kun testi tapahtuu

| Elementti               | Miksi tärkeä?                                               |
|-------------------------|-----------------------------------------------------------|
| 🧪 Testaus työkalut ja metodit | OWASP, OSINT, porttiskannaus, brute force... pitää kuvata selkeästi. |
| 📂 Löydösten dokumentointi | Mitä löytyi, miten löydettiin, toistettavuus.                    |
| 🤫 Tietojen käsittely       | Ei vuoda Slackiin, ei jaeta huvin vuoksi – vastuullisuus ennen kaikkea. |
| 📤 Ilmoittaminen           | Haavoittuvuudet ilmoitetaan heti, vastuullisesti → tiketöinti alkaa.   |
| 📸 Kuvakaappaukset, logit, ja tekniset tiedot | Talteen mutta suojatusti.                              |

---

#### 🧱 3. Jälkikäsittely – kun löydökset on saatu

| Elementti               | Miksi tärkeä?                                               |
|-------------------------|-----------------------------------------------------------|
| ✅ Tiketit tehtäviksi    | Jokaiseen haavoittuvuuteen tulee korjaus- tai tutkintatehtävä. |
| ⏳ Priorisointi          | Mikä on kriittinen, mikä voidaan korjata myöhemmin?         |
| 🧯 Korjaus               | Kuka korjaa, miten, milloin – ja testataanko uudelleen?     |
| 📘 Raportointi ja oppiminen | Dokumentoidaan opit: mitä tapahtui, miten toimittiin, mitä voi parantaa. |

---

### 📚 4. Arkistointi ja ohjeistus – että muutkin oppii

Tämä on SE kohta, jonka sä nostit hienosti esiin. 💬  
Usein jää tekemättä, vaikka juuri tästä syntyy se yrityksen oppiva kulttuuri.

#### 🗂️ Kirjataan:
- Mitä testattiin, miten meni?
- Mitä löydettiin, miten reagoitiin?
- Miten prosessi toimi? Mikä toimii, mitä voisi parantaa?
- Mistä löytyy yhteyshenkilöt ja vanhat raportit?

➡️ Tämä toimii mallina muille: ei tarvitse aloittaa tyhjästä, vaan voi käyttää aiempaa runkona.

---

### 💡 Vinkki: Näin rakennat ohjeen joka ei jää pölyttymään

- Tee yksi sivu: "Näin teet vastuullisen tietoturvatestauksen".
- Käytä emojia tai visuaalisia osioita – tekee sisällöstä kevyemmän omaksua.
- Älä tee 15 sivun dokumenttia – mieluummin yleisrakenne + linkit.
- Nimeä se selkeästi: "PENETEST VASTUULLISESTI – ohje tiimeille".

---

### 👏 Lopuksi – Sun ajatus tiivistettynä:

- 🧠 "Jos jotain opitaan, se pitää dokumentoida niin että seuraava ei aloita nollasta."
- 📘 "Ohje ei synny itsestään – ja jos kaikki odottaa että joku muu tekee sen, sitä ei tule ikinä."
- 🔐 "Responsible Disclosure on prosessi, jota pitää rakentaa, ei vain odottaa."

---

## Kuinka Responsible Disclosure -prosessin tuotokset päivitetään?

✅ **Vastaus:** Molemmat – mutta eri tavalla ja eri syistä.

---

### 🔄 Prosessin aikana ("reaaliaikaisesti")
➡️ Tärkeimmät havainnot ja toimenpiteet kirjataan jo heti testauksen ja ilmoittamisen yhteydessä:

- 🔹 Löydösten peruskuvaukset (mitä havaittiin, milloin, miten).
- 🔹 Tikettien/tehtävien luonti (ja seurantatiedot).
- 🔹 Viestintäketjut ja vastuuhenkilöt.
- 🔹 Alustava vaikutusarvio (kuinka kriittinen?).

🎯 **Miksi tämä tehdään heti?**
- Jotta tieto ei unohdu, katoa, tai jää henkilökohtaisten muistien varaan.
- Mahdollistaa nopean reagoinnin ja selkeän työnjaon.

---

### 🧾 Prosessin lopuksi ("jälkikäteen")
➡️ Kun koko case (testi, haavoittuvuus tai Disclosure-ilmoitus) on käsitelty, tehdään:

- 📘 Yhteenvetoraportti – mitä tapahtui, mitä opittiin.
- 📌 Dokumenttien päivittäminen – ohjeet, mallit, toimintakaaviot.
- 📊 Raportointi johdolle tai osastoille (jos tarpeen).
- 📚 Arkistointi – tieto säilytetään jatkoa varten.

🎯 **Miksi tämä tehdään lopussa?**
- Kokonaiskuva on selvä.
- Opit voidaan koostaa ja viedä muihin prosesseihin.
- Varmistetaan, ettei sama virhe toistu.

---

## 🧠 Vinkki käytäntöön:

| Aikapiste                 | Mitä tuotetaan?                          | Minne kirjataan?                      |
|---------------------------|------------------------------------------|---------------------------------------|
| 🔄 Testin aikana           | Tiketti, löydösraportti, tilannepäivitys | ServiceNow, Jira, OneNote, lokit      |
| 🧯 Korjauksen yhteydessä   | Mitä tehtiin, kuka teki, miten testattiin | Sama paikka kuin tiketti              |
| 🧾 Jälkikäteen             | Loppuraportti, päivittynyt ohjeistus, arkistointi | SharePoint, Confluence, tietoturvapankki |

---

### 👋 Lopputiivistys:

- 🔐 Responsible Disclosure -prosessissa tuotetaan sisältöä sekä matkan varrella että lopuksi.
- 💬 Reaaliaikaiset merkinnät pitävät homman käynnissä ja hallinnassa.
- 📘 Loppudokumentointi varmistaa, että seuraavat oppivat ja firma kehittyy.




