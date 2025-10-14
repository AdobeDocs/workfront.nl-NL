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
exl-id: fe213fe7-5bb8-479c-926b-761cbdd7ba4e
source-git-commit: 8fe93796b2bc89352ac2c924d6a5e3bf25551ff0
workflow-type: tm+mt
source-wordcount: '946'
ht-degree: 0%

---

# Een pakket voor milieubescherming installeren

Nadat u een pakket hebt gemaakt, kunt u het in een andere omgeving installeren.

U moet een pakket in het milieu installeren dat u voorwerpen **aan** wilt kopiëren. Bijvoorbeeld, als u een project in uw milieu van de Sandbox van de Vernieuwen van de Douane vormt en het bevordert aan uw milieu van de Productie, moet u het pakket in uw milieu van de Productie installeren.

>[!IMPORTANT]
>
>* Als uw Aangepaste vernieuwingssandbox wordt vernieuwd terwijl u een object configureert voor omgevingsbevordering, gaat die configuratie verloren in de update. We raden u aan uw aangepaste vernieuwingssandbox niet te vernieuwen, tenzij alle uitstekende milieupromotieobjecten en -pakketten met succes zijn bevorderd.
>* De voorwerpen die in het doelmilieu als deel van pakketinstallatie worden gecreeerd hebben **niet** zelfde identiteitskaart zoals het voorwerp in het originele milieu. Dit komt doordat id&#39;s door het systeem worden toegewezen wanneer objecten worden gemaakt.

## Toegangsvereisten

U moet het volgende hebben:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plan </strong>
   </td>
   <td> Prime of Ultimate (alleen nieuwe abonnementen)
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

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Vereisten

Er moet een milieubevorderingspakket worden gemaakt voordat het kan worden geïnstalleerd.

