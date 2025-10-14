---
product-area: workfront-integrations;projects
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: Update een  [!DNL Adobe Workfront]  punt van Google Workspace gebruikend e-mailinhoud
description: U kunt een bestaand project, een bestaande taak of een bestaand probleem bijwerken met informatie uit een niet-Adobe Workfront-e-mail.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 2ac392f5-98a3-4ab6-a0e3-cda378f0f68b
source-git-commit: 58543982fef6e7ba2d05787dc023a2099e47bbc7
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 0%

---

# Een [!DNL Adobe Workfront] item uit [!DNL Google Workspace] bijwerken met e-mailinhoud

>[!IMPORTANT]
>
>Om stabielere en scalable integratie te leveren, verschuiven wij naar een moderne, flexibele integratiebenadering gebruikend Workfront Automation and Integration (Fusion). Als deel van dit overgangsproces, zal volgende Workfront voor de functionaliteit van Google Workspace niet beschikbaar na **28 Februari, 2026** zijn:
>
>* Google Workspace-functionaliteit openen vanuit Workfront
>
>* Workfront-taken weergeven en beheren vanuit Gmail of het Google Calendar-sitevenster
>
>We raden u aan Workfront Automation and Integration te gebruiken voor de integratiebehoeften van uw organisatie met Google Workspace.
>
>Voor een overzicht van de Automatisering en de Integratie van Workfront, zie [&#x200B; het overzicht van de Fusie van Adobe Workfront &#x200B;](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Voor informatie over de specifieke mogelijkheden van de modules van de Automatisering en van de Integratie van Workfront voor Google Workspace, zie [&#x200B; modules van Gmail &#x200B;](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules) en [&#x200B; modules van de Kalender van Google &#x200B;](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules).

U kunt een bestaand project, een taak, of een kwestie bijwerken met informatie van niet [!DNL Adobe Workfront] e-mail.

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

Voordat u een [!DNL Workfront] -item kunt bijwerken met e-mailinhoud uit [!DNL Google Workspace] , moet u

* Installeren [!DNL Workfront for Google Workspace]\
   Voor instructies, zie [&#x200B; installeren  [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Een [!DNL Workfront] -item bijwerken met e-mailinhoud uit [!DNL Google Workspace]

1. Als het [!UICONTROL Workfront for Google Workspace] paneel niet wordt getoond, klik het pictogram van Workfront ![&#x200B; Workfront &#x200B;](assets/wf-lion-icon.png) in [!DNL Google Workspace] toe:voegen-ons sidebar bij uiterst rechts van de pagina.
1. Open het e-mailbericht in [!DNL Google Workspace] en klik op **[!UICONTROL Post as a new update]** in het deelvenster [!DNL Google Workspace] .
1. Klik onder **[!UICONTROL Type]** op de vervolgkeuzepijl en klik vervolgens op het type object waar u de update wilt toevoegen.
1. Klik op de optie **[!UICONTROL Search for]** , typ de naam van het object waaraan u de update wilt toevoegen en selecteer het item wanneer dit in de onderstaande lijst wordt weergegeven.

   Deze optie is afhankelijk van de optie die u in stap 3 hebt geselecteerd. Dit kan **[!UICONTROL Search for a project]** , **[!UICONTROL Search for a task]** of **[!UICONTROL Search for an issue]** zijn.

   >[!NOTE]
   >
   >Wanneer u de naam van een taak typt, worden persoonlijke ad-hoctaken uitgesloten van de onderstaande lijst met namen.

1. Voer een van de volgende optionele wijzigingen in:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Update]</td> 
      <td>Bewerk het gedeelte van deze tekst dat is ontleend aan de onderwerpregel en hoofdtekst van de e-mail.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Include email attachments]</td> 
      <td><p>(Alleen beschikbaar als het e-mailbericht ten minste één bijlage bevat.) Klik op deze optie om bijlagen op te slaan op het tabblad [!UICONTROL Documents] voor de taak of uitgave. </p><p>Als u geen bijlage wilt bewaren, klik X rechts van zijn naam. </p><p>Als het e-mailbericht koppelingen naar documenten bevat in [!DNL Google Drive] , worden de koppelingen opgeslagen op het tabblad [!UICONTROL Overview] van de taak of uitgave die u maakt. </p><p>Belangrijk: <span style="color: #ff1493;"><span style="color: #000000;"> opdat dit werkt, moet uw </span></span>[!DNL Workfront] beheerder <span style="color: #ff1493;"><span style="color: #000000;"> [!DNL Google Drive] om met [!DNL Workfront]</span></span> machtigen te werken</p>
      <p>Als u deze optie inschakelt, blijft deze ingeschakeld voor andere e-mails die u converteert naar taken, problemen en updates.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Waarschuwen</td> 
      <td>Klik op <strong>[!UICONTROL Notify]</strong> , klik op de optie <strong>[!UICONTROL Search for a user or team]</strong> die wordt weergegeven, typ vervolgens de naam van de persoon of het team en klik op de naam wanneer deze wordt weergegeven in de onderstaande lijst. Herhaal deze bewerking voor elke persoon en elk team dat u wilt toevoegen en klik op <strong>[!UICONTROL Save]</strong> .</td> 
     </tr> 
    </tbody> 
   </table>

1. Klik op **[!UICONTROL Update]**.

   Wanneer u de browser vernieuwt, wordt in een bericht met een koppeling onder aan het deelvenster [!DNL Workfront for Google Workspace] bevestigd dat u de e-mail hebt geconverteerd naar een update:

   U kunt op de koppeling klikken om naar de tab [!UICONTROL Updates] in [!DNL Workfront] te gaan voor het object dat u in stap 4 hebt opgegeven.

   U kunt deze stappen herhalen om zelfde e-mail in updates, taak, en kwesties (zie [&#x200B; tot een kwestie van Adobe Workfront in  [!DNL Google Workspace]  gebruikend e-mailinhoud &#x200B;](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md) leiden) om te zetten. Wanneer u uw browser vernieuwt of op een ander moment terugkeert naar de e-mail, worden alle koppelingen die u voor de e-mail hebt gemaakt, onder in het deelvenster [!UICONTROL Workfront for Google Workspace] weergegeven.

1. (Optioneel) Ga op een van de volgende manieren te werk om met de update te werken in het invoegvenster van [!DNL Workfront] :

   * Als u nog een update wilt toevoegen op het tabblad **[!UICONTROL Updates]** , klikt u op **[!UICONTROL Start a new update]** en typt u de informatie.

   * Als u wilt reageren op een update op het tabblad **[!UICONTROL Updates]** , klikt u op **[!UICONTROL Reply]** en typt u uw antwoord.

     Voor beide bovenstaande opties kunt u op **[!UICONTROL Notify]** klikken om ontvangers voor het antwoord op te geven, zoals in stap 5. Als u klaar bent, klikt u op **[!UICONTROL Post]** om de update of het antwoord toe te voegen.

   * Klik op het tabblad **[!UICONTROL Details]** om de details van het nieuwe project, de nieuwe taak of de nieuwe uitgave weer te geven.
