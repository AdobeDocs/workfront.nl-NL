---
product-area: workfront-integrations;projects
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: Creeer een  [!DNL Adobe Workfront]  kwestie in Google Workspace gebruikend e-mailinhoud
description: U kunt externe e-mail (niet geproduceerd door  [!DNL Adobe Workfront)]  in a  [!DNL Workfront]  kwestie omzetten.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7a15f557-67d8-4be8-8538-4bce06536c0a
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---

# Een [!DNL Adobe Workfront] uitgave in [!DNL Google Workspace] maken met e-mailinhoud

>[!NOTE]
>
>De meest recente versie van de Adobe Workfront-insteekmodule voor Google is uitgebracht op 26 juni 2023.

U kunt een externe e-mail (niet gegenereerd door [!DNL Adobe Workfront]) converteren naar een [!DNL Workfront] -uitgave.

U kunt ook een externe e-mail converteren naar een update over een bestaande uitgave. Voor meer informatie, zie [ Update een  [!DNL Adobe Workfront]  punt van  [!DNL Google Workspace]  gebruikend e-mailinhoud ](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md).

Voor informatie over het gebruiken van [!DNL Google Workspace] om met bericht te werken e-mails die door [!DNL Workfront] worden verzonden, zie [  [!DNL Adobe Workfront]  berichtdetails van  [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md) leiden.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
   </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw [!DNL Workfront] beheerder.

## Vereisten

Voordat u een uitgave kunt maken van [!DNL Google Workspace] , moet u

* Installeren [!DNL Workfront for Google Workspace]\
   Voor instructies, zie [ installeren  [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Een [!DNL Adobe Workfront] uitgave in [!DNL Google Workspace] maken met e-mailinhoud

1. Als het [!UICONTROL Workfront for Google Workspace] paneel niet wordt getoond, klik het [!DNL Workfront] pictogram ![ pictogram van Workfront ](assets/wf-lion-icon.png) in [!DNL Google Workspace] toe:voegen-ons sidebar bij uiterst rechts van de pagina.
1. Open het e-mailbericht in [!DNL Google Workspace] en klik op een optie in [!DNL Workfront for Google Workspace] om het e-mailbericht om te zetten in een nieuwe [!DNL Workfront] -uitgave.

   ![ zet e-mail ](assets/convert-email-task-issue-update.png) om

1. Als u de uitgave aan een ouderproject wilt vastmaken, klik **[!UICONTROL Project name]**, begin de naam van het project te typen waar u de kwestie wilt, dan klik de projectnaam wanneer het in de hieronder lijst verschijnt.
1. Breng een van de volgende wijzigingen aan:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Issue Name]</td> 
      <td>Bewerk het gedeelte van deze tekst dat is ontleend aan de onderwerpregel van de e-mail.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Bewerk het gedeelte van deze tekst dat uit de tekst van de e-mail is opgehaald.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Assign To]</td> 
      <td>Klik op <strong>[!UICONTROL Assign To]</strong> , klik op de optie <strong>[!UICONTROL Assign this to]</strong> die wordt weergegeven, typ vervolgens de naam van de persoon en klik op de naam wanneer deze wordt weergegeven in de onderstaande lijst. Herhaal deze bewerking voor elke persoon die u wilt toevoegen en klik op <strong>[!UICONTROL Save]</strong> .</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Priority]</td> 
      <td>Klik op de vervolgkeuzepijl en klik vervolgens op de gewenste prioriteit voor het probleem.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Include email attachments]</td> 
      <td> <p>(Alleen beschikbaar als het e-mailbericht ten minste één bijlage bevat.) Klik op deze optie om bijlagen op te slaan in de e-mail naar het gebied [!UICONTROL Documents] van de uitgave. </p> <p>Als u geen bijlage wilt bewaren, klik X rechts van zijn naam. </p> <p>Als het e-mailbericht koppelingen naar documenten bevat in [!DNL Google Drive] , worden deze opgeslagen op het tabblad [!UICONTROL Overview] van de uitgave die u maakt. </p> <p>Belangrijk: Om dit te werken, moet uw [!DNL Workfront] beheerder [!DNL Google Drive] machtigen om met documenten in [!DNL Workfront] te werken, zoals die in de sectie <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref"> wordt beschreven vormt integratie om documenten </a> in het artikel <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref"> te beheren documentintegratie </a>.</p> <p>Als u deze optie inschakelt, blijft deze ingeschakeld voor andere e-mails die u converteert naar taken, problemen en updates.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">E-mailbestand opnemen</td> 
      <td> <p>Klik deze optie om originele e-mail als EML (E-mail) dossier <span> aan het [!UICONTROL Documents] gebied </span> van de kwestie te bewaren. Vervolgens kunt u dubbelklikken op het bestand om het e-mailbericht te openen in uw e-mailtoepassing.</p> <p>Als u deze optie inschakelt, blijft deze ingeschakeld voor andere e-mails die u converteert naar taken, problemen en updates.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klik op **[!UICONTROL Create Issue]**.

   Het tabblad **[!UICONTROL Details]** voor de nieuwe uitgave wordt weergegeven in het deelvenster [!DNL Workfront for Google Workspace] . U kunt op **[!UICONTROL Updates]** klikken en direct met medewerkers communiceren zonder uw inbox te verlaten.

   Onder aan het tabblad **[!UICONTROL Details]** kunt u ook op **[!UICONTROL View in Workfront]** klikken om naar het nieuwe probleem in Workfront te gaan.

   Wanneer u de browser vernieuwt, wordt in een bericht met een koppeling onder aan het deelvenster [!UICONTROL Workfront for Google Workspace] bevestigd dat u het e-mailbericht hebt omgezet in een uitgave:

   U kunt op de koppeling klikken om naar de weergave Details in het deelvenster [!DNL Workfront for Google Workspace] te gaan voor de uitgave die u hebt gemaakt.

   U kunt deze stappen herhalen om hetzelfde e-mailbericht om te zetten in meerdere uitgaven. Wanneer u uw browser vernieuwt of op een ander moment terugkeert naar de e-mail, worden alle koppelingen die u voor de e-mail hebt gemaakt, onder in het deelvenster [!UICONTROL Workfront for Google Workspace] weergegeven.

1. (Optioneel) Ga op een van de volgende manieren te werk om met het probleem te werken in het deelvenster [!DNL Workfront for Google Workspace] :

   * Als u een update wilt toevoegen op het tabblad **[!UICONTROL Updates]** , klikt u op **[!UICONTROL Start a new update]** en typt u de update.

   * Als u wilt reageren op een update op het tabblad **[!UICONTROL Updates]** , klikt u op **[!UICONTROL Reply]** en typt u uw antwoord.

     Voor beide bovenstaande acties kunt u bepaalde gebruikers op de hoogte stellen van uw opmerking. Klik op **[!UICONTROL Notify]**, typ de naam van een gebruiker en klik vervolgens op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst. Herhaal dit proces voor andere gebruikers die u een melding wilt sturen en klik op **[!UICONTROL Post]** .

   * Klik op het tabblad **[!UICONTROL Documents]** om documenten weer te geven die met de uitgave zijn opgeslagen.
