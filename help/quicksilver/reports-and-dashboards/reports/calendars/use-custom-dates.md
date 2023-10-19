---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Aangepaste datumvelden gebruiken in een kalenderrapport
description: Een kalenderrapport is een dynamisch rapport dat een visuele vertegenwoordiging van uw werk verstrekt. U kunt de gebieden van de douanedatum in een kalenderrapport voor taken, kwesties, en projecten gebruiken.
author: Lisa
feature: Reports and Dashboards
exl-id: 40cc8628-7641-41ce-b8e5-7f5ed5ad36c7
source-git-commit: 880e82546ac0ca80be60f03db31b99ad1778c35a
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 0%

---

# Aangepaste datumvelden gebruiken in een kalenderrapport

A [!UICONTROL calendar] rapport is een dynamisch rapport dat een visuele vertegenwoordiging van uw werk verstrekt. U kunt aangepaste datumvelden in een kalenderrapport gebruiken voor de volgende objecten:

* Taken
* Problemen
* Projecten

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licentie*</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong></td> 
   <td> <p>[!UICONTROL Edit] toegang tot [!UICONTROL Reports], [!UICONTROL Dashboards], en [!UICONTROL Calendars]</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>[!UICONTROL Manage] toegang tot het kalenderverslag</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Vereisten

1. U moet aangepaste datumvelden en een waarde in het veld hebben dat beschikbaar is in het dialoogvenster [!DNL Workfront] -instantie. Als u geen aangepaste formulierinstelling met aangepaste datums hebt, volgt u de instructies in de eerste twee secties van [Een aangepast formulier maken of bewerken](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Voeg het aangepaste formulier toe aan een project, taak of uitgave die u wilt toevoegen aan de kalender en geef een datum op. Zie voor meer informatie [Een aangepast formulier toevoegen aan een object](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## De groep items instellen

U kunt kiezen hoe de groep items moet worden weergegeven in uw kalender.

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Calendars]**.

1. Selecteer de kalender waaraan u een nieuwe groep items wilt toevoegen.\
   of\
   Klikken **[!UICONTROL + New Calendar]** en voert u de naam van de kalender in.

   >[!NOTE]
   >
   >U moet [!UICONTROL Edit] toegang tot [!UICONTROL Reports], [!UICONTROL Dashboards], en [!UICONTROL Calendars] in uw toegangsniveau om een kalenderrapport te creëren.

1. Klik links op **[!UICONTROL Add to Calendar]** en klik vervolgens op **[!UICONTROL Add advanced items]**.

1. Geef het volgende op:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Name this group of items]</strong></td>
      <td>Typ een naam voor de groep items.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Color]</strong></td>
      <td>Selecteer een kleur voor de groep items. Alle items worden in de geselecteerde kleur in het kalenderrapport weergegeven.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Date Field]</strong></td>
      <td>Kies <strong>[!UICONTROL Custom dates]</strong>.<br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL On the calendar, show]</strong></td>
      <td><p>Kies hoe u de datums wilt weergeven:</p>
       <ul>
        <li><strong>[!UICONTROL Single Date]</strong>: In de kalender wordt het object op één datum weergegeven.</li>
        <li><strong>[!UICONTROL Duration] (Van begin tot eind)</strong>: Het object wordt in de kalender over een periode van dagen weergegeven.<br><p>Opmerking: als u <strong>[!UICONTROL Duration]</strong>, moet de opgegeven einddatum na de begindatum liggen, anders wordt het item niet weergegeven in de kalender.</p></li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Custom Dates]</strong></td>
      <td><p>Voer de aangepaste datumnaam in die is gekoppeld aan het object dat u wilt bijhouden.</p><p><strong>OPMERKING:</strong> U kunt maximaal 50 resultaten zoeken naar de aangepaste datumnaam om prestatieproblemen te voorkomen.</td>
     </tr>
    </tbody>
   </table>

1. Ga verder naar de volgende sectie.

## Objecten toevoegen aan de groep items

Nadat u hebt ingesteld hoe de items moeten worden weergegeven, moet u de objecten die u in de kalender wilt zien, aan de groep toevoegen.

1. In de **[!UICONTROL What would you like to add to the calendar?]** sectie, selecteert u

   * **[!UICONTROL Tasks]**
   * **[!UICONTROL Projects]**
   * **[!UICONTROL Issues]**

1. Klikken **[!UICONTROL Add Tasks]**, **[!UICONTROL Add Projects]**, of **[!UICONTROL Add Issues]**, afhankelijk van het objecttype dat u aan de kalender toevoegt.\
   ![Object selecteren voor kalender](assets/field-name.png)

1. Typ in het keuzemenu eerst de veldnaam en selecteer vervolgens de veldbron van het object dat u in de kalender wilt weergeven (bijvoorbeeld **[!UICONTROL Late Tasks]**).
1. Stel een voorwaardelijke instructie in voor de kalendergroep.

   ![Condition, instructie](assets/condition-statement-calendar.png)

   Ga voor meer informatie over het instellen van voorwaarden naar [Filter- en voorwaardenmodificatoren](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Optioneel) Geef aanvullende objecten voor de kalendergroep op door stap 1-4 te herhalen.
1. In de **[!UICONTROL Set the Tasks/Projects/Issues labels to be the...]** , selecteert u hoe de objecten in deze kalendergroep worden gelabeld in de kalender.

   >[!NOTE]
   >
   >Als de standaardlabelopties niet beschikbaar zijn voor een bepaald object, wordt in plaats daarvan de naam van het object weergegeven. Als u bijvoorbeeld [!UICONTROL Parent Task] label is geselecteerd en er is geen bovenliggende taak aan het object gekoppeld, [!DNL Adobe Workfront] geeft de objectnaam weer die u in de kalender weergeeft.

1. Klik op **[!UICONTROL Save]**.
