---
title: Toegang verlenen tot projecten
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
description: Als beheerder van Adobe Workfront, kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot projecten in Workfront te bepalen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ba6a9e68-68a1-4152-b024-cd39e06d556f
source-git-commit: e47f5d06d0c7d72c171583b53b69f951e4e99afe
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 0%

---

# Toegang verlenen tot projecten

<!-- Audited: 12/2023 -->

Als beheerder van Adobe Workfront, kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot projecten te bepalen, zoals die in de volgende artikelen wordt verklaard:
* [Overzicht van toegangsniveaus](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)
* [Overzicht van nieuwe toegangsniveaus](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)

Voor informatie over het gebruiken van douanetoegangsniveaus om gebruikers&#39; toegang tot andere objecten types in Workfront te beheren, zie [Aangepaste toegangsniveaus maken of wijzigen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## Toegangsvereisten

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
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Nieuw: Standaard </p>
 <p>of</p> 
<p>Huidig: Plan </p> 
</td> 
  </tr>

<tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Vorm gebruikerstoegang tot projecten gebruikend een niveau van de douanetoegang

1. Beginnen met het maken of bewerken van het toegangsniveau, zoals wordt uitgelegd in [Aangepaste toegangsniveaus maken of wijzigen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klik op het tandwielpictogram ![](assets/gear-icon-settings.png) op de **Weergave** of **Bewerken** rechts van Projecten selecteert u vervolgens de capaciteiten die u onder **Uw instellingen nauwkeurig afstellen**.

   ![](assets/planner-fine-tune-your-settings-with-copy-projects.png)

   >[!NOTE]
   >
   >* Gebruikers met een werkvergunning hebben beperkte projectrechten. Ze kunnen wel bijdragen aan een project, maar niet beheren.
   >* Gebruikers met een Revisielicentie hebben weergaverechten voor projecten van omgezette uitgaven, maar hun weergaverechten zijn beperkt.
   >* Voor informatie over toestemmingen kunnen de gebruikers verlenen wanneer het delen van projecten met anderen, zie [Een project delen in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
   >* Wanneer u een toegangsniveau het plaatsen voor een bepaald type van voorwerp vormt, beïnvloedt die configuratie niet de toegang van de gebruikers tot voorwerpen met een lagere rang. Bijvoorbeeld, kunt u gebruikers van het schrappen van projecten in hun toegangsniveau beperken, maar dit beperkt hen niet van het schrappen van taken, die lager rangschikken dan projecten.Voor meer informatie over de hiërarchie van voorwerpen, zie de sectie [Interdependentie en hiërarchie van objecten](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) in het artikel [Objecten in Adobe Workfront begrijpen](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (Optioneel) Klik op **standaardinstellingen voor delen instellen** rechts van de optie Maken **Regel toevoegen** om een regel voor delen toe te voegen voor nieuwe projecten.

   Wanneer de gebruiker met dit toegangsniveau tot een project leidt, wordt het project gedeeld automatisch met de gebruikers u in het menu op de linkerzijde selecteert.

   ![](assets/project-sharing-menu.png)

   In het menu aan de rechterkant geeft u op hoe u het project wilt delen met die gebruikers:

   ![](assets/project-sharing-right-menu.png)

   >[!NOTE]
   >
   >Als een gebruiker met dit toegangsniveau een malplaatje van de projecttoegang gebruikt, treedt het malplaatje de het delen montages op het toegangsniveau met voeten. Voor informatie over de malplaatjes van de projecttoegang, zie [Een project delen in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

   U kunt deze stap herhalen om zo vele project toe te voegen delend regels aangezien u voor het toegangsniveau nodig hebt.

1. Klik op de X om het dialoogvenster **Uw instellingen nauwkeurig afstellen** doos.
1. (Optioneel) Als u de toegangsinstellingen wilt configureren voor andere objecten en gebieden in het toegangsniveau waaraan u werkt, gaat u verder met een van de artikelen in [Toegang tot Adobe Workfront configureren](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), zoals [Toegang verlenen tot taken](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) en [Toegang tot financiële gegevens verlenen](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Klik op **Opslaan**.

   Nadat het toegangsniveau wordt gecreeerd, kunt u het aan een gebruiker toewijzen. Zie voor meer informatie [Gebruikersprofiel bewerken](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Toegang tot rapporten, dashboards en kalenders per licentietype

Zie de sectie voor informatie over wat gebruikers op elk toegangsniveau met problemen kunnen doen [Projecten](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#projects) in het artikel [Beschikbare functionaliteit voor elk objecttype](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Toegang tot gedeelde projecten

Als eigenaar of maker van een uitgave kunt u deze delen met andere gebruikers door hun machtigingen te verlenen, zoals wordt uitgelegd in [Een project delen in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

Wanneer u een object met een andere gebruiker deelt, worden de rechten van de ontvanger op het object bepaald door een combinatie van twee dingen:

* De machtigingen die u aan de ontvanger toekent voor het object
* De instellingen van het toegangsniveau van de ontvanger voor het objecttype
