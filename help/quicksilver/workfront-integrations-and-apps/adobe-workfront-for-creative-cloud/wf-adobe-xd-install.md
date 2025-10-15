---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Adobe Workfront voor XD installeren en openen
description: U kunt de Adobe Workfront for XD-insteekmodule installeren vanaf de Adobe Marketplace.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: d4971977-b5bd-4bb4-a1c2-44829a67d32d
source-git-commit: a65a4568c6428768ee6bc60a59a8499efdbec9f8
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 0%

---

# Installeren en openen [!DNL Adobe Workfront for XD]

U kunt de plug-in [!DNL Adobe Workfront for XD] installeren vanaf de Adobe Marketplace. De plug-in ondersteunt de volgende talen:

* Engels
* Frans
* Duits
* Italiaans
* Spaans
* Portugees
* Japans
* Vereenvoudigd Chinees
* Traditioneel Chinees
* Koreaans

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
 <!-- <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] package/td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td>
   <p>Standard</p>
    <p>Work or higher</p> </td> 
  </tr> -->
  <tr> 
   <td role="rowheader">Aanvullende producten</td> 
   <td><p>U moet een [!DNL Adobe Creative Cloud] licentie hebben naast een [!DNL Workfront] licentie.</p></td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

* U moet de [!DNL Adobe XD] -toepassing installeren voordat u de Workfront-insteekmodule installeert.

## Installeer de [!DNL Adobe Workfront for XD] -plug-in voor uw organisatie

Als u een [!DNL Adobe Admin Console] -beheerder bent, kunt u de plug-in opnemen in [!DNL Creative Cloud] -implementatiepakketten. Voor meer informatie, zie [ Including steekmodules in uw pakket ](https://helpx.adobe.com/in/enterprise/using/manage-extensions.html).

[ Mening hier een videoleerprogramma ](https://www.youtube.com/watch?v=zzvXNLIBzrc){target=_blank}.

[!DNL Adobe Admin Console] -beheerders kunnen ook pakketten met alleen plug-ins maken voor distributie naar gebruikers. Voor meer informatie, zie [ [!UICONTROL [!DNL Adobe Workfront] creëren voor  [!DNL Creative Cloud]]  pakketten voor uw gebruikers in  [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/configure-integrations/create-plugin-only-packages.md)

## De [!DNL Adobe Workfront for XD] -plug-in afzonderlijk installeren

U kunt de [!DNL Adobe Workfront for XD] -insteekmodule voor uzelf installeren vanuit de [!DNL Adobe Exchange] .

1. Ga naar [ Adobe Workfront voor XD installeert pagina ](https://exchange.adobe.com/apps/cc/4c3566f9?pluginId=4c3566f9&workflow=share) op Adobe Exchange.
1. In de dialoog die verschijnt, klik **Open [!DNL Adobe Creative Cloud] Desktop app**.
1. Klik op [!DNL Adobe XD] als **[!UICONTROL Install]** Plug-inbeheer wordt geopend.
1. Lees de informatie in het dialoogvenster en klik op **[!UICONTROL OK]** .
1. Ga naar de volgende sectie voor informatie over het openen van de plug-in.

## De plug-in [!DNL Adobe Workfront for XD] openen

1. Open [!DNL Adobe XD].

1. Maak een nieuw bestand of open een bestaand bestand.

1. In de bodem-linkerhoek, klik het **Plugins** pictogram.

![ XD plugin venster ](assets/xd-plugin-window-350x620.png)

1. Zoek **[!UICONTROL Plugins Panel]** in de **[!UICONTROL Adobe Workfront for XD]** .

1. Ga naar de volgende sectie voor informatie over hoe u zich aanmeldt bij de plug-in.

## Aanmelden bij [!DNL Adobe Workfront for XD]

1. Zorg ervoor dat het deelvenster Insteekmodule is geopend en klik op **[!DNL Adobe Workfront for XD]** .
1. Voer uw domein in en klik op **[!UICONTROL Log in]** . Er wordt een browserpagina geopend.

   >[!TIP]
   >
   >* Als u uw domein wilt zoeken, opent u een browser, navigeert u naar de instantie [!DNL Workfront] en kopieert u het eerste deel van de URL:\
   >![ plaats van domein ](assets/domain-350x50.png)
   >
   > * Als uw Workfront-exemplaar is geïntegreerd met Experience Cloud, vraagt u uw beheerder om het Workfront-domein dat u kunt vinden onder Product > Workfront in de Admin Console.

1. Voer in de browser uw [!DNL Workfront] -gegevens in en klik op **[!DNL Log in]** . Als uw bedrijf één enkel teken-op (SSO) gebruikt, zult u aan de pagina van uw leverancier worden geleid SSO om zich aan te melden.

   >[!NOTE]
   >
   >Mogelijk wordt u niet gevraagd om uw [!DNL Workfront] -referenties in te voeren als u zich onlangs hebt aangemeld.

   Volg de aanwijzingen om u aan te melden bij [!DNL Workfront] .

   >[!NOTE]
   >
   >* [!DNL Workfront] maakt verbinding met [!DNL Adobe Creative Cloud] via OAuth 2.0, een veilige standaard die door de meeste webgebaseerde integraties wordt gebruikt voor de verificatie en autorisatie van gebruikers.
   >* Wanneer u wordt ertoe aangezet om het [ domein of de gastheer ] van uw [!DNL Workfront] rekening in te gaan, typ het gebruikend dit formaat: *yourCompany&#39;sDomain.my.workfront.com*. Het domein van uw bedrijf is gewoonlijk de naam van uw bedrijf.

1. Klik op **[!UICONTROL Allow Access]** om uw aanmelding te voltooien en ga terug naar [!DNL Adobe XD] om uw werk te bekijken.

### Problemen met aanmeldingsfouten oplossen

**Er is iets fout gegaan en er wordt een fout weergegeven bij het aanmelden**


U kunt een URL die begint met `experience.adobe.com` niet gebruiken om u aan te melden bij de plug-in.

![ login fout ](assets/plugin-log-in-error.png) ![ domein ](assets/incorrect-domain.png)


U kunt dit probleem als volgt oplossen:

1. Verwijder de Adobe Workfront for XD-plug-in en installeer deze opnieuw om het domein en de fout te wissen.

1. Voer uw Workfront-domein in. Het domein moet `company-name.my.workfront.com` zijn en niet `experience.adobe.com`.

Ga naar
