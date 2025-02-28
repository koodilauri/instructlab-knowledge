Neuroverkot ovat informaation käsittelyn, matematiikan tai laskennan malleja,
jotka ovat saaneet inspiraationsa aivojen rakenteesta. Neuroverkko on graafi,
joka koostuu neuroneista, joita yhdistävät synapsit. Neuroni saa signaaleja ja
laskee niistä painotetun summan, jonka tietyn rajan ylitettyään lähettää
eteenpäin. Signaalit ovat neuroverkoissa yksinkertaisesti lukuja. Neuroverkko
järjestetään tasoiksi, joiden läpi signaali kulkee. Neuroverkko koulutetaan
syöttämällä sille esimerkkejä vastaantulevista syötteistä. Oppimisprosessin
aikana verkko muodostaa todennäköisyyksin painotetun sisäisen mallin syötteen
ja tuloksen välisestä suhteesta. Perinteisempiin koneoppimismalleihin verrattuna
neuroverkkojen keskeinen etu on, että ne kykenevät hyödyntämään koulutuksessa
syntynyttä malliaan tilanteissa, jotka eivät ole esiintyneet
koulutusaineistossa.

Siinä missä perinteisemmissä asiantuntijajärjestelmissä käytetään
”jos–niin”-sääntöpareja (esimerkiksi jos raidat, niin seepra; jos pitkät korvat,
niin aasi), neuroverkkoa opetetaan esimerkkien avulla (nämä ovat eri-ikäisiä
seeproja ja nämä aaseja). Tällä pyritään siihen, että neuroverkko itse havaitsee
muuttujien epälineaariset riippuvuussuhteet suoraan havaintoaineistosta (em.
esimerkissä neuroverkko oppii tarkastelemaan korvia ja värin kuvioita, ei
esimerkiksi jalkojen pituutta). Muilta osin neuraalilaskenta muistuttaa
tilastotieteessä käytettyjä yleistettyjä lineaarisia malleja (GLM).

Neuroverkot koostuvat joukosta (keinotekoisia) neuroneita. Neuronit ovat
yksinkertaisia, toisiinsa kytkettyjä tiedonkäsittely-yksiköitä. Keinotekoinen
neuroni muistuttaa karkeasti biologista hermosolua, ja koostuu seuraavista
osista: synapseista, summaajasta jsaktivaatiofunktiosta.

Synapsi on kahden neuronin välinen kytkentä, jolle on määritelty
kytkentäkohtainen paino. Summaajan tehtävä on laskea kaikilta syötesynapseilta
tulleiden signaalien summa. Lopulta neuroni tuottaa tämän summan perusteella
epälineaarisen aktivaation. Kustakin neuronista lähteviä synapseja, summaajia
ja aktivaatioita voidaan mallintaa yhdistetyllä funktiolla, joka koostuu
lineaarikuvauksesta, vakiotermistä ja aktivaatiofunktiosta.

Keinotekoisessa neuroverkossa neuronit järjestetään peräkkäisiksi kerroksiksi
(engl. layer), joissa on tietty joukko vektoriksi järjestettyjä neuroneja.
Syväoppivassa (engl. deeplearning) neuroverkossa on useita tällaisia kerroksia,
joilla voi olla toisistaan poikkeavia tehtäviä. Kunkin kerroksen aktivaatio on
seuraavan kerrokseen sisään tuleva signaali. Koska syöte- ja ulostulokerrosten
välissä olevat kerrokset eivät näy ulospäin, niitä nimitetään piilokerroksiksi
(engl. hidden layer).

Aivotutkijat Warren McCulloch ja Walter Pitts esittivät ensimmäisen ihmisaivojen
toimintaa ja matemaattista logiikkaa yhdistelevän laskentamallin vuonna 1943.
Ensimmäinen varsinainen neuroverkko on Frank Rosenblattin perseptroni
vuodelta 1958. Vaikka neuroverkkojen perusajatus perustuu luonnollisiin
hermoverkkoihin, jo David Rumelhart, Geoffrey Hinton ja Ronald J. Williams
vuoden 1986 artikkelissaan huomauttivat, ettei niiden kehittely enää perustu
luonnollisten hermoverkkojen jäljittelyyn. Neuroverkkotekniikoiden kehittäminen
oli jo tuolloin siirtynyt enemmän tilastotieteeseen ja signaalinkäsittelyn
teoriaan.

Monikerroksisen neuroverkon toimivuus edellyttää tapaa, jolla verkon
piilokerroksissa olevien neuronien painokertoimet saadaan päivitettyä. Ratkaisu
tähän on vastavirta-algoritmi. Tekoälytutkimuksen pioneereihin kuuluva Jürgen
Schmidhuber huomauttaa, että algoritmin ensimmäisen implementaation julkaisi
Seppo Linnainmaa pro gradu -työssään vuonna 1970 nimellä the reverse mode of
automatic differentiation. Käytännössä kaikki nykyisin tuotantokäytössä olevat
neuroverkkototeutukset perustuvat Linnainmaan algoritmiin.

Takaisinkytketyt neuroverkot (RNN) perustuvat David Rumelhartin, Geoffrey
Hintonin ja Ronald J. Williamsin julkaisuun Learning representations by
back-propagating errors vuodelta 1986. Hopfieldin verkko (aiemmin
assosiatiivinen neuroverkko) on RNN:n erikoistapaus, jonka kehitti John
Hopfield vuonna 1982.

Pitkä-lyhytkestomuistiverkon esittelivät Sepp Hochreiter ja Jürgen
Schmidhuber 1997. LSTM-verkot mullistivat puheentunnistuksen,
käsialantunnistuksen, konekäännöksen ja kielimallinnuksen vuodesta 2007
eteenpäin.

Google Brain -tutkimusryhmä julkaisi vuonna 2017 Transformer-mallin, joka on
käytännössä korvannut RNN ja LSTM-mallit. Transformer helpottaa rinnakkaista
koulutusta ja sen pohjalta tuotettu generatiivisia tekoälymalleja kuten OpenAI:n
GPT-mallit (engl. Generative Pre-trained Transformer), jotka on koulutettu
valtavan laajoilla tekstiaineistoilla.
