---
product-area: workfront-integrations;projects
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: Een [!DNL Adobe Workfront] in G Suite taken uitvoeren met e-mailinhoud
description: U kunt een externe e-mail (niet gegenereerd door Adobe) converteren [!DNL Workfront]) aan een Workfront-taak.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 6bbb4301-2791-4d72-bad8-fef63d6e892a
source-git-commit: 925e8f9d57d65fcb44068274800450d9db5c9d34
workflow-type: tm+mt
source-wordcount: '886'
ht-degree: 0%

---

# Een [!DNL Adobe Workfront] taak in [!DNL G Suite] e-mailinhoud gebruiken

>[!NOTE]
>
>Er is een [bekende kwestie](https://experienceleague.adobe.com/docs/workfront-known-issues/issues/new-workfront-experience/wf-current/wf-integrations-error-when-opening-wf-for-gsuite.html?lang=en) met de huidige versie van [!DNL Workfront for G Suite] werkt niet zoals verwacht. We werken aan een nieuwe versie en verwachten dat deze wordt vrijgegeven aan de [!DNL Google Marketplace] in de nabije toekomst .

U kunt een externe e-mail converteren (niet gegenereerd door [!DNL Adobe Workfront]) [!DNL Workfront] taak.

U kunt ook een externe e-mail converteren naar een update voor een bestaande taak. Zie voor meer informatie [Een update [!DNL Adobe Workfront] item van [!DNL G Suite] met e-mailinhoud](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md).

Voor informatie over het gebruik [!DNL G Suite] om te werken met e-mailberichten die zijn verzonden door [!DNL Workfront], zie [Beheren [!DNL Adobe Workfront] meldingsgegevens van [!DNL G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md).

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

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Vereisten

Voordat u een [!DNL Workfront] taak in [!DNL G Suite]moet u

* Installeren [!DNL Workfront for G suite]\
   Zie voor instructies [Installeren [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Een [!DNL Adobe Workfront] taak in [!DNL G Suite] e-mailinhoud gebruiken

1. Als de [!UICONTROL Workfront for G Suite] wordt niet weergegeven, klikt u op de knop [!DNL Workfront] pictogram ![](assets/wf-lion-icon.png) in de [!DNL G Suite] de zijbalk met invoegtoepassingen bevindt zich uiterst rechts op de pagina.
1. Open het e-mailbericht in [!DNL G Suite], klikt u op een optie in [!DNL Workfront for G Suite] om de e-mail naar een nieuwe [!DNL Workfront] taak.

1. Selecteer een **[!UICONTROL Create new]** optie om aan te geven of de taak deel zal uitmaken van een project of een persoonlijke taak die onafhankelijk is van een project.
1. Als u de taak aan een ouderproject wilt vastmaken, klik **[!UICONTROL Project name]**, begint de naam van het project te typen waar u de taak wilt uitvoeren en klikt u op de projectnaam wanneer deze in de onderstaande lijst wordt weergegeven.
1. Breng een van de volgende wijzigingen aan:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Task name]</td> 
      <td>Bewerk het gedeelte van deze tekst dat is ontleend aan de onderwerpregel van de e-mail.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Bewerk het gedeelte van deze tekst dat uit de tekst van de e-mail is opgehaald.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Assign To]</td> 
      <td>Klikken <strong>[!UICONTROL Assign To]</strong>klikt u op de knop <strong>[!UICONTROL Assign this to]</strong> die wordt weergegeven, typt u de naam van de persoon en klikt u erop wanneer deze in de onderstaande lijst wordt weergegeven. Herhaal deze bewerking voor elke persoon die u wilt toevoegen en klik vervolgens op <strong>[!UICONTROL Save]</strong>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Planned duration]</td> 
      <td> <p>Klikken <strong>[!UICONTROL Planned duration]</strong>Typ vervolgens het aantal dagen dat de taak moet worden uitgevoerd. </p> <p>Opmerking: Deze optie kan voor uw organisatie op verschillende manieren worden gevormd. Voor uw organisatie moet u bijvoorbeeld een aantal uren invoeren in plaats van dagen. Als u meer informatie nodig hebt, raadpleegt u uw [!DNL Workfront] beheerder. Als u een tijdspanne buiten het gevormde gebrek wilt specificeren, type <strong>m</strong>, <strong>h</strong>, <strong>d</strong>, <strong>w</strong>, of <strong>mo</strong> na het nummer minuten, uren, dagen, weken of maanden aangeven.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Priority]</td> 
      <td>Klik op de vervolgkeuzepijl en klik vervolgens op de gewenste prioriteit voor de taak.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Include email attachments]</td> 
      <td> <p>(Alleen beschikbaar als het e-mailbericht ten minste één bijlage bevat.) Klik op deze optie om bijlagen op te slaan in de e-mail naar de [!UICONTROL Documents] taakgebied. </p> <p>Als u geen bijlage wilt bewaren, klik X rechts van zijn naam. </p> <p>Als het e-mailbericht koppelingen bevat naar documenten in [!DNL Google Drive], worden ze opgeslagen in de [!UICONTROL Overview] van de taak die u maakt. </p> <p>Belangrijk: Om dit te laten werken, kunt u [!DNL Workfront] beheerder moet autoriseren [!DNL Google Drive] om te werken met documenten in [!DNL Workfront], zoals beschreven in de sectie <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">Integraties configureren om documenten te beheren</a> in het artikel <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">Documentintegratie configureren</a>.</p> <p>Als u deze optie inschakelt, blijft deze ingeschakeld voor andere e-mails die u converteert naar taken, problemen en updates.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Include email file]</td> 
      <td> <p>Klik op deze optie om de oorspronkelijke e-mail op te slaan als een e-mailbestand (EML) <span>aan de [!UICONTROL Documents] gebied</span> van de taak. Vervolgens kunt u dubbelklikken op het bestand om het e-mailbericht te openen in uw e-mailtoepassing.</p> <p>Als u deze optie inschakelt, blijft deze ingeschakeld voor andere e-mails die u converteert naar taken, problemen en updates.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klik op **[!UICONTROL Create Task]**.

   De **[!UICONTROL Details]** tabblad voor de nieuwe taak wordt weergegeven in het dialoogvenster [!DNL Workfront for G Suite] deelvenster. U kunt op **[!UICONTROL Updates]** en communiceer meteen met medewerkers zonder uw inbox te verlaten.

   Onder aan het dialoogvenster **[!UICONTROL Details]** kunt u ook op **[!UICONTROL View in [!DNL Workfront]]** om naar de nieuwe taak in Workfront te gaan.

   Wanneer u uw browser vernieuwt, verschijnt er een bericht met een koppeling onder aan het dialoogvenster [!DNL Workfront for G Suite] bevestigt dat u de e-mail naar een taak hebt geconverteerd:

   U kunt op de koppeling klikken om naar de weergave Details te gaan, in het dialoogvenster [!DNL Workfront for G Suite] voor de taak die u hebt gemaakt.

   U kunt deze stappen herhalen om dezelfde e-mail om te zetten in meerdere taken. Wanneer u uw browser vernieuwt of op een ander moment terugkeert naar de e-mail, worden alle koppelingen die u voor de e-mail hebt gemaakt, onder aan het dialoogvenster weergegeven [!UICONTROL Workfront for G Suite] deelvenster.

