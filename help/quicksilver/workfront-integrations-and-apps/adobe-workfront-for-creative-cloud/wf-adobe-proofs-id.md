---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Proefdrukken van InDesign uploaden
description: U kunt uw tekengebieden uploaden als documenten die u snel kunt bekijken en goedkeuren of die u gewoon in Adobe Workfront wilt opslaan.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: ee3dc446-6886-4285-a942-4f44f5c0ac31
source-git-commit: 68dae619348c3359ea8a7ae3ff84543d5e4171ec
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# Proefbestanden uploaden van [!DNL InDesign]

U kunt tekengebieden als proefdrukken rechtstreeks uploaden naar [!DNL Adobe Workfront] voor een grondige herziening en goedkeuring.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Huidig plan: [!UICONTROL Pro] of hoger</p> <p>of</p> <p>Ouder plan: [!UICONTROL Premium]</p> <p>Voor meer informatie over het proefdrukken van toegang met de verschillende plannen, zie.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td> <p>Huidig plan: [!UICONTROL Work] of [!UICONTROL Proof]</p> <p>Ouder plan: Willekeurig (proefdrukken moet zijn ingeschakeld voor de gebruiker)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>U moet beschikken over een [!DNL Adobe Creative Cloud] naast een [!DNL Workfront] licentie.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bewijs van machtigingsprofiel </td> 
   <td>[!UICONTROL Manager] of hoger</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toegang bewerken tot [!UICONTROL Documents]</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] of [!DNL Workfront Proof] beheerder.

## Vereisten

* U moet de [!DNL Adobe Workfront for design and video] insteekmodule voordat u proefdrukken kunt uploaden van [!DNL InDesign].

   Zie voor instructies [Installeren [!DNL Adobe Workfront for design and video]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-install-cc.md).

## Een basisproef uploaden

1. Klik op de knop **[!UICONTROL Menu]** in de rechterbovenhoek, en selecteer vervolgens **[!UICONTROL Work List]**. U kunt het menu ook gebruiken om naar bovenliggende objecten te navigeren.

   ![](assets/go-back-to-work-list-350x314.png)

1. Ga naar het werkitem waar u een proefdruk wilt uploaden.
1. Klik op de knop **[!UICONTROL Document]** pictogram ![](assets/documents.png) in de navigatiebalk.
1. Klikken **[!UICONTROL New File]** aan de onderkant van de plug-in.
1. De optie **[!UICONTROL Create a proof]** schakelen.
1. (Optioneel) Typ een naam voor de proefdruk in het dialoogvenster **[!UICONTROL Proof Name]** tekstvak.
1. In de **[!UICONTROL Proof Approvals]** sectie, selecteert u **[!UICONTROL Basic]**.
1. (Optioneel) Voeg fiatteurs toe.
1. (Optioneel) Typ een opmerking in het dialoogvenster **[!UICONTROL Updates]** gebied.

   ![](assets/add-comment.png)

1. Kies de optie **[!UICONTROL Asset Type]** in het keuzemenu.

1. (Optioneel) Selecteer **[!UICONTROL Add outside file]** om een bestand van uw computer toe te voegen.
1. Klikken **[!UICONTROL Upload]** Configureer vervolgens de gewenste exportopties op basis van het hierboven gekozen elementtype.

   ![](assets/plugin-files-350x307.png)\
   Het document wordt weergegeven in het dialoogvenster [!UICONTROL Documents] in de plug-in en de bureaubladtoepassing.


## Een automatische proefdruk uploaden

1. Klik op de knop **[!UICONTROL Menu]** in de rechterbovenhoek, en selecteer vervolgens **[!UICONTROL Work List]**. U kunt het menu ook gebruiken om naar bovenliggende objecten te navigeren.

   ![](assets/go-back-to-work-list-350x314.png)

1. Ga naar het werkitem waar u een proefdruk wilt uploaden.
1. Klik op de knop **[!UICONTROL Document]** pictogram ![](assets/documents.png) in de navigatiebalk.

1. Klikken **[!UICONTROL New File]** aan de onderkant van de plug-in.
1. De optie **[!UICONTROL Create a proof]** schakelen.
1. (Optioneel) Typ een naam voor de proefdruk in het dialoogvenster **[!UICONTROL Proof Name]** tekstvak.
1. In de **[!UICONTROL Proof Approvals]** sectie, selecteert u **[!UICONTROL Automated]**.
1. (Optioneel) In het dialoogvenster **[!UICONTROL Workflow Template]** typt u de naam van een sjabloon voor een proefdrukwerkstroom.

{{adjust-proof-settings}}

>[!NOTE]
>
> Als het werkstroomsjabloon lege verplichte velden bevat, worden de automatische proefdrukinstellingen automatisch geopend en moet u deze velden invullen om de proefdrukinstellingen te kunnen uploaden.


1. (Optioneel) Typ een opmerking in het dialoogvenster **[!UICONTROL Updates]** gebied.

   ![](assets/add-comment-automated-approval.png)

1. Kies de optie **[!UICONTROL Asset Type]** in het keuzemenu.
1. (Optioneel) Selecteer **[!UICONTROL Add outside file]** om een bestand van uw computer toe te voegen.
1. Klikken **[!UICONTROL Upload]**Configureer vervolgens de gewenste exportopties op basis van het hierboven gekozen elementtype.
Het document wordt weergegeven in het dialoogvenster [!UICONTROL Documents] in de plug-in en de bureaubladtoepassing.

## Een nieuwe proefdrukversie uploaden

U kunt een nieuwe versie van een proefdruk uploaden. De plug-in onthoudt de testworkflow die in de vorige versie is ingesteld, maar u kunt deze desgewenst wijzigen.

1. Klik op de knop **[!UICONTROL Menu]** in de rechterbovenhoek, en selecteer vervolgens **[!UICONTROL Work List]**. U kunt het menu ook gebruiken om naar bovenliggende objecten te navigeren.

   ![](assets/go-back-to-work-list-350x314.png)

1. Ga naar het werkitem waarnaar u een document moet uploaden.
1. Klik op de knop **[!UICONTROL Document]** pictogram ![](assets/documents.png)in de navigatiebalk.

1. Klikken **[!UICONTROL New Version]** aan de onderkant van de plug-in.
1. De optie **[!UICONTROL Create a proof]** schakelen.

1. In de *[!UICONTROL *Proof approvals]**, kiest u **[!UICONTROL Basic]** of **[!UICONTROL Automated]**.

1. Toevoegen **[!UICONTROL Reviewers]** of **[!UICONTROL Workflow template]** op basis van het goedkeuringstype dat u in stap 7 hebt geselecteerd.

1. (Optioneel) Typ een opmerking in het dialoogvenster **[!UICONTROL Updates]** gebied.
1. Kies de optie **[!UICONTROL Asset Type]** in het keuzemenu.
1. Klikken **[!UICONTROL Upload]**Configureer vervolgens de gewenste exportopties op basis van het hierboven gekozen elementtype.
Het document wordt weergegeven in het dialoogvenster [!UICONTROL Documents] in de plug-in en de bureaubladtoepassing.
