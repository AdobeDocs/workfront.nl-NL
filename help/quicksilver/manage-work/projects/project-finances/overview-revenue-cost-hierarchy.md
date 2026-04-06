---
content-type: overview
product-area: projects
navigation-topic: financials
title: Overzicht van de inkomsten- en kostenhiërarchie
description: Dit artikel schetst het geleidelijke proces om de aangewezen facturerings en kostentarieven voor baanrollen en gebruikers voor het de opbrengsttype en het kostentype van de Uur van de Gebruiker en van de Rol te bepalen.
author: Lisa
feature: Work Management
exl-id: 623828fb-e1ac-4cae-8b9f-567a6f8cb7ae
source-git-commit: 3a194bc2b2707c7b7e1cd5edffc3dd5ab43e91b3
workflow-type: tm+mt
source-wordcount: '3604'
ht-degree: 0%

---

# Overzicht van inkomsten en kostenhiërarchie

{{highlighted-preview-article-level}}

{{ultimate-package}}

Om precieze financiële berekeningen te kunnen maken, gebruikt Workfront de juiste factureringssnelheden bij het berekenen van de inkomsten van een taak of project. De rol en de gebruikerstarieven moeten op alle niveaus duidelijk gedefinieerd zijn om nauwkeurige financiële berekeningen te kunnen maken.

De secties in dit artikel schetsen het geleidelijke proces om de aangewezen facturerings en kostentarieven voor baanrollen en gebruikers voor het de opbrengsttype en het kostentype van de Gebruiker en van de Rol te bepalen.

>[!NOTE]
>
>De tariefhiërarchie die in dit artikel wordt getoond wordt gebruikt slechts wanneer de opbrengst van de Uur van de Gebruiker en van de Rol of kostentype op de taak wordt toegepast.

