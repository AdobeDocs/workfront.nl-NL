---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Proefbestanden uploaden vanuit InDesign
description: U kunt uw tekengebieden uploaden als documenten die u snel kunt bekijken en goedkeuren of die u gewoon in Adobe Workfront wilt opslaan.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: ee3dc446-6886-4285-a942-4f44f5c0ac31
source-git-commit: a65a4568c6428768ee6bc60a59a8499efdbec9f8
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 0%

---

# Proefdrukken uploaden vanuit [!DNL InDesign]

U kunt tekengebieden als proefdrukken rechtstreeks uploaden naar [!DNL Adobe Workfront] voor een grondige revisie en goedkeuring.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] package</td> 
   <td>Alle </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td> <p>Standard</p> <p>Werk of hoger</p> </td> 
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
   <td> <p>Toegang bewerken tot [!UICONTROL Documents]</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Vereisten

* U moet de plug-in [!DNL Adobe Workfront for design and video] installeren voordat u proefdrukken van [!DNL InDesign] kunt uploaden.

  Voor instructies, zie [&#x200B; installeren  [!DNL Adobe Workfront for design and video]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-install-cc.md).

## Een basisproef uploaden

1. Klik op het pictogram **[!UICONTROL Menu]** in de rechterbovenhoek en selecteer vervolgens **[!UICONTROL Work List]** . U kunt het menu ook gebruiken om naar bovenliggende objecten te navigeren.

   ![&#x200B; Terugkeer aan de Lijst van het Werk &#x200B;](assets/go-back-to-work-list-350x314.png)

1. Ga naar het werkitem waar u een proefdruk wilt uploaden.
1. Klik het **[!UICONTROL Document]** pictogram van het pictogram van het 1&rbrace; Document ![&#x200B; in de navigatiebar.](assets/documents.png)
1. Klik op **[!UICONTROL New File]** onder aan de plug-in.
1. Schakel de **[!UICONTROL Create a proof]** -schakeloptie in.
1. (Optioneel) Typ een naam voor de proefdruk in het tekstvak **[!UICONTROL Proof Name]** .
1. Selecteer **[!UICONTROL Proof Approvals]** in de sectie **[!UICONTROL Basic]** .
1. (Optioneel) Voeg fiatteurs toe.
1. (Optioneel) Typ een opmerking in het **[!UICONTROL Updates]** -gebied.

   ![&#x200B; voeg een commentaar &#x200B;](assets/add-comment.png) toe

1. Kies de **[!UICONTROL Asset Type]** in de vervolgkeuzelijst.

1. (Optioneel) Selecteer **[!UICONTROL Add outside file]** om een bestand van uw computer toe te voegen.
1. Klik op **[!UICONTROL Upload]** en configureer de gewenste exportopties op basis van het hierboven gekozen elementtype.

   ![&#x200B; Dossiers in plugin &#x200B;](assets/plugin-files-350x307.png)\
   Het document wordt weergegeven in het gebied [!UICONTROL Documents] in de plug-in en de bureaubladtoepassing.


## Een automatische proefdruk uploaden

1. Klik op het pictogram **[!UICONTROL Menu]** in de rechterbovenhoek en selecteer vervolgens **[!UICONTROL Work List]** . U kunt het menu ook gebruiken om naar bovenliggende objecten te navigeren.

   ![&#x200B; Terugkeer aan de Lijst van het Werk &#x200B;](assets/go-back-to-work-list-350x314.png)

1. Ga naar het werkitem waar u een proefdruk wilt uploaden.
1. Klik het **[!UICONTROL Document]** pictogram van het pictogram van het 1&rbrace; Document ![&#x200B; in de navigatiebar.](assets/documents.png)

1. Klik op **[!UICONTROL New File]** onder aan de plug-in.
1. Schakel de **[!UICONTROL Create a proof]** -schakeloptie in.
1. (Optioneel) Typ een naam voor de proefdruk in het tekstvak **[!UICONTROL Proof Name]** .
1. Selecteer **[!UICONTROL Proof Approvals]** in de sectie **[!UICONTROL Automated]** .
1. (Optioneel) Typ in het vak **[!UICONTROL Workflow Template]** de naam van een sjabloon voor de proefdrukworkflow.

{{adjust-proof-settings}}

>[!NOTE]
>
> Als het werkstroomsjabloon lege verplichte velden bevat, worden de automatische proefdrukinstellingen automatisch geopend en moet u deze velden invullen om de proefdrukinstellingen te kunnen uploaden.


1. (Optioneel) Typ een opmerking in het **[!UICONTROL Updates]** -gebied.

   ![&#x200B; voeg commentaargeautomatiseerde goedkeuring &#x200B;](assets/add-comment-automated-approval.png) toe

1. Kies de **[!UICONTROL Asset Type]** in de vervolgkeuzelijst.
1. (Optioneel) Selecteer **[!UICONTROL Add outside file]** om een bestand van uw computer toe te voegen.
1. Klik op **[!UICONTROL Upload]** en configureer de gewenste exportopties op basis van het hierboven gekozen elementtype.
Het document wordt weergegeven in het gebied [!UICONTROL Documents] in de plug-in en de bureaubladtoepassing.

## Een nieuwe proefdrukversie uploaden

U kunt een nieuwe versie van een proefdruk uploaden. De plug-in onthoudt de testworkflow die in de vorige versie is ingesteld, maar u kunt deze desgewenst wijzigen.

1. Klik op het pictogram **[!UICONTROL Menu]** in de rechterbovenhoek en selecteer vervolgens **[!UICONTROL Work List]** . U kunt het menu ook gebruiken om naar bovenliggende objecten te navigeren.

   ![&#x200B; Terugkeer aan de Lijst van het Werk &#x200B;](assets/go-back-to-work-list-350x314.png)

1. Ga naar het werkitem waarnaar u een document moet uploaden.
1. Klik het **[!UICONTROL Document]** pictogram van het pictogram van het 1&rbrace; Document ![&#x200B; in de navigatiebar.](assets/documents.png)

1. Klik op **[!UICONTROL New Version]** onder aan de plug-in.
1. Schakel de **[!UICONTROL Create a proof]** -schakeloptie in.

1. Kies *[!UICONTROL *Proof approvals]* of **[!UICONTROL Basic]** in de sectie **[!UICONTROL Automated]***.

1. Voeg **[!UICONTROL Reviewers]** of een **[!UICONTROL Workflow template]** toe op basis van het goedkeuringstype dat u in stap 7 hebt geselecteerd.

1. (Optioneel) Typ een opmerking in het **[!UICONTROL Updates]** -gebied.
1. Kies de **[!UICONTROL Asset Type]** in de vervolgkeuzelijst.
1. Klik op **[!UICONTROL Upload]** en configureer de gewenste exportopties op basis van het hierboven gekozen elementtype.
Het document wordt weergegeven in het gebied [!UICONTROL Documents] in de plug-in en de bureaubladtoepassing.
