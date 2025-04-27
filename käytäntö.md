# Responsible Disclosure -käytäntö

Responsible Disclosure -käytäntö tarkoittaa vastuullista tapaa ilmoittaa tietoturvahaavoittuvuuksista organisaatiolle ennen kuin ne paljastetaan julkisesti. Tämän käytännön avulla yrityksillä on mahdollisuus korjata ongelmat ennen kuin ne voivat aiheuttaa haittaa.

Yritykset, jotka ottavat tietoturvan vakavasti, voivat luoda ohjeistuksia ja periaatteita tämän vastuullisen ilmoittamisen mukaisesti.

## 🔐 Responsible Disclosure -käytäntö
Responsible Disclosure -käytännöllä tarkoitetaan, että jos joku (sisäinen tai ulkoinen henkilö) löytää haavoittuvuuden tai tietoturvapoikkeaman, hänen odotetaan ilmoittavan siitä vastuullisesti:
- **Ilman vahinkoa** järjestelmille tai tiedoille.
- **Yrityksen määrittelemiä kanavia** käyttäen.
- **Antaen aikaa korjauksille** ennen julkistamista.

## 🧪 Sisäinen penetraatiotestaus ja eettinen hakkerointi
Monissa organisaatioissa on tapana toteuttaa:
- Sisäisiä penetraatiotestauksia, joita tekevät:
  - Yrityksen IT- tai tietoturvatiimin asiantuntijat.
  - Eettiset hakkerit, jotka ovat osa organisaatiota.
  - IT-harrastajat tai työntekijät, joilla on osaamista ja lupa testaukseen.

**Tärkeää:** Kaiken testauksen tulee tapahtua luvallisesti, hallitusti ja vastuullisesti:
- Johdon hyväksynnällä.
- Suunnitellusti ja dokumentoidusti.
- Sovittuna ajankohtana väärinkäsitysten välttämiseksi.
- Aidosta hyökkäyksestä erottuen, vaikka ulkopuolista toimijaa simuloidaan.

## 💼 Käytännöt vaihtelevat yrityksittäin
Jotkut yritykset:
- **Eivät salli testausta** ilman virallista lupaa.
- Käyttävät vain ulkoisia toimijoita testaukseen.
- Kannustavat sisäisiä osaajia tutkimaan ja raportoimaan löydöksiä.

Joissakin yrityksissä järjestetään jopa sisäisiä "Hack Days"- tai "Security Challenges"-tapahtumia, joissa työntekijät voivat testata järjestelmiä turvallisesti.

## 🔐 Mikä on Responsible Disclosure?
Responsible Disclosure tarkoittaa vastuullista haavoittuvuuksien ilmoittamista organisaatiolle. Sen avulla tietoturva-aukot voidaan korjata ennen kuin ne aiheuttavat vahinkoa tai päätyvät rikollisten hyödynnettäviksi.

### 🎯 Periaatteet:
- **Ilmoita löydöksistä** yritykselle vastuullisesti.
- Älä hyödynnä haavoittuvuutta.
- Älä julkaise sitä ennen korjausta.
- Anna yritykselle riittävästi aikaa reagoida.

### 🧑‍💻 Kuka voi ilmoittaa?
- Ulkopuolinen tutkija tai eettinen hakkeri.
- Asiakas tai käyttäjä.
- Yrityksen sisäinen työntekijä (IT-asiantuntija, DevOps, tietoturvaosaaja).

## 🏛️ Vaikutus ISO 27000 -sarjaan ja GDPR:ään
Responsible Disclosure -käytäntö tukee organisaation tietoturvastandardeja:
- **ISO 27001**: Voi olla osa teknistä haavoittuvuuksien hallintaa (esim. A.12.6.1).
- **GDPR**: Vaikka vastuullista ilmoittamista ei velvoiteta, se auttaa tietosuoja-asetuksen vaatimusten täyttämisessä, kuten 72 tunnin ilmoitusvelvollisuudessa henkilötietovuodosta.

## 🛡️ Vastuullisuuden merkitys
Tietoturva koskee kaikkia toimialoja:
- Teollisuus: Rikkinäinen automaatio voi aiheuttaa fyysistä vaaraa.
- Elintarvikeala: Tietovuoto voi vaarantaa asiakastiedot tai laatujärjestelmät.
- Palveluyritykset: Asiakkaiden luottamus voi kärsiä nopeasti.

Selkeät ohjeet varmistavat, että työntekijät, konsultit ja ulkopuoliset toimijat toimivat oikein.

## 🏢 Viestintä prosessista
Viestinnässä on tärkeää erottaa sisäiset ja ulkoiset roolit:
- Ulkoisten käyttäjien tunnistaminen esimerkiksi nimessä (ext_etu.suku@yritys.fi).
- Dokumentaatio ulkoisten resurssien hallintaan:
  - Nimi | Yritys | Yhteystiedot | Ajanjakso | Osasto/projekti | Käyttöoikeudet ja lisenssit.

---

# 🛠️ Viestintävälineet & Responsible Disclosure – Miksi ne ovat tärkeitä?

