# Design

## Branding

We are required to follow the branding of the Flemish Government. They have extensive and transparent guidelines (colours, logo, fonts, ...)

### General guidelines&#x20;

Guidelines provided in Dutch. Get in touch if you would like to have more information in English.

{% embed url="https://overheid.vlaanderen.be/communicatie/huisstijl-merkbeleid" %}

### Custom icons

{% embed url="https://appuniversum.github.io/ember-appuniversum/docs/atoms/au-icon" %}
Our custom icon set
{% endembed %}

We do use a different set of icons, because of 2 reasons:

* We build applications. The size is different, which influences the legibility of the current icon set.
* We have created custom icons for some applications like Toegankelijk Vlaanderen.

### Digital guidelines

There are also specific guidelines for digital house style, which differ slightly from the general guidelines. In Dutch. Get in touch for more information in English.

{% embed url="https://overheid.vlaanderen.be/communicatie/huisstijl-en-merkbeleid/digitale-huisstijl" %}

#### Toegankelijkheid / Accessibility

All the applications and websites we publish must be accessible, according to the [WCAG 2.1 guidelines](https://www.w3.org/TR/WCAG21/).

Guide proviced in Dutch. Get in touch if you would like more information in English.

{% embed url="https://overheid.vlaanderen.be/digitale-toegankelijkheid" %}

#### Global Header & Footer

{% embed url="https://appuniversum.github.io/ember-appuniversum/docs/patterns/au-main-header" %}
Header
{% endembed %}

{% embed url="https://appuniversum.github.io/ember-appuniversum/docs/patterns/au-main-footer" %}
Footer
{% endembed %}

We currently do not use the global header & footer; for tracking and speed reasons.

_Header:_ To integrate smoothly with our codebase and increase speed, we recreated the header in Ember. It appears anytime, anywhere.

_Footer:_ The footer has also been recreated. We only use it on log-in pages, because our application patterns are different.

## Mock-ups

We are currently using a mix of clickable prototypes in Figma, and real prototypes in HTML and CSS. We are also working with other departments to build a solid component library here, both in vectors (Figma) and HTML and CSS.

### Figma

We use Figma, but we do not have a license yet. This is a discussion in progress.

In the meantime, we can base ourselves on the Figma library Mono Company created for creating apps for the Flemish Government.

{% content-ref url="feedback-geven-op-figma-mockups.md" %}
[feedback-geven-op-figma-mockups.md](feedback-geven-op-figma-mockups.md)
{% endcontent-ref %}

## Component libraries

### Webuniversum

{% embed url="https://overheid.vlaanderen.be/webuniversum/v3/" %}

The Flemish Government has built a web component library. We are not currently using it:

* In its current form, the 3.0 version, this library is available when we use their Web platform. Within our application architecture, we do not use that Web platform, and therefore cannot use the Web component library.
* The 3.0 version is not open source. We create open source applications, and thus need open source solution. Our applications are based on their Web components, an older version, when they were still published open source.

### Appuniversum, Webuniversum's Little Sister

To build our applications with, we created an open source component library.

The library is based on the old web components of the Flemish Government, [version 2.0](https://overheid.vlaanderen.be/webuniversum/webcomponenten-versie-2). This is where we built our applications with in the beginning, when they were still published open source. To make sure we could fix bugs, extend the library for specific application components and publish our applications open source, we created Appuniversum. Anyone who wishes to use this library, more specifically in the context of projects for the Flemish Government, may do so.

&#x20;This component library currently consists of two parts: Appuniversum & Ember-Appuniversum.

