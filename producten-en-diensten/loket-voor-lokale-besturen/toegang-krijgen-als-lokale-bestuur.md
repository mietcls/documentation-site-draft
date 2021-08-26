# Toegang krijgen als lokale bestuur

## Nieuwe besturen

Nieuwe besturen hebben een goedkeuring nodig van ABB, toegang tot het gebruikersbeheer van het facilitair bedrijf en het loket, en een connectie met Kalliope zodat tweewegscommunicatie kan gebeuren en ABB dossieropvolging kan doen.

![Wat er nodig is](../../.gitbook/assets/screenshot-2021-06-30-at-10.17.09.png)

Om dat te laten gebeuren, doen we het volgende:

* We verwachten een goedkeuringsbeslissing van het Agentschap Binnenlands Bestuur over het nieuwe lokale bestuur.
  * ABB verwittigt het loket voor Lokale Besturen.
* Dan kan het bestuur toegang vragen via het Gebruikersbeheer aan het Facilitair Bedrijf
  * ABB, de product manager van het loket, geeft verificatie en vraagt de OVO aan. Dit wordt teruggekoppeld, samen met de typering.
  * Hierna wordt connectie gemaakt met het KBO
* Er wordt een unieke code aangemaakt om het bestuur mee te identificeren, die we een URI noemen \(Unique Resource Identifier\)
  * Die wordt zowel gebruikt voor het Loket als in Kalliope, om dossieropvolging en tweewegscommunicatie mogelijk te maken. 

![Hoe gebeurt het](../../.gitbook/assets/screenshot-2021-06-30-at-10.30.48.png)

## Gebruikersbeheer & Inloggen

Lokale besturen krijgen toegang door eenmalig toegang te vragen via het [Toegangs- \(ACM\) en Gebruikersbeheer \(IDM\)](https://gebruikersbeheer.vlaanderen.be/) van de Vlaamse overheid. [Meer informatie over ACM-IDM](../../ontwikkeling/architectuur/rechtenbeheer-and-inloggen.md).

{% page-ref page="../toegang-krijgen-tot-de-producten-en-diensten-van-abb/toegang-verlenen-aan-gebruikers-tot-producten-en-diensten-via-gebruikersbeheer-vlaanderen.md" %}

* Het gebruikersrecht dat gebruikt wordt om in te loggen voor het Loket voor Lokale Besturen is "Loket Lokaal Bestuur Gebruiker".
* Per gebruiker kan ingesteld worden welke modules ze zien. De keuze bestaat momenteel uit: Toezicht, berichtencentrum, leidinggevenden, mandatenbeheer, personeelsbeheer, BBC-DR, subsidies. Dit kan later nog uitgebreid worden.
* Er bestaan drie gebruikersbeheren per doelgroep:
  * Vlaamse Overheid​
  * Economische actoren​
  * Lokale Besturen.​ _De doelgroepverantwoordelijke voor Lokale Besturen is ABB._

{% page-ref page="../toegang-krijgen-tot-de-producten-en-diensten-van-abb/aanmelden.md" %}

