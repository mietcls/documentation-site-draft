---
description: This section gives insight in how the scrum teams at Digiteam ABB use Jira.
---

# Jira

## Introduction

Briefly explained, a Jira project is a collection of various issue types \(a backlog\) that represent product development work for the agile product team to pick up during future product increments \(called sprints\).

Which issues \(tickets\) are planned in which increment depends on the product roadmap and the strategy behind it. At various time intervals during the calendar year, the agile product teams determine together the priorities for the near future using techniques such as impact mapping and story mapping.

Issues are being recorded in tickets. Tickets are created and kept in a product backlog. Once they are picked up by the scrum team they follow a particular flow, iterating from one status to another. Jira helps us to visualize the status these tickets are in and to track progress on the tickets along the process flow.

In this section we elaborate on the issue types, the statuses and the flows that are attached to these issue type. In every case there is a 'rationale' behind them that explains why we do the things the way we do them.

## Jira Issue Types

**An epic** is a collection of work to be done on a product to implement a new or improved element of the product. It can best be characterized as a feature of a product that will deliver value for the users of the product and/or the product manager and owner. For the business owners and stakeholders the epic is the key element to monitor the evolution of the product. It has a clear link to a solution, being a 'project' that will introduce a change to one or more products to deliver a particular value \(stream\).

**A user story** is a short, well described element - part of an epic - in which a certain change in the functionality\(ies\) of a product is being recorded. It is very tangible, i.e, the scrum team understand what is asked and how to build it, the tester understands what was asked and can test the delivered functionality accordingly. Later in this section - when describing the flow behind testing and releasing user stories we will further elaborate on this.

A user story can consist of one or many **subtasks** breaking down the work to be done to implement the user story. This is especially useful when various team members need to work together on the implementation. Making arrangements on who will do what and the order in which the things need to be done is a smart thing to do.

As long as we need to 'think' about the content of a user story we are refining the user story. For this we use a **refinement story** issue type in Jira. Refinement is done by whoever is needed to get the requirements, the acceptance criteria, the design and the way we will implement the user story sorted out. Various people can work together during one or more iterations to get the refinement done. The end result is one or more user stories with clear content.

**Technical stories** are reserved for the technical members of the agile teams and are used for purely technical work to be carried out, e.g. optimize hardware, organize back-ups, etc. They are carried out by technical team members and will not be tested and validated by others. 

**Innovation stories** are used to describe innovations where the team will work on during the IPI, the last sprint of a Groeispurt \(program increment\).

**Bugs** are defects that are being logged out of functional testing of the user stories that were delivered by the scrum \(dev\) team. They have a link to the user story they relate to and are usually logged by testers who test the delivered functionalities in coordination with the scrum \(dev\) team and the product owner. The follow a certain flow in Jira. Later in this section - when describing the flow behind testing and releasing user stories we will further elaborate on this.

**Meeting stories** are sometimes used by teams to capture work for long meetings \(e.g. the central planning day\) to make sure capacity is attributed to them. Some product teams use them, other just take into account a 'buffer' of time for meetings while planning tickets in a new sprint.

## Issue statusses and workflows in Jira

When tickets are part of a sprint and they begin to be worked on, their statusses obviously change. In our Jira configuration we defined meaningful statusses and transitions between statusses. Once a ticket is in a particular status, it is showed on one or more boards in a column that contains all tickets in the particular status. In this part we provide you an overview of the statusses and the flow behind them. It will help you understand their lifecycle from creation, refinement, development, testing and release. 

### Workflow and status transitions for user stories

User stories have the most elaborate status transitions flow since they are also used 'as vehicle' in the test and release process. Logically they contain functionalities of the product that need to be tested, \(bugfixed\) and released.

The entire flow from initial status 'BACKLOG' until the final status 'RELEASED TO PRD' looks like this:

![](../../.gitbook/assets/schermafbeelding-2021-09-10-om-09.25.21.png)

#### From backlog into development

Once a user story is planned into a sprint, the user story takes the initial status 'TE DOEN'. As soon as the team starts developing the elements described in the user story the story moves to ACTIEF. In case a \(code\) review is needed after the development is done, the status transitions to PEER REVIEW. Finally, when the team thinks the development of the user story is complete, the status is set to GEREED.

#### From development into \(release and\) testing on TEST

User stories can be submitted for testing. Once one or more stories are completed and the code deployments and configuration changes have been carried out on a testing environment, the dev team \(dev lead - deployment coordinator - individual developer\) changes the status of the user story to 'RELEASED TO TEST'. By changing the status, the user story ticket will appear on a testing board used by our testers. From there on the tester takes it over.

While testing the user story the tester changes the status of the user stories to 'WORDT GETEST'. The result of the testing can either be ok -&gt; status 'GETEST OP TEST' or not ok -&gt; status 'HEROPEND'. If testing is not ok, feedback is provided by the tester in the comment section of the user story and one or more bugs are logged and linked to this user story. The bugs are put in the backlog and await a decision by the product owner and the team on priority and on the question of they need to be taken up in the active sprint or not. The user story remains in the status HEROPEND until all bugs linked to the user story are resolved.

Once all the bugs are resolved the status of the user story can be changed from 'HEROPEND' to 'RERELEASE OP TEST'. This action makes the user story with linked bugs reappear on the testboard of the test team. From here on the same flow applies as described for the initial testing of the user story.

