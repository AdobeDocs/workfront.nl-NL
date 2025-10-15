---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Workflows gebruiken in de integratie met Experience Manager Assets Essentials
description: Workflows gebruiken in de integratie met Experience Manager Assets Essentials
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4c1e5ec1-3fd1-4527-ba8a-9db1a2350f69
source-git-commit: 430751f0e38c6c45145c965398990ee3652f36fe
workflow-type: tm+mt
source-wordcount: '1000'
ht-degree: 0%

---

# Workflows gebruiken in de Experience Manager Assets-integratie

Een werkstroom is een reeks acties die Workfront verbinden met Adobe Experience Manager as a Cloud Service. Een Workfront-beheerder kan workflows configureren in Workfront en deze vervolgens toewijzen aan projectsjablonen.

Wanneer een Project wordt gecreeerd gebruikend een Malplaatje van het Project waaraan een werkschema wordt toegewezen, worden de acties die in het werkschema worden bepaald teweeggebracht.

>[!NOTE]
>
>Workflows zijn alleen beschikbaar in een Adobe Experience Manager as a Cloud Service-integratie. Ze zijn niet beschikbaar in integraties met Adobe Experience Manager Assets Essentials.


## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p> Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licenties</td> 
   <td> 
   <p>Medewerker of hoger</p> 
   <p>Aanvraag of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Aanvullende producten</td> 
   <td>U moet Experience Manager as a Cloud Service of Assets Essentials hebben en u moet als gebruiker aan het product worden toegevoegd in de Admin Console.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Experience Manager-machtigingen</td> 
    <td>U moet schrijftoegang tot de map hebben.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot documenten bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toegang weergeven of hoger</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

Voordat u begint,

* Uw Workfront-beheerder moet workflows configureren in een Adobe Experience Manager-integratie. Voor meer informatie, zie [ de integratie van Experience Manager Assets as a Cloud Service ](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional) vormen.

## Een workflow toevoegen aan een sjabloon

U kunt een werkschema aan een projectmalplaatje toevoegen. De workflow wordt toegepast op alle projecten die op basis van de sjabloon zijn gemaakt.

1. Open een malplaatje door **Malplaatjes** in het Belangrijkste Menu te klikken, dan selecterend het malplaatje van de lijst.
1. Klik **Experience Manager Assets** in het linkernavigatievenster.

   >[!NOTE]
   >
   >Als de sectie Experience Manager Assets niet wordt weergegeven in de linkernavigatie, heeft uw Workfront-beheerder geen workflows voor uw organisatie ingeschakeld. <!--Is this right?-->

1. In **selecteer een integratie voor geautomatiseerd werkstroomgebied**, selecteer de integratie met de werkschema&#39;s u voor projecten wilt gebruiken die van dit malplaatje worden gecreeerd.
1. (Optioneel) Bewerk de workflowwaarden die u wilt toepassen op projecten die op basis van deze sjabloon zijn gemaakt.

   Voor instructies op specifieke werkschema&#39;s, zie [ werkschemawaarden in een project ](#edit-workflow-values-in-a-project) in dit artikel uitgeven.

   Alleen werkstromen die zijn geactiveerd in het gedeelte Experience Manager van Setup, zijn beschikbaar in sjablonen of projecten.

1. Uw wijzigingen worden automatisch opgeslagen. <!-- do they though??-->

## Een workflow toevoegen aan een project

U kunt een workflow toevoegen wanneer u een project maakt of een workflow toevoegen aan een bestaand project. In beide gevallen gebruikt u een projectsjabloon om de workflow toe te voegen.

### Een workflow toevoegen bij het maken van een project

