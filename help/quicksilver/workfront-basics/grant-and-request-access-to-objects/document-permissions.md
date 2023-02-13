---
title: Een document delen
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: Uw Adobe Workfront-beheerder verleent gebruikers toegang tot weergave- of bewerkingsdocumenten wanneer zij toegangsniveaus toewijzen, zoals wordt uitgelegd in Toegang verlenen tot documenten.
author: Alina
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# Een document delen

Uw Adobe Workfront-beheerder verleent gebruikers toegang tot weergave- of bewerkingsdocumenten wanneer zij toegangsniveaus toewijzen, zoals wordt uitgelegd in [Toegang tot documenten verlenen](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).

Het toegangsniveau dat de beheerder van Workfront aan gebruikers verleent staat hen toe om of documenten te bekijken of uit te geven. Daarnaast kunnen andere gebruikers andere gebruikers ook machtigingen verlenen voor het weergeven of beheren van specifieke documenten die ze zelf hebben geüpload of die ze kunnen delen.

Machtigingen gelden specifiek voor één item in Workfront en definiëren welke handelingen u op dat item kunt uitvoeren. Zie voor informatie over objectmachtigingen [Overzicht van het delen van machtigingen voor objecten](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

De gebruiker die een document naar Workfront uploadt, beschikt standaard over de machtiging Beheren.

Voor informatie over het delen van een volledige documentmap raadpleegt u [Een documentmap delen](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Overwegingen bij het delen van documenten

Naast de onderstaande overwegingen, zie ook [Overzicht van het delen van machtigingen voor objecten](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Een Workfront-beheerder kan machtigingen toevoegen of verwijderen voor alle items in het systeem, zonder de eigenaar van die items te zijn.

* Het delen van een document is vergelijkbaar met het delen van andere objecten in Workfront. Ga voor informatie over het delen van documenten in Workfront naar [Een object delen](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* U kunt documenten de volgende machtigingen geven:

   * Weergave
   * Beheren

* U kunt een document ook openbaar of systeembreed delen.

   >[!CAUTION]
   >
   >We raden u aan voorzichtig te zijn wanneer u een object met vertrouwelijke informatie deelt met externe gebruikers. Op deze manier kunnen ze informatie weergeven zonder dat ze een Workfront-gebruiker of onderdeel van uw organisatie zijn.

* U kunt een document delen met iemand die geen Workfront-account heeft, door het e-mailadres ervan toe te voegen in het veld Toegang tot document geven.
* Als u een document deelt, hebben gebruikers dezelfde toegang tot alle documentversies en alle documentproefdrukken.\
   Raadpleeg voor meer informatie over proefdrukken in Workfront de [Proofing](../../review-and-approve-work/proofing/proofing.md) sectie.

* U kunt machtigingen voor documenten overnemen van de objecten waaraan ze zijn gekoppeld. Uw Workfront-beheerder kan de overerving van machtigingen voor documenten op uw toegangsniveau beperken.

   Zie voor meer informatie over het beperken van overerfde machtigingen voor documenten [Aangepaste toegangsniveaus maken of wijzigen](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

   U kunt overgeërfde machtigingen voor documenten handmatig verwijderen. Zie voor meer informatie [Rechten van objecten verwijderen](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)

* Een bijgevoegd document neemt alleen machtigingen over van het object waaraan het is gekoppeld. Als u een map voor het object maakt en het document naar de map verplaatst, neemt deze de machtigingen van de map over. Maar als u een map maakt op een bovenliggend of bovenliggend object en het document naar die map verplaatst, worden de machtigingen van die map niet overgenomen.

## Documentmachtigingen

In de volgende tabel wordt aangegeven welke machtigingen u gebruikers kunt verlenen wanneer zij documenten mogen weergeven of beheren:

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Handeling</strong> </p> </th> 
   <th> <p><strong>Beheren</strong> </p> </th> 
   <th> <p><strong>Weergave</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="row">Maken</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Documentdetails bewerken</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Verwijderen*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Downloaden</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Afhandeling</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">fiatteurs toevoegen</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Document goedkeuren</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Aangepast formulier bijvoegen</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Aangepaste velden bewerken</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Verplaatsen naar (object)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Verzenden naar (integratie)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Updates/opmerkingen</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Nieuwe versie uploaden</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Versie verwijderen</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Document(en) weergeven</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Voorvertoning</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Proef**</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Proef genereren**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Proef verwijderen**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Delen*</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Delen op systeemniveau*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Documenten openbaar delen*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Delen met een extern e-mailadres</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Toevoegen/verwijderen</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Naam wijzigen</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Koppeling (met integratie)</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Ontkoppelen (met integratie)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Actie wordt gedeeld door zowel Documenten als Documentmappen.

&#42;&#42; U moet een aparte proeflicentie hebben voor uw Workfront-account om documenten te kunnen aantonen. Neem contact op met uw accountmanager voor het verkrijgen van een proefdruklicentie. Ga voor meer informatie over proefdrukken in Workfront naar [Proofing](../../review-and-approve-work/proofing/proofing.md).
