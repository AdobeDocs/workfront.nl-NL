---
title: Gebruikers importeren
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: U kunt gebruikers naar de Adobe Workfront-site importeren door gebruikers te synchroniseren vanuit een netwerkdirectoryservice (zoals Active Directory of een andere LDAP-directory), of u kunt gebruikers importeren met behulp van een spreadsheet-importbestand.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3dd99d01-a32f-4af8-90e3-f8c0e9027651
source-git-commit: 1949a0bb213553f1f1f252c4382a90514fcd0b5b
workflow-type: tm+mt
source-wordcount: '494'
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

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

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
   <td> <p>U moet een van de volgende opties hebben:</p> 
    <ul> 
     <li> <p>Het toegangsniveau voor systeembeheerders. Zie voor meer informatie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>. </p> </li> 
     <li> <p><b>Gebruikers</b> het plaatsen in uw toegangsniveau dat wordt gevormd aan <b>Bewerken</b> toegang, met <b>Maken</b> en ten minste één van beide <b>Gebruikersbeheerder</b> opties ingeschakeld onder <b>Uw instellingen nauwkeurig afstellen</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Van deze twee opties, als Gebruiker <b>Admin (Groepgebruikers)</b> wordt toegelaten, moet u een groepsbeheerder van een groep zijn waar de gebruiker een lid is.</p> <p>Voor meer informatie over de <b>Gebruikers</b> het plaatsen in een toegangsniveau, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Toegang verlenen aan gebruikers</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Een spreadsheet-importbestand gebruiken om gebruikers te importeren

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Gebruikers** ![](assets/users-icon-in-main-menu.png).

1. Klik op de knop **Nieuwe gebruiker** vervolgkeuzepijl en klik vervolgens op **Gebruikers importeren**.

1. In de **Gebruikers importeren** weergegeven, downloadt u het voorbeeldbestand en werkt u het voorbeeldbestand bij met persoonlijke gegevens van uw eigen gebruiker.

   Elke rij bevat de volgende velden:

   * **Voornaam**
   * **Achternaam**
   * **E-mailadres**

     E-mailadressen moeten uniek zijn.

   * **Toegangsniveau**

     Toegangsniveaus zijn hoofdlettergevoelig.

   * **SSO-aanmeldings-id**

     Dit veld wordt alleen opgenomen als SSO in uw systeem is ingeschakeld. U moet de federatie-id in dit veld toevoegen voor elke gebruiker. Wanneer u een gebruiker maakt op het tabblad Personen, kunt u een wachtwoord instellen voor de gebruiker als u gebruikers wilt toestaan zich aan te melden zonder SSO. Met de functie Importeren kunt u de id voor AANMELDING VAN DE SSO echter niet leeg laten.

   * Zorg ervoor dat er geen extra spaties bestaan voor of na het e-mailadres van een gebruiker.

   Wanneer u met een rij wordt gebeëindigd, zou het als volgt moeten kijken:

   ![importeren-new-users.png](assets/importing-new-users.png)

1. Sla het bestand op een locatie op uw werkstation op.
1. Klikken **Bestand kiezen** in de **Gebruikers importeren** doos.

1. Navigeer naar en selecteer het bestand dat u hebt opgeslagen.
1. (Optioneel) Selecteer de optie **E-mail met een uitnodiging verzenden aan deze gebruiker** om een e-mailuitnodiging naar de gebruiker te verzenden, deze op de hoogte te stellen van het feit dat een Workfront-account is gemaakt en hen te vragen hun wachtwoord in te stellen.

   Schakel deze optie uit als u het wachtwoord voor de gebruiker wilt instellen.

1. Klikken **Importeren**.

   U ontvangt boven aan het scherm een bevestigingsbericht dat de gebruiker is geïmporteerd.
