---
title: Filters, weergaven en groepen aanpassen met een lay-outsjabloon
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Als Workfront-beheerder kunt u een lay-outsjabloon gebruiken om op te geven welke lijstbesturingselementen worden weergegeven in de vervolgkeuzemenu's Filter, Weergave en Groeperen. Deze menu's worden boven op lijsten in Workfront weergegeven, zoals de takenlijst van een project.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: e9b61da8-2eca-4d88-969b-ae337e402540
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 0%

---

# Filters, weergaven en groepen aanpassen met een lay-outsjabloon

Als Adobe Workfront-beheerder kunt u een lay-outsjabloon gebruiken om op te geven welke lijstbesturingselementen worden weergegeven in de vervolgkeuzemenu&#39;s Filter, Weergave en Groeperen. Deze menu&#39;s worden boven op lijsten in Workfront weergegeven, zoals de lijst met taken voor een project:

![](assets/filter-view-grouping-layout-templates.png)

Voor meer informatie over lay-outsjablonen raadpleegt u [Lay-outsjablonen maken en beheren](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Voor informatie over lay-outsjablonen voor groepen raadpleegt u [De lay-outsjablonen van een groep maken en wijzigen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Nadat u een lay-outmalplaatje hebt gevormd, moet u het aan gebruikers voor veranderingen toewijzen u aanbracht om aan anderen zichtbaar te zijn. Voor informatie over het toewijzen van een lay-outsjabloon aan gebruikers raadpleegt u [Gebruikers toewijzen aan een lay-outsjabloon](../use-layout-templates/assign-users-to-layout-template.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Om deze stappen op systeemniveau uit te voeren, hebt u het toegangsniveau van de Beheerder van het Systeem nodig.
Om hen voor een groep uit te voeren, moet u een manager van die groep zijn.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Besturingselementen voor filters-, weergave- en groeperingslijsten aanpassen:

1. Beginnen met het werken aan een lay-outsjabloon, zoals beschreven in [Lay-outsjablonen maken en beheren](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Klik op de pijl omlaag ![](assets/down-arrow-blue.png) krachtens **Aanpassen wat gebruikers zien** en klik vervolgens op **Lijsten** in het vervolgkeuzemenu dat wordt weergegeven.

   ![](assets/customize-what-users-see-dropdown-on-pg-adobe-branding.png)

1. Klik op de pijl omlaag ![](assets/down-arrow-blue.png) krachtens **Selecteer een lijst die u wilt aanpassen** Selecteer vervolgens het type Workfront-object waarvoor u de besturingselementen voor de lijst Filter, Weergave en Groepering wilt aanpassen.

   ![](assets/select-a-list-to-customize-menu-on-pg-adobe-branding.png)

   >[!NOTE]
   >
   >Als u Projecten als lijst selecteert om aan te passen, dan Projecten onbruikbaar te maken ik of Projecten in de sectie van de Filter ben, zullen de gebruikers niet meer zien of die filter kunnen gebruiken:
   >
   >* In de lijst met filters die worden weergegeven wanneer ze op het filterpictogram klikken ![](assets/filter-nwepng.png) boven een lijst:
   >   
   >  ![](assets/disable-filters-projects-im-on-or-own.png)
   >   
   >* In de koptekst van het gebied Projecten:
   >   
   >  ![](assets/disable-filter-pills.png)

1. (Optioneel) Als u het standaardfilter, de standaardweergave of de standaardgroepering voor de lay-outsjabloon wilt wijzigen, plaatst u de aanwijzer boven het filter, de weergave of de groep en klikt u vervolgens op **Instellen als standaard**.

   De standaardwaarden die u kiest, bepalen welke gebruikers voor Filter, Weergave en Groeperen in lijsten in Workfront worden weergegeven wanneer de lay-outsjabloon aan hen wordt toegewezen. Als u deze gebreken niet verandert, zien de gebruikers alle lijsten als volgt:

   * **Filters**: Alles
   * **Weergave**: Norm (indien van toepassing); sommige lijsten hebben deze weergave niet)
   * **Groepering**: Niets

   U kunt de opties Alles, Standaard en Niets verbergen nadat u verschillende standaardinstellingen hebt geselecteerd (zie Stap 5), maar deze opties kunnen niet worden verwijderd.

   U kunt elke andere optie verwijderen die als standaard wordt gebruikt, maar u moet eerst een andere standaardinstelling selecteren.

   Voor informatie over het verwijderen van filters, weergaven en groepen raadpleegt u [Standaardfilters, weergaven en groepen maken, bewerken en delen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-and-share-default-fvgs.md).

1. Besturingselementen voor lijsten verbergen en toevoegen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Een besturingselement voor een lijst verbergen</td> 
      <td> <p>Schakel het vakje naast het lijstbesturingselement dat u wilt verbergen of weergeven uit of uit.</p> <p>Als een selectievakje grijs wordt weergegeven, kunt u het lijstbesturingselement niet verbergen. De standaardwaarde <img src="assets/default-pill.png"> het plaatsen voor elke lijstcontrole wordt gedimd omdat u niet het plaatsen kunt verbergen die momenteel als gebrek wordt gevormd.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Een besturingselement voor een aangepaste lijst toevoegen</td> 
      <td> <p> 
        <ol> 
         <li value="1"> Klikken <strong>Filter toevoegen</strong>, <strong>Weergave toevoegen</strong>, of <strong>Groepering toevoegen</strong> onder aan de lijst Filter, Weergave of Groepering. In het vakje dat toont, begin de naam van een bestaand controle van de douanelijst te typen die eerder voor uw organisatie wordt gecreeerd, dan klik de naam wanneer het verschijnt.</li> 
         <li value="2"> Als u de nieuwe controle van de douanelijst als standaardfilter, mening, of groepering voor het lay-outmalplaatje wilt plaatsen, klik <strong>Instellen als standaard</strong>. </li> 
         <li value="3"> <p>Klikken <strong>Toevoegen</strong> als u klaar bent.</p> <p><b>OPMERKING</b>: <p>Gebruikers kunnen aangepaste lijstbesturingselementen toevoegen aan hun eigen lijsten. Als u aangepaste besturingselementen voor lijsten toevoegt aan een lay-outsjabloon, worden uw besturingselementen voor lijsten toegevoegd en worden de elementen onder aan het deelvenster geplaatst. die u hebt, vervangt ze niet.</p> <p>Dit is ook waar als u de gebruiker aan een nieuw lay-outmalplaatje toewijst dat de controles van de douanelijst heeft. </p> <p>Voor informatie over het aanpassen van lijstcontroles, zie <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Overzicht van filters in Adobe Workfront</a>, <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Overzicht van weergaven in Adobe Workfront</a>, en <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Overzicht van groepen in Adobe Workfront</a>.</p> </p> </li> 
        </ol> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Blijf het lay-outmalplaatje aanpassen.

   of

   Als u klaar bent met het aanpassen, klikt u op **Opslaan**.

   >[!TIP]
   >
   >U kunt op elk gewenst moment op Opslaan klikken om de voortgang op te slaan en de sjabloon later blijven wijzigen.
