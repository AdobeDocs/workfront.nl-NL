---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: de breedte van een kolom permanent bewerken'
description: U kunt de breedte van kolommen tijdelijk aanpassen door de marges te slepen en neer te zetten, zodat deze overeenkomen met de gewenste breedte. Zie Kolombreedte en -volgorde wijzigen voor meer informatie.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: 261c1b73d785094de4ee8549c856a091920ba04a
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# Weergave: de breedte van een kolom permanent bewerken

<!-- Audited: 1/2024 -->

U kunt de breedte van kolommen tijdelijk aanpassen door de marges te slepen en neer te zetten, zodat deze overeenkomen met de gewenste breedte. Zie voor meer informatie [Kolombreedte en -volgorde wijzigen](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

Als u de breedte van een kolom van een weergave permanent wilt wijzigen, moet u de tekstmodus in de kolom gebruiken wanneer u de weergave bewerkt.

## Toegangsvereisten

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

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## De breedte van een kolom permanent bewerken

>[!IMPORTANT]
>
>Als u de breedte van een kolom handmatig wijzigt, zoals wordt beschreven in de sectie [De breedte en volgorde van kolommen tijdelijk wijzigen](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md#modify-width-and-order-of-columns-temporarily) in het artikel [Kolombreedte en -volgorde wijzigen](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) Nadat u de breedte van de kolom permanent hebt gewijzigd, blijft de breedte van de kolom behouden op basis van de grootte van de kolom. In dit geval wordt de breedte van de kolom die wordt bijgewerkt volgens de volgende stappen, overschreven. U kunt de kolom weergeven op basis van de breedte die in de volgende stappen is gedefinieerd nadat u de cache hebt gewist of zich hebt aangemeld vanuit een andere browser.
>
>Zie de definities &quot;breedte&quot; en &quot;uitrekken&quot; in het gedeelte [Woordenlijst met Adobe Workfront-terminologie](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

1. Ga naar een lijst met objecten.
1. Van de **Weergave** vervolgkeuzelijst, klikt u op **Nieuwe weergave**.

1. Klikken **Kolom toevoegen** een nieuwe kolom toevoegen.

   of

   Klik op de kolomkop van een bestaande kolom.

1. Klikken **Overschakelen naar tekstmodus**.
1. Houd de cursor boven het gebied van de tekstmodus en klik op **Klik om tekst te bewerken**.
1. Voeg de volgende code aan de tekstwijze van de kolom toe:

   ```
   width=200
   usewidths=true
   ```

   Voor de **width** Geef een willekeurig aantal (in pixels) op dat aangeeft in welke mate de kolom moet worden weergegeven in de weergave.

1. Klikken **Opslaan** vervolgens **Weergave opslaan**.


