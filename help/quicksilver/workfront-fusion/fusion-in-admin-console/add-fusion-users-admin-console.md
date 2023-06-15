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
source-git-commit: 392eee3c7b1aacf92d7877f07a8154924f3926a0
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 0%

---

# Gebruikers toevoegen aan [!DNL Adobe Workfront Fusion] via de [!DNL Adobe Admin Console]

>[!IMPORTANT]
>
>De procedures die op deze pagina worden beschreven, gelden alleen voor organisaties die aan [!DNL Adobe Admin Console].
>
>Als uw organisatie nog niet is aangemeld bij de [!DNL Adobe Admin Console], zie [Een gebruiker toevoegen aan een organisatie in [!DNL Adobe Workfront Fusion]](../organizations/add-user-to-an-organization.md).
>
>Voor een lijst met procedures die verschillen, afhankelijk van de vraag of uw organisatie is aangemeld bij de [!DNL Adobe Admin Console], zie [verschillen in toediening op basis van Platforms ([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../fusion-in-admin-console/fusion-adobe-admin-console.md).

U kunt een gebruiker toevoegen aan de [!DNL Adobe Admin Console] en toewijzen aan [!DNL Adobe Workfront Fusion], of een bestaande gebruiker toewijzen in de [!DNL Adobe Admin Console] tot [!DNL Workfront Fusion].

Voor een videobeschrijving [!DNL Workfront Fusion] in de [!DNL Adobe Admin Console], inclusief het toevoegen van gebruikers, raadpleegt u [[!DNL Fusion] op Adobe IMS](https://video.tv.adobe.com/v/3412464/){target=_blank}.

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
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> <p>[!UICONTROL Workfront Fusion for Work Automation] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td> 
  </tr>
   <tr> 
   <td role="rowheader">[!DNL Adobe] beheerdersrechten</td> 
   <td>U moet een [!UICONTROL Product Configuration Administrator] van [!DNL Adobe] producten voor uw organisatie.</td> 
  </tr>
  </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

&#42;&#42;Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md)



## Vereisten

Voordat u de [!DNL Admin Console] for [!DNL Workfront]ontvangt u een e-mail waarin u wordt uitgenodigd naar de console.

1. Als u nog geen ervaring hebt met [!DNL Adobe] en u hebt een e-mail ontvangen met de mededeling dat u nu beheerrechten hebt [!DNL Adobe] software en services voor uw organisatie, klikt u op de knop in de e-mail om een [!DNL Adobe] en open de [!DNL Admin Console].

   of

   Als u al een Adobe-account hebt, gaat u naar de [[!DNL Adobe Admin Console] page](https://adminconsole.adobe.com/).


## Een nieuwe gebruiker toevoegen aan de [!DNL Adobe Admin Console] en [!DNL Workfront Fusion]

1. Van de [[!DNL Adobe Admin Console] page](https://adminconsole.adobe.com/), selecteert u de **[!UICONTROL Products]** in de bovenste navigatiebalk en selecteer vervolgens de optie **[!DNL Workfront Fusion]** productegel.

   ![Fusie in Admin Console](assets/fusion-product-admin-console.png)

1. Selecteer in de lijst die wordt weergegeven de organisatie waaraan u een gebruiker wilt toevoegen.

   ![Fusion-instantie in Admin Console](assets/fusion-instances-admin-console.png)

1. In de lijst die wordt weergegeven, **[!UICONTROL Product Profiles]** geselecteerd, klikt u op de naam van de [!DNL Workfront Fusion] [!UICONTROL Product Profile] koppeling.

   ![Workfront Fusion-productprofiel](../../administration-and-setup/add-users/create-and-manage-users/assets/prod-profile-1.png)

   >[!IMPORTANT]
   >
   > Breng geen wijzigingen aan in de [!UICONTROL Product Profile] zelf.

1. Met de **[!UICONTROL Users]** geselecteerd boven de lijst, klikt u op **[!UICONTROL Add User]**.

1. In de **[!UICONTROL Add users to this product profile]** Voer het e-mailadres of de naam in van een gebruiker die u wilt toevoegen en selecteer vervolgens de gebruiker in de lijst die wordt weergegeven.

1. Klik op **[!UICONTROL Save]**.

   De gebruiker is gemaakt in [!DNL Workfront Fusion].

   <!--
    >[!IMPORTANT]
    >
    > Do not make any changes to the Product Profile itself.
    -->

1. (Optioneel) Doorgaan naar [Wijzig het toegangsniveau van een gebruiker in [!DNL Workfront Fusion]](#change-a-users-access-level-in-workfront-fusion)

## Het toegangsniveau van een gebruiker wijzigen in Workfront Fusion

### De rol van een gebruiker wijzigen in Beheerder

Een gebruiker een beheerdersrol geven moet worden uitgevoerd in het dialoogvenster [!DNL Adobe Admin Console].

1. Op de [!DNL Workfront Fusion] [!UICONTROL Product Profile] pagina waar u de gebruiker hebt toegevoegd, selecteert u de **[!UICONTROL Admins]** tab.

1. Klik op **[!UICONTROL Add Admin]**.

1. In de **[!UICONTROL Add product profile administrators]** Voer het e-mailadres of de naam in van een gebruiker die u wilt toevoegen en selecteer vervolgens de gebruiker in de lijst die wordt weergegeven.

1. Klik op **[!UICONTROL Save]**.

   Deze gebruiker is nu beheerder in [!DNL Workfront Fusion].

### De rol van een gebruiker wijzigen in [!UICONTROL Member], [!UICONTROL Accountant], of [!UICONTROL App Developer].

[!UICONTROL Member], [!UICONTROL Accountant], en [!UICONTROL App Developer] rollen worden verwerkt binnen [!DNL Workfront Fusion].

Zie voor instructies [Gebruikersrollen weergeven of bewerken](../organizations/manage-fusion-users.md#view-or-edit-user-roles) in het artikel [Beheren [!DNL Adobe Workfront Fusion] gebruikers in uw organisatie](../organizations/manage-fusion-users.md)

## Bestaande gebruikers toewijzen in het dialoogvenster [!DNL Adobe Admin Console] tot [!DNL Workfront Fusion]

1. Beginnen met het bewerken van de gebruiker zoals wordt beschreven in de sectie &quot;Gebruikersdetails bewerken&quot; van het artikel [Gebruikers individueel beheren](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) in de [!DNL Adobe Admin Console] documentatie.

1. Toevoegen **[!DNL Adobe Workfront Fusion]** aan de producten die aan de gebruiker zijn toegewezen.
