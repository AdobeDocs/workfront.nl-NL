---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-xd
title: XD tekengebieden als proefdrukken uploaden naar Workfront
description: U kunt uw tekengebieden als proefdrukken rechtstreeks uploaden naar Adobe Workfront voor een grondige revisie en goedkeuring.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: d6699fd7-f130-4231-8713-0cfa8dc3c910
source-git-commit: d0afdfc7be9177f6ff45dcc247253faa9dc57967
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Uploaden [!DNL XD] tekengebieden als proefdrukken naar [!DNL Workfront]

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

* U moet de [!DNL Adobe Workfront for XD] insteekmodule voordat u proefdrukken kunt uploaden [!DNL Adobe XD].

   Zie voor instructies [Installeren [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## Een statische proefdruk uploaden

1. Klik op de knop **[!UICONTROL Menu]** in de rechterbovenhoek, en selecteer vervolgens **[!UICONTROL Work List]**. U kunt het menu ook gebruiken om naar bovenliggende objecten te navigeren.

   ![](assets/menu-350x440.png)

1. Ga naar het het werkpunt waar u een statisch bewijs wilt uploaden.
1. Klik op de knop **[!UICONTROL Document]** pictogram ![](assets/documents.png) in de navigatiebalk.

1. Klikken **[!UICONTROL New File]** aan de onderkant van de plug-in.
1. Selecteer de tekengebieden die u wilt uploaden.

   >[!TIP]
   >
   >Als u meerdere tekengebieden wilt selecteren, klikt u en sleept u de muis over de gewenste tekengebieden.

1. Inschakelen **[!UICONTROL Create a Proof]**.

1. Geef de proefdruk een naam.

1. Kies het gewenste type proefdrukgoedkeuring:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic]: </td> 
      <td> <p>De basisgoedkeuringsprocessen zijn ad hoc en kunnen verschillende revisoren omvatten zoals nodig: </p> 
       <ul> 
        <li> <p>(Optioneel) Toevoegen <strong>Fiatteurs</strong> in de doos.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>Geautomatiseerde goedkeuringsprocessen worden vooraf ontwikkeld door beheerders en omvatten specifieke revisoren en fasen. Zie voor meer informatie <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Geautomatiseerd workflowoverzicht</a>.</p> 
       <ul> 
        <li> <p>Kies een [!UICONTROL Workflow Template] in het keuzemenu.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. (Optioneel) Typ een opmerking in het dialoogvenster **[!UICONTROL Updates]** gebied.

   ![](assets/proof-approvals-xd-350x396.png)

1. Kies de exportindeling in het menu **[!UICONTROL Asset Type]** vervolgkeuzemenu.


1. (Optioneel) Als u PDF selecteert als elementtype en u meerdere tekengebieden hebt geselecteerd, kiest u of u de tekengebieden wilt exporteren als **[!UICONTROL Single PDF file]s** of **M[!UICONTROL ultiple PDF files]**.

1. (Optioneel) Geef de PDF een naam.

   ![](assets/pdf-options.png)

1. Klik op **[!UICONTROL Upload]**.\
   Het document wordt weergegeven in het dialoogvenster [!UICONTROL Documents] in de plug-in en de bureaubladtoepassing.

## Een interactieve proefdruk uploaden {#upload-an-interactive-proof}

U kunt een interactieve proefdruk maken voor uw tekengebieden met de [!DNL Workfront for Adobe] insteekmodule. Het is een proces in twee stappen. Eerst moet u een interactieve koppeling maken en vervolgens moet u de proefdruk uploaden naar een tijdelijk onderdeel.

### Een interactieve koppeling maken voor uw tekengebied  {#create-an-interactive-link-for-your-art-board}

1. Open uw tekengebied en klik op **[!UICONTROL Share]** in de linkerbovenhoek van het scherm.
1. Geef de koppelingsinstellingen op:

   1. Geef de koppeling een naam.
   1. Kies een weergave-instelling.
   1. In de **[!UICONTROL Link Access]** sectie **[!UICONTROL Anyone with this link]** is geselecteerd.

      U moet dit type toegang inschakelen om een interactief bewijs te genereren.

   1. Klik op **[!UICONTROL Create Link]**.

1. Klik weer om **[!UICONTROL Design]** in de linkerbovenhoek van het scherm. Doorgaan naar de [Een interactieve proefdruk uploaden](#upload-an-interactive-proof) hieronder.

   >[!NOTE]
   >
   >Mogelijk moet u het deelvenster met de insteekmodule in de linkerbenedenhoek van het scherm opnieuw openen.

### Een interactieve proefdruk uploaden

1. Klik op de knop **[!UICONTROL Menu]** in de rechterbovenhoek, en selecteer vervolgens **[!UICONTROL Work List]**. U kunt het menu ook gebruiken om naar bovenliggende objecten te navigeren.

   ![](assets/menu-350x440.png)

1. Ga naar het werkitem waar u een interactieve proefdruk wilt uploaden.
1. Klik op de knop **[!UICONTROL Document]** pictogram ![](assets/documents.png) in de navigatiebalk.

1. Klikken **[!UICONTROL New File]** aan de onderkant van de plug-in.
1. Inschakelen **[!UICONTROL Create a Proof]**.

1. Kies het gewenste type proefdrukgoedkeuring:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic]: </td> 
      <td> <p>De basisgoedkeuringsprocessen zijn ad hoc en kunnen verschillende revisoren omvatten zoals nodig: </p> 
       <ul> 
        <li> <p>(Optioneel) Toevoegen <strong>Fiatteurs</strong> in de doos.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>Geautomatiseerde goedkeuringsprocessen worden vooraf ontwikkeld door beheerders en omvatten specifieke revisoren en fasen. Zie voor meer informatie <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Geautomatiseerd workflowoverzicht</a>.</p> 
       <ul> 
        <li> <p>Kies een [!UICONTROL Workflow Template] in het keuzemenu.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. (Optioneel) Typ een opmerking in het dialoogvenster **[!UICONTROL Updates]** gebied.

   ![](assets/proof-approvals-xd-350x396.png)

1. In de **[!UICONTROL Asset Type]** vervolgkeuzelijst, kiest u de koppeling die u zojuist hebt gemaakt onder het dialoogvenster **Gedeelde koppelingen** tab. Zie voor meer informatie [Een interactieve koppeling maken voor uw tekengebied](#create-an-interactive-link-for-your-artboard).\
   ![](assets/shared-links-xd-350x870.png)

1. Klik op **[!UICONTROL Upload]**.

   Het document wordt weergegeven in het dialoogvenster [!UICONTROL Documents] in de plug-in en de bureaubladtoepassing.

   >[!IMPORTANT]
   >
   >Gebruikers moeten toegang hebben tot [!UICONTROL Desktop Proofing Viewer] interactieve proefdrukken evalueren en goedkeuren. Zie voor meer informatie [Installeer de [!UICONTROL Desktop Proofing Viewer]](../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/installing-desktop-proofing-viewer.md).

## Een nieuwe proefdrukversie uploaden

U kunt een nieuwe versie van een proefdruk uploaden. De plug-in onthoudt de testworkflow die in de vorige versie is ingesteld, maar u kunt deze desgewenst wijzigen.

1. Klik op de knop **[!UICONTROL Menu]** in de rechterbovenhoek, en selecteer vervolgens **[!UICONTROL Work List]**. U kunt het menu ook gebruiken om naar bovenliggende objecten te navigeren.

   ![](assets/menu-350x440.png)

1. Ga naar het werkitem waarnaar u een document moet uploaden.
1. Klik op de knop **[!UICONTROL Document]** pictogram ![](assets/documents.png)in de navigatiebalk.

1. Klikken **[!UICONTROL New Version]** aan de onderkant van de plug-in.
1. Inschakelen **[!UICONTROL Create a Proof]**.
1. Selecteer de tekengebieden die u wilt uploaden.

   >[!NOTE]
   >
   >Als u een nieuwe versie van .svg, .png, of .jpg wilt uploaden, kunt u slechts één artboard uploaden.

1. Kies het gewenste type proefdrukgoedkeuring:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic]: </td> 
      <td> <p>De basisgoedkeuringsprocessen zijn ad hoc en kunnen verschillende revisoren omvatten zoals nodig: </p> 
       <ul> 
        <li> <p>(Optioneel) Toevoegen <strong>Fiatteurs</strong> in de doos.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>Geautomatiseerde goedkeuringsprocessen worden vooraf ontwikkeld door beheerders en omvatten specifieke revisoren en fasen. Zie voor meer informatie <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Geautomatiseerd workflowoverzicht</a>.</p> 
       <ul> 
        <li> <p>Kies een [!UICONTROL Workflow Template] in het keuzemenu.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. Kies de exportindeling in het menu **[!UICONTROL Asset Type]** vervolgkeuzemenu.

   ![](assets/create-a-proof-xd-350x202.png)

1. (Optioneel) Typ een opmerking in het dialoogvenster **[!UICONTROL Updates]** gebied.

   ![](assets/proof-approvals-xd-350x396.png)

1. (Optioneel) Als u PDF selecteert als elementtype en u meerdere tekengebieden hebt geselecteerd, kiest u of u de tekengebieden wilt exporteren als **[!UICONTROL Single PDF file]s** of **M[!UICONTROL ultiple PDF files]**.

1. (Optioneel) Geef de PDF een naam.

   ![](assets/pdf-options.png)

1. Klik op **[!UICONTROL Upload]**.\
   Het document wordt weergegeven in het dialoogvenster [!UICONTROL Documents] in de plug-in en de bureaubladtoepassing.
