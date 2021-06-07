---
description: >-
  An open-source text editor that enriches specific information from minutes
  with data, in a structured way, so that we can extract and reuse that
  information afterwards.
---

# Embeddable & Say-Editor

The Embeddable is a building block of Gelinkt Notuleren. It is a smart, open-source text editor that enriches specific information from minutes with data, in a structured way, so that we can extract and reuse that information afterwards.

Third-party note-taking software that help local boards create minutes, can also reuse this embeddable in their software package to extract the data.

We provide this word processor as an _embeddable_ \(easily plugged in\) for that boards or their software vendors can use in their notetaking packages. We also open up this embeddable under the name of **Say Editor** for anyone who wants to enrich their word processing with knowledge.

To find more detailed information about Say editor, visit [https://say-editor.com/](https://say-editor.com/).

{% embed url="https://say-editor.com/" %}

## Building Blocks

The embeddable consists out of multiple building blocks that make linked note taking possible.

{% embed url="https://www.figma.com/file/kYcCsAHp7rbvrsRE2w1NC0/GN-brainstorm?node-id=623%3A0" %}

### Data sources

We use multiple data sources to enrich notes and minutes

* **The Flemish Codex** – references to the legal grounds in decisions
* **Mandates** – to track attendees, appointing and dismissing
* **Executives** –  to track attendees

### Functionalities & Plugins

We have created separate small apps that can be plugged in the text editor.

* **Toolbar**: basic text editing functionalities.
* **Templates**: to make it easier to start with note taking.
* **Citation plugin**: makes use of the Flemish Codex, and you can use it to reference legal grounds in decisions.
* **Voting**: vote on decisions.
* **Attendees**: track who was part of the meeting, and was part of certain decisions.
* **Import – export**: make sure you can import- and export decisions \(in progress\).
* **Annotations**: annotate text with specific linked information, like mandates
* **Signing**: signing minutes, excerpts, agendas, decision lists.
* **Authentication**: log in via [Gebruikersbeheer](https://gebruikersbeheer.vlaanderen.be/) \(user management ACM-IDM\)
* **Anonymise**: Remove personal information for public view.

Ready the documents of Say Editor to see how they are set up: [https://say-editor.com/docs](https://say-editor.com/docs).

{% embed url="https://say-editor.com/docs" %}



## Code

All of our applications are built in the same way. Read the [Architecture](../../development/architecture/) page before you get started with our repositories.

### Embeddable

{% embed url="https://github.com/lblod/frontend-embeddable-notule-editor" %}

{% embed url="https://github.com/lblod/app-gn-embeddable" %}

### Tutorial: plug in your own smart text editor

Add your own text editor in your ember app:

{% embed url="https://github.com/lblod/say-editor-as-addon-tutorial" %}

### Documentation site Say-Editor

{% embed url="https://say-editor.com/docs" caption="Landing page" %}

{% embed url="https://github.com/lblod/frontend-say-editor-documentation" %}

{% embed url="https://github.com/lblod/app-say-editor-documentation" %}

