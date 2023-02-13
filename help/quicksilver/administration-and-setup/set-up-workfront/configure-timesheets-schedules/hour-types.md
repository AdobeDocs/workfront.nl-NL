---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Uurtypen beheren
description: U kunt uurtypen koppelen aan uw uren. De types van uren zijn etiketten u gebruikt om uw uuringangen te bepalen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: 9f7f8a50bb805b1d6845df79ecffaa329d5abc26
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 0%

---

# Uurtypen beheren

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

U kunt uurtypen koppelen aan uw uren. De types van uren zijn etiketten u gebruikt om uw uuringangen te bepalen.

Er zijn twee reeksen uurtypes:

* **Projectspecifieke uren**: Dit is tijd het programma geopende projecten, taken, en kwesties. Projectspecifieke uurtypen kunnen overal in [!DNL Adobe Workfront] waar u tijd voor projecten, taken, en kwesties kunt registreren.

   Bij aanmelden [!DNL Workfront], de project-specifieke uurtypes die beschikbaar zijn hangen van configuratieopties af die bij het systeem, het project, en gebruikersniveaus worden geplaatst.

   De volgende standaardproject-specifieke uurtypes zijn altijd beschikbaar:

   * Projecttijd
   * Taaktijd
   * Uitgiftetijd

   De [!DNL Workfront] de beheerder bepaalt welke project-specifieke uurtypes ter beschikking worden gesteld, zoals die in worden beschreven [Bepaal uurtypes en beschikbaarheid voor timesheets](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   >[!NOTE]
   >
   >Als u om het even welke project-specifieke uurtypes in uw toelaat [!DNL Workfront] systeem, moet minstens één project-specifiek uurtype op elk project in uw systeem worden toegelaten. U kunt geen project-specifiek uurtype op het systeemniveau toelaten, en geen project-specifieke uurtypes hebben beschikbaar op het projectniveau.

* **Algemene uurtypen**: De algemene uren kunnen niet met een project, een taak, of een kwestie worden geassocieerd, en worden het programma geopend direct in timesheet. Voor meer informatie over logboektijd, zie [Logtijd](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] plan</td> 
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

## Ingebouwde uurtypen

Workfront wordt geleverd met een aantal ingebouwde uurtypen. Deze uurtypen kunnen niet worden bewerkt en kunnen niet worden verborgen.

De uurtypes die met komen [!DNL Workfront] zijn:

* **[!UICONTROL Sick Time]**: Een algemeen uurtype dat niet met uuringangen op een project, een taak, of een kwestie kan worden geassocieerd.
* **[!UICONTROL Vacation Time]**: Een algemeen uurtype dat niet met uuringangen op een project, een taak, of een kwestie kan worden geassocieerd.
* **[!UICONTROL General Overhead]**: Een algemeen uurtype dat niet met uuringangen op een project, een taak, of een kwestie kan worden geassocieerd. Nochtans, kan het als opbrengst in uw project planningsproces tellen.
* **[!UICONTROL Project Time]**: Een algemeen uurtype dat slechts met uuringangen op een project kan worden geassocieerd.
* **[!UICONTROL Task Time]**: Een algemeen uurtype dat slechts met uuringangen op een taak kan worden geassocieerd.
* **[!UICONTROL Issue Time]**:Een type van algemene uren dat slechts met uuringangen op een kwestie kan worden geassocieerd.

## Urentypen maken

Als [!DNL Workfront] beheerder, kunt u nieuwe uurtypes voor uw organisatie op zowel systeem als projectniveaus tot stand brengen. Nadat u uurtypes op het systeem en projectniveaus creeert, kunnen de gebruikers bepalen welke uurtypes voor specifieke projecten en gebruikers beschikbaar zijn. Zie voor meer informatie de [Bepaal uurtypes en beschikbaarheid voor timesheets](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

Nieuwe uurtypen maken:

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe] Workfront, klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klik op **[!UICONTROL Timesheet & Hours]** > **[!UICONTROL Hour Types]**.

1. Klik op **[!UICONTROL New Hour Type].**
1. Geef de volgende informatie op over de **[!UICONTROL New Hour Type]** formulier:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Geef het nieuwe uur een naam die gemakkelijk herkenbaar is in het systeem.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Voeg een beschrijving toe voor het uurtype.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope]</td> 
      <td> <p>Bepaal of het uurtype een algemeen of project-specifiek uurtype door het correcte werkingsgebied in het drop-down menu te selecteren is.</p> <p>De types van algemene uren zijn zichtbaar slechts in timesheets en kunnen niet met projecten, taken, of kwesties worden geassocieerd.</p> <p><b>BELANGRIJK</b>: Als u een aangepast uurtype hebt dat [!UICONTROL Project Specific]en vervolgens wijzigt u deze in [!UICONTROL General], worden alle bestaande Taak, Kwesties en de uren van het Project geplaatst aan hun systeem standaardtypes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Count As Revenue]</td> 
      <td>Selecteer deze optie als u de uuringang verbonden aan dit uurtype uw opbrengstberekeningen wilt beïnvloeden.</td> 
     </tr> 
    </tbody> 
   </table>

   **[!UICONTROL Count As Revenue]**: Selecteer deze optie als u de uuringang verbonden aan dit uurtype uw opbrengstberekeningen wilt beïnvloeden.

1. Klik op **[!UICONTROL Create Hour Type].**

## Uren deactiveren

Als de uurtypes verouderd worden en u niet meer gebruikers hun uuringangen met hen wilt associëren, kunt u de uurtypes deactiveren.

Als u uurtypen deactiveert, worden de uurtypen overal verborgen [!DNL Workfront] waarbij uurtypen zichtbaar zijn.

Een uurtype deactiveren:

1. Klikken **[!UICONTROL Setup]** in de rechterbovenhoek van [!DNL Adobe Workfront] op de algemene navigatiebalk.

1. Uitbreiden **[!UICONTROL Timesheet & Hours Preferences]** en klik vervolgens op **[!UICONTROL Hour Types]**.

1. Selecteer het uurtype u wilt deactiveren.

1. Klik op **[!UICONTROL Deactivate]**.
