# Design

## Huisstijl / Branding

**\[NL\]** Wij zijn verplicht de huisstijl van de Vlaamse overheid te volgen. Zij hebben uitgebreide en transparante richtlijnen \(kleuren, logo, lettertypes, ...\)

**\[EN\]** We are required to follow the branding of the Flemish Government. They have extensive and transparent guidelines \(colours, logo, fonts, ...\)

### Algemene richtlijnen / General guidelines 

{% embed url="https://overheid.vlaanderen.be/communicatie/huisstijl-merkbeleid" %}

### Custom iconen / icons

{% embed url="https://appuniversum.github.io/ember-appuniversum/docs/atoms/au-icon" caption="Onze custom iconenset / Our custom icon set" %}

**\[NL\]** We maken gebruik van custom iconen, omwille van twee redenen:

1. We bouwen applicaties. De grootte verschilt vaak van websites waar ze vooral dienen als ornament.  De grootte beïnvloedt de leesbaarheid van de iconenset van de VO.
2. We hebben aangepaste iconen gemaakt voor sommige toepassingen zoals Toegankelijk Vlaanderen.

**\[EN\]** We do use a different set of icons, because of 2 reasons:

* We build applications. The size is different, which influences the legibility of the current icon set.
* We have created custom icons for some applications like Toegankelijk Vlaanderen.

### Digitale richtlijnen / Digital guidelines

**\[NL\]** Er zijn  ook specifieke richtlijnen voor de digitale huisstijl, die lichtjes verschillen van de algemene richtlijnen.

**\[EN\]** There are also specific guidelines for digital house style, which differ slightly from the general guidelines.

{% embed url="https://overheid.vlaanderen.be/communicatie/huisstijl-en-merkbeleid/digitale-huisstijl" %}

#### Toegankelijkheid / Accessibility

**\[NL\]** Al de applicaties en websites die we publiceren, moeten toegankelijk zijn, volgens de [WCAG 2.1 richtlijnen](https://www.w3.org/TR/WCAG21/).

**\[EN\]** All the applications and websites we publish must be accessible, according to the [WCAG 2.1 guidelines](https://www.w3.org/TR/WCAG21/).

{% embed url="https://overheid.vlaanderen.be/digitale-toegankelijkheid" %}

#### Global Header & Footer

{% embed url="https://appuniversum.github.io/ember-appuniversum/docs/patterns/au-main-header" caption="Header" %}

{% embed url="https://appuniversum.github.io/ember-appuniversum/docs/patterns/au-main-footer" caption="Footer" %}

**\[NL\]** We maken momenteel geen gebruik van de global header & footer; om tracking en snelheidsredenen.

_Header:_ Om vlot te integreren met onze codebase en snelheid te verhogen, hebben we de header nagemaakt in Ember. Deze verschijnt altijd en overal.

_Footer:_ De footer werd ook nagemaakt. Deze gebruiken we enkel op log-in pagina's, omdat onze applicatiepatronen anders in elkaar zitten.

**\[EN\]** We currently do not use the global header & footer; for tracking and speed reasons.

_Header:_ To integrate smoothly with our codebase and increase speed, we recreated the header in Ember. It appears anytime, anywhere.

_Footer:_ The footer has also been recreated. We only use it on log-in pages, because our application patterns are different.

## Mock-ups

**\[NL\]** We maken momenteel niet veel mock-ups, omdat we ook klikbare prototypes bouwen. Maar met een groeiend team van developers, designers en analisten merken we dat het maken van mock-ups het bouw- en testproces van applicatie kan versoepelen.

**\[EN\]** We currently don't create a lot of mock-ups , because we also build prototypes. But as our team is growing \(developers, designers, analysts\), we find that creating high-fidelity mock-ups can make the process of building and testing applications go smoother.

### Figma

**\[NL\]** We gebruiken Figma, maar we hebben nog geen licentie. Dit wordt besproken.

In de tussentijd kunnen we ons baseren op de Figma bibliotheek die Mono Company heeft gemaakt voor het maken van apps voor de Vlaamse overheid.

**\[EN\]** We use Figma, but we do not have a license yet. This is a discussion in progress.

In the meantime, we can base ourselves on the Figma library Mono Company created for creating apps for the Flemish Government.

{% embed url="https://www.figma.com/community/file/935528404464006391" %}

## Component libraries

### Webuniversum

{% embed url="https://overheid.vlaanderen.be/webuniversum/v3/" %}

**\[NL\]** De Vlaamse Overheid heeft een webcomponentenblibiotheek gebouwd. We maken daar momenteel geen gebruik van:

* In haar huidige vorm, de 3.0 versie, is deze bibliotheek beschikbaar wanneer we gebruik maken van hun Webplatform. Binnen onze applicatiearchitectuur maken we geen gebruik van dat Webplatform, en kunnen we dus ook geen gebruik maken van de webcomponentenbibliotheek.
* De 3.0 versie is niet open source. Wij maken open source applicaties, en hebben dus nood aan open source oplossing.

**\[EN\]** The Flemish Government has built a web component library. We are not currently using it:

* In its current form, the 3.0 version, this library is available when we use their Web platform. Within our application architecture, we do not use that Web platform, and therefore cannot use the Web component library.
* The 3.0 version is not open source. We create open source applications, and thus need open source solution. Our applications are based on their Web components, an older version, when they were still published open source.

### Appuniversum, Webuniversum's Little Sister

**\[NL\]** Om onze applicaties mee te bouwen, hebben we een open source componentenbibliotheek gebouwd.

De bibliotheek is gebaseerd op de oude webcomponenten van de Vlaamse Overheid, [versie 2.0](https://overheid.vlaanderen.be/webuniversum/webcomponenten-versie-2). Hier bouwden we onze applicaties mee in het begin, toen deze versie nog open source gepubliceerd werd. Om ervoor te zorgen dat we bugs konden oplossen, de bibliotheek konden uitbreiden voor specifieke applicatie componenten en onze applicaties open source konden publiceren, riepen we Appuniversum in het leven. Iedereen die gebruik wil maken van deze bibliotheek, meer specifiek in kader van projecten voor de Vlaamse Overheid, mag hier aan meewerken.

Deze componentenbibliotheek bestaat momenteel uit twee delen: Appuniversum & Ember-Appuniversum.

**\[EN\]** To build our applications with, we created an open source component library.

The library is based on the old web components of the Flemish Government, [version 2.0](https://overheid.vlaanderen.be/webuniversum/webcomponenten-versie-2). This is where we built our applications with in the beginning, when they were still published open source. To make sure we could fix bugs, extend the library for specific application components and publish our applications open source, we created Appuniversum. Anyone who wishes to use this library, more specifically in the context of projects for the Flemish Government, may do so.

 This component library currently consists of two parts: Appuniversum & Ember-Appuniversum.



