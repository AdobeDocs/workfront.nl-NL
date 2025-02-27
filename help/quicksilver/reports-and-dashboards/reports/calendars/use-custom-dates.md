---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Aangepaste datumvelden gebruiken in een kalenderrapport
description: Een kalenderrapport is een dynamisch rapport dat een visuele vertegenwoordiging van uw werk verstrekt. U kunt de gebieden van de douanedatum in een kalenderrapport voor taken, kwesties, en projecten gebruiken.
author: Lisa
feature: Reports and Dashboards
exl-id: 40cc8628-7641-41ce-b8e5-7f5ed5ad36c7
source-git-commit: c88c8dc7431f3bc711ae1942df12925fafa7eff0
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 0%

---

# Aangepaste datumvelden gebruiken in een kalenderrapport

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Het is beschikbaar slechts in het milieu van de Sandbox van de Voorproef.</span>

Een [!UICONTROL calendar] rapport is een dynamisch rapport dat een visuele vertegenwoordiging van uw werk verstrekt. U kunt aangepaste datumvelden in een kalenderrapport gebruiken voor de volgende objecten:

* Taken
* Problemen
* Projecten

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront plan]</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td><p>Nieuw: Standaard</p>
       <p>of</p>
       <p>Huidig: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>[!UICONTROL Edit] toegang tot [!UICONTROL Reports] , [!UICONTROL Dashboards] en [!UICONTROL Calendars]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td>[!UICONTROL Manage] toegang tot het kalenderverslag</td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

1. U moet aangepaste datumvelden hebben en een waarde binnen het veld dat beschikbaar is in uw [!DNL Workfront] -instantie. Als u geen opstelling van de douanevorm met douanedata hebt, volg de instructies in [ creeer een douanevorm ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
1. Voeg het aangepaste formulier toe aan een project, taak of uitgave die u wilt toevoegen aan de kalender en geef een datum op. Voor meer informatie, zie [ een douanevorm aan een voorwerp ](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md) toevoegen.

## De groep artikelen in productie instellen

U kunt kiezen hoe de groep items moet worden weergegeven in uw kalender.

{{step1-to-calendars}}

1. Selecteer de kalender waaraan u een nieuwe groep items wilt toevoegen.
of
Klik op **[!UICONTROL + New Calendar]** en voer de naam van de kalender in.

   >[!NOTE]
   >
   >U moet [!UICONTROL Edit] toegang hebben tot [!UICONTROL Reports] , [!UICONTROL Dashboards] en [!UICONTROL Calendars] in uw toegangsniveau om een kalenderrapport te maken.

1. Klik links in het scherm op **[!UICONTROL Add to Calendar]** en klik vervolgens op **[!UICONTROL Add advanced items]** .

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
      <td>Kies <strong>[!UICONTROL Custom dates]</strong> .<br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL On the calendar, show]</strong></td>
      <td><p>Kies hoe u de datums wilt weergeven:</p>
       <ul>
        <li><strong>[!UICONTROL Single Date]</strong>: In de kalender wordt het object op één datum weergegeven.</li>
        <li><strong>[!UICONTROL Duration] (Begin aan Eind) </strong>: De kalender toont het voorwerp over een spanwijdte van dagen.<br><p>Opmerking: als u <strong>[!UICONTROL Duration]</strong> kiest, moet de opgegeven einddatum na de begindatum liggen, anders wordt het item niet weergegeven in de kalender.</p></li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Custom Dates]</strong></td>
      <td><p>Voer de aangepaste datumnaam in die is gekoppeld aan het object dat u wilt bijhouden.</p><p><strong> NOTA:</strong> het onderzoek naar de naam van de douanedatum is beperkt tot 50 resultaten om prestatieskwesties te vermijden.</td>
     </tr>
    </tbody>
   </table>

1. Ga verder naar de volgende sectie.

## Objecten toevoegen aan de groep items in productie

Nadat u hebt ingesteld hoe de items moeten worden weergegeven, moet u de objecten die u in de kalender wilt zien, aan de groep toevoegen.

1. Selecteer in de sectie **[!UICONTROL What would you like to add to the calendar?]** de optie

   * **[!UICONTROL Tasks]**
   * **[!UICONTROL Projects]**
   * **[!UICONTROL Issues]**

1. Klik op **[!UICONTROL Add Tasks]** , **[!UICONTROL Add Projects]** of **[!UICONTROL Add Issues]** , afhankelijk van het objecttype dat u aan de kalender toevoegt.
   ![ Uitgezochte voorwerp voor kalender ](assets/field-name.png)

