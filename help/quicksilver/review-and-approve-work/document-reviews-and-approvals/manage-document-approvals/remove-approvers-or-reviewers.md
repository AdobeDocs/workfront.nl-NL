---
product-area: documents
navigation-topic: approvals
title: fiatteurs of revisoren verwijderen uit een workflow voor documentgoedkeuring
description: U kunt afzonderlijke fiatteurs of revisoren uit een document verwijderen.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6877ee90-9a70-4616-98f4-4b0ff932d79a
source-git-commit: 3fd4d18e1be14cc27b3b39d4abf399ec26ddcd51
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 0%

---

# fiatteurs of revisoren verwijderen uit een workflow voor documentgoedkeuring

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Het is beschikbaar slechts in het milieu van de Sandbox van de Voorproef.</span>

U kunt afzonderlijke fiatteurs of revisoren uit een element of document verwijderen nadat ze zijn toegewezen.

>[!IMPORTANT]
>
>De inhoud van dit artikel verwijst naar de functionaliteit voor bijgewerkte documentgoedkeuring die alleen beschikbaar is voor specifieke accounts. Voor informatie over standaardgoedkeuringsprocessen, zie de artikelen die in [ worden vermeld goedkeuringen van het Werk ](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
   <p>Medewerker of hoger</p>
   <p>Controleren of hoger</p>
   <p>Als u de integratie Frame.io gebruikt, moet u een Standaard vergunning hebben om goedkeuringswerkschema's tot stand te brengen.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot projecten, taken, problemen, sjablonen, portfolio's, programma's, rapporten, dashboards en agenda's, documenten weergeven of vergroten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toegang tot het object beheren dat is gekoppeld aan de toegang tot of goedkeuring van de aanvraag </p>  </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## fiatteurs of revisoren verwijderen van de pagina Documentdetails in de productieomgeving

1. Ga naar de documentpagina door op de naam van het document te klikken en selecteer vervolgens de versie van het document waarvoor u een goedkeuring wilt verwijderen in het vervolgkeuzemenu. De meest recente versie is standaard geselecteerd.

1. Selecteer **Goedkeuringen** in het linkerpaneel.

1. Beweeg over de naam van de fiatteur of de recensent u zou willen verwijderen, dan klikken op het **pictogram van de Schrapping** ![ pictogram van de Schrapping ](../assets/delete.png) dat na hun naam verschijnt.

   De goedkeuring of het revisieverzoek wordt verwijderd en de fiatteur ontvangt een melding dat zijn goedkeuring niet langer nodig is. Hun op goedkeuring betrekking hebbende aandeeltoegang wordt ook geschrapt.

1. (Facultatief) om een fiatteur aan een recensent te degraderen eerder dan hen volledig te verwijderen, uncheck **Approver** checkbox in lijn met hun naam.

1. Herhaal de vorige stap om extra fiatteurs of revisoren te verwijderen.

## fiatteurs of revisoren verwijderen uit het documentoverzicht in uw productieomgeving

1. Ga naar het project, de taak, of de kwestie die het document bevat, dan selecteren **Documenten**.

1. Klik op het gewenste document en het deelvenster Documentsamenvatting voor dat document wordt geopend.

1. Selecteer de versie van het document waarvoor u een fiatteur of revisor wilt verwijderen in het vervolgkeuzemenu. De meest recente versie is standaard geselecteerd.

1. De rol neer aan de **goedkeurt** sectie in het Summiere paneel van het Document. Beweeg over de naam van de fiatteur of de recensent u zou willen verwijderen, dan klikken op het **pictogram van de Schrapping** ![ pictogram van de Schrapping ](../assets/delete.png) dat na hun naam verschijnt.

   De goedkeuring of het revisieverzoek wordt verwijderd en de fiatteur ontvangt een melding dat zijn goedkeuring niet langer nodig is. Hun op goedkeuring betrekking hebbende aandeeltoegang wordt ook geschrapt.

1. (Facultatief) om een fiatteur aan een recensent te degraderen eerder dan hen volledig te verwijderen, uncheck **Approver** checkbox in lijn met hun naam.

1. Herhaal de vorige stap om extra fiatteurs of revisoren te verwijderen.


<div class="preview">

## fiatteurs of revisoren verwijderen uit een goedkeuringswerkstroom in de voorvertoningsomgeving in het gebied met oudere documenten

Als uw organisatie in Workfront is opgeslagen, wordt het gedeelte met verouderde documenten weergegeven wanneer u documenten in Workfront opent. Voor meer informatie over de opslag van Workfront, zie [ Opslag van Workfront vs. de ondernemingsopslag van Adobe ](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage).

Om fiatteurs of revisoren te verwijderen uit een goedkeuringswerkstroom:

1. Ga naar het project, de taak, of de kwestie die het document bevat, dan selecteren **Documenten** in het linkerpaneel.

1. Klik op het gewenste document en het deelvenster Documentsamenvatting voor dat document wordt geopend.

1. De rol neer aan de **goedkeurt** sectie in het Summiere paneel van het Document.

1. Klik **uitgeven werkschema**.

1. Bepaal de plaats van de deelnemer u wilt verwijderen, dan klik **verwijderen** pictogram naast hun naam.

   De goedkeuring of het revisieverzoek wordt verwijderd en de fiatteur ontvangt een melding dat zijn goedkeuring niet langer nodig is. Hun op goedkeuring betrekking hebbende aandeeltoegang wordt ook geschrapt.

   ![ geef goedkeuringswerkschema ](assets/edit-approval-in-legacy.png) uit

1. (Optioneel) Als u de rol van fiatteur wilt wijzigen in een revisor of andersom, klikt u op het vervolgkeuzemenu naast de gebruikersnaam en selecteert u de nieuwe rol.

1. Herhaal de vorige stap om extra fiatteurs of revisoren te verwijderen.

</div>


## fiatteurs of revisoren verwijderen uit een goedkeuringswerkstroom in het nieuwe documentgebied

Als uw organisatie bedrijfsopslag gebruikt, zult u het nieuwe documentengebied zien wanneer u tot documenten in Workfront toegang hebt. Voor meer informatie over ondernemingsopslag, zie [ de opslagoverzicht van de Onderneming ](/help/quicksilver/review-and-approve-work/esm-overview.md).

Een goedkeuringswerkstroom maken:

1. Ga naar het project, de taak, of de kwestie die het document bevat, dan selecteren **Documenten** in het linkerpaneel.

1. Klik op het document, dan klik het **goedkeurt** pictogram op de rechterkant van de pagina.

   ![ voegt fiatteurs in documentsamenvatting ](assets/approvals-icon-new.png) toe


1. Klik **uitgeven werkschema**.

1. Bepaal de plaats van de deelnemer u wilt verwijderen, dan klik **verwijderen** pictogram naast hun naam.

   De goedkeuring of het revisieverzoek wordt verwijderd en de fiatteur ontvangt een melding dat zijn goedkeuring niet langer nodig is.

1. (Optioneel) Als u de rol van fiatteur wilt wijzigen in een revisor of andersom, klikt u op het vervolgkeuzemenu naast de gebruikersnaam en selecteert u de nieuwe rol.

1. Herhaal de vorige stap om extra fiatteurs of revisoren te verwijderen.

   ![ verwijdert deelnemers uit een stadium ](assets/add-or-remove-participants.png)
1. Klik **sparen**.