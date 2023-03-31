---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Een aanvraagwachtrij insluiten in een dashboard
description: U kunt een nieuwe verzoekrij in een dashboard inbedden om directe toegang tot de verzoekrij aan uw gebruikers te verlenen, zonder het moeten naar het gebied van Verzoeken gaan.
author: Nolan
feature: Reports and Dashboards
exl-id: 2d129095-c7ee-45b1-94ce-055d1d91e2fe
source-git-commit: 2894161b61a00dab04c17ef642ace4a45179eb17
workflow-type: tm+mt
source-wordcount: '1178'
ht-degree: 0%

---

# Een aanvraagwachtrij insluiten in een dashboard

U kunt een nieuwe verzoekrij in een dashboard inbedden om directe toegang tot de verzoekrij aan uw gebruikers te verlenen, zonder het moeten naar het gebied van Verzoeken gaan. 

Bijvoorbeeld, als u een verzoekrij hebt die voor uw volledige organisatie, zoals een Rij van de Helpdesk, of een PTO rij van het Verzoek open is die iedereen op een regelmatige basis moet toegang hebben, zou het handig kunnen zijn om de verzoekrij direct in één van hun dashboards voor snelle en gemakkelijke toegang op te nemen. Het instellen van deze instelling lijkt op het maken van een externe pagina op een dashboard.

Eerst, moet u URL aan de verzoekrij verkrijgen. Ten tweede kunt u de URL insluiten in een dashboard door een externe pagina toe te voegen.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-abonnement*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licentie*</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong></td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>Rechten voor het dashboard beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Vereisten

Beide volgende elementen moeten worden gemaakt voordat u een aanvraagwachtrij kunt insluiten in een dashboard:

* **Het dashboard**: Voor informatie over het maken van dashboards raadpleegt u [Een dashboard maken](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).
* **De wachtrij met aanvragen**: Voor informatie bij het creëren van verzoekrijen, zie [Een aanvraagwachtrij maken](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)

## Verkrijg URL van de verzoekrij {#obtain-the-url-of-the-request-queue}

U kunt URL van een verzoekrij op veelvoudige manieren verkrijgen, afhankelijk van welk gedeelte van de verzoekrij u aan de gebruikers wilt blootstellen wanneer zij tot het van een dashboard toegang hebben.

