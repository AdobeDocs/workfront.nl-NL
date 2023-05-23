---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: de breedte van een kolom permanent bewerken'
description: U kunt de breedte van kolommen tijdelijk aanpassen door de marges te slepen en neer te zetten, zodat deze overeenkomen met de gewenste breedte. Zie Kolombreedte en -volgorde wijzigen voor meer informatie.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Weergave: De breedte van een kolom permanent bewerken

U kunt de breedte van kolommen tijdelijk aanpassen door de marges te slepen en neer te zetten, zodat deze overeenkomen met de gewenste breedte. Zie voor meer informatie [Kolombreedte en -volgorde wijzigen](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

U kunt de breedte van elke kolom van een weergave permanent wijzigen met de tekstmodus in de kolom terwijl u de weergave bewerkt.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Verzoek om een weergave te wijzigen </p>
   <p>Plan om een rapport te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een weergave te wijzigen</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een rapport beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## De breedte van een kolom permanent bewerken

>[!IMPORTANT]
>
>Als u de breedte van een kolom handmatig wijzigt zoals wordt beschreven in de sectie &quot;De breedte en volgorde van kolommen tijdelijk wijzigen&quot; in het artikel [Kolombreedte en -volgorde wijzigen](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) Nadat u de breedte van de kolom permanent hebt gewijzigd, blijft de breedte van de kolom behouden op basis van het handmatig wijzigen van de grootte en wordt de breedte van de kolom die wordt bijgewerkt volgens de volgende stappen, overschreven. U kunt de kolom weergeven op basis van de breedte die in de volgende stappen is gedefinieerd nadat u de cache hebt gewist of zich hebt aangemeld vanuit een andere browser.

1. Ga naar een lijst met objecten.
1. Van de **Weergave** vervolgkeuzelijst, klikt u op **Nieuwe weergave**.

1. Klikken **Kolom toevoegen** om een nieuwe kolom toe te voegen.

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
