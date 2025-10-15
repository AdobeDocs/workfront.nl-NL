---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Proefbestanden uploaden vanuit Adobe Photoshop
description: U kunt voorinstellingen van fotodocumenten rechtstreeks uploaden als proefdrukken naar  [!DNL Adobe Workfront]  voor een grondige revisie en goedkeuring.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: cbb12ee7-949e-44a1-9340-3ef93c003b21
source-git-commit: a65a4568c6428768ee6bc60a59a8499efdbec9f8
workflow-type: tm+mt
source-wordcount: '577'
ht-degree: 0%

---

# Proefdrukken uploaden vanuit [!DNL Photoshop]

U kunt bepaalde typen voorinstellingen voor Photoshop-documenten rechtstreeks uploaden naar [!DNL Adobe Workfront] voor een grondige revisie en goedkeuring.

>[!IMPORTANT]
>
>Het dossier moet een Vooraf ingesteld Vooraf ingesteld van het Document van de Foto zijn zoals die in [ wordt beschreven Malplaatjes en stelt in Photoshop ](https://helpx.adobe.com/photoshop/using/create-documents.html) vooraf in.



## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] package</td> 
   <td> Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td> 
   <p>Standard</p>
   <p>Werk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Aanvullende producten</td> 
   <td>U moet een [!DNL Adobe Creative Cloud] licentie hebben naast een [!DNL Workfront] licentie.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bewijs van machtigingsprofiel </td> 
   <td>[!UICONTROL Manager] of hoger</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toegang bewerken tot [!UICONTROL Documents]</p>  </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

* U moet [!DNL Adobe Workfront for Photoshop] installeren voordat u proefdrukken van [!DNL Adobe Photoshop] kunt uploaden.

  Voor instructies, zie [ installeren  [!DNL Adobe Workfront for Photoshop]](../../workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-ps.md).

## Een basisproef uploaden

1. Klik op het pictogram **[!UICONTROL Menu]** in de rechterbovenhoek en selecteer vervolgens **[!UICONTROL Work List]** . U kunt het menu ook gebruiken om naar bovenliggende objecten te navigeren.

   ![ Terugkeer aan de Lijst van het Werk ](assets/go-back-to-work-list-350x314.png)

1. Ga naar het werkitem waar u een proefdruk wilt uploaden.
1. Klik het **[!UICONTROL Document]** pictogram van het pictogram van het 1} Document ![ in de navigatiebar.](assets/documents.png)
1. Klik op **[!UICONTROL New File]** onder in het deelvenster [!DNL Workfront] .
1. Schakel de **[!UICONTROL Create a proof]** -schakeloptie in.
1. (Optioneel) Typ een naam voor de proefdruk in het tekstvak **[!UICONTROL Proof Name]** .
1. Selecteer **[!UICONTROL Proof Approvals]** in de sectie **[!UICONTROL Basic]** .
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
1. Klik het **[!UICONTROL Document]** pictogram van het pictogram van het 1} Document ![ in de navigatiebar.](assets/documents.png)

1. Klik op **[!UICONTROL New File]** onder in het deelvenster [!DNL Workfront] .
1. Schakel de **[!UICONTROL Create a proof]** -schakeloptie in.
1. (Optioneel) Typ een naam voor de proefdruk in het tekstvak **[!UICONTROL Proof Name]** .
1. Selecteer **[!UICONTROL Proof Approvals]** in de sectie **[!UICONTROL Automated]** .
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
1. Klik het **[!UICONTROL Document]** pictogram van het pictogram van het 1} Document ![ in de navigatiebar.](assets/documents.png)

1. Klik op **[!UICONTROL New Version]** onder in het deelvenster [!DNL Workfront] .
1. Schakel de **[!UICONTROL Create a proof]** -schakeloptie in.

1. Kies *[!UICONTROL *Proof approvals]* of **[!UICONTROL Basic]** in de sectie **[!UICONTROL Automated]***.

1. Voeg **[!UICONTROL Reviewers]** of een **[!UICONTROL Workflow template]** toe op basis van het goedkeuringstype dat u in stap 7 hebt geselecteerd.

1. (Optioneel) Typ een opmerking in het **[!UICONTROL Updates]** -gebied.
1. Kies de **[!UICONTROL Asset Type]** in de vervolgkeuzelijst.
1. Klik op **[!UICONTROL Upload]** en configureer de gewenste exportopties op basis van het hierboven gekozen elementtype.
Het document wordt weergegeven in het gebied [!UICONTROL Documents] in het deelvenster [!DNL Workfront] in [!DNL Photoshop] en in de bureaubladtoepassing van [!DNL Workfront] .
