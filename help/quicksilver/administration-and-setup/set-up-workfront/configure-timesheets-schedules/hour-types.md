---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Uurtypen beheren
description: U kunt uurtypen koppelen aan uw uren. De types van uren zijn etiketten u gebruikt om uw uuringangen te bepalen. De types van uren kunnen voor algemene tijd of voor project-specifieke tijd zijn.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1074'
ht-degree: 0%

---

# Uurtypen beheren

<!--Audited: 05/2025-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

<!--<div class="preview">

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.     

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). 

</div>-->

De types van uren zijn etiketten u gebruikt om uw uuringangen te bepalen. U kunt uurtypen koppelen aan uw uren.

Er zijn twee categorieën van uurtypes:

* **de Specifieke Types van Uur van het Project**: Dit is tijd het programma geopend projecten, taken, en kwesties. Projectspecifieke urentypen kunnen overal in [!DNL Adobe Workfront] met uurvermeldingen worden geassocieerd waar u tijd voor projecten, taken, en kwesties kunt registreren.

  Wanneer het registreren van tijd in [!DNL Workfront], de project-specifieke uurtypes die beschikbaar zijn afhangen van configuratieopties die op het systeem, het project, en gebruikersniveaus worden geplaatst.

  De volgende standaardproject-specifieke uurtypes zijn altijd beschikbaar:

   * Projecttijd
   * Taaktijd
   * Uitgiftetijd

  De [!DNL Workfront] beheerder bepaalt welke project-specifieke uurtypes beschikbaar worden gemaakt, zoals die in [ worden beschreven bepaalt uurtypes en beschikbaarheid ](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

  >[!NOTE]
  >
  >Als u om het even welke project-specifieke uurtypes in uw [!DNL Workfront] systeem toelaat, moet minstens één project-specifiek uurtype op elk project in uw systeem worden toegelaten. U kunt geen project-specifiek uurtype op het systeemniveau toelaten en geen project-specifieke uurtypes hebben beschikbaar op het projectniveau.

* **de Types van Uur van 0} Algemeen**: De algemene uren kunnen niet met een project, een taak, of een kwestie worden geassocieerd, en rechtstreeks in een timesheet het programma geopend.