1. Typ in het keuzemenu eerst de veldnaam en selecteer vervolgens de veldbron van het object dat u in de kalender wilt weergeven (bijvoorbeeld **[!UICONTROL Late Tasks]** ).
1. Stel een voorwaardelijke instructie in voor de kalendergroep.

   ![ verklaring van de Voorwaarde ](assets/condition-statement-calendar.png)

   Om over het plaatsen van voorwaarden te leren, zie [ Filter en voorwaardenbepalingen ](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Optioneel) Geef aanvullende objecten voor de kalendergroep op door stap 1-4 te herhalen.
1. Selecteer in het veld **[!UICONTROL Set the Tasks/Projects/Issues labels to be the...]** hoe de objecten in deze kalendergroep worden gelabeld in de kalender.

   >[!NOTE]
   >
   >Als de standaardlabelopties niet beschikbaar zijn voor een bepaald object, wordt in plaats daarvan de naam van het object weergegeven. Wanneer u bijvoorbeeld het label [!UICONTROL Parent Task] hebt geselecteerd en er geen bovenliggende taak aan het object is gekoppeld, geeft [!DNL Adobe Workfront] de objectnaam weer die u in de kalender weergeeft.

1. Klik op **[!UICONTROL Save]**.

<div class="preview">

## De groep items instellen in Voorvertoning

U kunt kiezen hoe de groep items moet worden weergegeven in uw kalender.

{{step1-to-calendars}}

1. Selecteer de kalender u een nieuwe groep punten wilt toevoegen, klik het Meer menu, dan **geeft** uit.
of
Klik op **[!UICONTROL + New Calendar]** , voer de projectnaam in en klik op **[!UICONTROL Add advanced items]** .

   >[!NOTE]
   >
   >U moet [!UICONTROL Edit] toegang hebben tot [!UICONTROL Reports] , [!UICONTROL Dashboards] en [!UICONTROL Calendars] in uw toegangsniveau om een kalenderrapport te maken.

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
      <td>Kies <strong>[!UICONTROL Custom dates]</strong> .<br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL On the calendar, show]</strong></td>
      <td><p>Kies hoe u de datums wilt weergeven:</p>
       <ul>
        <li><strong>[!UICONTROL Single Date]</strong>: In de kalender wordt het object op één datum weergegeven.</li>
        <li><strong>[!UICONTROL Duration] (Begin aan Eind) </strong>: De kalender toont het voorwerp over een spanwijdte van dagen.<br><p>Opmerking: als u <strong>[!UICONTROL Duration]</strong> kiest, moet de opgegeven einddatum na de begindatum liggen, anders wordt het item niet weergegeven in de kalender.</p></li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Custom Dates]</strong></td>
      <td><p>Voer de aangepaste datumnaam in die is gekoppeld aan het object dat u wilt bijhouden.</p><p><strong> NOTA:</strong> het onderzoek naar de naam van de douanedatum is beperkt tot 50 resultaten om prestatieskwesties te vermijden.</td>
     </tr>
    </tbody>
   </table>

1. Ga verder naar de volgende sectie.

### Objecten toevoegen aan de groep items in Voorvertoning

Nadat u hebt ingesteld hoe de items moeten worden weergegeven, moet u de objecten die u in de kalender wilt zien, aan de groep toevoegen.

1. Selecteer in de sectie **[!UICONTROL What would you like to add to the calendar?]** de optie

   * **[!UICONTROL Tasks]**
   * **[!UICONTROL Projects]**
   * **[!UICONTROL Issues]**
   * **Tijd weg**

1. Klik **[!UICONTROL Add Tasks]**, **[!UICONTROL Add Projects]**, **[!UICONTROL Add Issues]**, of **Tijd van** afhankelijk van het objecten type u aan de kalender toevoegt.

1. Typ in het keuzemenu eerst de veldnaam en selecteer vervolgens de veldbron van het object dat u in de kalender wilt weergeven (bijvoorbeeld **[!UICONTROL Late Tasks]** ).
1. Stel een voorwaardelijke instructie in voor de kalendergroep.


   Om over het plaatsen van voorwaarden te leren, zie [ Filter en voorwaardenbepalingen ](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   ![ Uitgezochte voorwerp voor kalender ](assets/calendar-field-name.png)

1. (Optioneel) Geef aanvullende objecten voor de kalendergroep op door stap 1-4 te herhalen.
1. Selecteer in het veld **[!UICONTROL Set the Tasks/Projects/Issues labels to be the...]** hoe de objecten in deze kalendergroep worden gelabeld in de kalender.

   >[!NOTE]
   >
   >Als de standaardlabelopties niet beschikbaar zijn voor een bepaald object, wordt in plaats daarvan de naam van het object weergegeven. Wanneer u bijvoorbeeld het label [!UICONTROL Parent Task] hebt geselecteerd en er geen bovenliggende taak aan het object is gekoppeld, geeft [!DNL Adobe Workfront] de objectnaam weer die u in de kalender weergeeft.

   ![ vastgestelde taaketiketten ](assets/set-task-labels.png)
1. Klik op **[!UICONTROL Save]**.

</div>