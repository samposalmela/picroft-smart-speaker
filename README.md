# Picroft älykaiutin

Projekti on tehty Haaga-Helian monialaprojekti kurssia varten. Tavoitteena on nopeuttaa tiedon hankkimista ja tehdä siitä vaivattomampaa. Projektin tuloksena syntyy toimiva älykaiutin hyödyntäen Raspberry Pi 4:sta ja Mycroft ääniavustajaa.

## 1. Picroftin lataaminen ja asentaminen muistikortille

Ensin ladattiin [Picroft disk image](https://drive.google.com/uc?id=1nyd5l5vgRy--Y3VG3AXUAiBio2QEF1O8&export=download).

Raspberry Pin muistikortti laitettiin USB-adapteriin, jonka avulla muistikortti saatiin liitettyä tietokoneeseen. Sen jälkeen asennettiin [balenaEtcher](https://www.balena.io/etcher/), jonka avulla saatiin Picroft asennettua muistikortille.

![Etcher](images/etcher.png)

Tämän jälkeen Raspberry Pi liitettiin kiinni ethernet yhteydellä ja kytkettiin päälle. 

## 2. Etähallinnan käyttöönotto

### 2.1 Porttien avaus

Määritetetään paikallinen IP-osoite, ulospäin menevä portti, sisäinen portti ja protokolla reitittimen asetuksista.

![Portti2](images/2.PNG)

Avattu portti ja IP-osoite SSH-yhteydelle (22). Lisäksi etätyöpöytä yhteydelle (3389) ja VNC viewerille (5800-5900), jos joskus tulevaisuudessa näille tulee tarvetta. 

![Portti3](images/3.PNG)

### 2.2 SSH-yhteyden ottaminen

Picroftissa on oletuksena SSH käyttöönotettuna, joten sitä ei tarvitse erikseen laitteesta ottaa käyttöönotettuna. Voidaan ottaa suoraan yhteys Picroftiin käyttäen PuTTYa ja Raspberry Pin sisäistä IP-osoitetta.

Kirjauduttiin sisään `käyttäjänimi: pi` ja `salasana: mycroft`.

Valittiin `Y` eli guided setup.


