---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: percentage gebruikersrol van beschikbaarheid van FTE'
description: U kunt een kolom aan de mening van een gebruikerslijst toevoegen om een lijst van de Rollen van de Baan te tonen de gebruiker met evenals het percentage van VTE beschikbaarheid voor elke baanrol wordt geassocieerd, zoals die in het gebruikersprofiel wordt bepaald.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: d479b0b1-8ad5-47d6-8ef8-80261b46ecea
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Weergave: Percentage gebruikersrol rol van beschikbaarheid van FTE

U kunt een kolom aan de mening van een gebruikerslijst toevoegen om een lijst van de Rollen van de Baan te tonen de gebruiker met evenals het percentage van VTE beschikbaarheid voor elke baanrol wordt geassocieerd, zoals die in het gebruikersprofiel wordt bepaald.

Voor informatie over het bepalen van het percentage van VTE beschikbaarheid voor gebruikers, zie [Gebruikersprofiel bewerken](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

![user_with_percent_avialbility_per_role.png](assets/user-with-percent-avialbility-per-role-350x138.png)

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een rapport beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Het percentage van de Rol van de Taak van de gebruiker van de Mening van VTE beschikbaarheid

1. Ga naar een lijst met gebruikers.
1. Van de **Weergave** vervolgkeuzelijst, selecteert u **Nieuwe weergave**.

1. In de **Kolomvoorvertoning** gebied, klikken **Kolom toevoegen**.

1. Klik op de kop van de nieuwe kolom en klik vervolgens op **Overschakelen naar tekstmodus**.
1. Plaats de muis boven het gebied in de tekstmodus en klik op **Klik om tekst te bewerken**.
1. Verwijder de tekst die u vindt in het dialoogvenster **Tekstmodus** en vervang deze door de volgende code:

   <pre>displayname=Roltijd Percentage<br>listdelimiter=<p><br>listmethod=nested(userRoles).lists<br>textmode=true<br>type=iterate<br>valueexpression=CONCAT({role},'-',{timePercentage},'%')<br>valueformat=HTML</pre>

1. Klikken **Opslaan** vervolgens **Weergave opslaan**.

1. (Optioneel) Geef een naam op voor uw weergave en klik vervolgens op **Weergave opslaan**.