Kun joku (konsultti, työntekijä, alihankkija…) huomaa haavoittuvuuden tai riskin, hän tarvitsee selkeän tavan ilmoittaa siitä. Tässä viestintävälineet astuvat peliin:
- Jos ei tiedä missä tai miten viestiä, voi:
  - Ilmoittaa väärälle henkilölle 😬
  - Jättää kokonaan ilmoittamatta 😶
  - Jakaa arkaluontoista tietoa väärässä kanavassa 🚨

## 💬 Yleisiä viestintäkanavia yrityksissä

| Väline                          | Käyttötarkoitus                     | Huomio Responsible Disclosure -tilanteissa                                           |
|---------------------------------|-------------------------------------|-------------------------------------------------------------------------------------|
| 🧵 Microsoft Teams              | Pika- ja ryhmäviestintä, tiimityö   | Ei arkaluontoisia löydöksiä yleisiin chateihin! Käytä turvakanavaa tai suoraa viestiä. |
| 📧 Sähköposti (Outlook yms.)    | Virallisempi viestintä              | Hyvä valinta, jos tiedät oikean osoitteen (esim. tietoturva@firma.fi).               |
| 📄 Service desk / tikettijärjestelmä (esim. Jira, ServiceNow) | IT-tuki, ongelmien raportointi | Hyvä, jos on valmiit lomakkeet turvallisuusilmoituksille.                            |
| 🌐 Intra / turvallisuusportaali  | Sisäinen tiedonjakelu ja lomakkeet  | Usein Responsible Disclosure -ohje löytyy täältä – jos ei löydy, pitää tehdä!       |
| ☁️ SharePoint, Confluence yms.  | Dokumentointi                      | Ei ilmoittamiseen, mutta hyvä paikka ohjeistukselle.                                 |

### 🧭 Käytetään yhteistä kanavaa (esim. tietoturva@firma.fi), jos roolista ei ole varmuutta.

---

## 📍 Mistä ja miten tunnistaa oikea väline ilmoittamiseen?
- 🔍 **Tarkista ensin**: Onko firmassa virallinen ohjeistus? (Esim. "Kaikki tietoturvahavainnot Teams-kanavaan X tai sähköpostilla osoitteeseen Y.")
- 🤔 **Jos ei ole ohjeistusta**: Kysy esimieheltä tai IT:ltä ennen kuin lähetät mitään.
- 🚫 **Älä koskaan jaa herkkää sisältöä**:
  - Yleisissä tiimikanavissa (esim. Teamsin yleiset kanavat).
  - Väärissä tiketteissä, joita muut voivat nähdä.
  - Sähköposteissa, joiden vastaanottajasta et ole varma.

---

## 📝 Esimerkki Responsible Disclosure -ohjeesta

🧭 **Viestintä Responsible Disclosure -tilanteissa**  
Kun havaitset haavoittuvuuden tai poikkeaman:
- Käytä ensisijaisesti [turvallisuus@firma.fi] tai [ServiceNow-lomaketta].
- Älä jaa tietoa Teamsin yleisiin kanaviin tai sähköpostilla, ellet tiedä oikeaa osoitetta.
- Jos et ole varma, käänny välittömästi esimiehesi tai tietoturvavastaavan puoleen.  

✅ Näin varmistetaan, että tieto kulkee turvallisesti ja oikeille ihmisille.

---

## ✅ Tiivistettynä: Responsible Disclosure & Viestintä

### 👥 Kenellä on vastuu?  
Olipa henkilö:
- 🧑‍💼 Firman oma työntekijä (vakituinen tai määräaikainen).
- 👨‍💻 Konsultti (toisen yrityksen kautta, mutta työskentelee firmassa).
- 🧱 Alihankkija (esim. ulkoinen tekninen resurssi).

➡️ **Kaikilla on vastuu** ilmoittaa havaituista tietoturvaloukkauksista tai haavoittuvuuksista vastuullisesti – eli Responsible Disclosure -periaatteen mukaan.  
Rooli ei poista vastuuta. 🔐  

---

## 💬 Viestintä – mitä kanavia käytetään?

1. 🧵 **Teams** – yleinen työkalu, mutta:
   - Älä laita yleisiin kanaviin mitään arkaluontoista!
   - Käytä suoraa viestiä oikealle henkilölle/kanavalle (jos tiedossa).

2. 📧 **Sähköposti** – hyvä vaihtoehto, jos:
   - Tiedät oikean osoitteen (esim. tietoturva@firma.fi tai it@firma.fi).
   - Olet epävarma kanavasta → sähköposti on usein turvallisin aloittaa.

3. 🎫 **Tikettijärjestelmä** (esim. Jira, ServiceNow) – jos on käytössä:
   - Tee ilmoitus, vaikka ei olisi oikea osasto – järjestelmä siirtää sen tarvittaessa.

🚨 **Muistutus**:
- Jos tapahtuma on akuutti tai vakava, ilmoita heti – kanavan ei tarvitse olla täydellinen, kunhan tieto menee perille ajoissa.
- Älä jaa tietoa vääriin kanaviin tai henkilöille, jos asia ei heille kuulu.
- Älä koskaan jaa salassa pidettävää tietoa julkisesti (Teams, Slack, ryhmäpostit).
- Rooli ei poista vastuuta – ilmoita aina oikealla tavalla, oikeille ihmisille ja turvallisesti. 🔒💬