1. Beginnen met het maken van een project.

   Voor instructies, zie [ een project creëren gebruikend een malplaatje ](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. Wanneer het selecteren van een malplaatje voor het project, selecteer het malplaatje dat de werkschema&#39;s bevat u voor dit project wilt gebruiken.
1. (Facultatief) geef om het even welke werkschemawaarden voor het project uit, zoals die in [ worden beschreven werkschemawaarden in een project ](#edit-workflow-values-in-a-project) uitgeven.

   Alleen werkstromen die zijn geactiveerd in het gedeelte Experience Manager van Setup, zijn beschikbaar in sjablonen of projecten.


### Een workflow toevoegen aan een bestaand project

>[!NOTE]
>
>De werkschema&#39;s die lopen wanneer een project (zoals verbonden omslagverwezenlijking) wordt gecreeerd lopen niet wanneer het malplaatje aan een bestaand project in bijlage is. Zij lopen slechts wanneer een project van een malplaatje wordt gecreeerd.

1. Begin een malplaatje aan het project toe te voegen.

   Voor instructies, zie [ een malplaatje aan een project ](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md) vastmaken.

1. Wanneer het selecteren van een malplaatje voor het project, selecteer het malplaatje dat de werkschema&#39;s bevat u voor dit project wilt gebruiken.
1. (Facultatief) geef om het even welke werkschemawaarden voor het project uit, zoals die in [ worden beschreven werkschemawaarden in een project ](#edit-workflow-values-in-a-project) uitgeven.

   Alleen werkstromen die zijn geactiveerd in het gedeelte Experience Manager van Setup, zijn beschikbaar in sjablonen of projecten.



### Werkstroomwaarden in een project bewerken

U kunt werkstroomwaarden op projectniveau bewerken. Workflowwaarden op projectniveau overschrijven de waarden die zijn ingesteld op de projectsjabloon, die de standaardwaarden overschrijven die zijn ingesteld in de Adobe Experience Manager Assets-integratie.

Alle werkstroomwaarden vindt u in:

* De sectie Workflows of Gekoppelde mappen van het projectvenster Maken of Bewerken.
* De sectie Adobe Experience Manager van de linkernavigatie.


  >[!NOTE]
  >
  >Als deze gebieden niet zichtbaar zijn, heeft uw Workfront-beheerder Workflows voor uw organisatie niet ingeschakeld.



#### Gekoppelde mappen

>[!NOTE]
>
>Omdat gekoppelde mappen worden gemaakt wanneer het project wordt gemaakt, is het bewerken van de gekoppelde mapworkflow voor een bestaand project niet effectief. Deze waarden bewerken wanneer u projectfuncties maakt zoals u had verwacht.

De workflow voor gekoppelde mappen bewerken:

1. Schakel **[!UICONTROL Create Linked folder]** naar wens in of uit. Als u dit inschakelt, kunt u de configuratie van de gekoppelde map bewerken.

   Voor details op de verbonden omslagconfiguratie, zie [ Adobe Experience Manager verbonden omslagen ](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md#create-adobe-experience-manager-linked-folders) in het artikel [ vormen de [!UICONTROL Experience Manager Assets as a Cloud Service] integratie ](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

1. (Facultatief) als u de omslagboom wilt worden gebouwd slechts als bepaalde waarden op een douaneformulier aanwezig zijn in bijlage aan het project, **filter** voor die omslagboom toepassen, dan de douaneformulier selecteren die het gebied, het gebied, en de gebiedswaarde bevat. Als het veld op het aangepaste formulier dat is gekoppeld aan het nieuwe project de gekozen waarde bevat, wordt de mapstructuur gemaakt.
1. (Optioneel) Bij het configureren van mapnamen kunt u een van de volgende opties kiezen:

   * **Naam**: Type in een naam voor de omslag.

   * **gegevens van Objecten**: Selecteer de bron voor de omslagnaam, zoals de naam van het Project.

   * **de vormgegevens van de Douane**: Selecteer de gegevens van de douanevorm om als omslagnaam te gebruiken.

     Het gebruik van aangepaste formuliergegevens voor mapnamen is alleen beschikbaar op sjabloonniveau en kan niet worden geconfigureerd op integratieniveau.

     Als een omslagnaam aan douanegegevens wordt geplaatst die niet op de douane voor in bijlage aan het project bestaan, zal willekeurige identiteitskaart als omslagnaam worden toegewezen.

1. Om de omslagboom te bekijken, klik het **** pictogram van de Voorproef ![](assets/preview-icon.png)
1. Klik op **[!UICONTROL Save]**.

#### Elementen publiceren

De workflow voor het publiceren van elementen bewerken:

1. Knevel **publiceer automatisch activa** of weg zoals gewenst.
1. (Voorwaardelijk) Als u het publiceren toestaat, selecteer of u aan de publicatieservice, het merkportaal, of allebei wilt publiceren.
1. Klik op **[!UICONTROL Save]**.
