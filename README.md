## CI-harjoitus

Tein tunnilla opettajan esimerkin pohjalta harjoituksen, jossa rakennettiin ja testattiin valmis repositorio GitHub Actionsin avulla.

Lisäsin harjoitukseen deployn kotipalvelimelle SSH:n kautta.

Ensin loin ssh-avaimet githubia varten ja lisäsin julkisen avaimen kotipalvelimelle sekä yksityisen avaimen GitHubin Secrets-kohtaan.

Sitten muokkasin workflow-tiedostoa siten, että deploy vaihe suoritetaan, kun koodi on testattu onnistuneesti.

Deploy vaihetta varten loin docker konfiguraation, sillä se oli helpoin tapa saada sovellus pyörimään kotipalvelimella.

Kaiken tämän jälkeen workflow toimii kuten pitää ja deploy tapahtuu automaattisesti kun pusken koodin tähän repoon.
