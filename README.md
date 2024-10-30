# TuotekuvastoApp

Model-View-Controller (MVC), jonka keskeisimmät komponentit ovat HomeController.cs, products.json ja Product.cshtml. Komponentit kommunikoivat keskenään ja tiedot haetaan ja näytetään
alla kuvatulla tavalla:

# HomeController

Toimii sovelluksen ohjauskeskuksena (controller). Se käsittelee käyttäjän pyyntöjä ja toimii välikätenä näkymän ja tiedon välillä. HomeController hakee tuotteiden tiedot products.json-tiedostosta, luo niiden perusteella olioita tai tietorakenteita, ja lähettää ne näkymään.

# products.json

Toimii datavarastona, jossa tuoteinformaatio on tallennettu JSON-muodossa. Kun HomeController tarvitsee tuotelistaa, se lukee tiedot tästä tiedostosta ja deserialisoi ne (muuntaa ne C#-olioksi tai tietorakenteeksi).

# Product.cshtml

Näkymä (view) jossa tuotteiden tiedot näytetään käyttäjälle. Kun HomeController lähettää tuotteiden tiedot Product.cshtml-tiedostoon, näkymä renderöi (eli piirtää) tiedot käyttäjälle näkyvään muotoon esimerkiksi HTML
ja CSS avulla.

Data siis kulkee products.json → HomeController → Product.cshtml.

Lisäksi pieniä määrityksiä sivuston ulkoasuun ja CSS:n.