Voor instructies, zie [&#x200B; creeer of geef een pakket van de milieubevordering &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md) uit.

## Pakketstatus voor installatie

Een pakket moet de actieve status hebben om in uw productieomgeving te worden geïnstalleerd.

We raden u aan het pakket naar de status TESTING te verplaatsen en in een andere sandbox te installeren om het pakket te testen.  Als deze test zonder fouten is gelukt, verplaatst u het pakket naar ACTIVE om het in de productieomgeving te installeren.

De status van een pakket bewerken:

1. Selecteer het pakket zoals die in [&#x200B; wordt beschreven uitgeven of een bestaand pakket &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md#create-or-edit-an-environment-promotion-package) in het artikel assembleren creeer en geef de pakketten van de milieubevordering uit.
1. Klik **uitgeven Pakket**.
1. Klik **Status**.
1. Selecteer de gewenste status in de keuzelijst.

Voor meer informatie over statussen, zie [&#x200B; Status van de Bevordering van het Milieu &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses) in het artikelOverzicht van het bewegen van voorwerpen tussen de milieu&#39;s van Workfront.

## Een pakket installeren

>[!NOTE]
>
>* Als u een pakket wilt installeren, moet u zijn aangemeld bij de omgeving waarin u het pakket wilt installeren. Dit is het milieu dat u voorwerpen **aan** kopieert.

1. Ga naar de omgeving waarin u het pakket wilt installeren.
1. Klik het **[!UICONTROL Main Menu]** pictogram ![&#x200B; Belangrijkste Menu &#x200B;](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![&#x200B; Belangrijkste Menu &#x200B;](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **[!UICONTROL Setup]** ![&#x200B; pictogram van de Opstelling &#x200B;](/help/_includes/assets/gear-icon-setup.png).
1. Selecteer **Systeem** in de linkernavigatie, dan selecteren **Bevordering van het Milieu**.
1. Selecteer het pakket in de weergegeven lijst.
1. Voor elk voorwerp dat een botsing heeft, selecteer hoe te om de botsing op te lossen.

   Als u een botsing wilt oplossen, klikt u op de vervolgkeuzepijl naast het objecttype en selecteert u de actie die u wilt uitvoeren.

   Voor meer informatie, zie [&#x200B; Toelichtingen &#x200B;](#collisions) in dit artikel
1. Om het pakket in het nieuwe milieu op te stellen, klik **opstellen** bij het hoger-recht van het scherm.

## Botsingdetectie

Een botsing is een voorwerp dat in het doelmilieu van een installatie wordt gevonden die één van de voorwerpen aanpast die van het bronmilieu worden geïnstalleerd. De botsingen worden ontdekt door de namen en IDs van de bronvoorwerpen met voorwerpen in het doelmilieu te vergelijken. De botsingen worden ook ontdekt door bronvoorwerpen met verslagen van eerder geïnstalleerde voorwerpen te vergelijken.

Wanneer een botsing voorkomt, kunt u selecteren hoe te om de botsing op te lossen. De botsingen worden opgelost op het objecten niveau.

U kunt botsingen bekijken door op drop-down naast elk objecten type te klikken. De botsingen worden getoond in de kolom van de Botsing.

>[!NOTE]
>
>De ontdekte botsingen kunnen niet de voorwerpen zijn die u in uw installatie met voeten wilt treden of gebruiken. Wij adviseren het bevestigen van ontdekte botsingen om ervoor te zorgen dat de installatiedoelstellingen correct zijn.

Om een botsing op te lossen, selecteer een actie in de kolom van de Actie van de Plaatsing, of gebruik de standaardactie die reeds wordt getoond.

* **creeer met nieuwe naam**: Creeer een nieuw voorwerp in het doelmilieu. Als het object bestaat in de doelomgeving, kunt u een nieuw object met een nieuwe naam maken. Als het niet bestaat in de doelomgeving, kunt u het object maken met een nieuwe naam of met de naam die het object in het pakket heeft.
* **Gebruik bestaand**: Het voorwerp in het pakket is niet geïnstalleerd, en het voorwerp dat reeds in het doelmilieu bestond is onveranderd.
* **beschrijven**: Het voorwerp in het pakket vervangt het bestaande voorwerp in het doelmilieu.

  U kunt ook objecten kiezen die u wilt overschrijven, zelfs als er geen botsing wordt gedetecteerd.

  Voor details op hoe het beschrijven ouder en kindvoorwerpen beïnvloedt, zie [&#x200B; het Schrijven ouder en kindvoorwerpen &#x200B;](#overwriting-parent-and-child-objects) in dit artikel.
<!--
* Do not use: The object in the package is not installed in the target environment. If you select Do not use, an error message will appear detailing how this choice will affect other objects or fields.
-->

Standaardwaarden zijn `Create new` als het object niet bestaat in de doelomgeving en `Use existing` als het object wel bestaat in de doelomgeving. U kunt aan de standaardafbeelding terugkeren door **Terugstellen aan standaardafbeelding** te klikken.

## Bovenliggende en onderliggende objecten overschrijven

Sommige objecten in je promotiepakket kunnen onderliggende objecten hebben. Een project (ouder) heeft bijvoorbeeld taken (kinderen). Bij het overschrijven van een bovenliggend object worden onderliggende objecten als volgt verwerkt:

* De voorwerpen van het kind die in zowel het pakket als het doel bestaan zullen in het doel worden bijgewerkt om het pakket aan te passen.
* Onderliggende objecten die wel in het pakket staan, maar niet in het doel worden gemaakt.
* Onderliggende objecten die wel in het doel staan, maar niet in het pakket, blijven ongewijzigd.

Deze functionaliteit is van invloed op de volgende bovenliggende en onderliggende objecten:

| Bovenliggend object | Onderliggende objecten |
|---|---|
| Project | Taak <br> QueueDef (de Definitie van de Rij) <br> RoutingRule |
| Sjabloon | TemplateTask <br> QueueDef (de Definitie van de Rij) <br> RoutingRule |
| Parameter (aangepast formulierveld) | ParameterOption (optie Aangepast formulierveld) |
| CalendarInfo | CalendarSection |
| QueueDef (definitie van wachtrij) | QueueTopicGroup <br> QueueTopic |

