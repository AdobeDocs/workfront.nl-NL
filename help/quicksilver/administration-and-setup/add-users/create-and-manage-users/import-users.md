---
title: Gebruikers importeren
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: U kunt gebruikers naar de Adobe Workfront-site importeren door gebruikers te synchroniseren vanuit een netwerkdirectoryservice (zoals Active Directory of een andere LDAP-directory), of u kunt gebruikers importeren met behulp van een spreadsheet-importbestand.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3dd99d01-a32f-4af8-90e3-f8c0e9027651
source-git-commit: 554e08c22f6ee142a9ced8fa991d0126b6360b0c
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Gebruikers importeren

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Add users" in the article [Bulk Upload Users](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

-->

U kunt gebruikers importeren met behulp van een spreadsheet-importbestand.

Voordat u een nieuwe gebruiker maakt, moet u eerst controleren of u alle objecten hebt gemaakt die u aan de gebruiker wilt koppelen. Bijvoorbeeld, als u geen programma hebt gecreeerd, kunt u geen programma aan de nieuwe gebruiker toewijzen, en het gebied u gebruikt om een programma met de nieuwe gebruiker te associëren verschijnt niet in het Nieuwe scherm van de Gebruiker.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

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
   <td><p>Nieuw: Standaard</p><p>of</p><p>Huidig: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een van de volgende opties hebben:</p> 
    <ul> 
     <li> <p>Het toegangsniveau voor systeembeheerders. </li> 
     <li> <p><b> Gebruikers </b> het plaatsen in uw toegangsniveau dat aan <b> wordt gevormd geeft </b> toegang uit, met <b> creeert </b> en minstens één van de twee <b> die gebruikers Admin </b> opties onder <b> worden toegelaten verfijnen uw montages </b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Van deze twee opties, als <b> Admin van de Gebruiker (de Gebruikers van de Groep) </b> wordt toegelaten, moet u een groepsbeheerder van een groep zijn waar de gebruiker een lid is.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een spreadsheet-importbestand gebruiken om gebruikers te importeren

{{step-1-to-users}}

1. Klik de **Nieuwe Gebruiker** drop-down pijl, dan klik **de Gebruikers van de Invoer**.

1. In het **vakje van de Gebruikers van de Invoer** dat toont, download het steekproefdossier, dan werk het steekproefdossier bij om de persoonlijke informatie van uw eigen gebruiker te omvatten.

   Elke rij bevat de volgende velden:

   * **Voornaam**
   * **Achternaam**
   * **E-mailadres**

     E-mailadressen moeten uniek zijn.

   * **Niveau van de Toegang**

     Toegangsniveaus zijn hoofdlettergevoelig.

   * **identiteitskaart van de Login SSO**

     Dit veld wordt alleen opgenomen als SSO in uw systeem is ingeschakeld. U moet de federatie-id in dit veld toevoegen voor elke gebruiker. Wanneer u een gebruiker maakt op het tabblad Personen, kunt u een wachtwoord instellen voor de gebruiker als u gebruikers wilt toestaan zich aan te melden zonder SSO. Met de functie Importeren kunt u de id voor AANMELDING VAN DE SSO echter niet leeg laten.

   * Zorg ervoor dat er geen extra spaties bestaan voor of na het e-mailadres van een gebruiker.

   Wanneer u met een rij wordt gebeëindigd, zou het als volgt moeten kijken:

   ![ het invoeren-nieuw-users.png ](assets/importing-new-users.png)

1. Sla het bestand op een locatie op uw werkstation op.
1. Klik **kiezen Dossier** in de **Gebruikers van de Invoer** doos.

1. Navigeer naar en selecteer het bestand dat u hebt opgeslagen.
1. (Facultatief) selecteer **verzend een uitnodigingsE-mail naar deze gebruiker** optie om een e-mailuitnodiging naar de gebruiker te verzenden, hen op de hoogte te brengen dat een rekening van Workfront is gecreeerd en hen ertoe te brengen om hun wachtwoord te plaatsen.

   Schakel deze optie uit als u het wachtwoord voor de gebruiker wilt instellen.

1. Klik **Invoer**.

   U ontvangt boven aan het scherm een bevestigingsbericht dat de gebruiker is geïmporteerd.
