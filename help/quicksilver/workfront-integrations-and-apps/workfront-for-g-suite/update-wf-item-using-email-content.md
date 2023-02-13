---
product-area: workfront-integrations;projects
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: Een update [!DNL Adobe Workfront] item uit G Suite gebruiken met e-mailinhoud
description: U kunt een bestaand project, een bestaande taak of een bestaand probleem bijwerken met informatie uit een niet-Adobe Workfront-e-mail.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 2ac392f5-98a3-4ab6-a0e3-cda378f0f68b
source-git-commit: 3143e5a4988b7234d8225da442f5af1d756d461d
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 0%

---

# Een update [!DNL Adobe Workfront] item van [!DNL G Suite] e-mailinhoud gebruiken

U kunt een bestaand project, een bestaande taak of een bestaande uitgave bijwerken met informatie van een niet-[!DNL Adobe Workfront] e-mail.

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

Voordat u een [!DNL Workfront] item met e-mailinhoud van [!DNL G Suite]moet u

* Installeren [!DNL Workfront for G suite]\
   Zie voor instructies [Installeren [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Een update [!DNL Workfront] item met e-mailinhoud van [!DNL G Suite]

1. Als de [!UICONTROL Workfront for G Suite] wordt niet weergegeven, klikt u op het Workfront-pictogram ![](assets/wf-lion-icon.png) in de [!DNL G Suite] de zijbalk met invoegtoepassingen bevindt zich uiterst rechts op de pagina.
1. Open het e-mailbericht in [!DNL G Suite], klikt u op **[!UICONTROL Post as a new update]** in de [!DNL G Suite] deelvenster.
1. Onder **[!UICONTROL Type]** Klik op de vervolgkeuzepijl en klik vervolgens op het type object waar u de update wilt toevoegen.
1. Klik op de knop **[!UICONTROL Search for]** typt u de naam van het object waar u de update wilt toevoegen en selecteert u vervolgens het item wanneer dit wordt weergegeven in de onderstaande lijst.

   ![](assets/click-search-for-task-issue.png)

   Deze optie is afhankelijk van de optie die u in stap 3 hebt geselecteerd. Misschien is het **[!UICONTROL Search for a project]**, **[!UICONTROL Search for a task]**, of **[!UICONTROL Search for an issue]**.

   >[!NOTE]
   >
   >Wanneer u de naam van een taak typt, worden persoonlijke ad-hoctaken uitgesloten van de lijst met namen die hieronder wordt weergegeven.

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
      <td><p>(Alleen beschikbaar als het e-mailbericht ten minste één bijlage bevat.) Klik op deze optie om bijlagen op te slaan in het dialoogvenster [!UICONTROL Documents] tabblad voor de taak of uitgave. </p><p>Als u geen bijlage wilt bewaren, klik X rechts van zijn naam. </p><p>Als het e-mailbericht koppelingen bevat naar documenten in [!DNL Google Drive], worden de koppelingen opgeslagen naar de [!UICONTROL Overview] tabblad van de taak of uitgave die u maakt. </p><p>Belangrijk: <span style="color: #ff1493;"><span style="color: #000000;">Om dit te laten werken, kunt u</span></span>[!DNL Workfront] beheerder<span style="color: #ff1493;"><span style="color: #000000;"> autoriseren [!DNL Google Drive] werken met [!DNL Workfront]</span></span></p>
      <p>Als u deze optie inschakelt, blijft deze ingeschakeld voor andere e-mails die u converteert naar taken, problemen en updates.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Waarschuwen</td> 
      <td>Klikken <strong>[!UICONTROL Notify]</strong>klikt u op de knop <strong>[!UICONTROL Search for a user or team]</strong> die wordt weergegeven, typt u de naam van de persoon of het team en klikt u erop wanneer deze in de onderstaande lijst wordt weergegeven. Herhaal dit voor elke persoon en elk team u wilt toevoegen, dan klik <strong>[!UICONTROL Save]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klik op **[!UICONTROL Update]**.

   Wanneer u uw browser vernieuwt, verschijnt er een bericht met een koppeling onder aan het dialoogvenster [!DNL Workfront for G Suite] bevestigt dat u de e-mail hebt geconverteerd naar een update:

   ![](assets/email-was-converted-as-update.png)

   U kunt op de koppeling klikken om naar de [!UICONTROL Updates] tab in [!DNL Workfront] voor het object dat u hebt opgegeven in stap 4.

   U kunt deze stappen herhalen om dezelfde e-mail om te zetten naar updates, taken en problemen (zie [Adobe Workfront-uitgave maken in [!DNL G Suite] met e-mailinhoud](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md)). Wanneer u uw browser vernieuwt of op een ander moment terugkeert naar de e-mail, worden alle koppelingen die u voor de e-mail hebt gemaakt, onder aan het dialoogvenster weergegeven [!UICONTROL Workfront for G Suite] deelvenster.

1. (Optioneel) Ga verder met de update in het dialoogvenster [!DNL Workfront] in het invoegvenster op een van de volgende manieren:

   * Als u nog een update wilt toevoegen aan het dialoogvenster **[!UICONTROL Updates]** tabblad, klikt u op **[!UICONTROL Start a new update]** en typ de informatie.

   * Als u wilt reageren op een update van de **[!UICONTROL Updates]** tabblad, klikt u op **[!UICONTROL Reply]** en typ uw antwoord.

      Voor beide bovenstaande opties kunt u op **[!UICONTROL Notify]** om ontvangers voor het antwoord te specificeren zoals in stap 5. Wanneer u klaar bent, klikt u op **[!UICONTROL Post]** om de update of het antwoord toe te voegen.

   * Klik op de knop **[!UICONTROL Details]** om de details voor het nieuwe project, de nieuwe taak, of de kwestie te bekijken.
