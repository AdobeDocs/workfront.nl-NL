---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Uurtypen beheren
description: U kunt uurtypen koppelen aan uw uren. De types van uren zijn etiketten u gebruikt om uw uuringangen te bepalen.
author: Alina, Lisa
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: 3827e834a71084f14a99cb27aadefd97327b02d7
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 0%

---

# Uurtypen beheren

<!--Audited: 05/2025-->

<!--Audited: 07/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

De types van uren zijn etiketten u gebruikt om uw uuringangen te bepalen. U kunt uurtypen koppelen aan uw uren.

Er zijn twee reeksen uurtypes:

* Typen projectspecifieke uren: dit is tijd die projecten, taken, en kwesties wordt het programma geopend. Projectspecifieke urentypen kunnen overal in [!DNL Adobe Workfront] met uurvermeldingen worden geassocieerd waar u tijd voor projecten, taken, en kwesties kunt registreren.

  Wanneer het registreren van tijd in [!DNL Workfront], de project-specifieke uurtypes die beschikbaar zijn afhangen van configuratieopties die op het systeem, het project, en gebruikersniveaus worden geplaatst.

  De volgende standaardproject-specifieke uurtypes zijn altijd beschikbaar:

   * Projecttijd
   * Taaktijd
   * Uitgiftetijd

  De [!DNL Workfront] beheerder bepaalt welke project-specifieke uurtypes beschikbaar worden gemaakt, zoals die in [ worden beschreven bepaalt uurtypes en beschikbaarheid ](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

  >[!NOTE]
  >
  >Als u om het even welke project-specifieke uurtypes in uw [!DNL Workfront] systeem toelaat, moet minstens één project-specifiek uurtype op elk project in uw systeem worden toegelaten. U kunt geen project-specifiek uurtype op het systeemniveau toelaten en geen project-specifieke uurtypes hebben beschikbaar op het projectniveau.

* De Algemene Types van Uur: De algemene uren kunnen niet met een project, een taak, of een kwestie worden geassocieerd, en worden geregistreerd direct in timesheet.

Voor informatie over het registreren van uren en het associëren van hen met uurtypes, zie [ tijd van het Logboek ](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

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
   <td> <p>Nieuw: Standaard</p>
   <p>of</p>
   <p>Huidig: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>Systeembeheerder</td>
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ingebouwde uurtypen

Workfront wordt geleverd met een aantal ingebouwde uurtypen. Deze uurtypen kunnen niet worden bewerkt of verborgen.

De uurtypen die bij [!DNL Workfront] worden geleverd, zijn:

* **[!UICONTROL Sick Time]**: Een type van algemene uren dat niet met uuringangen op een project, een taak, of een kwestie kan worden geassocieerd. Zieke uren kunnen niet als opbrengst worden geteld.
* **[!UICONTROL Vacation Time]**: Een type van algemene uren dat niet met uuringangen op een project, een taak, of een kwestie kan worden geassocieerd. De tijd van de vakantie kan niet als opbrengst worden gerekend.
* **[!UICONTROL General Overhead]**: Een type van algemene uren dat niet met uuringangen op een project, een taak, of een kwestie kan worden geassocieerd. Het kan als opbrengst in uw project planningsproces tellen.
* **[!UICONTROL Project Time]**: Een uurtype van algemeen dat slechts met uuringangen op een project kan worden geassocieerd.
* **[!UICONTROL Task Time]**: een type van algemene uren dat slechts met uuringangen op een taak kan worden geassocieerd.
* **[!UICONTROL Issue Time]**: Een uurtype van het algemeen dat slechts met uuringangen over een kwestie kan worden geassocieerd.

## Urentypen maken

Als [!DNL Workfront] beheerder, kunt u nieuwe uurtypes voor uw organisatie op zowel systeem als projectniveaus tot stand brengen. Daarna, kunnen de gebruikers bepalen welke uurtypes voor specifieke projecten en gebruikers beschikbaar zijn. Voor meer informatie, zie [ de types en beschikbaarheid van uren bepalen ](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

Nieuwe uurtypen maken:

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Tijdopmaak &amp; Uren**, dan klik **de Types van Uur**.

1. In de **sectie van de Types van Uur 0} {, klik** + Nieuw Type van Uur **.**
1. In het **Nieuwe de dialoogvakje van de Types van Uur**, specificeer de volgende informatie:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Voer een naam in voor het uurtype dat gemakkelijk herkenbaar is in het systeem.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Voeg een beschrijving toe voor het uurtype.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope]</td> 
      <td> <p>Selecteer of het uurtype een algemeen of project-specifiek uurtype in het <strong> drop-down menu van het Toepassingsgebied </strong> is.</p> <p>De algemene uurtypes zijn zichtbaar slechts in timesheets en kunnen niet met projecten, taken, of kwesties worden geassocieerd.</p> <p><b> BELANGRIJK </b>: Als u een Type van douaneuren hebt dat [!UICONTROL Project Specific] is en u het in [!UICONTROL General] verandert, worden alle bestaande Taak, Kwesties en de uren van het Project geplaatst aan hun systeem standaardtypes.</p> </td> 
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

1. Klik op **[!UICONTROL Create Hour Type].**

## Uren deactiveren

U kunt uurtypen deactiveren als u niet langer wilt dat gebruikers hun uren aan hen koppelen. Als u uurtypen deactiveert, worden ze overal in [!DNL Workfront] verborgen, waar uurtypen zichtbaar zijn.

Een uurtype deactiveren:

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op **[!UICONTROL Timesheet & Hours]** en klik vervolgens op **[!UICONTROL Hour Types]** .

1. Selecteer het uurtype u wilt deactiveren.

1. Klik op **[!UICONTROL Deactivate]**.

   ![ Deactivate knoop ](assets/deactivate-button.png)
