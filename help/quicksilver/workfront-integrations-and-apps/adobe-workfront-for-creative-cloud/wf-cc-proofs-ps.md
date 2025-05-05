---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Proefbestanden uploaden vanuit Adobe Photoshop
description: U kunt uw tekengebieden als proefdrukken rechtstreeks uploaden naar Adobe Workfront voor een grondige revisie en goedkeuring.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: cbb12ee7-949e-44a1-9340-3ef93c003b21
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 0%

---

# Proefdrukken uploaden vanuit [!DNL Photoshop]

U kunt tekengebieden als proefdrukken rechtstreeks uploaden naar [!DNL Adobe Workfront] voor een grondige revisie en goedkeuring.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Huidig abonnement: [!UICONTROL Pro] of hoger</p> <p>of</p> <p>Ouder plan: [!UICONTROL Premium]</p> <p>Voor meer informatie over het proefdrukken van toegang met de verschillende plannen, zie.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td> <p>Huidig abonnement: [!UICONTROL Work] of [!UICONTROL Proof]</p> <p>Ouder plan: Willekeurig (proefdrukken moet zijn ingeschakeld voor de gebruiker)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>U moet een [!DNL Adobe Creative Cloud] licentie hebben naast een [!DNL Workfront] licentie.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bewijs van machtigingsprofiel </td> 
   <td>[!UICONTROL Manager] of hoger</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toegang bewerken tot [!UICONTROL Documents]</p> <p>Voor informatie bij het verzoeken van extra toegang, zie <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> Toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, rol, of Profiel van de Toestemming van het Bewijs u hebt, contacteer uw beheerder van Workfront of van Workfront Proof.

+++

## Vereisten

* U moet [!DNL Adobe Workfront for Photoshop] installeren voordat u proefdrukken van [!DNL Adobe Photoshop] kunt uploaden.

  Voor instructies, zie [ installeren  [!DNL Adobe Workfront for Photoshop]](../../workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-ps.md).

## Een basisproef uploaden

1. Klik op het pictogram **[!UICONTROL Menu]** in de rechterbovenhoek en selecteer vervolgens **[!UICONTROL Work List]** . U kunt het menu ook gebruiken om naar bovenliggende objecten te navigeren.

   ![ Terugkeer aan de Lijst van het Werk ](assets/go-back-to-work-list-350x314.png)