#### Acceptance testing by business stakeholders

After the user stories have been sucessfully tested and validated  on the test environment, they can be tested/ validated for acceptance on a QA or ACC environment. This is an environment that acts as a representative staging area for the production environment where the code ultimately needs to be released and found to be working as expected.

A similar flow is being used as for the initial testing of the user story on the \(first\) TEST environment but with ACC instead of TEST. Once the acceptance testing of the user stories is completed on ACC, the status of the user story is changed - by the tester/ business stakeholder to 'GETEST op ACC'. This leaves the user story in the final but one state. It is up to the release coordinator, changeman to bring the code into production and after doing so change the status to 'RELEASED TO PRD'.

### Workflows and statusses for all other issue types in Jira

All other issue types in Jira, described above, share the same process flow. This process flow is less elaborate than the one being used for user stories. This is because we do not expect any testing to be done on other issue types so we do not need the issues to evolve to a status after 'GEREED'. Therefore the share flow and statusses for all other issue types in Jira looks like:

![](../../.gitbook/assets/schermafbeelding-2021-09-10-om-12.42.27.png)

## Template for a user story

A user story is a short, well described element - part of an epic - in which a certain change in the functionality\(ies\) of a product is being recorded. It is very tangible, i.e, the scrum team understand what is asked and how to build it, the tester understands what was asked and can test the delivered functionality accordingly. 

**ABB-template for a user story**

**Short title** 

Korte, kernachtige titel die de \(User\) Story in treffend verwoord. Deze korte titel is nodig in functie van de weergave in Jira waar slechts een beperkt aantal karakters waarmee de \(User\) Story begint worden getoond. Doel van de korte titel is de \(User\) Story makkelijk terug vinden in overzichtslijsten getoond in JIRA. 

**Long title**

Volledige titel van de \(User\) Story. Deze titel kan de klassieke \(User\) Story terminologie bevatten zoals “ Als gebruiker van de toepassing kan ik … zodat… ”  

**Link to the epic**

A user story is \(always linked\) to an epic. All the user stories that are linked to an epic \(as children of the epic\) form the 'feature' of the application part that will be built and released. When a user story is **ready** it can or may be tested. When all the user stories of an epic are completed the entire feature must be tested and validated before the epic can be marked as **done**.

**Context**

De context rubriek geeft meer achtergrond en duiding bij de \(User\) Story. Hiervoor kan verwezen worden naar de beschrijving van de Epic waar de \(User\) Story toe behoort. Klassiek wordt in de Epic de reden toegelicht waarom de \(User\) Stories werden gecreëerd. Daarnaast kan de context ook informatie bevatten hoe de \(User\) Story in kwestie zich verhoudt tot andere \(User\) Stories, al of niet in dezelfde Epic. De context bevat nuttige informatie voor de lezer van de \(User\) Story over het waarom \(van waar komt de vraag?\) en de prioriteit die aan de \(User\) Story werd gegeven door de Product Manager.

**Decription**

De beschrijving van de \(User\) Story bevat alle nodige informatie voor het team dat de \(User\) Story dient uit te voeren. Deze informatie verschilt naargelang het type \(User\) Story en de specifieke inhoud ervan. Enige vereiste daar is dat de informatie die hierin wordt opgenomen op zijn minst een keer werd nagelezen door het team dat de \(User\) Story moet uitvoeren. In de beschrijving komt een duidelijke beschrijving van de scope met daarnaast de nodige inhoudelijke informatie zoals gebruikersbehoeften, schermontwerpen, sequentiediagrammen, informatiemodellen, niet-functionele vereisten, contextdiagrammen, ...

**Definition of Ready**

Deze rubriek bevat een duidelijke omschrijving van alle voorwaarden waaraan de uitvoering van de \(User\) Story moet voldoen om deze als klaar te kunnen aanduiden. Het is als het ware een controlelijst om bij oplevering van de \(User\) Story te kunnen beoordelen of de \(User\) Story helemaal afgewerkt is. 

**Out of Scope**

In vele gevallen is het - naast het uitdrukkelijk omschrijven van wat er in scope zit van de \(User\) Story - ook nuttig om expliciet neer te schrijven wat er niet in scope is. Dit moet vrije interpretaties van de scope tijdens de uitvoeringsfase vermijden, zeker in geval de beschrijving van wat er in scope is ruimte voor interpretatie zou laten.

**Attachments**

Eventuele documenten of externe informatiebronnen waar naar verwezen wordt in de \(User\) Story, dit kunnen bijvoorbeeld technische standaarden zijn of verslagen, gebruikersbevragingen, onderzoeken, mock-up schermen, user flows, etc. 

**Labels** \(= trefwoorden of tags\)

Trefwoorden toekennen \(uit een voorafbepaalde lijst bij ABB of zelf bedacht\) biedt het voordeel dat hierop filters kunnen toegepast worden wat het bundelen en opzoeken van \(User\) Stories en het communiceren over \(User\) Stories met anderen vergemakkelijkt. Verder in dit document is een ABB-trefwoordenlijst voor \(User\) Stories opgenomen waar trefwoorden uit gebruikt kunnen worden.

