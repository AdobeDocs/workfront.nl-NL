---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Het wachtwoord wijzigen voor een gebruiker met automatische provisioning
description: Wanneer een nieuwe gebruiker zijn tijdelijke wachtwoord probeert te wijzigen, voert hij zijn e-mailadres in en ontvangt hij een fout wegens een onjuiste gebruikersnaam. Zij moeten hun systeem-toegewezen gebruikersnaam ingaan, die hun Globally Unique Identifier (GUID) is. Omdat een GUID moeilijk is te herinneren en te gebruiken, adviseren wij dat u een gebruikersnaam van een nieuwe gebruiker in hun Workfront e-mailadres verandert, dan hen toestaan om hun wachtwoord te veranderen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 14124911-e5e1-4a4f-9b25-8b4fab0329e1
source-git-commit: 7bd3d2252b124a07a112aaa2b7798063087e7cab
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 0%

---

# Het wachtwoord wijzigen voor een gebruiker met automatische provisioning

Wanneer u gebruikers door autolevering creeert, wijst Adobe Workfront hen een GUID (Globally Unique Identifier) voor een gebruikersnaam toe. Een GUID is een uniek koord van willekeurige aantallen en brieven, bijvoorbeeld, *5489cb430012526e1ea635e8c29f377f*.

Wanneer een nieuwe gebruiker zijn tijdelijke wachtwoord probeert te wijzigen, voert hij zijn e-mailadres vaak in voor zijn gebruikersnaam en ontvangt hij een fout voor een onjuiste gebruikersnaam. Opdat de gebruiker hun wachtwoord verandert, moeten zij hun systeem-toegewezen gebruikersnaam ingaan, die een GUID is.

Omdat de gebruikersnamen GUID moeilijk kunnen zijn te gebruiken, adviseren wij u eerst de gebruikersnaam van een gebruiker in hun Workfront e-mailadres veranderen, dan hen toestaan om hun wachtwoord te veranderen.

>[!TIP]
>
>U kunt GUID van een gebruiker op de volgende manieren vinden:
>
>* Ga naar het profiel van de gebruiker en kopieer GUID van URL in uw browser.
>
>  In de URL `https://acme.workfront.com/user/61941ab1000af22d7104628efa1c738b/details` kopieert u bijvoorbeeld de reeks getallen en letters tussen de laatste twee slashes: `61941ab1000af22d7104628efa1c738b` .
>
>  Voor meer informatie, zie [ het profiel van een gebruiker ](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.
>
>* Creeer een gebruikersrapport met een Gebruiker > GUID kolom. Voor meer informatie, zie [ een rapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md) creëren.
>
>* Vraag de Workfront API op.
>

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
   <td> <p>U moet een Workfront-beheerder zijn.</p> <p><b> NOTA </b>: Als u nog geen toegang hebt, vraag uw beheerder van Workfront als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Het wachtwoord wijzigen voor een gebruiker met automatische provisioning

1. Bepaal een gebruiker GUID- gebruikersnaam door een API verzoek, zoals aangetoond in het volgende voorbeeld over te gaan:

   https://`<domain>` .my.workfront.com/attask/api/v14.0/USER/search?fields=username&amp;ID= `<ID of User>` Waar *`<domain>`* is het domein van uw bedrijf en *`<ID of User>`* is identiteitskaart van Workfront van de gebruiker.

   U ontvangt een reactie die vergelijkbaar is met het volgende:

   ![](assets/get-guid.png)

   De terugkeer voor &quot;gebruikersbenaming&quot;is GUID van de gebruiker.

1. Gebruikend hun GUID als hun gebruikersnaam, verander het wachtwoord van de gebruiker.

   Voor meer informatie bij het veranderen van uw wachtwoord, zie [ het Terugstellen van uw wachtwoord ](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md).

   Als uw organisatie een SSO-systeem gebruikt, kan alleen een Workfront-systeembeheerder het wachtwoord van een gebruiker wijzigen. Voor meer informatie, zie [ Overzicht van enig teken-op in Adobe Workfront ](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)

1. Blader met de gebruiker aangemeld bij Workfront naar:

```
   https://<your domain>.my.workfront.com/login/convertUsername
```

1. In het **Uw login e-mailadres** vakje, verifieer dat het e-mailadres van de gebruiker correct is, dan klik **Rekening van de Update**.

   ![](assets/guidusername-350x272.png)

   De gebruikersnaam van de gebruiker wordt gewijzigd in het Workfront-e-mailadres.

>[!TIP]
>
>De id van een gebruiker zoeken:
>
>1. Klik het **Belangrijkste pictogram van het Menu** ![](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, dan klik **Gebruikers** ![](assets/users-icon-in-main-menu.png).
>
>1. Selecteer de gebruiker.
>
>   De profielpagina van de gebruiker wordt geopend en de gebruiker - identiteitskaart toont in URL.
>
