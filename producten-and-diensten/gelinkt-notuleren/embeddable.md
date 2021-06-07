---
description: >-
  Een open-source tekstverwerker die specifieke informatie uit notulen verrijkt
  met data, op een gestructureerde manier, zodat we achteraf die informatie
  kunnen extraheren en hergebruiken.
---

# Embeddable & Say-Editor

**De Embeddable** is een bouwsteen van Gelinkt Notuleren. Het is een slimme, open-source tekstverwerker die specifieke informatie uit notulen verrijkt met data, op een gestructureerde manier, zodat we achteraf die informatie kunnen extraheren en hergebruiken. 

Externe notuleringpakketten die lokale besturen helpen met het opstellen van notulen, kunnen deze embeddable ook hergebruiken in hun software pakket om de data te extraheren.

We bieden deze tekstverwerker aan als _embeddable_ \(eenvoudig inplugbaar\) voor die besturen of hun software leveranciers kunnen gebruiken in hun notuleringpakketten. We stellen deze embeddable ook open onder de naam van **Say Editor** voor eender wie die hun tekstverwerking willen verrijken met kennis.

Om meer gedetailleerde informatie over Say editor te vinden, bezoek [https://say-editor.com/](https://say-editor.com/).

{% embed url="https://say-editor.com/" %}

## Bouwblokken

De embeddable bestaat uit verschillende bouwblokken die gelinkt notuleren mogelijk maken.

{% embed url="https://www.figma.com/file/kYcCsAHp7rbvrsRE2w1NC0/GN-brainstorm?node-id=623%3A0" %}

### Databronnen.

Wij gebruiken meerdere gegevensbronnen om notulen en besluiten te verrijken:

* **De Vlaamse Codex** – verwijzingen naar de rechtsgronden in beslissingen.
* **Mandaten** – om aanwezigen bij te houden, te benoemen en te ontslaan.
* **Leidinggevenden** –  om aanwezigen bij te houden.

### Functionaliteiten & Plugins

We hebben aparte kleine apps gemaakt die in de teksteditor kunnen worden gestopt:

* **Toolbar**: basisfuncties voor tekstbewerking.
* **Sjablonen**: om het makkelijker te maken om te beginnen met noteren.
* **Citaten plugin**: maakt gebruik van de Vlaamse Codex – om te verwijzen naar juridische gronden in beslissingen.
* **Stemming**: stem over beslissingen.
* **Aanwezigen**: volg wie deel uitmaakte van de vergadering, en deel uitmaakt van bepaalde beslissingen.
* **Import – export**: beslissingen kunnen geïmporteerd en geëxporteerd worden \(in uitvoering\).
* **Annotaties**: annoteer tekst met specifieke gekoppelde informatie, zoals mandaten.
* **Ondertekenen**: ondertekenen van notulen, uittreksels, agenda's, besluitenlijsten.
* **Authenticatie**: inloggen via [Gebruikersbeheer](https://gebruikersbeheer.vlaanderen.be/) \(ACM-IDM\).
* **Anonimiseren**: verwijder persoonlijke informatie voor publieke weergave.

Lees de documenten van Say Editor om te zien hoe ze worden opgezet: [https://say-editor.com/docs](https://say-editor.com/docs).

{% embed url="https://say-editor.com/docs" %}



## Code

Al onze applicaties worden op dezelfde manier opgebouwd. Lees eerst de [Architectuur](../../ontwikkeling/architectuur/) pagina voor je start met deze repositories.

### Embeddable

{% embed url="https://github.com/lblod/frontend-embeddable-notule-editor" %}

{% embed url="https://github.com/lblod/app-gn-embeddable" %}

### Tutorial: je eigen slimme tekstverwerker

Voeg zelf de slimme tekstverwerker toe aan je ember applicatie:

{% embed url="https://github.com/lblod/say-editor-as-addon-tutorial" %}

### Documentatiesite Say-Editor

{% embed url="https://say-editor.com/" caption="Landingspagina" %}

{% embed url="https://github.com/lblod/frontend-say-editor-documentation" %}

{% embed url="https://github.com/lblod/app-say-editor-documentation" %}





