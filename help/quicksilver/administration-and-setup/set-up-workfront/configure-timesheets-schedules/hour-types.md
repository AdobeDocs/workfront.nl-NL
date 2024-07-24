---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Uurtypen beheren
description: U kunt uurtypen koppelen aan uw uren. De types van uren zijn etiketten u gebruikt om uw uuringangen te bepalen.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: 212dda4289e4d29dbfbff0dbdc55315215b5ad91
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 0%

---

# Uurtypen beheren

<!--Audited: 07/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

U kunt uurtypen koppelen aan uw uren. De types van uren zijn etiketten u gebruikt om uw uuringangen te bepalen.

Er zijn twee reeksen uurtypes:

* **de Specifieke Types van Uur van het Project**: Dit is tijd het programma geopend projecten, taken, en kwesties. Projectspecifieke urentypen kunnen overal in [!DNL Adobe Workfront] met uurvermeldingen worden geassocieerd waar u tijd voor projecten, taken, en kwesties kunt registreren.

  Wanneer het registreren van tijd in [!DNL Workfront], de project-specifieke uurtypes die beschikbaar zijn afhangen van configuratieopties die op het systeem, het project, en gebruikersniveaus worden geplaatst.

  De volgende standaardproject-specifieke uurtypes zijn altijd beschikbaar:

   * Projecttijd
   * Taaktijd
   * Uitgiftetijd

  De [!DNL Workfront] beheerder bepaalt welke project-specifieke uurtypes beschikbaar worden gemaakt, zoals die in [ worden beschreven bepaalt uurtypes en beschikbaarheid ](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

  >[!NOTE]
  >
  >Als u om het even welke project-specifieke uurtypes in uw [!DNL Workfront] systeem toelaat, moet minstens één project-specifiek uurtype op elk project in uw systeem worden toegelaten. U kunt geen project-specifiek uurtype op het systeemniveau toelaten, en geen project-specifieke uurtypes hebben beschikbaar op het projectniveau.

* **de Types van Uur van 0} Algemeen**: De algemene uren kunnen niet met een project, een taak, of een kwestie worden geassocieerd, en rechtstreeks in een timesheet het programma geopend.

Voor informatie over het registreren van uren en het associëren van hen met uurtypes, zie [ tijd van het Logboek ](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td> <p>Nieuw: [!UICONTROL Standard]</p>
   <p>Huidige: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Toegangsniveau</td> 
   <td> <p>U moet een [!DNL Workfront] beheerder zijn.</p> <p> </td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ingebouwde uurtypen

Workfront wordt geleverd met een aantal ingebouwde uurtypen. Deze uurtypen kunnen niet worden bewerkt en kunnen niet worden verborgen.

De uurtypen die bij [!DNL Workfront] worden geleverd, zijn:

* **[!UICONTROL Sick Time]**: Een type van algemene uren dat niet met uuringangen op een project, een taak, of een kwestie kan worden geassocieerd. Zieke uren kunnen niet als opbrengst worden geteld.
* **[!UICONTROL Vacation Time]**: Een type van algemene uren dat niet met uuringangen op een project, een taak, of een kwestie kan worden geassocieerd. Vakantieduur kan niet als inkomsten worden geteld.
* **[!UICONTROL General Overhead]**: Een type van algemene uren dat niet met uuringangen op een project, een taak, of een kwestie kan worden geassocieerd. Nochtans, kan het als opbrengst in uw project planningsproces tellen.
* **[!UICONTROL Project Time]**: Een uurtype van algemeen dat slechts met uuringangen op een project kan worden geassocieerd.
* **[!UICONTROL Task Time]**: een type van algemene uren dat slechts met uuringangen op een taak kan worden geassocieerd.
* **[!UICONTROL Issue Time]**:Een type van algemene uren dat slechts met uuringangen over een kwestie kan worden geassocieerd.

## Urentypen maken

Als [!DNL Workfront] beheerder, kunt u nieuwe uurtypes voor uw organisatie op zowel systeem als projectniveaus tot stand brengen. Nadat u uurtypes op het systeem en projectniveaus creeert, kunnen de gebruikers bepalen welke uurtypes voor specifieke projecten en gebruikers beschikbaar zijn. Voor meer informatie, zie [ de types en beschikbaarheid van uren bepalen ](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

Nieuwe uurtypen maken:

{{step-1-to-setup}}

1. Klik op **[!UICONTROL Timesheet & Hours]** > **[!UICONTROL Hour Types]** .

1. Klik op **[!UICONTROL New Hour Type].**
1. Geef de volgende informatie op in het **[!UICONTROL New Hour Type]** -formulier:

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
      <td> <p>Bepaal of het uurtype een algemeen of project-specifiek uurtype door het correcte werkingsgebied in het drop-down menu te selecteren is.</p> <p>De types van algemene uren zijn zichtbaar slechts in timesheets en kunnen niet met projecten, taken, of kwesties worden geassocieerd.</p> <p><b> BELANGRIJK </b>: Als u een Type van douaneuren hebt dat [!UICONTROL Project Specific] is, dan verandert u het in [!UICONTROL General], worden alle bestaande Taak, Kwesties en de uren van het Project geplaatst aan hun systeem standaardtypes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Count As Revenue]</td> 
      <td><p>Selecteer deze optie als u de uuringang verbonden aan dit uurtype uw opbrengstberekeningen wilt beïnvloeden.</p>
      <p>De tijd van de ick en van de Vakantie kan niet als opbrengst worden geteld.</p>
      <p><b>OPMERKING</b></p>
      <p>Wanneer de algemene uurtypes als opbrengst worden geteld, wordt het tarief van Kosten verbonden aan het profiel van de gebruiker die de tijd registreert geassocieerd met de uurkosten.  
      </td> 
     </tr> 
    </tbody> 
   </table>

   **[!UICONTROL Count As Revenue]**: Selecteer deze optie als u wilt dat de uren die aan dit uurtype zijn gekoppeld uw inkomstenberekeningen beïnvloeden.

1. Klik op **[!UICONTROL Create Hour Type].**

## Uren deactiveren

Als de uurtypes verouderd worden en u niet meer gebruikers hun uuringangen met hen wilt associëren, kunt u de uurtypes deactiveren.

Als u uurtypen deactiveert, worden de uurtypen verborgen vanaf elke locatie in [!DNL Workfront] waar uurtypen zichtbaar zijn.

Een uurtype deactiveren:

{{step-1-to-setup}}

1. Vouw **[!UICONTROL Timesheet & Hours Preferences]** uit en klik op **[!UICONTROL Hour Types]** .

1. Selecteer het uurtype u wilt deactiveren.

1. Klik op **[!UICONTROL Deactivate]**.
