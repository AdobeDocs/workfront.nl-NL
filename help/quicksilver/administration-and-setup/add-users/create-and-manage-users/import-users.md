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
source-git-commit: 0239cad2d9173da20770934e6132b29301117cdf
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---

# Gebruikers importeren

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Add users" in the article [Bulk Upload Users](https://helpx.adobe.com/nl/enterprise/using/bulk-upload-users.html) or contact your Adobe Admin Console Administrator.
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

1. In het **vakje van de Invoer gebruikers** dat toont, download het steekproefdossier, dan werk het steekproefdossier bij om de persoonlijke informatie van uw eigen gebruiker te omvatten.

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
1. Klik **kiezen dossier** in het **de gebruikers van de Invoer** vakje.

1. Navigeer naar en selecteer het bestand dat u hebt opgeslagen.

<!--
1. (Optional) Select the **Send an invite email to this user** option to send an email invitation to the user, notifying them that a Workfront account has been created and prompting them to set their password.

   Deselect this option if you want to set the password for the user.

-->

1. Klik **Invoer**.

   U ontvangt boven aan het scherm een bevestigingsbericht dat de gebruikers correct zijn geïmporteerd.

>[!NOTE]
>
>De gebruikers worden aangemaakt in een gedeactiveerde en in afwachting van de goedkeuringsstatus.
> 
>Als een gebruiker binnen een paar minuten niet de status Uitgeschakeld en In afwachting van goedkeuring verlaat en het scherm vernieuwt de badge In afwachting van goedkeuring niet verwijdert, kunt u de batch gebruikers rechtstreeks aan de Adobe Admin Console toevoegen.
>
>Voor instructies, zie [ veelvoudige gebruikers beheren | Bulk CSV upload ](https://helpx.adobe.com/nl/enterprise/using/bulk-upload-users.html) in de documentatie van Adobe.
