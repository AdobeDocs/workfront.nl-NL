---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Aangepaste uitgaventypen maken
description: Als [!DNL Adobe Workfront] beheerder, kunt u de types van douanefontages tot stand brengen om de uitgaven te bepalen en te volgen verbonden aan uw taken en projecten. De kosten zijn niet-arbeidskosten die met taken of projecten kunnen worden geassocieerd.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7b76b9e8-fbb8-45a7-9e26-1ddc6d5176d8
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 1%

---

# Aangepaste uitgaventypen maken

<!--**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Als [!DNL Adobe Workfront] beheerder, kunt u de types van douanefontages tot stand brengen om de uitgaven te bepalen en te volgen verbonden aan uw taken en projecten. De kosten zijn niet-arbeidskosten die met taken of projecten kunnen worden geassocieerd.

U kunt alle onkostentypen die u maakt, bewerken of verwijderen. U kunt de ingebouwde [!DNL Workfront] kostentypen.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een [!DNL Workfront] beheerder.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Standaardkostentypen

De kostentypen waarin [!DNL Workfront] U kunt standaard het volgende niet verwijderen of bewerken:

* [!UICONTROL Advertising]
* [!UICONTROL Consulting]
* [!UICONTROL Entertainment]
* [!UICONTROL General]
* [!UICONTROL Materials]
* [!UICONTROL Travel]

## Aangepaste uitgaventypen maken

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront].
1. Klik op **[!UICONTROL Expense Types]**.
1. Klik op **[!UICONTROL New Expense Type]**.
1. In de **[!UICONTROL New Expense Type]** Geef de volgende informatie op in het vak dat wordt weergegeven:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Geef een naam op voor de uitgave.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Geef een beschrijving voor de uitgave op.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Calculated Unit]</td> 
      <td> <p>Selecteer in de vervolgkeuzelijst de maateenheid voor uw uitgaven.</p> <p>De volgende maateenheid is beschikbaar:</p> 
       <ul> 
        <li>Mile</li> 
        <li>Kilometer</li> 
        <li>Kilogram</li> 
        <li>Dollar</li> 
        <li>Dollar</li> 
        <li>Dag</li> 
        <li>Anders - Als u deze optie selecteert, wordt u gevraagd de maateenheid een naam te geven en de maateenheid te definiëren als iets dat uw organisatie kent.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Snelheid</td> 
      <td> <p>Geef de prijs per eenheid op. Dit is een valutaveld dat de kosten vertegenwoordigt van elke eenheid die in het <strong>[!UICONTROL Calculated Unit]</strong> veld. </p> <p>De snelheid kan een numerieke waarde met maximaal 4 cijfers achter de komma bevatten. Bijvoorbeeld 1,0375</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klik op **[!UICONTROL Create Expense Type]**.\
   Het uitgaventype is nu beschikbaar voor gebruikers om het met hun uitgaven op projecten en taken te associëren.

## Aangepaste kostentypen wijzigen

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront].
1. Klik op **[!UICONTROL Expense Types]**.
1. Selecteer het type uitgave dat u wilt wijzigen en klik vervolgens op **[!UICONTROL Edit]**.

   De **[!UICONTROL Edit Expense Type]** wordt weergegeven.

1. Breng de gewenste wijzigingen aan en klik op **[!UICONTROL Save Changes]**.\
   Het uitgaventype is nu beschikbaar voor gebruikers om het met hun uitgaven op projecten en taken te associëren.

Raadpleeg het artikel voor meer informatie over het gebruik van kosten en de manier waarop deze de kosten van een project kunnen beïnvloeden [Projectkosten beheren](../../../manage-work/projects/project-finances/manage-project-expenses.md).
