---
title: Toegang tot documenten verlenen
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: Als Adobe Workfront-beheerder kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot documenten in Workfront te definiëren.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ba1d9a9b-7a1f-498b-a6e5-c548a11ac87c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 0%

---

# Toegang tot documenten verlenen

Als Adobe Workfront-beheerder kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot documenten te definiëren, zoals wordt uitgelegd in [Overzicht van toegangsniveaus](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Deze toegang geldt ook voor documentmappen.

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
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.&gt;.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Gebruikerstoegang tot documenten configureren met behulp van een aangepast toegangsniveau

1. Beginnen met het maken of bewerken van het toegangsniveau, zoals wordt uitgelegd in [Aangepaste toegangsniveaus maken of wijzigen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klik op het tandwielpictogram ![](assets/gear-icon-settings.png) op de **Weergave** of **Bewerken** rechts van Documenten en selecteer vervolgens de mogelijkheden die u onder **Uw instellingen nauwkeurig afstellen**.

   ![document_access.png](assets/document-access.png)

   U kunt gebruikers toestaan het volgende te doen op projecten, taken, en kwesties die zij toegang hebben tot:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Maken</td> 
      <td>Documenten uploaden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verwijderen</td> 
      <td> <p>Geüploade documenten verwijderen.</p> <p>De <b>Maken</b> Deze optie wordt automatisch ingeschakeld wanneer deze optie is ingeschakeld.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Delen</td> 
      <td>Deel documenten met specifieke gebruikers, baanrollen, teams.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documenten openbaar delen</td> 
      <td>Documenten delen met externe gebruikers (geen Workfront-licentie).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Delen op systeemniveau</td> 
      <td> <p>Documenten beschikbaar stellen voor iedereen in uw Workfront-exemplaar.</p> <p>Iedereen in het systeem kan een document zien op deze manier wordt gedeeld als:</p> 
       <ul> 
        <li> <p>U verzendt hen een verbinding aan de pagina van Documenten waar het wordt geupload.</p> </li> 
        <li> <p>Ze zoeken ernaar in Workfront</p> </li> 
       </ul> <p>De <b>Delen</b> Deze optie wordt automatisch ingeschakeld wanneer deze optie is ingeschakeld.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Wanneer u een toegangsniveau het plaatsen voor een bepaald type van voorwerp vormt, beïnvloedt die configuratie niet de toegang van de gebruikers tot voorwerpen met een lagere rang. Bijvoorbeeld, kunt u gebruikers van het schrappen van projecten in hun toegangsniveau beperken, maar dit beperkt hen niet van het schrappen van documenten, die lager rangschikken dan projecten.Voor meer informatie over de hiërarchie van voorwerpen, zie de sectie [Interdependentie en hiërarchie van objecten](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) in het artikel [Objecten in Adobe Workfront begrijpen](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (Optioneel) Als u overerfde machtigingen voor documenten van objecten met een hogere classificatie wilt beperken, klikt u op **Aanvullende beperkingen instellen** selecteert u vervolgens **Documenttoegang nooit overerven van projecten, taken, problemen, enzovoort**.
1. (Optioneel) Als u de toegangsinstellingen wilt configureren voor andere objecten en gebieden in het toegangsniveau waaraan u werkt, gaat u verder met een van de artikelen in [Toegang tot Adobe Workfront configureren](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), zoals [Toegang verlenen tot taken](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) en [Toegang tot financiële gegevens verlenen](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Als u klaar bent, klikt u op **Opslaan**.

   Nadat het toegangsniveau wordt gecreeerd, kunt u het aan een gebruiker toewijzen. Zie voor meer informatie [Gebruikersprofiel bewerken](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Toegang tot documenten per licentietype

Zie de sectie voor meer informatie over wat gebruikers op elk toegangsniveau met documenten kunnen doen [Documenten](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#document) in het artikel [Beschikbare functionaliteit voor elk objecttype](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Toegang tot gedeelde documenten

Nadat u een document naar Workfront hebt geüpload, kunt u het delen met andere gebruikers door hun machtigingen te verlenen, zoals wordt uitgelegd in [Een document delen](../../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data<
* issue
-->

Wanneer u een object met een andere gebruiker deelt, worden de rechten van de ontvanger op het object bepaald door een combinatie van twee dingen:

* De machtigingen die u aan de ontvanger toekent voor het object
* De instellingen van het toegangsniveau van de ontvanger voor het objecttype