Voor informatie over het registreren van uren en het associëren van hen met uurtypes, zie [ tijd van het Logboek ](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licentie</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

Als [!DNL Workfront] beheerder, kunt u uurtypes voor uw organisatie op systeem en project-niveau tot stand brengen.

Nadat u uurtypes op systeem-niveau bepaalt, kunnen de gebruikers bepalen welke uurtypes voor specifieke projecten of voor specifieke gebruikers beschikbaar zijn.

Voor meer informatie, zie [ de types en beschikbaarheid van uren bepalen ](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

U kunt als volgt uurtypen maken:

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Tijdopmaak &amp; Uren**, dan klik **de Types van Uur**.

1. In de **sectie van de Types van Uur**, klik **Nieuw Type van Uur**.
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
      <td> <p>Selecteer of het uurtype een algemeen of project-specifiek uurtype in het <strong> drop-down menu van het Toepassingsgebied </strong> is.</p> <p>De algemene uurtypes zijn zichtbaar slechts in timesheets en kunnen niet met projecten, taken, of kwesties worden geassocieerd.</p> <p><b>BELANGRIJK</b></p><p> Als u een Type van douaneuren hebt dat [!UICONTROL Project Specific] is en u het in [!UICONTROL General] verandert, worden alle bestaande Taak, Kwesties en de uren van het Project geplaatst aan hun systeemstandaardtypes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Count as Revenue]</td> 
      <td><p>Selecteer deze optie als u de uuringang verbonden aan dit uurtype uw opbrengstberekeningen wilt beïnvloeden.</p>
      <p>De tijd van de ick en van de Vakantie kan niet als opbrengst worden geteld.</p>
      <p><b>OPMERKING</b></p>
      <p>Wanneer de algemene uurtypes als opbrengst worden geteld, wordt het tarief van Kosten verbonden aan het profiel van de gebruiker die de tijd registreert geassocieerd met de uurkosten.  
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Klik **sparen**.

   Het uurtype wordt toegevoegd aan uw Workfront-systeem en wordt standaard geactiveerd.

## Uren bewerken

Als [!DNL Workfront] beheerder, kunt u uurtypes voor uw organisatie op systeem en project-niveau uitgeven.

>[!NOTE]
>
>* U kunt ingebouwde uurtypen niet bewerken.
>* U kunt uurtypen niet bulksgewijs bewerken.

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Tijdopmaak &amp; Uren**, dan klik **de Types van Uur**.

1. Klik een het type van uur naam of selecteer het uurtype, dan klik **uitgeven** pictogram ![ pictogram ](assets/edit-icon.png) bij de bovenkant van de lijst uitgeven.
1. In **geef de dialoogdoos van de Types van Uur** uit, specificeer de volgende informatie:

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
      <td> <p>Selecteer of het uurtype een algemeen of project-specifiek uurtype in het <strong> drop-down menu van het Toepassingsgebied </strong> is.</p> <p>De algemene uurtypes zijn zichtbaar slechts in timesheets en kunnen niet met projecten, taken, of kwesties worden geassocieerd.</p> <p><b>BELANGRIJK</b></p> <p>Als u een Type van douaneuren hebt dat [!UICONTROL Project Specific] is en u het in [!UICONTROL General] verandert, worden alle bestaande Taak, Kwesties en de uren van het Project geplaatst aan hun systeemstandaardtypes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Count as Revenue]</td> 
      <td><p>Selecteer deze optie als u de uuringang verbonden aan dit uurtype uw opbrengstberekeningen wilt beïnvloeden.</p>
      <p>De tijd van de ick en van de Vakantie kan niet als opbrengst worden geteld.</p>
      <p><b>OPMERKING</b></p>
      <p>Wanneer de algemene uurtypes als opbrengst worden geteld, wordt het tarief van Kosten verbonden aan het profiel van de gebruiker die de tijd registreert geassocieerd met de uurkosten.  
      </td> 
     </tr> 
    </tbody> 
   </table>


1. Klik **sparen**.

   De wijzigingen worden opgeslagen en het uurtype wordt bewerkt.

## Uren deactiveren

U kunt uurtypen deactiveren als u niet langer wilt dat gebruikers hun uren aan hen koppelen. Als u uurtypen deactiveert, worden ze overal in [!DNL Workfront] verborgen, waar uurtypen zichtbaar zijn.

>[!NOTE]
>
>* U kunt ingebouwde uurtypen niet deactiveren.
>* U kunt uurtypen bulksgewijs deactiveren.
>* Wanneer u een project-specifiek Type van Uur deactiveert, al tijd die voor dat type automatisch wordt geregistreerd blijft aan een ingebouwd project-specifiek uurtype in gebreke. Bijvoorbeeld, tijd die voor een project wordt geregistreerd blijft aan het het uurtype van de Tijd van het Project; tijd die voor een taak wordt geregistreerd blijft aan het het uurtype van de Tijd van de Taak in gebreke.
>* Wanneer u een algemeen uurtype deactiveert, blijft de geregistreerde tijd op timesheet, maar de gebruikers kunnen niet meer tijd voor dat uurtype in de toekomst registreren.



Een uurtype deactiveren:

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op **[!UICONTROL Timesheet & Hours]** en klik vervolgens op **[!UICONTROL Hour Types]** .

1. Selecteer het uurtype u wilt deactiveren. U kunt meerdere uurtypen selecteren.

1. Klik **Meer**, toen **** deactivate.

   ![ activeer en deactiveer de verbindingen van het uurtype ](assets/activate-and-deactivate-hour-type-links.png)

   Het uurtype wordt gedeactiveerd en de gebruikers kunnen het niet meer vinden wanneer het registreren uren.

1. (Facultatief) om een uurtype opnieuw te activeren, selecteer het in de **lijst van de Types van Uur**, dan klik **Meer** > **activeert**.

