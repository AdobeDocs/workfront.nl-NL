---
product-area: timesheets;setup
navigation-topic: configure-timesheet-preferences
title: Configureer of de tijd uren of dagen is aangemeld
description: Als gebruiker met een Plan-licentie kunt u configureren of u zich binnen uren of dagen aanmeldt bij Adobe Workfront. Systeembeheerders kunnen deze instelling configureren voor individuele gebruikers of voor meerdere gebruikers in hun organisatie. Standaard kunnen gebruikers zich aanmelden in uren.
author: Alina
feature: Timesheets
exl-id: 4f801a13-182d-4e06-98ea-f6863f6a8edf
source-git-commit: b4ab350af22afa44774f06d82daf1c3fb266d2b9
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---

# Configureer of de tijd uren of dagen is aangemeld

Als gebruiker met een Planner-licentie kunt u configureren of u zich binnen uren of dagen aanmeldt bij Adobe Workfront. Systeembeheerders kunnen deze instelling configureren voor individuele gebruikers of voor meerdere gebruikers in hun organisatie. Standaard kunnen gebruikers zich aanmelden in uren. Voor informatie over hoe u zich kunt aanmelden in Workfront raadpleegt u [Logtijd](../../timesheets/create-and-manage-timesheets/log-time.md).

>[!NOTE]
>
>Wij adviseren registrerentijd op dezelfde manier, of uren of dagen, over de organisatie om rapporteringsnauwkeurigheid te verzekeren.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Planners kunnen tijd voor zichzelf configureren. Alleen een Workfront-beheerder kan tijd configureren voor andere gebruikers.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

1. Voer een van de volgende handelingen uit, afhankelijk van uw doel en uw toegangsniveau in het systeem:

   * **De gebruiker van de planter die tijd registreren voor zich vormt:** Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op uw gebruikersnaam naast de profielafbeelding. Klik vervolgens op de knop **Meer** pictogram naast uw naam en selecteer **Bewerken**.

   * **Systeembeheerder configureert tijdregistratie voor anderen:** Beginnen met het bewerken van een of meer gebruikersaccounts, zoals beschreven in [Gebruikersprofiel bewerken](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. In het resulterende dialoogvenster, in het dialoogvenster **Bronplanning** de sectie, bepaal de plaats van **Aanmeldtijd** optie.

   ![](assets/new-timesheet-log-hours-350x249.png)

1. (Voorwaardelijk) Als u een systeembeheerder bent die meerdere gebruikers tegelijk bewerkt, selecteert u **Aanmeldtijd**.
1. Maak een keuze uit de volgende opties voor logtijd:

   | Option | Beschrijving |
   |---|---|
   | **Uren** | Gebruikers geven uren op wanneer ze zich aanmelden in Workfront. |
   | **Dagen** | Gebruikers geven dagen op wanneer ze zich aanmelden in Workfront. |

1. (Voorwaardelijk) Als u hebt geselecteerd om de tijd in dagen in te loggen, in de **Equivalente uren voor volledige Workday** veld, typt u het aantal uren dat gelijk is aan een volledige dag. Een dag op het tijdsplaat van een gebruiker is het equivalent van het aantal uren u hier ingaat.

   Denk aan het volgende wanneer u deze instelling configureert:

   * Deze optie is niet beschikbaar wanneer het vormen aan logboektijd in uren.
   * Deze optie wordt gebruikt slechts voor het doel van logboektijd. Deze optie heeft geen betrekking op de **Schema** Deze optie is ook beschikbaar wanneer u een gebruiker bewerkt. De **Schema** wordt gebruikt bij het berekenen van tijdlijnen en in andere gebieden van Workfront. (Voor meer informatie over het gebruik van de **Schema** optie, zie [Een schema maken](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).) 

1. Klikken **Wijzigingen opslaan**.
