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
exl-id: 0ac8c7df-2d38-4291-861e-52fb5e748537
source-git-commit: 7ca27795ec115a112acb55113bfade4a5fee15ad
workflow-type: tm+mt
source-wordcount: '782'
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
   <td>Adobe Workfront-pakket
   </td>
   <td> <p>Prime of Ultimate</p>
   </td>
  </tr>
  <tr>
   <td><strong> de vergunningen van Workfront </strong>
   </td>
   <td> <p>Standard</p>&gt;
   </td>
  </tr>
   <tr>
   <td>Configuraties op toegangsniveau
   </td>
   <td><p>U moet een Workfront-beheerder zijn.</p>
   </td>
  </tr>
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Een pakket maken

1. Ga naar de omgeving waarin u het pakket wilt maken. Dit is het milieu dat u voorwerpen **van** kopieert.
1. Klik het **[!UICONTROL Main Menu]** pictogram ![&#x200B; Belangrijkste Menu &#x200B;](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![&#x200B; Belangrijkste Menu &#x200B;](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **[!UICONTROL Setup]** ![&#x200B; pictogram van de Opstelling &#x200B;](/help/_includes/assets/gear-icon-setup.png).
1. Selecteer **Systeem** in de linkernavigatie, dan selecteren **Bevordering van het Milieu**.
1. Klik **Create Pakket**.

   De pagina Nieuw promotiepakket wordt geopend.

1. Op het **gebied van de naam van het Pakket** &lbrace;, ga een naam voor het pakket in.
1. Op het **gebied van de Beschrijving**, ga een beschrijving voor dit pakket in.
1. Als u een object aan het pakket wilt toevoegen, selecteert u in de linkernavigatie het type object dat u wilt toevoegen.
1. Selecteer een of meer objecten in de lijst die wordt weergegeven of typ de naam in de zoekbalk en selecteer het object wanneer dit in de lijst wordt weergegeven. U kunt meerdere objecten in de lijst selecteren.

   De lijst bevat maximaal 500 objecten van het geselecteerde objecttype. Als u een object wilt zoeken dat niet in de lijst voorkomt, gebruikt u de zoekbalk.
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

Een pakket moet de status `DRAFT` hebben om te kunnen worden bewerkt.

1. Ga naar de omgeving waarin u het pakket wilt bewerken. Dit is de omgeving waarin het pakket oorspronkelijk is gemaakt.
1. Klik het **[!UICONTROL Main Menu]** pictogram ![&#x200B; Belangrijkste Menu &#x200B;](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![&#x200B; Belangrijkste Menu &#x200B;](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **[!UICONTROL Setup]** ![&#x200B; pictogram van de Opstelling &#x200B;](/help/_includes/assets/gear-icon-setup.png).
1. Selecteer **Systeem** in de linkernavigatie, dan selecteren **Bevordering van het Milieu**.
1. Selecteer het pakket in de weergegeven lijst.
1. (Voorwaardelijk) om gehandicapte pakketten te zien, laat **toe tonen gepensioneerde pakketten** optie.
1. (Facultatief) om de inhoud, met inbegrip van alle voorwerpen en hun sub-voorwerpen te bekijken, klik de drop-down pijl naast het objecten type in de **sectie van de Inhoud**.
1. (Facultatief) om vorige installaties en installatiepogingen van dit pakket te bekijken, klik **Plaatsingen**.
1. (Facultatief) om het pakket uit te geven, klik **uitgeven Pakket** bij het hoger-recht van het scherm.
Een pakket moet de status `DRAFT` hebben om te kunnen worden bewerkt. Om het pakket aan `DRAFT` status, op het **2&rbrace; gebied van de Status te bewegen &lbrace;, selecteer**. `Draft` U kunt het pakket vervolgens blijven bewerken.
1. Om het pakket te installeren, klik **installeer** bij het hoger-recht van het scherm.

   Voor instructies bij het installeren van een pakket, zie [&#x200B; een pakket van de milieubevordering installeren &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md).

## Een pakket maken op basis van een objectvergelijking

U kunt een pakket rechtstreeks op basis van een objectvergelijking maken.

1. Creeer een objecten vergelijking, zoals die in [&#x200B; wordt beschreven vergelijkt voorwerpen tussen milieu&#39;s &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-compare.md).
1. Selecteer in de gegenereerde vergelijking de objecten die u in het pakket wilt opnemen.
1. Klik **creeer pakket** in de hoger-juiste hoek van het scherm.
1. Voer een naam en beschrijving in voor het pakket.
1. Klik **creeer pakket** in het Create pakketvenster.

   Het pakket wordt gegenereerd.
