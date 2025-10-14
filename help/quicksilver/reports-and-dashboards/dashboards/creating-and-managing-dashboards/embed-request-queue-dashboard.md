---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Een aanvraagwachtrij insluiten in een dashboard
description: U kunt een nieuwe verzoekrij in een dashboard inbedden om directe toegang tot de verzoekrij aan uw gebruikers te verlenen, zonder het moeten naar het gebied van Verzoeken gaan.
author: Nolan
feature: Reports and Dashboards
exl-id: 2d129095-c7ee-45b1-94ce-055d1d91e2fe
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1150'
ht-degree: 0%

---

# Een aanvraagwachtrij insluiten in een dashboard

<!-- Audited: 1/2025 -->

U kunt een nieuwe verzoekrij in een dashboard inbedden om directe toegang tot de verzoekrij aan uw gebruikers te verlenen, zonder het moeten naar het gebied van Verzoeken gaan.

Bijvoorbeeld, als u een verzoekrij hebt die voor uw volledige organisatie, zoals een Rij van de Helpdesk, of een PTO rij van het Verzoek open is die iedereen op een regelmatige basis moet toegang hebben, zou het handig kunnen zijn om de verzoekrij direct in één van hun dashboards voor snelle en gemakkelijke toegang op te nemen. Het instellen van deze instelling lijkt op het maken van een externe pagina op een dashboard.

Eerst, moet u URL aan de verzoekrij verkrijgen. Ten tweede kunt u de URL insluiten in een dashboard door een externe pagina toe te voegen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-plan</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licentie</strong></td> 
   <td> 
      <p>Nieuw:</p>
         <ul>
         <li><p>Standaard</p></li>
         </ul>
      <p>Huidige:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau</strong></td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>Rechten voor het dashboard beheren</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

Beide volgende elementen moeten worden gemaakt voordat u een aanvraagwachtrij kunt insluiten in een dashboard:

