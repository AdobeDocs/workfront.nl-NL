---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Een pakket voor milieubescherming installeren
description: Het milieu bevorderend vermogen is bedoeld om de capaciteit te verstrekken om op configuratie betrekking hebbende voorwerpen van één milieu aan een andere te bewegen. Leer hoe u een milieupromotiepakket in een doelomgeving installeert.
author: Becky
feature: System Setup and Administration
role: Admin
recommendations: noDisplay, noCatalog
exl-id: fe213fe7-5bb8-479c-926b-761cbdd7ba4e
source-git-commit: d249751b78e9d40fe7a351db14cbf0f3b7c79889
workflow-type: tm+mt
source-wordcount: '852'
ht-degree: 0%

---

# Een pakket voor milieubescherming installeren

Nadat u een pakket hebt gemaakt, kunt u het in een andere omgeving installeren.

U moet een pakket in de omgeving installeren dat u objecten wilt kopiëren **tot**. Bijvoorbeeld, als u een project in uw milieu van de Sandbox van de Vernieuwen van de Douane vormt en het bevordert aan uw milieu van de Productie, moet u het pakket in uw milieu van de Productie installeren.

>[!IMPORTANT]
>
>Als uw Aangepaste vernieuwingssandbox wordt vernieuwd terwijl u een object configureert voor omgevingsbevordering, gaat die configuratie verloren in de update. We raden u aan uw aangepaste vernieuwingssandbox niet te vernieuwen, tenzij alle uitstekende milieupromotieobjecten en -pakketten met succes zijn bevorderd.

## Toegangsvereisten

U moet het volgende hebben:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plan</strong>
   </td>
   <td> Uw organisatie moet zich op het nieuwe prijsmodel bevinden, en een Premier of Ultimate-plan hebben.
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

## Vereisten

Er moet een milieubevorderingspakket worden gemaakt voordat het kan worden geïnstalleerd.

Zie voor instructies [Een pakket voor milieubescherming maken of bewerken](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md).

## Pakketstatus voor installatie

Een pakket moet de actieve status hebben om in uw productieomgeving te worden geïnstalleerd.

We raden u aan het pakket naar de status TESTING te verplaatsen en in een andere sandbox te installeren om het pakket te testen.  Als deze test zonder fouten is gelukt, verplaatst u het pakket naar ACTIVE om het in de productieomgeving te installeren.

De status van een pakket bewerken:

1. Selecteer het pakket zoals beschreven in  [Een bestaand pakket bewerken of samenvoegen](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md#create-or-edit-an-environment-promotion-package) in het artikel Aanmaken en bewerken van pakketten voor milieubescherming.
1. Klikken **Pakket bewerken**.
1. Klikken **Status**.
1. Selecteer de gewenste status in de keuzelijst.

Zie voor meer informatie over statussen [Status van milieubescherming](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses) in het artikel Overzicht van het verplaatsen van objecten tussen Workfront-omgevingen.

## Een pakket installeren

>[!NOTE]
>
>* Als u een pakket wilt installeren, moet u zijn aangemeld bij de omgeving waarin u het pakket wilt installeren. Dit is de omgeving waarin u objecten kopieert **tot**.

1. Ga naar de omgeving waarin u het pakket wilt installeren.
1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront of (indien beschikbaar) op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon-left-nav.png) in de linkerbovenhoek klikt u op **[!UICONTROL Setup]** ![Pictogram Instellen](/help/_includes/assets/gear-icon-setup.png).
1. Selecteren **Systeem** in de linkernavigatie selecteert u vervolgens **Milieubevordering**.
1. Selecteer het pakket in de weergegeven lijst.
1. Voor elk voorwerp dat een botsing heeft, selecteer hoe te om de botsing op te lossen.

   Als u een botsing wilt oplossen, klikt u op de vervolgkeuzepijl naast het objecttype en selecteert u de actie die u wilt uitvoeren.

   Zie voor meer informatie [Botsingdetectie](#collisions) in dit artikel
1. Als u het pakket in de nieuwe omgeving wilt implementeren, klikt u op **Implementeren** rechtsboven in het scherm.

## Botsingdetectie

Er treden botsingen op wanneer een object dat deel uitmaakt van het installatiepakket, dezelfde naam heeft als een object dat al bestaat in de doelomgeving. Wanneer dit voorkomt, kunt u selecteren hoe te om de botsing op te lossen. De botsingen worden opgelost op het objecten niveau.

U kunt botsingen bekijken door op drop-down naast elk objecten type te klikken. De botsingen worden getoond in de kolom van de Botsing.

Om een botsing op te lossen, selecteer een actie in de kolom van de Actie van de Plaatsing, of gebruik de standaardactie die reeds wordt getoond.

* **Maken met nieuwe naam**: Maak een nieuw object in de doelomgeving. Als het object bestaat in de doelomgeving, kunt u een nieuw object met een nieuwe naam maken. Als het niet bestaat in de doelomgeving, kunt u het object maken met een nieuwe naam of met de naam die het object in het pakket heeft.
* **Bestaande gebruiken**: Het object in het pakket is niet geïnstalleerd en het object dat al in de doelomgeving bestond, blijft ongewijzigd.
* **Overschrijven**: Het object in het pakket vervangt het bestaande object in de doelomgeving.

  U kunt ook objecten kiezen die u wilt overschrijven, zelfs als er geen botsing wordt gedetecteerd.

  Zie voor meer informatie over de invloed van overschrijven op bovenliggende en onderliggende objecten [Bovenliggende en onderliggende objecten overschrijven](#overwriting-parent-and-child-objects) in dit artikel.
<!--
* Do not use: The object in the package is not installed in the target environment. If you select Do not use, an error message will appear detailing how this choice will affect other objects or fields.
-->

Standaardwaarden zijn `Create new` als het object niet bestaat in de doelomgeving, en `Use existing` als het object wel bestaat in de doelomgeving. U kunt terugkeren naar de standaardtoewijzing door op **Standaardtoewijzing herstellen**.

## Bovenliggende en onderliggende objecten overschrijven

Sommige objecten in je promotiepakket kunnen onderliggende objecten hebben. Een project (ouder) heeft bijvoorbeeld taken (kinderen). Bij het overschrijven van een bovenliggend object worden onderliggende objecten als volgt verwerkt:

* De voorwerpen van het kind die in zowel het pakket als het doel bestaan zullen in het doel worden bijgewerkt om het pakket aan te passen.
* Onderliggende objecten die wel in het pakket staan, maar niet in het doel worden gemaakt.
* Onderliggende objecten die wel in het doel staan, maar niet in het pakket, blijven ongewijzigd.

Deze functionaliteit is van invloed op de volgende bovenliggende en onderliggende objecten:

| Bovenliggend object | Onderliggende objecten |
|---|---|
| Project | Taak<br>QueueDef (definitie van wachtrij)<br>RoutingRule |
| Sjabloon | TemplateTask<br>QueueDef (definitie van wachtrij)<br>RoutingRule |
| Parameter (aangepast formulierveld) | ParameterOption (optie Aangepast formulierveld) |
| CalendarInfo | CalendarSection |
| QueueDef (definitie van wachtrij) | QueueTopicGroup<br>QueueTopic |