1. Ga naar het werkitem waar u een proefdruk wilt uploaden.
1. Klik het **[!UICONTROL Document]** pictogram van het pictogram van het 1&rbrace; Document ![&#128279;](assets/documents.png) in de navigatiebar.
1. Klik op **[!UICONTROL New File]** onder in het deelvenster [!DNL Workfront] .
1. Schakel de **[!UICONTROL Create a proof]** -schakeloptie in.
1. (Optioneel) Typ een naam voor de proefdruk in het tekstvak **[!UICONTROL Proof Name]** .
1. Selecteer **[!UICONTROL Basic]** in de sectie **[!UICONTROL Proof Approvals]** .
1. (Optioneel) Voeg fiatteurs toe.
1. (Optioneel) Typ een opmerking in het **[!UICONTROL Updates]** -gebied.

   ![ voeg een commentaar ](assets/add-comment.png) toe

1. Kies de **[!UICONTROL Asset Type]** in de vervolgkeuzelijst.

1. (Optioneel) Selecteer **[!UICONTROL Add outside file]** om een bestand van uw computer toe te voegen.
1. Klik op **[!UICONTROL Upload]** en configureer de gewenste exportopties op basis van het hierboven gekozen elementtype.

   ![ Dossiers in plugin ](assets/plugin-files-350x307.png)\
   Het document wordt weergegeven in het gebied [!UICONTROL Documents] in het deelvenster [!DNL Workfront] in [!DNL Photoshop] en in de bureaubladtoepassing van [!DNL Workfront] .


## Een automatische proefdruk uploaden

1. Klik op het pictogram **[!UICONTROL Menu]** in de rechterbovenhoek en selecteer vervolgens **[!UICONTROL Work List]** . U kunt het menu ook gebruiken om naar bovenliggende objecten te navigeren.

   ![ Terugkeer aan de Lijst van het Werk ](assets/go-back-to-work-list-350x314.png)

1. Ga naar het werkitem waar u een proefdruk wilt uploaden.
1. Klik het **[!UICONTROL Document]** pictogram van het pictogram van het 1&rbrace; Document ![&#128279;](assets/documents.png) in de navigatiebar.

1. Klik op **[!UICONTROL New File]** onder in het deelvenster [!DNL Workfront] .
1. Schakel de **[!UICONTROL Create a proof]** -schakeloptie in.
1. (Optioneel) Typ een naam voor de proefdruk in het tekstvak **[!UICONTROL Proof Name]** .
1. Selecteer **[!UICONTROL Automated]** in de sectie **[!UICONTROL Proof Approvals]** .
1. (Optioneel) Typ in het vak **[!UICONTROL Workflow Template]** de naam van een sjabloon voor de proefdrukworkflow.

{{adjust-proof-settings}}

>[!NOTE]
>
> Als het werkstroomsjabloon lege verplichte velden bevat, worden de automatische proefdrukinstellingen automatisch geopend en moet u deze velden invullen om de proefdrukinstellingen te kunnen uploaden.


1. (Optioneel) Typ een opmerking in het **[!UICONTROL Updates]** -gebied.

   ![ voeg commentaargeautomatiseerde goedkeuring ](assets/add-comment-automated-approval.png) toe

1. Kies de **[!UICONTROL Asset Type]** in de vervolgkeuzelijst.
1. (Optioneel) Selecteer **[!UICONTROL Add outside file]** om een bestand van uw computer toe te voegen.
1. Klik op **[!UICONTROL Upload]** en configureer de gewenste exportopties op basis van het hierboven gekozen elementtype.
Het document wordt weergegeven in het gebied [!UICONTROL Documents] in het deelvenster [!DNL Workfront] in [!DNL Photoshop] en in de bureaubladtoepassing van [!DNL Workfront] .

## Een nieuwe proefdrukversie uploaden

U kunt een nieuwe versie van een proefdruk uploaden. De plug-in onthoudt de testworkflow die in de vorige versie is ingesteld, maar u kunt deze desgewenst wijzigen.

1. Klik op het pictogram **[!UICONTROL Menu]** in de rechterbovenhoek en selecteer vervolgens **[!UICONTROL Work List]** . U kunt het menu ook gebruiken om naar bovenliggende objecten te navigeren.

   ![ Terugkeer aan de Lijst van het Werk ](assets/go-back-to-work-list-350x314.png)

1. Ga naar het werkitem waarnaar u een document moet uploaden.
1. Klik het **[!UICONTROL Document]** pictogram van het pictogram van het 1&rbrace; Document ![&#128279;](assets/documents.png) in de navigatiebar.

1. Klik op **[!UICONTROL New Version]** onder in het deelvenster [!DNL Workfront] .
1. Schakel de **[!UICONTROL Create a proof]** -schakeloptie in.

1. Kies **[!UICONTROL Basic]** of **[!UICONTROL Automated]** in de sectie *[!UICONTROL *Proof approvals]**.

1. Voeg **[!UICONTROL Reviewers]** of een **[!UICONTROL Workflow template]** toe op basis van het goedkeuringstype dat u in stap 7 hebt geselecteerd.

1. (Optioneel) Typ een opmerking in het **[!UICONTROL Updates]** -gebied.
1. Kies de **[!UICONTROL Asset Type]** in de vervolgkeuzelijst.
1. Klik op **[!UICONTROL Upload]** en configureer de gewenste exportopties op basis van het hierboven gekozen elementtype.
Het document wordt weergegeven in het gebied [!UICONTROL Documents] in het deelvenster [!DNL Workfront] in [!DNL Photoshop] en in de bureaubladtoepassing van [!DNL Workfront] .
