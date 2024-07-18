---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: de breedte van een kolom permanent bewerken'
description: U kunt de breedte van kolommen tijdelijk aanpassen door de marges te slepen en neer te zetten, zodat deze overeenkomen met de gewenste breedte. Zie Kolombreedte en -volgorde wijzigen voor meer informatie.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# Weergave: de breedte van een kolom permanent bewerken

<!-- Audited: 1/2024 -->

U kunt de breedte van kolommen tijdelijk aanpassen door de marges te slepen en neer te zetten, zodat deze overeenkomen met de gewenste breedte. Voor meer informatie, zie [ kolombreedte en orde wijzigen ](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

Als u de breedte van een kolom van een weergave permanent wilt wijzigen, moet u de tekstmodus in de kolom gebruiken wanneer u de weergave bewerkt.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Nieuw:<ul><li>Medewerker om een weergave te wijzigen</li><li>Standaard voor het wijzigen van een rapport</li></ul></p><p>of</p>Huidige:<ul><li>Verzoek om een weergave te wijzigen</li><li>Plan om een rapport te wijzigen</li></ul></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een weergave te wijzigen</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## De breedte van een kolom permanent bewerken

>[!IMPORTANT]
>
>Als u manueel de breedte van een kolom zoals die in de sectie [ wordt beschreven wijzigt tijdelijk breedte en orde van kolommen ](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md#modify-width-and-order-of-columns-temporarily) in het artikel [ wijzigt kolombreedte en orde ](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) nadat u permanent de breedte van de kolom hebt gewijzigd, wordt de breedte van de kolom bewaard volgens uw handresizing. In dit geval wordt de breedte van de kolom die wordt bijgewerkt volgens de volgende stappen, overschreven. U kunt de kolom weergeven op basis van de breedte die in de volgende stappen is gedefinieerd nadat u de cache hebt gewist of zich hebt aangemeld vanuit een andere browser.
>
>Voor extra informatie over het aanpassen van de breedte van kolommen wanneer het gebruiken van de interface van de Wijze van de Tekst, zie de &quot;breedte&quot;en &quot;uitrekbare&quot;definities in de [ Verklarende woordenlijst van de terminologie van Adobe Workfront ](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

1. Ga naar een lijst met objecten.
1. Van het **drop-down menu van de Mening**, klik **Nieuwe Mening**.

1. Klik **toevoegen Kolom** om een nieuwe kolom toe te voegen.

   of

   Klik op de kolomkop van een bestaande kolom.

1. Klik **Schakelaar aan de Wijze van de Tekst**.
1. Beweeg over het gebied van de tekstwijze, en klik **Klik om tekst** uit te geven.
1. Voeg de volgende code aan de tekstwijze van de kolom toe:

   ```
   width=200
   usewidths=true
   ```

   Voor de **breedte** lijn, specificeer om het even welk aantal (in pixel) dat vertegenwoordigt hoe breed u de kolom in de mening wilt tonen.

1. Klik **sparen**, dan **sparen Mening**.