Voor meer informatie over het factureren van tarieven, opbrengsttypes, en hoe de opbrengst wordt berekend, zie [&#x200B; Overzicht van het Factureren en de Ontvangsten &#x200B;](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Uitzonderingen voor de hiërarchie en het de opbrengsttype van de Gebruiker en van de Rol.

* Bedrijfstarieven worden niet ondersteund binnen de hiërarchie.
* Alleen de primaire rol wordt gebruikt voor de hiërarchische berekeningen. Andere rollen worden niet gebruikt.
* Wanneer het de opbrengsttype van een taak Gebruiker en Rol Hourly is, kan een gebruiker die uren op de taak heeft het programma geopend niet van die taak worden unassigned.

## Overzicht van effectieve datums

Workfront-beheerders kunnen desgewenst effectieve datums instellen die bepalen wanneer factureringstarieven, kostentarieven en andere financiële kenmerken in het systeem van kracht worden. Een taakrol of gebruiker kan bijvoorbeeld een standaardfactureringsfrequentie van $50 hebben. Met effectieve datums zou het tarief van $50 kunnen worden ingesteld om op 31 maart te verlopen, en een nieuw tarief van $55 zou automatisch op 1 April beginnen.

Voor de berekening van de geplande inkomsten zijn de factureringstarieven gebaseerd op de datum van de geplande uren. De geplande uren worden gelijkmatig verdeeld over de taakduur. Gebruikend het vorige voorbeeld, gebruiken de uren die voor 31 Maart of vroeger worden gepland $50 tarief, en de uren die voor 1 April worden gepland of later $55 tarief gebruiken.

Voor daadwerkelijke opbrengstberekeningen, zijn de het factureringspercentages gebaseerd op de datum voor de geregistreerde uren. Gebruikend het vorige voorbeeld, gebruiken de uren het programma werden geopend op 31 Maart of vroeger het tarief $50, en de uren het programma geopend op 1 April of later gebruiken het tarief $55.

>[!NOTE]
>
>Taken worden niet toegewezen met effectieve datums. In plaats daarvan, trekken de taken de toepasselijke tarieven van het systeem, of van een tariefkaart, een gebruikersprofiel, of een opdracht-vlakke opheffing. Effectieve datums zorgen ervoor dat de juiste frequentie wordt toegepast op basis van de timing van de werkzaamheden, maar ze bepalen niet rechtstreeks de toewijzingen.

## Overzicht van de functie die voor facturering wordt gebruikt

A **baanrol voor het factureren** wordt geplaatst voor een gebruiker op het taakniveau of het projectniveau. Het is alleen van toepassing op gebruikers en kan niet worden gebruikt voor andere functies. De primaire functie van een gebruiker is bijvoorbeeld Designer, maar op één taak of project fungeren ze als Senior Designer en het percentage moet dat weerspiegelen.

Een taakrol op toewijzingsniveau voor facturering is alleen voor die specifieke toewijzing en wordt niet automatisch toegepast op de andere toewijzingen van de gebruiker. Een de baanrol op projectniveau voor het factureren is op alle taken van de gebruiker op dat project van toepassing. U kunt deze desgewenst op het afzonderlijke toewijzingsniveau overschrijven.

Wanneer een baanrol voor het factureren op of de gebruikerstaak of het projectniveau wordt toegepast, kan het tarief verbonden aan de baanrol voor het factureren in plaats van de gebruikers of baanroltarieven in opbrengstberekeningen worden gebruikt. De baanrol voor het factureren is slechts beschikbaar wanneer het de opbrengsttype van de Uur van de Gebruiker en van de Rol wordt gebruikt.

>[!NOTE]
>
>Terwijl een gebruiker met een verschillende rol voor factureringsdoeleinden kan handelen, blijven de kostenberekeningen hun primaire baanrol gebruiken. De functie voor facturering is alleen van invloed op factureringsberekeningen.

Voor meer informatie, zie [&#x200B; Opstelling een baanrol voor het factureren &#x200B;](/help/quicksilver/manage-work/projects/project-finances/set-up-job-role-for-billing.md).

## Overzicht van de bewaarde rentevoeten

De **informatie van de het facturerings van het project** vlag op een project controleert of het systeem de factureringsinformatie voor taken in de tijd gebruikt wanneer de tariefkaart wordt gebeëindigd, of wijzigingen toestaat die op veranderingen tijdens de loop van het project worden gebaseerd. Wijzigingen in de rol, het salaris, de tariefkaart of andere factureringsgerelateerde informatie van de gebruiker hebben geen invloed op de factureringssnelheden voor toewijzingen. De tarieven blijven behouden op basis van de laatste tariefkaart op het moment dat de projectvlag werd geactiveerd. Deze toewijzingseigenschappen (zoals de functie en het salaris) worden nog steeds bijgewerkt, zodat de werkelijke kosten van de toewijzing correct zijn.

Wanneer de vlag wordt aangezet, sluit het systeem de datum-efficiënte het factureringspercentages (die op de gefinaliseerde tariefkaart in bijlage aan het project worden geplaatst) voor de duur van het project.

De vlag kan op een project worden geactiveerd wanneer het werk is begonnen en taken en uren reeds bestaan. Op dat moment:

* Het definitieve goedgekeurde tarief kaarttarief wordt de bron van het factureren tarieven voor alle projecttaken.
* Alle vroegere, huidige, en toekomstige taken worden opnieuw berekend gebruikend de definitieve goedgekeurde tarieven.
* Werkelijke en geplande waarden worden opnieuw berekend.

>[!NOTE]
>
>Als de vlag is ingeschakeld om de factureringssnelheden te behouden, kan deze niet worden uitgeschakeld tenzij het project geen toewijzingen en geen uren heeft. Dit zorgt ervoor dat alle financiële verslaggeving de ware contractuele tarieven weerspiegelt.
>Wanneer de vlag weg is, staat het systeem toe dat de het facturerings tarieven worden opnieuw berekend of dynamisch aangepast. Wijzigingen in de rol, het salaris of de factureringssnelheid van de gebruiker worden direct weerspiegeld in de factureringssnelheid van de toewijzing.

Voor meer informatie, zie [&#x200B; projecten &#x200B;](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md) uitgeven en [&#x200B; tariefkaarten &#x200B;](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md) beheren.

## Geplande inkomsten - Uur gebruiker en rol

Wanneer het opbrengsttype op de taak Gebruiker en Rol Hourly is, gebruikt Workfront zowel gebruiker als het tariefhiërarchieën van de baanrol om het factureringstarief voor geplande opbrengst te bepalen.

Dit beeld toont de stroom van de geplande opbrengsthiërarchie:

![&#x200B; Geplande Inkomsten voor Gebruiker en Rol het type van opbrengst van de Uur &#x200B;](assets/planned-revenue-chart.png)

Wanneer een gebruiker aan de taak wordt toegewezen, zoekt Workfront volgens deze hiërarchie:

1. Het systeem zoekt eerst naar een bewaarde snelheid bij de toewijzing voor de gebruiker.

   Een bewaarde tarief volgt nog de hiërarchie, maar het tarief wordt bevroren wanneer het project wordt bewaard. Voor meer informatie, zie [&#x200B; Overzicht van bewaarde tarieven &#x200B;](#overview-of-preserved-rates).

1. Vervolgens zoekt het systeem naar de factureringsfrequentie op een tariefkaart, voor de primaire taakrol of de taakrol voor het factureren van de gebruiker die aan de taak is toegewezen. Als een tarief bestaat en het gesloten is, dan wordt dat tarief gebruikt in de opbrengstberekening.

   Als een tarief op de tariefkaart bestaat en het ontgrendeld is, dan gebruikt het systeem niet dat tarief en zoekt naar het volgende tarief in de hiërarchie.

1. Vervolgens zoekt het systeem naar de overschrijvingssnelheid op toewijzingsniveau voor de gebruiker. Dit is een handmatig toegevoegde snelheid die is gekoppeld aan de specifieke toewijzing en negeert alle andere snelheden voor de gebruiker bij deze toewijzing (behalve een snelheid die is vergrendeld met een creditcard). Indien een percentage wordt gevonden, wordt dat percentage gebruikt bij de berekening van de opbrengsten.
1. Vervolgens zoekt het systeem naar een taakrol voor facturering op taaktoewijzingsniveau.

   De taakrol voor facturering is alleen voor een specifieke toewijzing en is van toepassing op de toewijzing in plaats van de primaire taakrolsnelheid van de gebruiker. De primaire functie van een gebruiker is bijvoorbeeld Designer, maar in één taak fungeren ze als Senior Designer met een hogere factureringsgraad.

   Workfront zoekt naar de functie voor factureringspercentage:

   * Het systeem zoekt eerst naar de factureringsgraad van de functie voor facturering van de taak (in het voorbeeld Senior Designer), rekening houdend met effectieve datums. U zult dit op de Tarieven > het Factureren gebied van het project, in Source van het a **Tarief zien: Overschrijvingen > Type van Middel: De Rol van de Taak** groeperen. Dit is een overschrijvingstarief voor het project.
   * Vervolgens zoekt het systeem naar de taakrol voor het factureringspercentage van een betaalkaart, rekening houdend met effectieve datums. U zult dit op de Tarieven > het Facturerings gebied van het project, in Source van het a **Tarief zien: De Bijgesloten Kaart van het Tarief > het Type van Middel: De Rol van de Taak** groeperen.
   * Als het tarief voor de baanrol voor het factureren niet op het project of op de tariefkaart is, zoekt het systeem het systeem-vlakke baanroltarief (Hogere Designer in het voorbeeld), met inachtneming van effectieve data.
   * Als een baanrol voor het factureren wordt toegewezen, en geen van de tarieven van de vorige stappen worden gevonden, is het het factureringspercentage 0.

     >[!NOTE]
     >
     >Wanneer een baanrol voor het factureren wordt toegewezen, maar het het factureringstarief is 0, is dit een indicator om de tariefopstelling opnieuw te bekijken. Een percentage van 0 betekent dat er in Workfront geen tarieven voor die functie zijn vastgesteld (in het voorbeeld Senior Designer). U moet ofwel tarieven voor de rol van de taak toevoegen, ofwel de rol van de taak voor facturering uit de toewijzing verwijderen.
     >
     >Omdat de taken baanroltarieven van het project erven wanneer die tarieven op het projectniveau beschikbaar zijn, zouden om het even welke tarieven van een onderzoek naar de baanrol voor het factureren op het project reeds gevestigd zijn wanneer Workfront op de baanrol voor het factureren op het niveau van de taaktaak zocht. Het project-vlakke onderzoek naar een baanrol voor het factureren blijft in de onderzoekshiërarchie.

1. Als een baanrol voor het factureren niet beschikbaar op het niveau van de taaktaak was, zoekt het systeem dan het factureringspercentage op het project, voor de specifieke gebruiker die aan de taak wordt toegewezen, rekening houdend effectieve data. U zult dit op de Tarieven > het Factureren gebied van het project, in Source van het a **Tarief zien: Overschrijvingen > Type van Middel: Gebruiker** groeperen. Dit is een overschrijvingstarief voor het project.
1. Vervolgens zoekt het systeem naar de factureringssnelheid op systeemniveau op het profiel van de gebruiker, rekening houdend met effectieve datums.
1. Vervolgens zoekt het systeem naar de factureringssnelheid van de primaire taakrol van de gebruiker (Designer in het voorbeeld).

   * Het systeem zoekt eerst naar het factureringspercentage voor het project, voor de primaire functie van de gebruiker, rekening houdend met effectieve datums. U zult dit op de Tarieven > het Factureren gebied van het project, in Source van het a **Tarief zien: Overschrijvingen > Type van Middel: De Rol van de Taak** groeperen. Dit is een overschrijvingstarief voor het project.
   * Vervolgens zoekt het systeem naar het aantal taken met een tariefkaart, rekening houdend met effectieve datums. U zult dit op de Tarieven > het Facturerings gebied van het project, in Source van het a **Tarief zien: De Bijgesloten Kaart van het Tarief > het Type van Middel: De Rol van de Taak** groeperen.
   * Vervolgens zoekt het systeem naar het taakrolpercentage op systeemniveau, rekening houdend met effectieve datums.

1. Als geen van deze tarieven wordt gevonden, is het factureringstarief 0.

Wanneer een gebruiker niet aan de taak wordt toegewezen, zoekt Workfront de baan roltarieven volgens deze hiërarchie:

1. Het systeem zoekt eerst naar een behouden percentage bij de toewijzing voor de taakrol.
1. Het systeem zoekt naar de factureringssnelheid op een tariefkaart, voor de taakrol die aan de taak wordt toegewezen. Als een tarief bestaat en het gesloten is, dan wordt dat tarief gebruikt in de opbrengstberekening.

   Als een tarief op de tariefkaart bestaat en het ontgrendeld is, dan gebruikt het systeem niet dat tarief en zoekt naar het volgende tarief in de hiërarchie.

1. Vervolgens zoekt het systeem naar de taakoverschrijvingstarief voor de taakrol. Dit is een handmatig toegevoegde snelheid voor de rol van de taak in de specifieke toewijzing en overschrijft alle andere tarieven voor de rol van de taak in deze taak. Indien een percentage wordt gevonden, wordt dat percentage gebruikt bij de berekening van de opbrengsten.
1. Vervolgens zoekt het systeem naar de factureringsfrequentie voor de taakrol die aan de taak is toegewezen.

   * Het systeem zoekt eerst naar het factureringspercentage voor het project voor de functie, rekening houdend met effectieve datums. U zult dit op de Tarieven > het Factureren gebied van het project, in Source van het a **Tarief zien: Overschrijvingen > Type van Middel: De Rol van de Taak** groeperen. Dit is een overschrijvingstarief voor het project.
   * Vervolgens zoekt het systeem naar het aantal taken met een tariefkaart, rekening houdend met effectieve datums. U zult dit op de Tarieven > het Facturerings gebied van het project, in Source van het a **Tarief zien: De Bijgesloten Kaart van het Tarief > het Type van Middel: De Rol van de Taak** groeperen.
   * Vervolgens zoekt het systeem naar het taakrolpercentage op systeemniveau, rekening houdend met effectieve datums.

1. Als geen van deze tarieven wordt gevonden, is het factureringstarief 0.

## Werkelijke inkomsten - Uur gebruiker en rol

Wanneer het opbrengsttype op de taak Gebruiker en Rol Hourly is, gebruikt Workfront twee hiërarchieën om het factureringstarief voor daadwerkelijke opbrengst te bepalen. De factureringssnelheid is gebaseerd op de aanmelduren van de gebruiker op een taak.

De &quot;gebruiker&quot;in de hiërarchieën is de persoon die aan de taak wordt toegewezen. De &quot;eigenaar&quot;is de persoon van wie tijd tegen de taak wordt geregistreerd, zelfs als zij niet aan de taak worden toegewezen. Michael wordt bijvoorbeeld toegewezen aan een taak, maar Joanna voltooit het werk omdat Michael ziek was. De manager kan de tijd tegen de taak registreren en de eigenaar van de geregistreerde uren aan Joanna plaatsen. De geplande opbrengstwaarden zijn gebaseerd op de taak en de tarief van Michael in de hiërarchie, maar de Ware opbrengstwaarden zijn gebaseerd op het tarief van Joanna.

Deze afbeelding toont de stroom van de eigenlijke inkomstenhiërarchie:

![&#x200B; Ware Ware Inkomsten voor Gebruiker en Rol het kostentype van de Uur &#x200B;](assets/actual-revenue-chart.png)

### Wanneer de eigenaar van de geregistreerde uren en de toegewezen gebruiker op de taak het zelfde zijn

Workfront zoekt eerst naar een factureringssnelheid op basis van de gebruikerstoewijzing. Als een gebruiker niet aan de taak wordt toegewezen, dan zoekt het naar een het factureren tarief door de baan roltoewijzing.

De hiërarchie voor dit scenario is het zelfde als de geplande opbrengsthiërarchie. Zie [&#x200B; Geplande opbrengst - Gebruiker en Rol Uur &#x200B;](#planned-revenue--user-and-role-hourly) voor dit werkschema.

### Wanneer de eigenaar van de geregistreerde uren niet de toegewezen gebruiker op de taak is

Workfront zoekt in de gebruikerseigenschappen van de eigenaar volgens deze hiërarchie:

1. Het systeem zoekt eerst naar een bewaarde snelheid bij de toewijzing voor de eigenaar.
1. Vervolgens zoekt het systeem naar de factureringssnelheid op een tariefkaart, voor de primaire functie van de eigenaar. Als een tarief bestaat en het gesloten is, dan wordt dat tarief gebruikt in de opbrengstberekening.

   Als een tarief op de tariefkaart bestaat en het ontgrendeld is, dan gebruikt het systeem niet dat tarief en zoekt naar het volgende tarief in de hiërarchie.

1. Vervolgens zoekt het systeem naar het factureringspercentage voor het project, voor de eigenaar, rekening houdend met effectieve data. U zult dit op de Tarieven > het Facturerings gebied van het project, in een Tarief Source zien: Met voeten treedt > het Type van Middel: De groepering van de Gebruiker. Dit is een overschrijvingstarief voor het project.
1. Vervolgens zoekt het systeem naar een taakrol voor facturering op projectniveau.

   De baanrol voor het factureren is slechts voor een specifiek project en is op het project van toepassing in plaats van het primaire baanroltarief van de eigenaar. De primaire functie van de eigenaar is bijvoorbeeld Designer, maar in één project fungeren ze als Senior Designer met een hogere factureringsgraad.

   Workfront zoekt naar de functie voor factureringspercentage:

   * Het systeem zoekt eerst naar de taakrol voor het factureringspercentage van een tariefkaart, rekening houdend met effectieve datums. U zult dit op de Tarieven > het Facturerings gebied van het project, in Source van het a **Tarief zien: De Bijgesloten Kaart van het Tarief > het Type van Middel: De Rol van de Taak** groeperen.
   * Als het tarief voor de baanrol voor het factureren niet op de tariefkaart is, zoekt het systeem het systeem-vlakke baanroltarief (Hogere Designer in het voorbeeld), met inachtneming van effectieve data.
   * Als een baanrol voor het factureren wordt toegewezen, en geen van de tarieven van de vorige stappen worden gevonden, is het het factureringspercentage 0.

     >[!NOTE]
     >
     >Wanneer een baanrol voor het factureren wordt toegewezen, maar het het factureringstarief is 0, is dit een indicator om de tariefopstelling opnieuw te bekijken. Een percentage van 0 betekent dat er in Workfront geen tarieven voor die functie zijn vastgesteld (in het voorbeeld Senior Designer). U zou of tarieven voor de baanrol moeten toevoegen, of de baanrol voor het factureren van het project schrappen.

1. Vervolgens zoekt het systeem naar de factureringssnelheid op systeemniveau op basis van het gebruikersprofiel van de eigenaar, rekening houdend met effectieve datums.
1. Vervolgens zoekt het systeem naar de factureringsgraad van de primaire functie van de eigenaar (Designer in het voorbeeld).

   * Het systeem zoekt eerst naar het factureringspercentage voor het project, voor de primaire functie van de eigenaar, rekening houdend met effectieve datums. U zult dit op de Tarieven > het Factureren gebied van het project, in Source van het a **Tarief zien: Overschrijvingen > Type van Middel: De Rol van de Taak** groeperen. Dit is een overschrijvingstarief voor het project.
   * Vervolgens zoekt het systeem naar het aantal taken met een tariefkaart, rekening houdend met effectieve datums. U zult dit op de Tarieven > het Facturerings gebied van het project, in Source van het a **Tarief zien: De Bijgesloten Kaart van het Tarief > het Type van Middel: De Rol van de Taak** groeperen.
   * Vervolgens zoekt het systeem naar het taakrolpercentage op systeemniveau, rekening houdend met effectieve datums.

1. Als geen van deze tarieven wordt gevonden, is het factureringstarief 0.

## Geplande kosten - Uur gebruiker en Rol

Wanneer het kostentype op de taak Gebruiker en Rol Hourly is, gebruikt Workfront zowel gebruiker als het tarief van het baanroltarief hiërarchieën om het tarief voor geplande kosten te bepalen.

Deze afbeelding toont de stroom van de geplande kostenhiërarchie:

![&#x200B; Geplande Kosten voor Gebruiker en Rol het kostentype van de Uur &#x200B;](assets/planned-cost-chart.png)

Wanneer een gebruiker aan de taak wordt toegewezen, zoekt Workfront volgens deze hiërarchie:

1. Het systeem zoekt naar de taakoverschrijvingstarief voor de gebruiker. Dit is een manueel toegevoegde tarief voor de gebruiker op de specifieke taak en treedt alle andere tarieven voor de gebruiker op deze taak met voeten. Indien een percentage wordt gevonden, wordt dat percentage gebruikt bij de kostenberekening.
1. Vervolgens zoekt het systeem naar het kostenpercentage voor het project, voor de specifieke gebruiker die aan de taak is toegewezen, rekening houdend met effectieve datums. U zult dit op het gebied van Tarieven > Kosten van het project, in Source van het a **Tarief zien: Overschrijvingen > Type van Middel: Gebruiker** groeperen. Dit is een overschrijvingstarief voor het project.
1. Vervolgens zoekt het systeem naar het kostenpercentage op systeemniveau voor het profiel van de gebruiker, rekening houdend met effectieve datums.
1. Daarna, zoekt het systeem het kostentarief van de primaire baanrol van de gebruiker met de toegewezen attributencombinatie, die op de attributenscore wordt gebaseerd.
1. Als geen van deze tarieven wordt gevonden, is het kostenpercentage 0.

Wanneer een gebruiker niet aan de taak wordt toegewezen, zoekt Workfront de tarieven van de baanrolkosten volgens deze hiërarchie:

1. Het systeem zoekt naar de taakoverschrijvingstarief voor de taakrol. Dit is een handmatig toegevoegde snelheid voor de rol van de taak in de specifieke toewijzing en overschrijft alle andere tarieven voor de rol van de taak in deze taak. Indien een percentage wordt gevonden, wordt dat percentage gebruikt bij de kostenberekening.
1. Daarna, zoekt het systeem het systeem-vlakke kostentarief van de baanrol met de toegewezen attributencombinatie, die op de attributenscore wordt gebaseerd, die efficiënte data in aanmerking nemen.
1. Als geen van deze tarieven wordt gevonden, is het kostenpercentage 0.

## Werkelijke kosten - Uur gebruiker en rol

Wanneer het kostentype op de taak Gebruiker en Rol Hourly is, gebruikt Workfront twee hiërarchieën om het factureringstarief voor daadwerkelijke kosten te bepalen. De factureringssnelheid is gebaseerd op de aanmelduren van de gebruiker op een taak.

De &quot;gebruiker&quot;in de hiërarchieën is de persoon die aan de taak wordt toegewezen. De &quot;eigenaar&quot;is de persoon van wie tijd tegen de taak wordt geregistreerd, zelfs als zij niet aan de taak worden toegewezen. Michael wordt bijvoorbeeld toegewezen aan een taak, maar Joanna voltooit het werk omdat Michael ziek was. De manager kan de tijd tegen de taak registreren en de eigenaar van de geregistreerde uren aan Joanna plaatsen. De geplande opbrengstwaarden zijn gebaseerd op de taak en de tarief van Michael in de hiërarchie, maar de Ware opbrengstwaarden zijn gebaseerd op het tarief van Joanna.

Deze afbeelding laat de stroom zien van de werkelijke kostenhiërarchie:

![&#x200B; Ware Kosten voor Gebruiker en Rol het kostentype van de Uur &#x200B;](assets/actual-cost-chart.png)

### Wanneer de eigenaar van de geregistreerde uren en de toegewezen gebruiker op de taak het zelfde zijn

Workfront zoekt eerst naar een kostenpercentage op basis van de gebruikerstoewijzing. Als een gebruiker niet aan de taak wordt toegewezen, dan zoekt het naar een kostenpercentage door de baan roltoewijzing.

De hiërarchie voor dit scenario is het zelfde als de geplande kostenhiërarchie. Zie [&#x200B; Geplande kosten - Gebruiker en Rol Uur &#x200B;](#planned-cost--user-and-role-hourly) voor dit werkschema.

### Wanneer de eigenaar van de geregistreerde uren niet de toegewezen gebruiker op de taak is

Workfront zoekt in de gebruikerseigenschappen van de eigenaar volgens deze hiërarchie:

1. Het systeem zoekt naar het kostenpercentage voor het project, voor de eigenaar, rekening houdend met effectieve data. U zult dit op het gebied van Tarieven > Kosten van het project, in Source van het a **Tarief zien: Overschrijvingen > Type van Middel: Gebruiker** groeperen. Dit is een overschrijvingstarief voor het project.
1. Vervolgens zoekt het systeem naar het kostenpercentage op systeemniveau op basis van het gebruikersprofiel van de eigenaar, rekening houdend met effectieve datums.
1. Vervolgens zoekt het systeem naar het kostenpercentage van de primaire functie van de eigenaar (Designer in het voorbeeld).

   * Het systeem zoekt eerst naar het kostenpercentage voor het project, voor de primaire functie van de eigenaar, rekening houdend met effectieve datums. U zult dit op het gebied van Tarieven > Kosten van het project, in Source van het a **Tarief zien: Overschrijvingen > Type van Middel: De Rol van de Taak** groeperen. Dit is een overschrijvingstarief voor het project.
   * Vervolgens zoekt het systeem naar het aantal taken met een tariefkaart, rekening houdend met effectieve datums. U zult dit op het gebied van Tarieven > Kosten van het project, in Source van het a **Tarief zien: De Bijgevoegde Kaart van het Tarief > het Type van Middel: De Rol van de Taak** groeperen.
   * Vervolgens zoekt het systeem naar het taakrolpercentage op systeemniveau, rekening houdend met effectieve datums.

1. Als geen van deze tarieven wordt gevonden, is het factureringstarief 0.
