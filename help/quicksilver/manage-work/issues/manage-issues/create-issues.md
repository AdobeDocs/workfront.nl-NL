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
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '1540'
ht-degree: 0%

---

# Problemen maken

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> 

<span class="preview">For information about the current release, see [Fourth Quarter 2023 release overview](../../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md). </span> 

-->

Tijdens het werken aan een project, zou u kunnen ontdekken dat de onverwachte gebeurtenissen zich voordoen. U kunt die onverwachte gebeurtenissen als kwesties voor een bepaald project of van een taak registreren. Gebruikers met de juiste toegang kunnen de status van problemen bekijken en controleren terwijl het project of de taak wordt voltooid, zodat er geen lange e-mailketens of statusvergaderingen nodig zijn. In tegenstelling tot taken, die geplande gebeurtenissen zijn, vormen kwesties ongeplande het werkpunten in Adobe Workfront.

U kunt kwesties aan projecten als verzoeken ook toevoegen. Voor informatie, zie [ Adobe Workfront verzoeken ](../../../manage-work/requests/create-requests/create-submit-requests.md) creëren en voorleggen.

>[!TIP]
>
>Kwesties en verzoeken worden door elkaar gebruikt in Workfront. U kunt kwesties over zowel projecten als taken registreren om op onvoorzien werk te wijzen dat moet worden gericht. U kunt verzoeken ook voorleggen die als kwesties op een project worden geregistreerd dat als Rij van het Verzoek wordt aangewezen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

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
   <td> <p>Toegang tot problemen bewerken</p> <p>De mening of hogere toegang tot Projecten en Taken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over toegang tot kwesties in uw Niveau van de Toegang, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref"> Toegang van de Verlening tot kwesties </a>. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Contribute of hoger met de mogelijkheid om uitgaven toe te voegen aan de taak of het project waar u de uitgave maakt</p> <p> Voor informatie over het verlenen van toestemmingen aan kwesties, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref"> een kwestie delen </a></p> <p>Voor informatie bij het vragen van extra toestemmingen, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> Toegang tot voorwerpen verzoeken </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

+++

