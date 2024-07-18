---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Weergeven: rolpercentage van gebruiker in beschikbaarheid FTE''s'''
description: U kunt een kolom toevoegen aan de weergave van een gebruikerslijst om een lijst weer te geven met de functies waaraan de gebruiker is gekoppeld en het percentage beschikbare FTE's voor elke functie, zoals is gedefinieerd in het gebruikersprofiel.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: d479b0b1-8ad5-47d6-8ef8-80261b46ecea
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

---

# Weergave: percentage gebruikersrol van FTE-beschikbaarheid

U kunt een kolom aan de mening van een gebruikerslijst toevoegen om een lijst van de Rollen van de Baan te tonen de gebruiker met evenals het percentage van VTE beschikbaarheid voor elke baanrol wordt geassocieerd, zoals die in het gebruikersprofiel wordt bepaald.

Voor informatie over het bepalen van het percentage van VTE beschikbaarheid voor gebruikers, zie [ het profiel van een gebruiker ](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

![user_with_percent_avialbility_per_role.png](assets/user-with-percent-avialbility-per-role-350x138.png)

## Vereisten voor toegang

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-lidmaatschap*</td> 
   <td> <p>Enig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Verzoek voor het wijzigen van een weergave </p>
   <p>Plan om een rapport te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een weergave te wijzigen</p> <p><b>NOTITIE</b>

Als je nog steeds geen toegang hebt, vraag je je Workfront-beheerder of deze extra beperkingen instelt voor je toegangsniveau. Zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus</a> maken of wijzigen voor informatie over de wijze waarop een Workfront-beheerder je toegangsniveau kan wijzigen.</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen voor een rapport beheren</p> <p>Zie Toegang aanvragen tot objecten </a>voor meer informatie over het aanvragen van aanvullende toegang<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met je Workfront-beheerder als je wilt kijken welk lidmaatschap, welk licentietype of welke toegang je hebt.

## Het percentage functies van gebruiker in de beschikbaarheid van FTE&#39;s weergeven

1. Ga naar een lijst met gebruikers.
1. Van het **drop-down menu van de Mening**, uitgezochte **Nieuwe Mening**.

1. In het **gebied van de Voorproef van de Kolom**, klik **voegt Kolom** toe.

1. Klik op de koptekst van de nieuwe kolom en klik vervolgens op Overschakelen naar **de tekstmodus**.
1. Plaats de muis boven het tekstmodusgebied en klik op **Klik om de tekst** te bewerken.
1. Verwijder de tekst die u vindt in het **vak Tekstmodus** en vervang deze door de volgende code:
   <pre>displayname=Roles Time Percentage<br>listdelimiter=<p><br>listmethod=nested(userRoles).lists<br>textmode=true<br>type=iterate<br>valueexpression=CONCAT({role},'-',{timePercentage}'%')<br>valueformat=HTML</pre>

1. Klik op Opslaan **en vervolgens** op **Weergave** opslaan.

1. (Optioneel) Geef een naam op voor uw weergave en klik op **Weergave** opslaan.
