---
product-area: projects
navigation-topic: manage-issues
title: Problemen maken
description: Tijdens het werken aan een project, zou u kunnen ontdekken dat de onverwachte gebeurtenissen zich voordoen. U kunt die onverwachte gebeurtenissen als kwesties voor een bepaald project of van een taak registreren. Gebruikers met de juiste toegang kunnen de status van problemen bekijken en controleren terwijl het project of de taak wordt voltooid, zodat er geen lange e-mailketens of statusvergaderingen nodig zijn. In tegenstelling tot taken, die geplande gebeurtenissen zijn, vormen kwesties ongeplande het werkpunten in Adobe Workfront.
author: Alina
feature: Work Management
topic: Collaboration
role: User
exl-id: 2a4488fb-fe2f-422a-887c-996f6367afc5
source-git-commit: b6ea67f28b498cc0de4325a2350545c660574d4c
workflow-type: tm+mt
source-wordcount: '2024'
ht-degree: 0%

---

# Problemen maken

<!--remove Preview and Prod references when this comes to Prod-->

<span class="preview">De gemarkeerde informatie op deze pagina verwijst naar functionaliteit die nog niet algemeen beschikbaar is. Deze functie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten of in de productieomgeving voor klanten die snelle releases hebben ingeschakeld. </span>

