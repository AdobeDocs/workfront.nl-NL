---
product-area: documents
navigation-topic: approvals
title: Een workflow voor documentgoedkeuring maken
description: U kunt goedkeuring aanvragen bij andere gebruikers voor een document in Adobe Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: a02699e1-3557-47f0-89b7-dbecb507a174
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: b3c8559ddac934cc41461f88503b2fa71abaf452
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---

# Een workflow voor documentgoedkeuring maken

U kunt goedkeuring aanvragen bij andere gebruikers of teams voor een document in Adobe Workfront, of ze vragen een document te bekijken zonder het goed te keuren.

>[!IMPORTANT]
>
>De inhoud van dit artikel verwijst naar de functionaliteit voor bijgewerkte documentgoedkeuring die alleen beschikbaar is voor specifieke accounts. Voor informatie over standaardgoedkeuringsprocessen, zie de artikelen die in [&#x200B; worden vermeld goedkeuringen van het Werk &#x200B;](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Elk Workfront-pakket om goedkeuringen te beheren met behulp van verouderde Workfront-opslag</p>
<p>Elk workflowpakket om goedkeuringen te beheren met behulp van Adobe Enterprise Storage</p> </td> 
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
   <td> <p>Toegang tot het object beheren dat is gekoppeld aan de toegang tot of goedkeuring van de aanvraag </p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een goedkeuringswerkstroom maken vanuit het deelvenster Samenvatting in het gebied met oudere documenten

Als uw organisatie in Workfront is opgeslagen, wordt het gedeelte met verouderde documenten weergegeven wanneer u documenten in Workfront opent. Voor meer informatie over de opslag van Workfront, zie [&#x200B; Opslag van Workfront vs. de ondernemingsopslag van Adobe &#x200B;](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage).

Een goedkeuringswerkstroom maken:

1. Ga naar het project, de taak, of de kwestie die het document bevat, dan selecteren **Documenten** in het linkerpaneel.

1. Klik op het gewenste document en het deelvenster Documentsamenvatting voor dat document wordt geopend.

1. Selecteer de versie van het document waarvoor u goedkeuring wilt maken in het vervolgkeuzemenu Versie. De meest recente versie is standaard geselecteerd.

1. De rol neer aan de **goedkeurt** sectie, dan klikt **creeert werkschema**.


1. Vul de volgende gegevens in:

   <table>
   <tr>
   <td><strong>Werkgebiednaam</strong></td>
   <td>Voeg een werkgebiednaam toe. U kunt de naam in iets beschrijvender veranderen, zoals <em> Eerste Overzicht </em> of <em> Definitieve Goedkeuring </em>.</td>
   </tr>
   <tr>
   <td><strong>Namen of e-mails toevoegen</strong></td>
   <td>Typ een gebruiker- of teamnaam die u als fiatteur of revisor wilt toevoegen. Als u alleen revisoren hebt, worden deze op de hoogte gesteld en hebben ze de mogelijkheid de revisie te voltooien, maar er wordt geen beslissing vereist of genomen.</td>
   </tr>
   <tr>
   <td><strong>Eén beslissing vereist (facultatief)</strong></td>
   <td>De eerste persoon die een besluit neemt, voltooit het stadium.</td>
   </tr>
   <tr>
   <td><strong>Vervaldatum (optioneel)</strong></td>
   <td>Stel een vervaldatum in voor de goedkeuring. Gebruikers en teams worden 72 uur per e-mail op de hoogte gesteld en 24 uur vóór de opgegeven vervaldatum.</td>
   </tr>
   </table>

1. (Optioneel) Herhaal de vorige stap om zo nodig extra stappen toe te voegen.

   >[!NOTE]
   >
   >Als u meerdere fasen toevoegt, gaat de goedkeuringswerkstroom verder in de volgorde waarin de fasen worden weergegeven. Wanneer alle vereiste beslissingen worden genomen, begint de volgende fase en wordt de vorige fase vergrendeld.

   ![&#x200B; de details van het Document &#x200B;](assets/new-stage.png)


## Een goedkeuringswerkstroom maken vanuit het deelvenster Samenvatting in het gebied Nieuwe documenten

Als uw organisatie bedrijfsopslag gebruikt, ziet u het nieuwe gebied Documenten wanneer u documenten in Workfront opent. Voor meer informatie over ondernemingsopslag, zie [&#x200B; de opslagoverzicht van de Onderneming &#x200B;](/help/quicksilver/review-and-approve-work/esm-overview.md).

Een goedkeuringswerkstroom maken:

1. Ga naar het project, de taak, of de kwestie die het document bevat, dan selecteren **Documenten** in het linkerpaneel.

1. Klik op het document en klik vervolgens op het pictogram Goedkeuringen rechts op de pagina.

   ![&#x200B; voegt fiatteurs in documentsamenvatting &#x200B;](assets/approvals-icon-new.png) toe

1. Klik **creeer werkschema**, dan vul de volgende details in:

   <table>
   <tr>
   <td><strong>Werkgebiednaam</strong></td>
   <td>Voeg een werkgebiednaam toe. U kunt de naam in iets beschrijvender veranderen, zoals <em> Eerste Overzicht </em> of <em> Definitieve Goedkeuring </em>.</td>
   </tr>
   <tr>
   <td><strong>Namen of e-mails toevoegen</strong></td>
   <td>Typ een gebruiker- of teamnaam die u als fiatteur of revisor wilt toevoegen. Als u alleen revisoren hebt, worden deze op de hoogte gesteld en hebben ze de mogelijkheid de revisie te voltooien, maar er wordt geen beslissing vereist of genomen.</td>
   </tr>
   <tr>
   <td><strong>Eén beslissing vereist (facultatief)</strong></td>
   <td>De eerste persoon die een besluit neemt, voltooit het stadium.</td>
   </tr>
   <tr>
   <td><strong>Vervaldatum (optioneel)</strong></td>
   <td>Stel een vervaldatum in voor de goedkeuring. Gebruikers en teams worden 72 uur per e-mail op de hoogte gesteld en 24 uur vóór de opgegeven vervaldatum.</td>
   </tr>
   </table>

1. (Optioneel) Herhaal de vorige stap om zo nodig extra stappen toe te voegen.

   >[!NOTE]
   >
   >Als u meerdere fasen toevoegt, gaat de goedkeuringswerkstroom verder in de volgorde waarin de fasen worden weergegeven. Wanneer alle vereiste beslissingen worden genomen, begint de volgende fase en wordt de vorige fase vergrendeld.

   ![&#x200B; de details van het Document &#x200B;](assets/new-stage.png)



<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![Resubmit approval](assets/nwe-resubmit-approval-350x149.png)
-->