* [Verkrijg een verbinding aan een specifiek rijonderwerp met capaciteit om het verzoektype te veranderen](#obtain-a-link-to-a-specific-queue-topic-with-ability-to-change-the-request-type)
* [Verkrijg een verbinding aan een verzoekrij en capaciteit om het verzoektype te veranderen](#obtain-a-link-to-a-request-queue-and-ability-to-change-the-request-type)
* [Verkrijg een verbinding aan een verzoekrij zonder capaciteit om het verzoektype te veranderen](#obtain-a-link-to-a-request-queue-with-no-ability-to-change-the-request-type)

### Verkrijg een verbinding aan een specifiek rijonderwerp met capaciteit om het verzoektype te veranderen {#obtain-a-link-to-a-specific-queue-topic-with-ability-to-change-the-request-type}

Wanneer u een verbinding met een specifiek rijonderwerp met andere gebruikers deelt, opent de verzoekvorm bij het nauwkeurige rijonderwerp dat zij moeten gebruiken om het verzoek voor te leggen. Dit is nuttig wanneer de gebruikers niet zeker kunnen zijn welk rijonderwerp te kiezen wanneer het registreren verzoeken om een specifieke verzoekrij.

De gebruikers kunnen het verzoektype veranderen of een ander onderwerp kiezen als zij moeten. De navigatie van het gebied van Verzoeken toont ook.

1. Klik op de knop **Hoofdmenu** > **Verzoeken** > **Nieuwe aanvraag**.
1. Ga door het selecteren van onderwerpgroepen en rijonderwerpen tot u de rij bereikt u op het dashboard wilt delen, als u specifieke rij wilt delen. Voor informatie over het verzenden van verzoeken raadpleegt u [Adobe Workfront-aanvragen maken en verzenden](../../../manage-work/requests/create-requests/create-submit-requests.md).

   >[!TIP]
   >
   >Het selecteren van onderwerpgroepen en rijonderwerpen is facultatief.

1. Klikken **Pad delen** in de rechterbovenhoek van het gebied Nieuw verzoek.

   Dit kopieert de verbinding aan de verzoekrij of het rijonderwerp aangezien u het op het scherm toont. De gebruikers kunnen het Type van Verzoek of om het even welke onderwerpgroepen en rijonderwerpen bijwerken beschikbaar.

   ![](assets/share-request-queue-with-share-path-link-embedded-in-dashboard-nwe-350x116.png)

### Verkrijg een verbinding aan een verzoekrij en capaciteit om het verzoektype te veranderen {#obtain-a-link-to-a-request-queue-and-ability-to-change-the-request-type}

Wanneer u een koppeling naar een aanvraagtype deelt, wordt het aanvraagtype geselecteerd voor de gebruiker. Dit is nuttig wanneer de gebruikers van veelvoudige onderwerpgroepen of rijonderwerpen voor het zelfde verzoektype moeten kiezen. Gebruikers kunnen het type aanvraag wijzigen en een ander type aanvraag kiezen. De navigatie van het gebied van Verzoeken toont ook.

1. Ga naar een project dat als verzoekrij wordt aangewezen.

   Voor informatie over het creëren van een verzoekrij van een project, ga naar [Een aanvraagwachtrij maken](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Ga naar **Wachtrij**.
1. Kopieer de code die u vindt in het dialoogvenster **URL voor directe toegang** veld.

   De code moet er ongeveer als volgt uitzien:

   `https://<yourdomain>.my.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=50062d6f000849c95ab3513c0e84a51e&path=`

   Dit is de verbinding aan de verzoekrij verbonden aan het geselecteerde project. Het verzoektype wordt vooraf geselecteerd.

   De gebruikers kunnen om het even welk onderwerpgroep of rijonderwerp selecteren zij, of zij kunnen een ander verzoektype kiezen.

   ![](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

### Verkrijg een verbinding aan een verzoekrij zonder capaciteit om het verzoektype te veranderen {#obtain-a-link-to-a-request-queue-with-no-ability-to-change-the-request-type}

Wanneer u een koppeling deelt naar een vooraf geselecteerd aanvraagtype, wordt het aanvraagtype geselecteerd voor de gebruiker en kan het niet worden gewijzigd (de koppeling wordt grijs weergegeven). De gebruikers kunnen de onderwerpgroepen of rijonderwerpen kiezen zij hebben nodig. Dit is handig als u niet wilt dat gebruikers andere aanvraagtypen kunnen bekijken en selecteren. De navigatie van het gebied Verzoeken wordt niet weergegeven.

1. Ga naar een project dat als verzoekrij wordt aangewezen.

   Voor informatie over het creëren van een verzoekrij van een project, ga naar [Een aanvraagwachtrij maken](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Ga naar **Wachtrij**.
1. Kopieer de code die u vindt in het dialoogvenster **Ingesloten code** veld.

   De code moet er ongeveer als volgt uitzien:

   `<iframe src="https://<yourdomain>my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71" frameborder="0" width="500" height="600"></iframe>`

1. Bewerk de code om alleen de onderstaande informatie te behouden:

   `https://<yourdomain>.my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71`

   >[!TIP]
   >
   >U kunt een `<samp>iframe </samp>` -tags toepassen wanneer de code wordt ingesloten in een andere toepassing dan Workfront.

   Dit is de verbinding aan de verzoekrij verbonden aan het geselecteerde project. Het verzoektype wordt vooraf geselecteerd en kan niet worden veranderd.

   De gebruikers kunnen om het even welk onderwerpgroep of rijonderwerp selecteren zij voor het geselecteerde verzoektype nodig hebben. Gebruikers kunnen geen ander aanvraagtype selecteren.

   ![](assets/share-request-queue-with-embedded-code-embedded-in-dashboard-nwe-350x210.png)

## Een aanvraagwachtrij insluiten in een dashboard

U kunt een verbinding aan de verzoekrij of aan een rijonderwerp inbedden dat onder een verzoekrij in een dashboard wordt genesteld om gebruikers directe toegang tot het ingaan van verzoeken te geven.

1. Verkrijg een URL van de verzoekrij gebruikend één van de methodes die in worden beschreven [Verkrijg URL van de verzoekrij](#obtain-the-url-of-the-request-queue) van dit artikel.
1. Klik op de knop **Hoofdmenu** > **Dashboards** > **Nieuw dashboard**.
1. Typ a **Naam** voor het dashboard. Dit is een verplicht veld.
1. Klikken **Externe pagina toevoegen**.

   ![](assets/add-external-page-highlighted---nwe-350x214.png)

1. In de **Externe pagina toevoegen** bewerkt u de volgende velden:

   * **Naam**: Voer de naam van de aanvraagwachtrij in zoals u deze wilt weergeven op het dashboard. Dit is een verplicht veld.

   * **Beschrijving**: Voer een beschrijving in over de weergave van deze externe pagina. Dit is geen verplicht veld en is alleen voor rapportagedoeleinden van belang. Deze wordt niet weergegeven in het dashboard.
   * **URL**: plak de URL die u hebt verkregen met een van de methoden die in Stap 1 worden beschreven.

      <!--   
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     <MadCap:conditionalText data-mc-conditions="">   
     (NOTE: ensure this stays accurate)   
     </MadCap:conditionalText>   
     </MadCap:conditionalText>   
     -->

   * **Hoogte**: Voer de hoogte van de externe pagina in. Hiermee bepaalt u hoeveel ruimte de externe pagina met de aanvraagwachtrij inneemt op het dashboard. Dit is een verplicht veld en de standaardwaarde is 500.

1. Klikken **Opslaan**.
1. Klikken **Opslaan + Sluiten**. 

   De verzoekrij toont in het dashboard als afzonderlijke dashboardcomponent.

   ![](assets/new-dashboard-with-embedded-request-queue-nwe-350x260.png)

1. (Optioneel) Klik op **Dashboardhandelingen** vervolgens **Bewerken** om rapporten, kalenders of extra externe pagina&#39;s aan hetzelfde dashboard toe te voegen.\
   Voor informatie over het toevoegen van componenten aan een dashboard, zie [Een dashboard maken](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

 

 

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted - old information)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1"> <p class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Main Menu</strong> > Requests >&nbsp;<strong>New Request</strong>. </p> </li>
<li class="preview" value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Continue entering the request.&nbsp;For information about submitting requests, see <a href="../../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref">Create and submit Adobe Workfront requests</a>. </p> </li>
<li value="3"> <p>Select the <strong>Request Type</strong> for the queue you would like added to the dashboard.</p> </li>
<li value="4"> <p>(Optional) Select a Queue Topic and a Topic Group. Depending on how the project manager set up the request queue, the names of these fields are different in each Workfront instance.</p> </li>
<li class="preview" value="5" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Click <strong>Share path</strong> to obtain a shared link from the request queue you want to embed on a dashboard.</p> <p>For information about sharing a request queue, see <a href="../../../manage-work/requests/create-requests/share-link-to-request-queue.md" class="MCXref xref">Share a link to a request queue</a></p> </li>
<li value="6"> <p>For example, enter a URL similar to one of the following: </p> </li>
</ol>
-->