<span class="preview">Voor informatie over snelle versies raadpleegt u [Snelle releases voor uw organisatie in- of uitschakelen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

<span class="preview">Voor informatie over de huidige versie raadpleegt u [Overzicht release 4de kwartaal 2023](../../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md). </span>



Tijdens het werken aan een project, zou u kunnen ontdekken dat de onverwachte gebeurtenissen zich voordoen. U kunt die onverwachte gebeurtenissen als kwesties voor een bepaald project of van een taak registreren. Gebruikers met de juiste toegang kunnen de status van problemen bekijken en controleren terwijl het project of de taak wordt voltooid, zodat er geen lange e-mailketens of statusvergaderingen nodig zijn. In tegenstelling tot taken, die geplande gebeurtenissen zijn, vormen kwesties ongeplande het werkpunten in Adobe Workfront.

U kunt kwesties aan projecten als verzoeken ook toevoegen. Zie voor meer informatie [Adobe Workfront-aanvragen maken en verzenden](../../../manage-work/requests/create-requests/create-submit-requests.md).

>[!TIP]
>
>Kwesties en verzoeken worden door elkaar gebruikt in Workfront. U kunt kwesties over zowel projecten als taken registreren om op onvoorzien werk te wijzen dat moet worden gericht. U kunt verzoeken ook voorleggen die als kwesties op een project worden geregistreerd dat als Rij van het Verzoek wordt aangewezen.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Reviseren of hoger om problemen aan een project of taak toe te voegen</p> <p>Vraag of hoger om problemen als verzoeken toe te voegen, gebruikend een Rij van het Verzoek.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot problemen bewerken</p> <p>De mening of hogere toegang tot Projecten en Taken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over toegang tot kwesties in uw Niveau van de Toegang, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Toegang verlenen tot kwesties</a>. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Contribute of hoger met de mogelijkheid om uitgaven toe te voegen aan de taak of het project waar u de uitgave maakt</p> <p> Voor informatie over het verlenen van machtigingen voor uitgaven raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Een uitgave delen </a></p> <p>Voor informatie over het aanvragen van aanvullende machtigingen raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

<!--
(NOTE: in NWE Requestors CAN see the Issues tab on a project but in classic they cannot! However, even when they DO see it, they cannot enter the issues - logged this issue for it but they might decide not to fix it: https://hub.workfront.com/issue/60181e28000058980cce29597185b2d6/updates?email-source=comm)</p>
-->

## Beperkingen bij het maken van problemen

Wanneer u de correcte toegang en de toestemmingen hebt kunt u kwesties op een project of een taak tot stand brengen. Het volgende is echter het geval wanneer u mogelijk geen problemen kunt maken:

* Uw Workfront-beheerder of groepsbeheerder moet het toevoegen van problemen aan een project in de status Voltooid of Dode inschakelen in het gedeelte Projectvoorkeuren. Voor informatie over het instellen van projectvoorkeuren raadpleegt u [Projectvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* U kunt geen kwesties aan een project toevoegen dat in Hangende Goedkeuring is.

## Het formulier Nieuwe uitgave voorbereiden

Uw organisatie zou een duidelijk bepaald proces voor moeten hebben wanneer en hoe te om een kwestie te registreren. Wanneer u dit proces configureert, moet u eerst het formulier maken dat nodig is voor het verzenden van een uitgave. Of u toestaat dat uitgaven direct aan taken en projecten worden toegevoegd, of als u aanvraagrijen hebt waar de kwesties worden voorgelegd, kunt u bepalen welke gebieden van Workfront evenals welke douanevelden voor gebruikers beschikbaar zijn wanneer zij nieuwe kwesties voorleggen en moeten worden voltooid. Het formulier New Issue kan belangrijke informatie bevatten die nuttig zal zijn om het probleem snel op te lossen.

De gebieden voor de nieuwe kwesties op een project worden bepaald in de sectie van de Details van de Rij van het project waar de kwesties zullen worden geregistreerd. Voor informatie over het vormen van de sectie van de Details van de Rij van het project, zie [Een aanvraagwachtrij maken](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Voor informatie over het creëren van kwesties door hen aan een verzoekrij voor te leggen, zie [Uitgaven maken door een nieuwe aanvraag in te voeren](#create-issues-by-entering-a-new-request) in dit artikel.

## Problemen op een taak of project maken met de knop Nieuw probleem

Nadat u de velden van een nieuw uitgaveformulier voor uw project hebt gedefinieerd, kunt u beginnen met het maken van uitgaven.

Het maken van problemen hangt af van de omgeving waarin u de uitgave maakt.

### Creeer kwesties op een taak of een project gebruikend de Nieuwe knoop van de Kwestie in het milieu van de Productie

Om een kwestie op een taak of een project tot stand te brengen:

1. Ga naar een project waar u de kwestie wilt tot stand brengen.
1. (Optioneel) Als u het probleem voor een taak wilt registreren, gaat u naar de **Taken** en klikt u op de naam van een taak.
1. Klik op de knop **Problemen** sectie.

   ![](assets/qs-issues-icon-highlighted-on-project-350x216.png)

1. Klikken **Nieuw probleem**.

   ![](assets/qs-issue-list-on-project-with-new-issue-button-highlighted-350x270.png)

1. (Voorwaardelijk) als de projectmaker de Onderwerpen van de Rij of de Groepen van het Onderwerp op het project creeerde worden zij toegevoegd aan de nieuwe uitgifteformulier. Geef de **Onderwerpgroep** of de **Onderwerp van wachtrij** van uw nieuwe uitgave. De Groepen van het onderwerp en de Onderwerpen van de Rij hebben namen die aan uw milieu worden aangepast.\
   Voor meer informatie over het creëren van de Groepen van het Onderwerp, zie [Onderwerpgroepen maken](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). Voor meer informatie over het creëren van de Onderwerpen van de Rij, zie [Werkvoorraadonderwerpen maken](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   ![](assets/new-issue-screen-when-creating-issue-from-list-project-level-nwe-350x422.png)

   * Als er slechts één die Onderwerp van de Rij op het project wordt geplaatst is, wordt het automatisch getoond.
   * Als de Groep van het Onderwerp geen Onderwerpen van de Rij of de Groepen van het Onderwerp onder het heeft, is niets beschikbaar in de drop-down Groep van het Onderwerp.

1. (Voorwaardelijk) Als de projectmaker toestemming heeft verleend voor de **Type aanvraag** in het veld Nieuw probleem dat u wilt weergeven, selecteert u het type uitgave op basis van de volgende opties:

   * Foutrapport
   * Volgorde wijzigen
   * Probleem
   * Verzoek\
     Afhankelijk van hoe uw Workfront-beheerder uw projectvoorkeuren heeft geconfigureerd, kunnen de namen van de uitgavetypen voor u verschillen.

   >[!TIP]
   >
   >De types van Verzoek moeten in de Details van de Rij worden toegelaten en evenals wanneer het creëren van het Onderwerp van de Rij om als selectie in de Nieuwe vorm van de Uitgave te tonen. Raadpleeg de volgende artikelen voor meer informatie:
   >* [Een aanvraagwachtrij maken](../../requests/create-and-manage-request-queues/create-request-queue.md)
   >  * [Werkvoorraadonderwerpen maken](../../requests/create-and-manage-request-queues/create-queue-topics.md)


1. Voeg een naam voor de nieuwe uitgave toe in het dialoogvenster **Naam van uitgave** veld.
1. Geef de velden op die beschikbaar zijn in het dialoogvenster **Nieuw probleem** formulier. Ga voor meer informatie over de velden die beschikbaar zijn wanneer u een nieuwe uitgave invoert naar [Problemen bewerken](../../../manage-work/issues/manage-issues/edit-issues.md).

   >[!IMPORTANT]
   >
   >Niet alle velden met betrekking tot uitgaven zijn beschikbaar in het formulier Nieuwe uitgave. De projectschepper laat de gebieden beschikbaar toe wanneer het creëren van een kwestie wanneer zij het gebied van de Details van de Rij van het project bepalen. Zie voor meer informatie [Een wachtrij met verzoeken maken](../../requests/create-and-manage-request-queues/create-request-queue.md).


1. (Voorwaardelijk) Als de onderwerpen van de Rij met een douaneformulier worden geassocieerd, zal dat aangepaste vorm in **Nieuw probleem** formulier.\
   of\
   Als het project met een kwestie douaneformulier door het gebied van de Details van de Rij wordt geassocieerd, toont de vorm in **Nieuw probleem** na de standaard Workfront-velden.

   Zie voor meer informatie [Een aanvraagwachtrij maken](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Klikken **Nieuw probleem opslaan.**

De kwesties kunnen aan veelvoudige gebruikers, baanrollen of aan een team worden toegewezen. Voor meer informatie over het toewijzen en beheren van verzoeken raadpleegt u [Werk- en teamverzoeken beheren](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

<!--When this is coming to Production, remove the "Production" section above and replace it with the following content: -->

<div class="preview">

### Problemen op een taak of project maken met de knop Nieuw probleem in de voorvertoningsomgeving

Om een kwestie op een taak of een project tot stand te brengen:

1. Ga naar een project waar u de kwestie wilt tot stand brengen.
1. (Optioneel) Als u het probleem voor een taak wilt registreren, gaat u naar de **Taken** en klikt u op de naam van een taak.
1. Klik op de knop **Problemen** sectie.

   ![](assets/qs-issues-icon-highlighted-on-project-350x216.png)

1. Klikken **Nieuw probleem**.
Het vak Nieuwe uitgave wordt weergegeven.

   ![](assets/new-issue-box-matches-new-request-ui.png)

1. (Voorwaardelijk) als de projectmaker de Onderwerpen van de Rij of de Groepen van het Onderwerp op het project creeerde worden zij toegevoegd aan de nieuwe uitgifteformulier. Geef de **Onderwerpgroep** of de **Onderwerp van wachtrij** van uw nieuwe uitgave. De Groepen van het onderwerp en de Onderwerpen van de Rij hebben namen die aan uw milieu worden aangepast.\
   Voor meer informatie over het creëren van de Groepen van het Onderwerp, zie [Onderwerpgroepen maken](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). Voor meer informatie over het creëren van de Onderwerpen van de Rij, zie [Werkvoorraadonderwerpen maken](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   * Als er slechts één die Onderwerp van de Rij op het project wordt geplaatst is, wordt het automatisch getoond.
   * Als de Groep van het Onderwerp geen Onderwerpen van de Rij of de Groepen van het Onderwerp onder het heeft, is niets beschikbaar in de drop-down Groep van het Onderwerp.

1. Voeg de naam van de uitgave toe in het dialoogvenster **Onderwerp** veld, voeg vervolgens een **Beschrijving**.

1. (Voorwaardelijk) Als de projectmaker toestemming heeft verleend voor de **Type aanvraag** in het veld Nieuw probleem dat u wilt weergeven, selecteert u het type uitgave op basis van de volgende opties:

   * Foutrapport
   * Volgorde wijzigen
   * Probleem
   * Verzoek\
     Afhankelijk van hoe uw Workfront-beheerder uw projectvoorkeuren heeft geconfigureerd, kunnen de namen van de uitgavetypen voor u verschillen.

   >[!TIP]
   >
   >De types van Verzoek moeten in de Details van de Rij worden toegelaten en evenals wanneer het creëren van het Onderwerp van de Rij om als selectie in de Nieuwe vorm van de Uitgave te tonen. Raadpleeg de volgende artikelen voor meer informatie:
   >* [Een aanvraagwachtrij maken](../../requests/create-and-manage-request-queues/create-request-queue.md)
   >  * [Werkvoorraadonderwerpen maken](../../requests/create-and-manage-request-queues/create-queue-topics.md)

1. Geef de velden op die beschikbaar zijn in het dialoogvenster **Nieuwe uitgave** formulier. Ga voor meer informatie over de velden die beschikbaar zijn wanneer u een nieuwe uitgave invoert naar [Problemen bewerken](../../../manage-work/issues/manage-issues/edit-issues.md).

   >[!IMPORTANT]
   >
   >Niet alle velden met betrekking tot uitgaven zijn beschikbaar in het formulier Nieuwe uitgave. De projectschepper laat de gebieden beschikbaar toe wanneer het creëren van een kwestie wanneer zij het gebied van de Details van de Rij van het project bepalen. Zie voor meer informatie [Een wachtrij met verzoeken maken](../../requests/create-and-manage-request-queues/create-request-queue.md).


1. (Voorwaardelijk) Als de onderwerpen van de Rij met een douaneformulier worden geassocieerd, zal dat aangepaste vorm in **Nieuwe uitgave** formulier.\
   of\
   Als het project met een kwestie douaneformulier door het gebied van de Details van de Rij wordt geassocieerd, toont de vorm in **Nieuwe uitgave** na de standaard Workfront-velden.

   Zie voor meer informatie [Een aanvraagwachtrij maken](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Klikken **Verzenden**.

   De kwesties kunnen aan veelvoudige gebruikers, baanrollen of aan een team worden toegewezen. Voor meer informatie over het toewijzen en beheren van verzoeken raadpleegt u [Werk- en teamverzoeken beheren](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

</div>

## Problemen op een taak of project inline maken

>[!IMPORTANT]
>
>De eigenaar van het project moet **Gebruikers toestaan inline uitgaven toe te voegen** wanneer het bepalen van kwesties voor het project alvorens u kwesties inline aan het project of de taken kunt toevoegen. Voor informatie over het vormen van uitgaven montages op een project, zie [Projecten bewerken](../../../manage-work/projects/manage-projects/edit-projects.md).
>

Wanneer u snel meerdere problemen wilt toevoegen, kunt u inline problemen voor een taak of project maken door deze toe te voegen aan een lijst met problemen.

>[!NOTE]
>
>Als u inline uitgaven toevoegt, past Workfront het formulier New Issue niet toe op de nieuwe uitgaven. We raden u niet aan inline kwesties toe te voegen als u wilt dat gebruikers bepaalde informatie verstrekken wanneer ze problemen invoeren. Dit kan een negatief effect hebben op het rapporteren van problemen en later op de mogelijkheid voor de gebruiker die aan het probleem is toegewezen om alle informatie te hebben die nodig is om het probleem op te lossen.

Inline uitgaven maken:

1. Ga naar een project waar u de kwestie wilt tot stand brengen.
1. (Optioneel) Als u het probleem voor een taak wilt registreren, gaat u naar de **Taken** en klikt u op de naam van een taak.
1. Klik op de knop **Problemen** sectie.
1. Klikken **Meer problemen toevoegen**.

   Er wordt een nieuwe regel gemaakt in de lijst met problemen in de sectie Problemen.

   >[!TIP]
   >
   >Deze optie is grijs als de optie Gebruikers toestaan inline uitgaven toe te voegen in het vak Project bewerken is uitgeschakeld. Zie voor meer informatie [Projecten bewerken](../../../manage-work/projects/manage-projects/edit-projects.md).

   ![](assets/add-more-issues-button-highlighted-issue-list-nwe-350x272.png)

1. Typ de naam van de uitgave in het veld Naam en voeg vervolgens meer informatie over de uitgave inline toe.

   >[!TIP]
   >
   >De velden die inline kunnen worden bewerkt, zijn beschikbaar in de weergave die u toepast op de lijst met uitgaven. Het is mogelijk dat u het volgende type velden niet kunt inline bewerken:
   >   
   >* Velden die bij een ander object horen
   >* Velden die u niet kunt bewerken
   >* Velden die berekeningen zijn en die automatisch door Workfront worden bijgewerkt

1. Klik op Enter om het inline bewerken te voltooien en de uitgave toe te voegen aan het project of de taak.

## Uitgaven maken door een nieuwe aanvraag in te voeren {#create-issues-by-entering-a-new-request}

U kunt projecten aanwijzen die u wilt ontvangen voor het ontvangen van problemen. Dit type projecten wordt Request Queues genoemd in Workfront. U kunt tot de Queues van het Verzoek door uw gebied van Verzoeken in het Belangrijkste Menu toegang hebben.

>[!TIP]
>
>De termen &quot;issue&quot; en &quot;request&quot; zijn onderling verwisselbaar in Workfront.

Voor meer informatie over hoe te opstellingsprojecten als de Queuten van het Verzoek om kwesties te ontvangen, zie [Een aanvraagwachtrij maken](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md). Voor informatie over het verzenden van verzoeken raadpleegt u [Adobe Workfront-aanvragen maken en verzenden](../../../manage-work/requests/create-requests/create-submit-requests.md).