1. (Optioneel) Ga door met het werken met de taak in de [!DNL Workfront for G Suite] door een van de volgende handelingen uit te voeren:

   * Een update toevoegen op de knop **[!UICONTROL Updates]** tabblad, klikt u op **[!UICONTROL Start a new update]** en typ de update.

   * Als u wilt reageren op een update van de **[!UICONTROL Updates]** tabblad, klikt u op **[!UICONTROL Reply]** en typ uw antwoord.

      Voor beide bovenstaande acties kunt u bepaalde gebruikers op de hoogte stellen van uw opmerking. Klikken **[!UICONTROL Notify]** begint u de naam van een gebruiker te typen en klikt u vervolgens op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst. Herhaal dit proces voor andere gebruikers die u een melding wilt sturen en klik vervolgens op **[!UICONTROL Post]**.

   * Klik op de knop **[!UICONTROL Documents]** om documenten weer te geven die met de taak zijn opgeslagen.

U kunt deze stappen herhalen om dezelfde e-mail om te zetten in meerdere taken. Wanneer u uw browser vernieuwt of op een ander moment terugkeert naar de e-mail, worden alle koppelingen die u voor de e-mail hebt gemaakt, onder aan het dialoogvenster weergegeven [!DNL Workfront for G Suite] deelvenster.