<!--
(NOTE: in NWE Requestors CAN see the Issues tab on a project but in classic they cannot! However, even when they DO see it, they cannot enter the issues - logged this issue for it but they might decide not to fix it: https://hub.workfront.com/issue/60181e28000058980cce29597185b2d6/updates?email-source=comm)</p>
-->

## Beperkingen bij het maken van problemen

Wanneer u de correcte toegang en de toestemmingen hebt kunt u kwesties op een project of een taak tot stand brengen. Het volgende is echter het geval wanneer u mogelijk geen problemen kunt maken:

* Uw Workfront-beheerder of groepsbeheerder moet het toevoegen van problemen aan een project in de status Voltooid of Dode inschakelen in het gedeelte Projectvoorkeuren. Voor informatie over het plaatsen van projectvoorkeur, zie [ systeem-brede projectvoorkeur ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen.
* U kunt geen kwesties aan een project toevoegen dat in Hangende Goedkeuring is.

## Het formulier Nieuwe uitgave voorbereiden

Uw organisatie zou een duidelijk bepaald proces voor moeten hebben wanneer en hoe te om een kwestie te registreren. Wanneer u dit proces configureert, moet u eerst het formulier maken dat nodig is voor het verzenden van een uitgave. Of u toestaat dat uitgaven direct aan taken en projecten worden toegevoegd, of als u aanvraagrijen hebt waar de kwesties worden voorgelegd, kunt u bepalen welke gebieden van Workfront evenals welke douanevelden voor gebruikers beschikbaar zijn wanneer zij nieuwe kwesties voorleggen en moeten worden voltooid. Het formulier New Issue kan belangrijke informatie bevatten die nuttig zal zijn om het probleem snel op te lossen.

De gebieden voor de nieuwe kwesties op een project worden bepaald in de sectie van de Details van de Rij van het project waar de kwesties zullen worden geregistreerd. Voor informatie over het vormen van de sectie van de Details van de Rij van het project, zie [ een Rij van het Verzoek ](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md) creëren.

Voor informatie over het creëren van kwesties door hen aan een verzoekrij voor te leggen, zie [ kwesties creëren door een nieuwe verzoek ](#create-issues-by-entering-a-new-request) sectie in dit artikel in te gaan.

## Problemen op een taak of project maken met de knop Nieuw probleem

Nadat u de velden van een nieuw uitgaveformulier voor uw project hebt gedefinieerd, kunt u beginnen met het maken van uitgaven.

<!-- OLD UI: redesigned on Oct 26, 2023:

Creating issues differs depending on which environment you choose to create the issue. 

### Create issues on a task or project using the New Issue button in the Production environment

To create an issue on a task or a project:

1. Go to a project where you want to create the issue. 
1. (Optional) If you want to log the issue for a task, go to the **Tasks** area, then click the name of a task. 
1. Click the **Issues** section.

   
1. Click **New Issue**.

  

1. (Conditional) If the project creator created Queue Topics or Topic Groups on the project they are added to the new issue form. Specify the **Topic Group** or the **Queue Topic** of your new issue. Topic Groups and Queue Topics have names customized to your environment.  
   For more information about creating Topic Groups, see [Create Topic Groups](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). For more information about creating Queue Topics, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   ![New issue screen](assets/new-issue-screen-when-creating-issue-from-list-project-level-nwe-350x422.png)

   * If there is only one Queue Topic set on the project, it is displayed automatically.
   * If the Topic Group does not have any Queue Topics or Topic Groups under it, nothing is available in the Topic Group drop-down.

1. (Conditional) If the project creator allowed for the **Request Type** field to display on the New Issue form, select the type of your issue from the following options:

   * Bug Report
   * Change Order
   * Issue
   * Request  
     Depending on how your Workfront administrator has configured your Project Preferences, the names of the issue types might be different for you. 

   >[!TIP]
   >
   >The Request Types must be enabled in the Queue Details and as well as when creating the Queue Topic to display as a selection in the New Issue form. For information, see the following articles: 
   >* [Create a Request Queue](../../requests/create-and-manage-request-queues/create-request-queue.md)
   >  * [Create Queue Topics](../../requests/create-and-manage-request-queues/create-queue-topics.md)


1. Add a name for the new issue in the **Issue Name** field. 
1. Continue specifying the fields available in the **New Issue** form. For more information about the fields available as you enter a new issue, see [Edit issues](../../../manage-work/issues/manage-issues/edit-issues.md).

   >[!IMPORTANT]
   >
   >Not all the issue-related fields are available in the New Issue form. The project creator enables the fields available when creating an issue when they define the Queue Details area of the project. For more information, see [Create a Requests Queue](../../requests/create-and-manage-request-queues/create-request-queue.md). 


1. (Conditional) If the Queue Topics are associated with a custom form, that custom form will display in the **New Issue** form.  
   Or  
   If the project is associated with an issue custom form through the Queue Details area, the form displays in the **New Issue** form, after the default Workfront fields.

   For information, see [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Click **Save New Issue.**

Issues can be assigned to multiple users, job roles or to a team. For more information about assigning and managing requests, see [Manage work and team requests](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

<!--When this is coming to Production, remove the "Production" section above and replace it with the following content:
-->

Om een kwestie op een taak of een project tot stand te brengen:

1. Ga naar een project waar u de kwestie wilt tot stand brengen.
1. (Facultatief) als u de kwestie voor een taak wilt registreren, ga naar het **gebied van Taken**, dan klik de naam van een taak.
1. Klik de **sectie van Kwesties**.

   De lijst met projectproblemen wordt weergegeven

1. Klik **Nieuwe Uitgave** bij de bovenkant van de lijst van de kwestie.
Het vak Nieuwe uitgave wordt weergegeven.

   ![ Nieuwe uitgavvakje ](assets/new-issue-box-matches-new-request-ui.png)

1. (Voorwaardelijk) als de projectmaker de Onderwerpen van de Rij of de Groepen van het Onderwerp op het project creeerde worden zij toegevoegd aan de nieuwe uitgifteformulier. Specificeer de **Groep van het Onderwerp** of **Onderwerp van de Rij** van uw nieuwe kwestie. De Groepen van het onderwerp en de Onderwerpen van de Rij hebben namen die aan uw milieu worden aangepast.\
   Voor meer informatie over het creëren van de Groepen van het Onderwerp, zie [ tot de Groepen van het Onderwerp ](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md) leiden. Voor meer informatie over het creëren van de Onderwerpen van de Rij, zie [ de Onderwerpen van de Rij ](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md) creëren.

   * Als er slechts één die Onderwerp van de Rij op het project wordt geplaatst is, wordt het automatisch getoond.
   * Als de Groep van het Onderwerp geen Onderwerpen van de Rij of de Groepen van het Onderwerp onder het heeft, is niets beschikbaar in de drop-down Groep van het Onderwerp.

1. Voeg de voorwaardennaam op het **Onderwerp** gebied toe, dan voeg a **Beschrijving** toe.

1. (Voorwaardelijk) als de projectschepper voor het **gebied van het Type van Verzoek** om op de Nieuwe vorm van de Uitgave toestond te tonen, selecteer het type van uw kwestie van de volgende opties:

   * Foutrapport
   * Volgorde wijzigen
   * Probleem
   * Verzoek\
     Afhankelijk van hoe uw Workfront-beheerder uw projectvoorkeuren heeft geconfigureerd, kunnen de namen van de uitgavetypen voor u verschillen.

   >[!TIP]
   >
   >De types van Verzoek moeten in de Details van de Rij worden toegelaten en evenals wanneer het creëren van het Onderwerp van de Rij om als selectie in de Nieuwe vorm van de Uitgave te tonen. Raadpleeg de volgende artikelen voor meer informatie:
   >* [ creeer een Rij van het Verzoek ](../../requests/create-and-manage-request-queues/create-request-queue.md)
   >  * [ creeer de Onderwerpen van de Rij ](../../requests/create-and-manage-request-queues/create-queue-topics.md)

1. Ga verder specificerend de gebieden beschikbaar in de **Nieuwe kwestie** vorm. Voor meer informatie over de beschikbare gebieden aangezien u een nieuwe kwestie ingaat, zie [ kwesties ](../../../manage-work/issues/manage-issues/edit-issues.md) uitgeven.

   >[!IMPORTANT]
   >
   >Niet alle velden met betrekking tot uitgaven zijn beschikbaar in het formulier Nieuwe uitgave. De projectschepper laat de gebieden beschikbaar toe wanneer het creëren van een kwestie wanneer zij het gebied van de Details van de Rij van het project bepalen. Voor meer informatie, zie [ een Rij van Verzoeken ](../../requests/create-and-manage-request-queues/create-request-queue.md) creëren.


1. (Voorwaardelijk) als de Onderwerpen van de Rij met een douaneformulier worden geassocieerd, zal dat douaneformulier in de **Nieuwe kwestie** vorm tonen.\
   of\
   Als het project met een vorm van de uitgaven douanevorm door het gebied van de Details van de Rij wordt geassocieerd, toont de vormvertoningen in de **Nieuwe kwestie** vorm, na de standaardgebieden van Workfront.

   Voor informatie, zie [ een Rij van het Verzoek ](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md) creëren.

1. Klik **voorleggen**.

   De kwesties kunnen aan veelvoudige gebruikers, baanrollen of aan een team worden toegewezen. Voor meer informatie over het toewijzen van en het beheren van verzoeken, zie [ werk en teamverzoeken ](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md) leiden.


## Problemen op een taak of project inline maken

>[!IMPORTANT]
>
>De projecteigenaar moet **toestaan gebruikers om kwesties toe te voegen gealigneerd** wanneer het bepalen van uitgeven montages voor het project alvorens u kwesties aan het project of de taken kunt inline toevoegen. Voor informatie over het vormen van uitgeven montages op een project, zie [ projecten ](../../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.
>

Wanneer u snel meerdere problemen wilt toevoegen, kunt u inline problemen voor een taak of project maken door deze toe te voegen aan een lijst met problemen.

>[!NOTE]
>
>Als u inline uitgaven toevoegt, past Workfront het formulier New Issue niet toe op de nieuwe uitgaven. We raden u niet aan inline kwesties toe te voegen als u wilt dat gebruikers bepaalde informatie verstrekken wanneer ze problemen invoeren. Dit kan een negatief effect hebben op het rapporteren van problemen en later op de mogelijkheid voor de gebruiker die aan het probleem is toegewezen om alle informatie te hebben die nodig is om het probleem op te lossen.

Inline uitgaven maken:

1. Ga naar een project waar u de kwestie wilt tot stand brengen.
1. (Facultatief) als u de kwestie voor een taak wilt registreren, ga naar de **sectie van Taken**, dan klik de naam van een taak.
1. Klik de **sectie van Kwesties** in het linkerpaneel.
1. Klik **toevoegen Meer Kwesties** bij de bodem van de lijst van de kwestie.

   Er wordt een nieuwe regel gemaakt in de lijst met problemen in de sectie Problemen.

   >[!TIP]
   >
   >Deze optie is grijs als de optie Gebruikers toestaan inline uitgaven toe te voegen in het vak Project bewerken is uitgeschakeld. Voor informatie, zie [ projecten ](../../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.

   ![ voeg meer kwesties toe knoop ](assets/add-more-issues-button-highlighted-issue-list-nwe-350x272.png)

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

Voor meer informatie over hoe te opstellingsprojecten als de Rijen van het Verzoek om kwesties te ontvangen, zie [ een Rij van het Verzoek ](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md) creëren. Voor informatie over het voorleggen van verzoeken, zie [ Adobe Workfront verzoeken ](../../../manage-work/requests/create-requests/create-submit-requests.md) creëren en voorleggen.
