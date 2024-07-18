---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Gebruikers aan Adobe Workfront Fusion toevoegen via de Adobe Admin Console
description: U kunt een gebruiker toevoegen aan de Adobe Admin Console en deze toewijzen aan Adobe Workfront Fusion, of een bestaande gebruiker in de Adobe Admin Console toewijzen aan Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: c8924e00-1154-4cf8-84e8-472251b5fc28
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# Voeg gebruikers toe aan [!DNL Adobe Workfront Fusion] door [!DNL Adobe Admin Console]

>[!IMPORTANT]
>
>De procedures die op deze pagina worden beschreven, gelden alleen voor organisaties die aan de [!DNL Adobe Admin Console] zijn toegevoegd.
>
>Als uw organisatie nog niet aan [!DNL Adobe Admin Console] is bezet, zie [ een gebruiker aan een organisatie binnen  [!DNL Adobe Workfront Fusion]](../organizations/add-user-to-an-organization.md) toevoegen.
>
>Voor een lijst van procedures die verschillen gebaseerd op of uw organisatie aan [!DNL Adobe Admin Console] is genegeerd, zie [ Op platform-gebaseerde beleidsverschillen ([!DNL Adobe Workfront Fusion]/ [!DNL Adobe Business Platform]) ](../fusion-in-admin-console/fusion-adobe-admin-console.md).

U kunt een gebruiker aan [!DNL Adobe Admin Console] toevoegen en hen toewijzen aan [!DNL Adobe Workfront Fusion], of een bestaande gebruiker in [!DNL Adobe Admin Console] toewijzen aan [!DNL Workfront Fusion].

Voor video beschrijvend [!DNL Workfront Fusion] in [!DNL Adobe Admin Console], met inbegrip van hoe te om gebruikers toe te voegen, zie [[!DNL Fusion]  op Adobe IMS ](https://video.tv.adobe.com/v/3412464/){target=_blank}.

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] of hoger</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licentie**</td> 
   <td>
   <p>Huidige licentievereiste: geen [!DNL Workfront Fusion] licentievereiste.</p>
   <p>of</p>
   <p>Vereiste voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en integratie] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereiste: als u het [!UICONTROL Select] - of [!UICONTROL Prime] [!DNL Adobe Workfront] -abonnement hebt, moet uw organisatie [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken. [!DNL Workfront Fusion] wordt opgenomen in het [!UICONTROL Ultimate] [!DNL Workfront] -abonnement.</p>
   <p>of</p>
   <p>Vereiste verouderd product: uw organisatie moet [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken.</p>
   </td> 
  </tr>
   <tr> 
   <td role="rowheader">[!DNL Adobe] beheerdersrechten</td> 
   <td>U moet een [!UICONTROL Product Configuration Administrator] van [!DNL Adobe] producten voor uw organisatie zijn.</td> 
  </tr>
  </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw [!DNL Workfront] beheerder.

&#42;&#42; voor informatie over [!DNL Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen ](../../workfront-fusion/get-started/license-automation-vs-integration.md)



## Vereisten

Voordat u [!DNL Admin Console] for [!DNL Workfront] gebruikt, ontvangt u een e-mail waarin u wordt uitgenodigd naar de console.

1. Als u [!DNL Adobe] nog niet eerder hebt gebruikt en u een e-mail hebt ontvangen waarin u wordt gemeld dat u nu beheerrechten hebt voor [!DNL Adobe] -software en -services voor uw organisatie, klikt u op de knop in de e-mail om een [!DNL Adobe] -account te maken en opent u [!DNL Admin Console] .

   of

   Als u reeds een rekening van de Adobe hebt, ga naar de [[!DNL Adobe Admin Console]  pagina ](https://adminconsole.adobe.com/).


## Een nieuwe gebruiker toevoegen aan de [!DNL Adobe Admin Console] en [!DNL Workfront Fusion]

1. Van de [[!DNL Adobe Admin Console]  pagina ](https://adminconsole.adobe.com/), selecteer het **[!UICONTROL Products]** lusje in de hoogste navigatiebar, en selecteer dan de **[!DNL Workfront Fusion]** producttegel.

   ![ Fusie in Admin Console ](assets/fusion-product-admin-console.png)

1. Selecteer in de lijst die wordt weergegeven de organisatie waaraan u een gebruiker wilt toevoegen.

   ![ instantie van de Fusie in Admin Console ](assets/fusion-instances-admin-console.png)

1. Klik in de lijst die wordt weergegeven met de tab **[!UICONTROL Product Profiles]** geselecteerd op de naam van de koppeling [!DNL Workfront Fusion] [!UICONTROL Product Profile] .

   ![ het Profiel van het Product van de Fusie van Workfront ](../../administration-and-setup/add-users/create-and-manage-users/assets/prod-profile-1.png)

   >[!IMPORTANT]
   >
   > Breng geen wijzigingen aan in de [!UICONTROL Product Profile] zelf.

1. Selecteer de tab **[!UICONTROL Users]** boven de lijst en klik op **[!UICONTROL Add User]** .

1. Voer in het vak **[!UICONTROL Add users to this product profile]** het e-mailadres of de naam in van de gebruiker die u wilt toevoegen en selecteer vervolgens de gebruiker in de lijst die wordt weergegeven.

1. Klik op **[!UICONTROL Save]**.

   De gebruiker wordt gemaakt in [!DNL Workfront Fusion] .

   <!--
    >[!IMPORTANT]
    >
    > Do not make any changes to the Product Profile itself.
    -->

1. (Optioneel) Ga door met [ Wijzig het toegangsniveau van een gebruiker in  [!DNL Workfront Fusion]](#change-a-users-access-level-in-workfront-fusion)

## Het toegangsniveau van een gebruiker wijzigen in Workfront Fusion

### De rol van een gebruiker wijzigen in Beheerder

Het geven van een gebruiker een Admin rol moet in [!DNL Adobe Admin Console] worden gedaan.

1. Selecteer de tab **[!UICONTROL Admins]** op de pagina [!DNL Workfront Fusion] [!UICONTROL Product Profile] waaraan u de gebruiker hebt toegevoegd.

1. Klik op **[!UICONTROL Add Admin]**.

1. Voer in het vak **[!UICONTROL Add product profile administrators]** het e-mailadres of de naam in van de gebruiker die u wilt toevoegen en selecteer vervolgens de gebruiker in de lijst die wordt weergegeven.

1. Klik op **[!UICONTROL Save]**.

   Deze gebruiker is nu Beheerder in [!DNL Workfront Fusion].

### Wijzig de rol van een gebruiker in [!UICONTROL Member] , [!UICONTROL Accountant] of [!UICONTROL App Developer] .

[!UICONTROL Member] -, [!UICONTROL Accountant] - en [!UICONTROL App Developer] -rollen worden binnen [!DNL Workfront Fusion] verwerkt.

Voor instructies, zie [ Mening of geef gebruikersrollen ](../organizations/manage-fusion-users.md#view-or-edit-user-roles) in artikel [ uit leidt  [!DNL Adobe Workfront Fusion]  gebruikers in uw organisatie ](../organizations/manage-fusion-users.md)

## Bestaande gebruikers toewijzen in de [!DNL Adobe Admin Console] aan [!DNL Workfront Fusion]

1. Begin het uitgeven van de gebruiker zoals die in de &quot;uitgeef gebruikersdetails&quot;sectie van het artikel [ wordt beschreven individuele gebruikers ](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) in de [!DNL Adobe Admin Console] documentatie leidt.

1. Voeg **[!DNL Adobe Workfront Fusion]** toe aan de producten die aan de gebruiker zijn toegewezen.
