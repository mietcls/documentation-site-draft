# Design

## Huisstijl

 Wij zijn verplicht de huisstijl van de Vlaamse overheid te volgen. Zij hebben uitgebreide en transparante richtlijnen \(kleuren, logo, lettertypes, ...\)

### Algemene richtlijnen 

{% embed url="https://overheid.vlaanderen.be/communicatie/huisstijl-merkbeleid" %}

### Custom iconen 

{% embed url="https://appuniversum.github.io/ember-appuniversum/docs/atoms/au-icon" caption="Onze custom iconenset / Our custom icon set" %}

We maken gebruik van custom iconen, omwille van twee redenen:

1. We bouwen applicaties. De grootte verschilt vaak van websites waar ze vooral dienen als ornament.  De grootte beïnvloedt de leesbaarheid van de iconenset van de VO.
2. We hebben aangepaste iconen gemaakt voor sommige toepassingen zoals Toegankelijk Vlaanderen.

### Digitale richtlijnen

Er zijn  ook specifieke richtlijnen voor de digitale huisstijl, die lichtjes verschillen van de algemene richtlijnen.

{% embed url="https://overheid.vlaanderen.be/communicatie/huisstijl-en-merkbeleid/digitale-huisstijl" %}

#### Toegankelijkheid

Al de applicaties en websites die we publiceren, moeten toegankelijk zijn, volgens de [WCAG 2.1 richtlijnen](https://www.w3.org/TR/WCAG21/) \[EN\].

{% embed url="https://overheid.vlaanderen.be/digitale-toegankelijkheid" %}

#### Global Header & Footer

{% embed url="https://appuniversum.github.io/ember-appuniversum/docs/patterns/au-main-header" caption="Header" %}

{% embed url="https://appuniversum.github.io/ember-appuniversum/docs/patterns/au-main-footer" caption="Footer" %}

We maken momenteel geen gebruik van de global header & footer; om tracking en snelheidsredenen.

_Header:_ Om vlot te integreren met onze codebase en snelheid te verhogen, hebben we de header nagemaakt in Ember. Deze verschijnt altijd en overal.

_Footer:_ De footer werd ook nagemaakt. Deze gebruiken we enkel op log-in pagina's, omdat onze applicatiepatronen anders in elkaar zitten.

## Mock-ups

We maken momenteel gebruik van een mix van klikbare prototypes in Figma, en echte prototypes in HTML en CSS. We werken ook samen met andere departementen om hier een degelijke componenten bibliotheek aan te leggen, zowel in vectoren \(Figma\) en HTML en CSS.

### Figma

We gebruiken Figma, maar we hebben nog geen licentie. Dit wordt besproken.

{% page-ref page="feedback-geven-op-figma-mockups.md" %}

## Component libraries

### Webuniversum

{% embed url="https://overheid.vlaanderen.be/webuniversum/v3/" %}

De Vlaamse Overheid heeft een webcomponentenblibiotheek gebouwd. We maken daar momenteel geen gebruik van:

* In haar huidige vorm, de 3.0 versie, is deze bibliotheek beschikbaar wanneer we gebruik maken van hun Webplatform. Binnen onze applicatiearchitectuur maken we geen gebruik van dat Webplatform, en kunnen we dus ook geen gebruik maken van de webcomponentenbibliotheek.
* De 3.0 versie is niet open source. Wij maken open source applicaties, en hebben dus nood aan open source oplossing.

### Appuniversum, Webuniversum's Little Sister

Om onze applicaties mee te bouwen, hebben we een open source componentenbibliotheek gebouwd.

De bibliotheek is gebaseerd op de oude webcomponenten van de Vlaamse Overheid, [versie 2.0](https://overheid.vlaanderen.be/webuniversum/webcomponenten-versie-2). Hier bouwden we onze applicaties mee in het begin, toen deze versie nog open source gepubliceerd werd. Om ervoor te zorgen dat we bugs konden oplossen, de bibliotheek konden uitbreiden voor specifieke applicatie componenten en onze applicaties open source konden publiceren, riepen we Appuniversum in het leven. Iedereen die gebruik wil maken van deze bibliotheek, meer specifiek in kader van projecten voor de Vlaamse Overheid, mag hier aan meewerken.

Deze componentenbibliotheek bestaat momenteel uit twee delen: Appuniversum & Ember-Appuniversum.

