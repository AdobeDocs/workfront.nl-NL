---
product-area: documents
navigation-topic: approvals
title: Overzicht van de evaluatie en goedkeuring van bedrijfsmiddelen
description: Meer weten over de formele beoordelings- en goedkeuringsprocedure in Workfront?
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: 68b91aad-af76-473f-861d-da846fdfb84c
source-git-commit: 7e970f4f707937a62f68c191a7cbd5dfa26e471c
workflow-type: tm+mt
source-wordcount: '909'
ht-degree: 0%

---

# Overzicht van de evaluatie en goedkeuring van bedrijfsmiddelen

De nieuwe workflow voor het beoordelen en goedkeuren van bedrijfsmiddelen is gebaseerd op een verregaande integratie tussen Workfront en Frame.io. Deze integratie neemt het beste van wat elk product moet aanbieden en combineert het om een ervaring tot stand te brengen die alle mensen die betrokken bij de verwezenlijking van inhoud om in hun hulpmiddelen van keus, terwijl het hebben van toegang tot commentaren, dossiers, en statusupdates die over beide systemen in echt - tijd worden gesynchroniseerd.

Zie voor meer informatie over Frame.io [Aan de slag met Frame.io](https://support.frame.io/en/collections/49298-getting-started).

## Starten en plannen van werkzaamheden in Workfront

De beheerder van Workfront laat de integratie tussen Workfront en Frame.io toe door de standaardrekening Frame.io in het gebied van de Opstelling te vormen en dan gebruikers Frame.io in Workfront aan te wijzen. Op die manier kan de coördinator met behulp van Workfront-projecten en formele evaluatie en goedkeuring werkzaamheden plannen en op gang brengen.

### Een standaard Frame.io-account configureren

Workfront-beheerders starten de integratie met Workfront en Frame.io door een standaard Frame.io-account toe te voegen in het gedeelte Setup van Workfront. Zodra een standaardrekening Frame.io opstelling is, leidt de integratie tot verbonden projecten tussen Workfront en Frame.io.

Zie voor meer informatie [].

<!-- in procedure article we need to cover how groups work with projects and how the frame account is associated with a group. And that accounts other than the default can be added on a 1:1 basis using the dev token. -->

### Gebruikers van Frame.io inschakelen

Workfront-gebruikers die regelmatig Frame.io gebruiken, moeten worden gemarkeerd als Frame.io-gebruikers. Workfront-beheerders kunnen Frame.io-gebruikers aanwijzen in het Workfront-gebruikersprofiel.

Wanneer een gebruiker duidelijk als gebruiker Frame.io in Workfront is en aan een project wordt toegevoegd,

* Ze worden als deelnemer toegevoegd aan Frame.io
* Ze kunnen elementen van Frame.io naar Workfront sturen voor formele controle en goedkeuring

>[!TIP]
>
>We raden gebruikers aan die regelmatig met creatieve gereedschappen werken, middelen te uploaden om deze te beoordelen en goed te keuren als gebruikers van Frame.io.


Zie voor meer informatie [].

![](assets/Frame-enabled-user.png)


### Een project maken dat is verbonden met Frame.io

Zodra de standaardrekening Frame.io wordt toegevoegd en de gebruikers Frame.io worden aangewezen, kunnen de projectcoördinatoren Workfront projecten tot stand brengen die met Frame.io worden verbonden. Wanneer u een verbonden project maakt, kunt u

* **Frame.io-gebruikers toewijzen aan taken**: Gebruikers met Frame.io-functionaliteit worden via e-mail op de hoogte gesteld wanneer zij aan een taak zijn toegewezen. Er moet dus een taak worden voltooid.
* **Deel het project met Gebruikers Frame.io**: De projecten die met Frame.io toegelaten gebruikers worden gedeeld verlenen hen toegang tot het project binnen Frame.io.
* **Creatieve materialen delen met Frame.io**: U kunt instructies en materialen van Workfront rechtstreeks naar de creatieve gebruiker in Frame.io verzenden via een eenrichtingsprojectmap voor synchronisatie.
* **Taakvoortgang volgen**: Creatieve personen kunnen voltooide middelen en markeringstaken verzenden zonder Frame.io te verlaten.

Zie voor meer informatie [].

<!--Preassign approval templates to tasks coming in the future-->


## Inhoud maken en samenwerken in Frame.io

Creatieve personen kunnen hun keuze blijven maken en de vrijheid hebben om collegiale beoordelingen te maken, te herhalen en uit te voeren in Frame.io.

Wanneer creatief wordt toegevoegd aan een verbonden project, kunnen zij het volgende doen zonder Frame.io te verlaten:

* Toegangsinstructies van de projectcoördinator
* informele peer reviews uitvoeren
* Voltooide middelen naar Workfront verzenden voor formele controle en goedkeuring
* De status van een taak wijzigen of markeren als deze is voltooid
<!-- * Notification of decision
* Upload new versions of connected assets marked as needs more work < will automatically connect>-->

Zie voor meer informatie over het controleren van elementen in Frame.io

## Elementen controleren en goedkeuren

Als een creatief bedrijf eenmaal een voltooid middel van Frame.io naar Workfront verzendt, kan de projectcoördinator het formele beoordelings- en goedkeuringsproces in Workfront starten.

Nadat de goedkeuring is gemaakt, gaan gebruikers terug naar Frame.io om opmerkingen over het element te plaatsen en het element op te halen. Zij kunnen een goedkeuringsbesluit in de kijker Frame.io ook nemen.

### In Workfront formele beoordelingen en goedkeuringen starten

Projectcoördinatoren kunnen eenmalige beoordelingen en goedkeuringen of herbruikbare goedkeuringssjablonen maken in het gedeelte Setup van Workfront. Alle controle- en goedkeuringsactiviteiten die in Frame.io worden uitgevoerd, worden ook in Workfront geregistreerd.

De projectcoördinatoren kunnen revisoren, fiatteurs of een combinatie van beide toewijzen:

* **Revisoren** U kunt opmerkingen plaatsen over elementen en markeringen maken. Als ze klaar zijn, kunnen ze de revisie als voltooid markeren. <!--example of when to add reviewers-->
* **Fiatteurs** kan opmerkingen plaatsen over opmaakelementen. Zij moeten een besluit nemen om het goedkeuringsproces vooruit te helpen.



Alle opmerkingen die in Frame.io worden gemaakt, worden weergegeven op het tabblad Updates in Workfront. Reacties in Workfront worden niet weergegeven in Frame.io.

Opmerkingen met de markering Alleen team worden niet weergegeven op het tabblad Workfront-updates.

Revisoren en fiatteurs kunnen worden toegevoegd aan sjablonen voor eenmalig gebruik of goedkeuring:

<!--can also assign teams and set deadline-->

* **Goedkeuring voor eenmalig gebruik**: Goedkeuringstermijnen instellen

* **Goedkeuringssjablonen**
In het gedeelte Workfront Setup kunnen gebruikers met een standaardlicentie herbruikbare goedkeuringssjablonen maken. In een sjabloon kunnen gebruikers een tijdframe opgeven en revisoren en fiatteurs toevoegen. <!--do we want to mention any upcoming plans here? -->

  Nadat een sjabloon is gemaakt, kan deze worden toegepast op elementen die vanuit Frame.io worden verzonden om het formele beoordelings- en goedkeuringsproces in Workfront te starten.
  ![](assets/assign-template.png)

<!-- can set timreframe which calculates deadline once approval is started. >

    For more information, see [Create and manage Approval Templates](/)<!--don't forget link-->

* Middelen van Workfront uploaden en naar het frame verzenden voor revisie en goedkeuring - Binnenkort beschikbaar?

### Elementen goedkeuren in Frame.io

Met Frame.io verbonden betrokkenen kunnen gegevens bekijken en goedkeuren in de Frame.io-viewer met opmerkingen die worden gesynchroniseerd met de updatestream van Workfront, beslissingen enzovoort.

<!-- include screenshot from frame.io-->

Als u uitsluitend in Frame werkt, kunt u via e-mail op de hoogte worden gesteld van een aanvraag.

Als u alleen in Workfront werkt, kunt u thuis de goedkeuringswidget gebruiken.

u kunt tot Frame.io kijker van toegang hebben wanneer u werkt

**Elementen van Frame.io goedkeuren**
de wijze van kennisgeving

een besluit nemen - goedkeuren , goedkeuren met wijzigingen , werk nodig maken

**Middelen van Workfront goedkeuren**
de wijze van kennisgeving

Home in afwachting van mijn goedkeuringswidget

E-mail - deadline e-mails 72, 24 en op deadline.

Externe WF-gebruikers wordt gevraagd om een aanmelding voor een frame te maken

Als het element geen verbonden kader is, kunnen zij duimnagel in WF bekijken en commentaarstroom gebruiken. Besluiten tot herziening en goedkeuring kunnen worden genomen.

<!-- upload assets directly to workfront to be reviewed in Frame.io/ Will have to send manually at first

Reviewer/approver needs to go through email to get to frame vier
-->


### Metrische gegevens voor beoordeling en goedkeuring bijhouden

Snelheidsrapport voor widgets in thuisgoedkeuring?

<!--
### Published approved assets to Adobe Experience Manager Assets

Use the native integration to send approved assets to AEM.
-->


## Voorbeeld van een workflow voor het goedkeuren van campagneelementen

intro para?

![](assets/example-workflow.png) <!-- probbly need a different version of this but add something similar rather than typing all out?-->
