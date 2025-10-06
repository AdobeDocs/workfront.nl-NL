---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Een Outlook-e-mail aan een project toevoegen als een taak of een probleem
description: U kunt e-mails in  [!DNL Adobe Workfront]  taken of kwesties omzetten. Nadat een e-mail is geconverteerd, wordt de taak of uitgave weergegeven in het project dat is geselecteerd tijdens de conversie.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 00755c27-9fc9-4357-a39b-4f9772484252
source-git-commit: 793c8c940c8cb7ac53169edf21ddf28af2554120
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 0%

---

# Een [!DNL Outlook] e-mail aan een project toevoegen als een taak of een uitgave


>[!IMPORTANT]
>
>[ Microsoft heeft steun voor online tokens van de erfenisUitwisseling ](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens) onbruikbaar gemaakt, die door toe:voegen-binnen van Workfront Outlook voor authentificatie werden gebruikt. Deze verandering door Microsoft werd in fasen doorgevoerd en is voltooid op 1 oktober 2025.
>
>**omdat Microsoft deze tokens heeft onbruikbaar gemaakt, werkt Workfront voor de integratie van Microsoft Outlook niet meer.**

U kunt e-mailberichten converteren naar [!DNL Adobe Workfront] taken of uitgaven. Nadat een e-mail is geconverteerd, wordt de taak of uitgave weergegeven in het project dat is geselecteerd tijdens de conversie.

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

Uw [!DNL Workfront] beheerder moet [!DNL Outlook for Office] with [!DNL Workfront] inschakelen voordat u deze integratie kunt gebruiken.

## Een [!DNL Outlook] e-mail aan een project toevoegen als een taak of uitgave

1. Selecteer de e-mail binnen [!DNL Outlook] die u naar een taak of een uitgave wilt converteren.
1. Klik op het pictogram **[!DNL Workfront]** rechtsboven in het e-mailbericht om de invoegtoepassing Workfront weer te geven.

   Mogelijk moet u op de pijl omlaag in de rechterbovenhoek van uw e-mail klikken om het pictogram [!DNL Workfront] te openen.

1. Klik het **[!UICONTROL Menu]** pictogram ![ o365_addin_menu_icon.png ](assets/o365-addin-menu2-icon.png) om de lijst van beschikbare [!DNL Workfront] opties te tonen.



1. Klik op **[!UICONTROL Add to Work]**.

1. Selecteer het veld **[!UICONTROL Add to Project]** .
1. Typ de naam van een project in het veld **[!UICONTROL Project]** en selecteer het vervolgens wanneer het in de lijst wordt weergegeven.
1. Selecteer het keuzerondje **[!UICONTROL Task]** als u een taak wilt toevoegen aan het geselecteerde project.

   of

   Selecteer het keuzerondje **[!UICONTROL Issue]** als u een uitgave aan het geselecteerde project wilt toevoegen.

1. (Optioneel) Geef in het veld **[!UICONTROL Assign this to]** aan aan wie deze taak of uitgave is toegewezen.

   >[!TIP]
   >
   >U kunt de taak of de kwestie aan een team toewijzen, als u verscheidene mensen hiervan bewust wilt zijn. Als de teamleden hun e-mailmeldingen hebben ingeschakeld, ontvangen zij een e-mail over de nieuwe taak of uitgave die aan hen is toegewezen.


1. (Optioneel) Geef de waarde **[!UICONTROL Due by date]** op. Dit wordt de [!UICONTROL Planned Completion Date] van de taak of kwestie.
1. (Optioneel) Werk de volgende gegevens uit de e-mail bij voordat deze als taak of uitgave wordt opgeslagen (verplichte velden worden voorafgegaan door een sterretje).

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL Task or Issue Name]</td>
        <td>Standaard is de naam van de taak gelijk aan de naam van het e-mailonderwerp. U kunt de taaknaam naar wens wijzigen.</td>
        <td></td>
      </tr>
      <tr>
        <td>[!UICONTROL Description]</td>
        <td>Standaard is de beschrijving hetzelfde als de e-mailtekst. U kunt de beschrijving naar wens wijzigen.</td>
      </tr>
      <tr>
        <td>[!UICONTROL Attachments]</td>
        <td>Eventuele e-mailbijlagen worden opgeslagen in het [!UICONTROL Documents] -gebied van de taak of uitgave. U kunt bijlagen verwijderen voordat u het e-mailbericht opslaat als een taak of uitgave.</td>
      </tr>
   </table>

1. Klik op **[!UICONTROL Add]**.

   De taak of kwestie wordt toegevoegd aan het gespecificeerde project

1. (Optioneel) Klik op **[!UICONTROL View in [!DNL Workfront]]** om de taak in de [!DNL Workfront] -toepassing op een nieuw tabblad weer te geven.

1. (Optioneel) Ga terug naar [!DNL Outlook] en selecteer het geconverteerde e-mailbericht.

   Boven aan het venster voor de [!DNL Workfront] invoegtoepassing ziet u de bevestiging met een koppeling dat het e-mailbericht aan [!DNL Workfront] is toegevoegd als een taak of een uitgave. De koppeling bevat de datum waarop deze is geconverteerd.



