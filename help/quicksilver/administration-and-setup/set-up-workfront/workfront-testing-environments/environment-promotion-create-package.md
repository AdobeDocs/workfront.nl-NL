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

U moet in de omgeving een pakket maken dat u objecten wilt kopiëren **van**. Bijvoorbeeld, als u een project in uw milieu vormt van de Sandbox van de Douane verfrist en het aan uw milieu van de Productie bevordert, moet u het pakket in uw milieu van de Sandbox van de Douane creëren vernieuwt.

>[!IMPORTANT]
>
>Als uw Aangepaste vernieuwingssandbox wordt vernieuwd terwijl u een object configureert voor omgevingsbevordering, gaat die configuratie verloren in de update. We raden u aan uw aangepaste vernieuwingssandbox niet te vernieuwen, tenzij alle uitstekende milieupromotieobjecten en -pakketten met succes zijn bevorderd.

## Toegangsvereisten

U moet het volgende hebben:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plan</strong>
   </td>
   <td> Premier of Ultimate (alleen nieuwe plannen)
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licenties</strong>
   </td>
   <td> [!UICONTROL Standard]
   </td>
  </tr>
   <tr>
   <td>Configuraties op toegangsniveau
   </td>
   <td>U moet een [!DNL Workfront] beheerder.
   </td>
  </tr>
</table>

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Een pakket maken

1. Ga naar de omgeving waarin u het pakket wilt maken. Dit is de omgeving waarin u objecten kopieert **van**.
1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront of (indien beschikbaar) op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon-left-nav.png) in de linkerbovenhoek klikt u op **[!UICONTROL Setup]** ![Pictogram Instellen](/help/_includes/assets/gear-icon-setup.png).
1. Selecteren **Systeem** in de linkernavigatie selecteert u vervolgens **Milieubevordering**.
1. Klikken **Pakket maken**.

   De pagina Nieuw promotiepakket wordt geopend.

1. In de **Pakketnaam** voert u een naam in voor het pakket.
1. In de **Beschrijving** Voer een beschrijving in voor dit pakket.
1. Als u een object aan het pakket wilt toevoegen, klikt u op **Objecten toevoegen** in de linkernavigatie en selecteer het type van voorwerp u wilt toevoegen.
1. Selecteer een of meer objecten in de lijst of typ de naam in de zoekbalk en selecteer het object wanneer het in de lijst wordt weergegeven. U kunt meerdere objecten in de lijst selecteren.
1. Klikken **Toevoegen (X-objecten)** om de geselecteerde objecten aan het pakket toe te voegen.

   >[!INFO]
   >
   >**Voorbeeld**
   >
   >Als u drie projecten hebt geselecteerd om aan het project toe te voegen, zegt de knoop **3 projecten toevoegen**.

   De objecten die u hebt toegevoegd, worden weergegeven in het gebied Inhoud pakket rechts van de pagina.

1. Herhaal stap 7-9 om een ander type object toe te voegen.
1. (Optioneel) Als u een object uit het pakket wilt verwijderen, beweegt u de muisaanwijzer over het object in het gebied Inhoud pakket en klikt u op de X naast het object.
1. Nadat u alle gewenste objecten aan het pakket hebt toegevoegd, klikt u **Opslaan en sluiten** om het pakket op te slaan zonder het samen te stellen.

   of

   Klikken **Opslaan en samenstellen** om het pakket op te slaan en samen te stellen.

   >[!NOTE]
   >
   >* De knoppen Opslaan en Sluiten en Opslaan en Samenstellen zijn beschikbaar als een pakket een naam heeft met vijf of meer tekens en er ten minste één object aan is toegevoegd.
   >* U kunt geen pakket samenstellen dat een installeerbare status heeft, zoals Testen of Actief.

## Een bestaand pakket bewerken of samenvoegen

1. Ga naar de omgeving waarin u het pakket wilt maken. Dit is de omgeving waarin u objecten kopieert **van**.
1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront of (indien beschikbaar) op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon-left-nav.png) in de linkerbovenhoek klikt u op **[!UICONTROL Setup]** ![Pictogram Instellen](/help/_includes/assets/gear-icon-setup.png).
1. Selecteren **Systeem** in de linkernavigatie selecteert u vervolgens **Milieubevordering**.
1. Selecteer het pakket in de weergegeven lijst.
1. (Voorwaardelijk) Schakel de optie **Gecodeerde pakketten tonen** -optie.
1. (Optioneel) Als u de inhoud wilt weergeven, inclusief alle objecten en de bijbehorende subobjecten, klikt u op de vervolgkeuzepijl naast het objecttype in het dialoogvenster **Inhoud** sectie.
1. (Optioneel) Klik op **Inzet**.
1. (Optioneel) Klik op **Pakket bewerken** rechtsboven in het scherm.
1. Klik op **Installeren** rechtsboven in het scherm.

   Zie voor instructies over het installeren van een pakket [Een pakket voor milieubescherming installeren](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md).