* **het dashboard**: Voor informatie bij het creëren van dashboards, zie [&#x200B; een dashboard &#x200B;](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md) creëren.

* **de verzoekrij**: Voor informatie bij het creëren van verzoekrijen, zie [&#x200B; een Rij van het Verzoek &#x200B;](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md) creëren

## Verkrijg URL van de verzoekrij {#obtain-the-url-of-the-request-queue}

U kunt URL van een verzoekrij op veelvoudige manieren verkrijgen, afhankelijk van welk gedeelte van de verzoekrij u aan de gebruikers wilt blootstellen wanneer zij tot het van een dashboard toegang hebben.

* [&#x200B; verkrijg een verbinding aan een specifiek rijonderwerp met capaciteit om het verzoektype te veranderen &#x200B;](#obtain-a-link-to-a-specific-queue-topic-with-ability-to-change-the-request-type)

* [&#x200B; verkrijg een verbinding aan een verzoekrij en capaciteit om het verzoektype te veranderen &#x200B;](#obtain-a-link-to-a-request-queue-and-ability-to-change-the-request-type)

* [Verkrijg een verbinding aan een verzoekrij zonder capaciteit om het verzoektype te veranderen](#obtain-a-link-to-a-request-queue-with-no-ability-to-change-the-request-type)

### Verkrijg een verbinding aan een specifiek rijonderwerp met capaciteit om het verzoektype te veranderen {#obtain-a-link-to-a-specific-queue-topic-with-ability-to-change-the-request-type}

Wanneer u een verbinding met een specifiek rijonderwerp met andere gebruikers deelt, opent de verzoekvorm bij het nauwkeurige rijonderwerp dat zij moeten gebruiken om het verzoek voor te leggen. Dit is nuttig wanneer de gebruikers niet zeker kunnen zijn welk rijonderwerp te kiezen wanneer het registreren verzoeken om een specifieke verzoekrij.

De gebruikers kunnen het verzoektype veranderen of een ander onderwerp kiezen als zij moeten. De navigatie van het gebied van Verzoeken toont ook.

1. Klik het **Belangrijkste Menu** > **Verzoeken** > **Nieuwe Verzoek**.
1. Ga door het selecteren van onderwerpgroepen en rijonderwerpen tot u de rij bereikt u op het dashboard wilt delen, als u specifieke rij wilt delen. Voor informatie over het voorleggen van verzoeken, zie [&#x200B; Adobe Workfront verzoeken &#x200B;](../../../manage-work/requests/create-requests/create-submit-requests.md) creëren en voorleggen.

   >[!TIP]
   >
   >Het selecteren van onderwerpgroepen en rijonderwerpen is facultatief.

1. Klik **weg van het Aandeel** in de hoger-juiste hoek van het Nieuwe gebied van het Verzoek.

   Dit kopieert de verbinding aan de verzoekrij of het rijonderwerp aangezien u het op het scherm toont. De gebruikers kunnen het Type van Verzoek of om het even welke onderwerpgroepen en rijonderwerpen bijwerken beschikbaar.

   ![&#x200B; rij van het Verzoek met aandeelweg &#x200B;](assets/share-request-queue-with-share-path-link-embedded-in-dashboard-nwe-350x116.png)

### Verkrijg een verbinding aan een verzoekrij en capaciteit om het verzoektype te veranderen {#obtain-a-link-to-a-request-queue-and-ability-to-change-the-request-type}

Wanneer u een koppeling naar een aanvraagtype deelt, wordt het aanvraagtype geselecteerd voor de gebruiker. Dit is nuttig wanneer de gebruikers van veelvoudige onderwerpgroepen of rijonderwerpen voor het zelfde verzoektype moeten kiezen. Gebruikers kunnen het type aanvraag wijzigen en een ander type aanvraag kiezen. De navigatie van het gebied van Verzoeken toont ook.

1. Ga naar een project dat als verzoekrij wordt aangewezen.

   Voor informatie over het creëren van een verzoekrij van een project, ga [&#x200B; tot een Rij van het Verzoek &#x200B;](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md) leiden.

1. Ga naar **Details van de Rij**.
1. Kopieer de code die u in het **Directe gebied van de Toegang URL** vindt.

   De code moet er ongeveer als volgt uitzien:

   `https://<yourdomain>.my.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=50062d6f000849c95ab3513c0e84a51e&path=`

   Dit is de verbinding aan de verzoekrij verbonden aan het geselecteerde project. Het verzoektype wordt vooraf geselecteerd.

   De gebruikers kunnen om het even welk onderwerpgroep of rijonderwerp selecteren zij hebben vereist, of zij kunnen een ander verzoektype kiezen.

   ![&#x200B; de rij URL van het Verzoek &#x200B;](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

### Verkrijg een verbinding aan een verzoekrij zonder capaciteit om het verzoektype te veranderen {#obtain-a-link-to-a-request-queue-with-no-ability-to-change-the-request-type}

Wanneer u een koppeling deelt naar een vooraf geselecteerd aanvraagtype, wordt het aanvraagtype geselecteerd voor de gebruiker en kan het niet worden gewijzigd (de koppeling wordt grijs weergegeven). De gebruikers kunnen de onderwerpgroepen of rijonderwerpen kiezen zij hebben nodig. Dit is handig als u niet wilt dat gebruikers andere aanvraagtypen kunnen bekijken en selecteren. De navigatie van het gebied Verzoeken wordt niet weergegeven.

1. Ga naar een project dat als verzoekrij wordt aangewezen.

   Voor informatie over het creëren van een verzoekrij van een project, ga [&#x200B; tot een Rij van het Verzoek &#x200B;](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md) leiden.

1. Ga naar **Details van de Rij**.
1. Kopieer de code die u op het **Ingebedde gebied van de Code** vindt.

   De code moet er ongeveer als volgt uitzien:

   `<iframe src="https://<yourdomain>my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71" frameborder="0" width="500" height="600"></iframe>`

1. Bewerk de code om alleen de onderstaande informatie te behouden:

   `https://<yourdomain>.my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71`

   >[!TIP]
   >
   >U kunt een tag `<samp>iframe </samp>` toevoegen wanneer u de code insluit in een andere toepassing dan Workfront.

   Dit is de verbinding aan de verzoekrij verbonden aan het geselecteerde project. Het verzoektype wordt vooraf geselecteerd en kan niet worden veranderd.

   De gebruikers kunnen om het even welk onderwerpgroep of rijonderwerp selecteren zij voor het geselecteerde verzoektype nodig hebben. Gebruikers kunnen geen ander aanvraagtype selecteren.

   ![&#x200B; de rijcode van het Verzoek &#x200B;](assets/share-request-queue-with-embedded-code-embedded-in-dashboard-nwe-350x210.png)

## Een aanvraagwachtrij insluiten in een dashboard

U kunt een verbinding aan de verzoekrij of aan een rijonderwerp inbedden dat onder een verzoekrij in een dashboard wordt genesteld om gebruikers directe toegang tot het ingaan van verzoeken te geven.

1. Verkrijg een verzoekrij URL gebruikend één van de methodes die in [&#x200B; worden beschreven verkrijgen URL van de 1&rbrace; sectie van de verzoekrij &lbrace;van dit artikel.](#obtain-the-url-of-the-request-queue)

1. Klik het **Belangrijkste Menu** > **Dashboards** > **Nieuw Dashboard**.

1. Typ a **Naam** voor het dashboard. Dit is een verplicht veld.

1. Klik **toevoegen Externe Pagina**.

   ![&#x200B; Externe pagina &#x200B;](assets/add-external-page-highlighted---nwe-350x214.png)

1. In **voeg Externe de doos van de Pagina** toe, geef de volgende gebieden uit:

   * **Naam**: ga de naam van de verzoekrij in aangezien u het op het dashboard wilt verschijnen. Dit is een verplicht veld.

   * **Beschrijving**: ga een beschrijving over dat in deze externe paginavertoningen. Dit is geen verplicht veld en is alleen voor rapportagedoeleinden van belang. Deze wordt niet weergegeven in het dashboard.

   * **URL**: kleef URL die u gebruikend één van de methodes die in Stap 1 worden beschreven verkregen.

   * **Hoogte**: ga de hoogte van de externe pagina in. Hiermee bepaalt u hoeveel ruimte de externe pagina met de aanvraagwachtrij inneemt op het dashboard. Dit is een verplicht veld en de standaardwaarde is 500.

1. Klik **sparen**.

1. Klik **sparen + Sluiten**.

   De verzoekrij toont in het dashboard als afzonderlijke dashboardcomponent.

1. (Facultatief) klik **Acties van het Dashboard**, dan **geef** uit om rapporten, kalenders, of extra externe pagina&#39;s aan het zelfde dashboard toe te voegen.

   Voor informatie over het toevoegen van componenten aan een dashboard, zie [&#x200B; een dashboard &#x200B;](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md) creëren.

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
