---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-xd
title: XD tekengebieden als proefdrukken uploaden naar Workfront
description: U kunt uw tekengebieden als proefdrukken rechtstreeks uploaden naar Adobe Workfront voor een grondige revisie en goedkeuring.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: d6699fd7-f130-4231-8713-0cfa8dc3c910
source-git-commit: 4256e1ecd16179d0a2aa8e623b05be754d8bbd2d
workflow-type: tm+mt
source-wordcount: '915'
ht-degree: 0%

---

# [!DNL XD] tekengebieden als proefdrukken uploaden naar [!DNL Workfront]

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
   <td> <p>Toegang bewerken tot [!UICONTROL Documents]</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, rol, of Profiel van de Toestemming van het Bewijs u hebt, contacteer uw [!DNL Workfront] of [!DNL Workfront Proof] beheerder.

+++

## Vereisten

* U moet de plug-in [!DNL Adobe Workfront for XD] installeren voordat u proefdrukken kunt uploaden in [!DNL Adobe XD] .

  Voor instructies, zie [ installeren  [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## Een statische proefdruk uploaden

1. Klik op het pictogram **[!UICONTROL Menu]** in de rechterbovenhoek en selecteer vervolgens **[!UICONTROL Work List]** . U kunt het menu ook gebruiken om naar bovenliggende objecten te navigeren.

   ![](assets/menu-350x440.png)

1. Ga naar het het werkpunt waar u een statisch bewijs wilt uploaden.
1. Klik op het pictogram **[!UICONTROL Document]** ![](assets/documents.png) op de navigatiebalk.

1. Klik op **[!UICONTROL New File]** onder aan de plug-in.
1. Selecteer de tekengebieden die u wilt uploaden.

   >[!TIP]
   >
   >* Tekengebieden worden in de proefdruk weergegeven in de volgorde waarin ze zijn geselecteerd. Het eerste geselecteerde tekengebied wordt de eerste pagina in de proefdruk, enzovoort.
   >* Als u snel meer dan één tekengebied wilt selecteren, klikt u en sleept u de muis over de gewenste tekengebieden. Hierdoor kunt u de volgorde van tekengebieden in de proefdruk niet bepalen.

1. Schakel **[!UICONTROL Create a Proof]** in.

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
        <li> <p>(Facultatief) voeg <strong> Approvers </strong> in de doos toe.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>Geautomatiseerde goedkeuringsprocessen worden vooraf ontwikkeld door beheerders en omvatten specifieke revisoren en fasen. Voor meer informatie, zie <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref"> Geautomatiseerd overzicht van het Werkschema </a>.</p> 
       <ul> 
        <li> <p>Kies een [!UICONTROL Workflow Template] in de keuzelijst.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. (Optioneel) Typ een opmerking in het **[!UICONTROL Updates]** -gebied.

   ![](assets/proof-approvals-xd-350x396.png)

1. Kies de exportindeling in het keuzemenu **[!UICONTROL Asset Type]** .


1. (Facultatief) als u PDF als activatype selecteert en meer dan één geselecteerd artboard hebt, kies als u uw artboards als **[!UICONTROL Single PDF file]s** of **M[!UICONTROL ultiple PDF files]** wilt uitvoeren.

1. (Optioneel) Geef de PDF een naam.

   ![](assets/pdf-options.png)

1. Klik op **[!UICONTROL Upload]**.\
   Het document wordt weergegeven in het gebied [!UICONTROL Documents] in de plug-in en de bureaubladtoepassing.

## Een interactieve proefdruk uploaden {#upload-an-interactive-proof}

Met de [!DNL Workfront for Adobe] -plug-in kunt u een interactieve proefdruk maken voor uw tekengebieden. Het is een proces in twee stappen. Eerst moet u een interactieve koppeling maken en vervolgens moet u de proefdruk uploaden naar een tijdelijk onderdeel.

### Een interactieve koppeling maken voor uw tekengebied  {#create-an-interactive-link-for-your-art-board}

1. Open het tekengebied en klik vervolgens op **[!UICONTROL Share]** linksboven in het scherm.
1. Geef de koppelingsinstellingen op:

   1. Geef de koppeling een naam.
   1. Kies een weergave-instelling.
   1. Controleer of **[!UICONTROL Anyone with this link]** is geselecteerd in de sectie **[!UICONTROL Link Access]** .

      U moet dit type toegang inschakelen om een interactief bewijs te genereren.

   1. Klik op **[!UICONTROL Create Link]**.

1. Klik weer op **[!UICONTROL Design]** in de linkerbovenhoek van het scherm. Ga aan [ verder uploaden een interactieve proefdruk ](#upload-an-interactive-proof) hieronder sectie.

   >[!NOTE]
   >
   >Mogelijk moet u het deelvenster met de insteekmodule in de linkerbenedenhoek van het scherm opnieuw openen.

### Een interactieve proefdruk uploaden

1. Klik op het pictogram **[!UICONTROL Menu]** in de rechterbovenhoek en selecteer vervolgens **[!UICONTROL Work List]** . U kunt het menu ook gebruiken om naar bovenliggende objecten te navigeren.

   ![](assets/menu-350x440.png)

1. Ga naar het werkitem waar u een interactieve proefdruk wilt uploaden.
1. Klik op het pictogram **[!UICONTROL Document]** ![](assets/documents.png) op de navigatiebalk.

1. Klik op **[!UICONTROL New File]** onder aan de plug-in.
1. Schakel **[!UICONTROL Create a Proof]** in.

1. Kies het gewenste type proefdrukgoedkeuring:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic]: </td> 
      <td> <p>De basisgoedkeuringsprocessen zijn ad hoc en kunnen verschillende revisoren omvatten zoals nodig: </p> 
       <ul> 
        <li> <p>(Facultatief) voeg <strong> Approvers </strong> in de doos toe.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>Geautomatiseerde goedkeuringsprocessen worden vooraf ontwikkeld door beheerders en omvatten specifieke revisoren en fasen. Voor meer informatie, zie <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref"> Geautomatiseerd overzicht van het Werkschema </a>.</p> 
       <ul> 
        <li> <p>Kies een [!UICONTROL Workflow Template] in de keuzelijst.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. (Optioneel) Typ een opmerking in het **[!UICONTROL Updates]** -gebied.

   ![](assets/proof-approvals-xd-350x396.png)

1. In het **[!UICONTROL Asset Type]** drop-down menu, kies de verbinding u enkel onder **Gedeelde verbindingen** tabel creeerde. Voor meer informatie, zie [ een interactieve verbinding voor uw artboard ](#create-an-interactive-link-for-your-artboard) creëren.\
   ![](assets/shared-links-xd-350x870.png)

1. Klik op **[!UICONTROL Upload]**.

   Het document wordt weergegeven in het gebied [!UICONTROL Documents] in de plug-in en de bureaubladtoepassing.

   >[!IMPORTANT]
   >
   >Gebruikers moeten toegang hebben tot [!UICONTROL Desktop Proofing Viewer] om interactieve proefdrukken te kunnen beoordelen en goedkeuren. Voor meer informatie, zie [ installeer [!UICONTROL Desktop Proofing Viewer]](../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/installing-desktop-proofing-viewer.md).

## Een nieuwe proefdrukversie uploaden

U kunt een nieuwe versie van een proefdruk uploaden. De plug-in onthoudt de testworkflow die in de vorige versie is ingesteld, maar u kunt deze desgewenst wijzigen.

1. Klik op het pictogram **[!UICONTROL Menu]** in de rechterbovenhoek en selecteer vervolgens **[!UICONTROL Work List]** . U kunt het menu ook gebruiken om naar bovenliggende objecten te navigeren.

   ![](assets/menu-350x440.png)

1. Ga naar het werkitem waarnaar u een document moet uploaden.
1. Klik op het **[!UICONTROL Document]** pictogram ![](assets/documents.png) op de navigatiebalk.

1. Klik op **[!UICONTROL New Version]** onder aan de plug-in.
1. Schakel **[!UICONTROL Create a Proof]** in.
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
        <li> <p>(Facultatief) voeg <strong> Approvers </strong> in de doos toe.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>Geautomatiseerde goedkeuringsprocessen worden vooraf ontwikkeld door beheerders en omvatten specifieke revisoren en fasen. Voor meer informatie, zie <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref"> Geautomatiseerd overzicht van het Werkschema </a>.</p> 
       <ul> 
        <li> <p>Kies een [!UICONTROL Workflow Template] in de keuzelijst.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. Kies de exportindeling in het keuzemenu **[!UICONTROL Asset Type]** .

   ![](assets/create-a-proof-xd-350x202.png)

1. (Optioneel) Typ een opmerking in het **[!UICONTROL Updates]** -gebied.

   ![](assets/proof-approvals-xd-350x396.png)

1. (Facultatief) als u PDF als activatype selecteert en meer dan één geselecteerd artboard hebt, kies als u uw artboards als **[!UICONTROL Single PDF file]s** of **M[!UICONTROL ultiple PDF files]** wilt uitvoeren.

1. (Optioneel) Geef de PDF een naam.

   ![](assets/pdf-options.png)

1. Klik op **[!UICONTROL Upload]**.\
   Het document wordt weergegeven in het gebied [!UICONTROL Documents] in de plug-in en de bureaubladtoepassing.
