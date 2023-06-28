---
filename: manage-fusion-users
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Beheren [!DNL Adobe Workfront Fusion] gebruikers in uw organisatie
description: Beheren [!DNL Adobe Workfront Fusion] gebruikers in uw organisatie
author: Becky
feature: Workfront Fusion
exl-id: fbb858a6-1230-41b4-892a-4ffeb2711922
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 0%

---

# Beheren [!DNL Adobe Workfront Fusion] gebruikers in uw organisatie

[!DNL Adobe Workfront Fusion] beheerders kunnen gebruikersrollen beheren binnen [!DNL Workfront Fusion].

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on adding a user in the Adobe Admin Console:
>
>* See [Add a user to an organization in Adobe Workfront Fusion](../../workfront-fusion/organizations/add-user-to-an-organization.md#create)
>* See the section "Add users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html)
>* Contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront Fusion/Adobe Business Platform)](../../workfront-fusion/fusion-in-admin-console/fusion-adobe-admin-console.md).

-->

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] of hoger</p> </td> 
  </tr> 
   <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
    <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
   </tr>
   <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] licentie**</td> 
   <td>
   <p>Huidige vergunningsvereiste: Nee [!DNL Workfront Fusion] vergunningsvereiste.</p>
   <p>of</p>
   <p>Vereisten voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor arbeidsautomatisering en -integratie],  [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereisten: Als u de [!UICONTROL Select] of [!UICONTROL Prime] [!DNL Adobe Workfront] Abonnement, uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken. [!DNL Workfront Fusion] is opgenomen in de [!UICONTROL Ultimate] [!DNL Workfront] plannen.</p>
   <p>of</p>
   <p>Oudere productvereisten: Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> 
     <p>U moet een [!DNL Workfront Fusion] beheerder van uw organisatie.</p>
     <p>U moet een [!DNL Workfront Fusion] beheerder voor uw team.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Gebruikersrollen weergeven of bewerken {#view}

[!DNL Adobe Workfront Fusion] beheerders kunnen gebruikersrollen weergeven en bijwerken.

1. Tijdens het aanmelden [!DNL Workfront Fusion] beheerder, selecteer **[!UICONTROL Users]** in de linkernavigatie.
1. Klikken **[!UICONTROL Details]** in de rij van de gebruiker die u wilt bekijken.
1. (Optioneel) Als u de rol van de gebruiker wilt bijwerken, klikt u op het vervolgkeuzemenu in het dialoogvenster **[!DNL Role]** kolom in de rij van de organisatie waar u de rol van de gebruiker wilt veranderen, dan selecteer de nieuwe rol.

## Gebruikersgegevens weergeven of bewerken {#view2}

[!DNL Adobe Workfront Fusion] beheerders kunnen gebruikersgegevens weergeven en bijwerken.

1. Tijdens het aanmelden [!DNL Workfront Fusion] beheerder, selecteer **[!UICONTROL Users]** in de linkernavigatie.
1. Klikken **[!UICONTROL Details]** in de rij van de gebruiker die u wilt bekijken.
1. (Optioneel) Klik op **[!UICONTROL Options]** in de rechterbovenhoek van het scherm selecteert u **[!UICONTROL Change Details]**.

## Een gebruiker verwijderen {#delete}

[!DNL Adobe Workfront Fusion] beheerders kunnen gebruikers verwijderen.

1. Tijdens het aanmelden [!DNL Workfront Fusion] beheerder, selecteer [!UICONTROL Users] in de linkernavigatie.
1. Klikken **[!UICONTROL Details]** in de rij van de gebruiker die u wilt bekijken.
1. (Optioneel) Klik op **[!UICONTROL Options]** in de rechterbovenhoek van het scherm selecteert u **[!UICONTROL Delete]**.

### Overwegingen bij het verwijderen van een gebruiker in Workfront Fusion

* Wanneer een gebruiker wordt verwijderd, worden de verbindingen, toetsen en webhaken van de gebruiker verwijderd. Alle scenario&#39;s die bij de gebruiker horen, worden overgedragen aan de eigenaar van de organisatie. De verbindingen in deze scenario&#39;s moeten worden bijgewerkt, omdat de verbindingen die tot de gebruiker behoren niet meer geldig zijn.
* Als de verwijderde gebruiker eigenaar is van toepassingen of openbare sjablonen, worden de toepassingen of openbare sjablonen overgebracht naar de eigenaar van de organisatie. Als er geen organisatieeigenaar is, worden de toepassingen of openbare sjablonen overgebracht naar een andere gebruiker.
