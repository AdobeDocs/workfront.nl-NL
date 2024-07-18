---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Een pakket voor milieubescherming maken of bewerken
description: Het milieu bevorderend vermogen is bedoeld om de capaciteit te verstrekken om op configuratie betrekking hebbende voorwerpen van één milieu aan een andere te bewegen. Leer hoe u een milieupromotiepakket maakt dat u vervolgens in een andere omgeving kunt installeren.
author: Becky
feature: System Setup and Administration
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 0ac8c7df-2d38-4291-861e-52fb5e748537
source-git-commit: 6f5da5ede6bb8c98b26d7d37366670c89ded6c49
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 0%

---

# Een pakket voor milieubescherming maken of bewerken

U moet een pakket in het milieu tot stand brengen dat u voorwerpen **van** wilt kopiëren. Bijvoorbeeld, als u een project in uw milieu vormt van de Sandbox van de Douane verfrist en het aan uw milieu van de Productie bevordert, moet u het pakket in uw milieu van de Sandbox van de Douane creëren vernieuwt.

>[!IMPORTANT]
>
>Als uw Aangepaste vernieuwingssandbox wordt vernieuwd terwijl u een object configureert voor omgevingsbevordering, gaat die configuratie verloren in de update. We raden u aan uw aangepaste vernieuwingssandbox niet te vernieuwen, tenzij alle uitstekende milieupromotieobjecten en -pakketten met succes zijn bevorderd.

## Toegangsvereisten

U moet het volgende hebben:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plan </strong>
   </td>
   <td> Premier of Ultimate (alleen nieuwe plannen)
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licenties </strong>
   </td>
   <td> [!UICONTROL Standard]
   </td>
  </tr>
   <tr>
   <td>Configuraties op toegangsniveau
   </td>
   <td>U moet een [!DNL Workfront] beheerder zijn.
   </td>
  </tr>
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Een pakket maken

1. Ga naar de omgeving waarin u het pakket wilt maken. Dit is het milieu dat u voorwerpen **van** kopieert.
1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **[!UICONTROL Setup]** ![ pictogram van de Opstelling ](/help/_includes/assets/gear-icon-setup.png).
1. Selecteer **Systeem** in de linkernavigatie, dan selecteren **Bevordering van het Milieu**.
1. Klik **Create Pakket**.

   De pagina Nieuw promotiepakket wordt geopend.

1. Op het **gebied van de naam van het Pakket** {, ga een naam voor het pakket in.
1. Op het **gebied van de Beschrijving**, ga een beschrijving voor dit pakket in.
1. Om een voorwerp aan het pakket toe te voegen, klik **voegt Voorwerpen** in de linkernavigatie toe en selecteert het type van voorwerp u wilt toevoegen.
1. Selecteer een of meer objecten in de lijst of typ de naam in de zoekbalk en selecteer het object wanneer het in de lijst wordt weergegeven. U kunt meerdere objecten in de lijst selecteren.
1. Klik **toevoegen (de Voorwerpen van X)** om de geselecteerde voorwerpen aan het pakket toe te voegen.

   >[!INFO]
   >
   >**Voorbeeld**
   >
   >Als u drie projecten hebt geselecteerd om aan het project toe te voegen, zegt de knoop **3 Projecten** toevoegen.

   De objecten die u hebt toegevoegd, worden weergegeven in het gebied Inhoud pakket rechts van de pagina.

1. Herhaal stap 7-9 om een ander type object toe te voegen.
1. (Optioneel) Als u een object uit het pakket wilt verwijderen, beweegt u de muisaanwijzer over het object in het gebied Inhoud pakket en klikt u op de X naast het object.
1. Nadat u alle gewenste voorwerpen aan het pakket hebt toegevoegd, klik **sparen en sluit** om het pakket te bewaren zonder het te assembleren.

   of

   Klik **sparen en assembleren** om het pakket te bewaren en samen te stellen.

   >[!NOTE]
   >
   >* De knoppen Opslaan en Sluiten en Opslaan en Samenstellen zijn beschikbaar als een pakket een naam heeft met vijf of meer tekens en er ten minste één object aan is toegevoegd.
   >* U kunt geen pakket samenstellen dat een installeerbare status heeft, zoals Testen of Actief.

## Een bestaand pakket bewerken of samenvoegen

1. Ga naar de omgeving waarin u het pakket wilt maken. Dit is het milieu dat u voorwerpen **van** kopieert.
1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **[!UICONTROL Setup]** ![ pictogram van de Opstelling ](/help/_includes/assets/gear-icon-setup.png).
1. Selecteer **Systeem** in de linkernavigatie, dan selecteren **Bevordering van het Milieu**.
1. Selecteer het pakket in de weergegeven lijst.
1. (Voorwaardelijk) om gehandicapte pakketten te zien, laat **toe tonen gepensioneerde pakketten** optie.
1. (Facultatief) om de inhoud, met inbegrip van alle voorwerpen en hun sub-voorwerpen te bekijken, klik de drop-down pijl naast het objecten type in de **sectie van de Inhoud**.
1. (Facultatief) om vorige installaties en installatiepogingen van dit pakket te bekijken, klik **Plaatsingen**.
1. (Facultatief) om het pakket uit te geven, klik **uitgeven Pakket** bij het hoger-recht van het scherm.
1. Om het pakket te installeren, klik **installeer** bij het hoger-recht van het scherm.

   Voor instructies bij het installeren van een pakket, zie [ een pakket van de milieubevordering installeren ](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md).
