---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Een milieubevorderingspakket terugdraaien
description: Het milieu bevorderend vermogen is bedoeld om de capaciteit te verstrekken om op configuratie betrekking hebbende voorwerpen van één milieu aan een andere te bewegen. Leer hoe u een geïnstalleerd promotiepakket kunt terugdraaien vanuit een doelomgeving.
author: Becky
feature: System Setup and Administration
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 70f7e2a8-bb27-4546-afb7-53e0eec30bf1
source-git-commit: 7e15301dae4b761d19c85a3581bfdb4540ed40fd
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Een milieubevorderingspakket terugdraaien



Nadat u een pakket hebt geïnstalleerd, kunt u het terugdraaien. Hiermee verwijdert u de wijzigingen die het pakket in de doelomgeving heeft aangebracht en herstelt u de betrokken objecten in hun vorige configuraties.

Je kunt een promotiepakket binnen 24 uur na de installatie terugdraaien. Na 24 uur is de terugdraaifunctionaliteit niet meer beschikbaar voor die installatie.

## Toegangsvereisten

U moet het volgende hebben:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plan </strong>
   </td>
   <td> <p>Nieuw: Premier of Ultimate</p><p>of</p><p>Huidig: Niet beschikbaar</p>
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licenties </strong>
   </td>
   <td> <p>[!UICONTROL Standard]</p><p>of</p><p>Huidig: Niet beschikbaar</p>
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

* Een milieubevorderingspakket moet worden geïnstalleerd alvorens het kan worden teruggedraaid.

  Voor instructies, zie [&#x200B; een pakket van de milieubevordering installeren &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md).


## Bepalen of een specifieke pakketimplementatie kan worden teruggedraaid

Om te weten of een specifieke pakketplaatsing kan worden teruggedraaid, overweeg het volgende:

* Minder dan 24 uur moet zijn verstreken sinds de verpakking is geïnstalleerd.
* Alleen de meest recente pakketimplementatie kan worden teruggedraaid.
* Een mislukte implementatie kan worden teruggedraaid.
* Terugdraaiversies zijn niet mogelijk.


## Een geïnstalleerd pakket voor milieubescherming terugdraaien

1. Ga naar de omgeving waarin het pakket is geïnstalleerd.
1. Klik het **[!UICONTROL Main Menu]** pictogram ![&#x200B; Belangrijkste Menu &#x200B;](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![&#x200B; Belangrijkste Menu &#x200B;](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **[!UICONTROL Setup]** ![&#x200B; pictogram van de Opstelling &#x200B;](/help/_includes/assets/gear-icon-setup.png).
1. Selecteer **Bevordering van het Milieu** in de linkernavigatie.
1. Selecteer het pakket dat u terug wilt rollen, en **Plaatsingen** klikken.
1. Houd de muis boven de implementatie (installatie) die u wilt terugdraaien en klik vervolgens op Terugdraaien wanneer deze rechts van de regel van die implementatie wordt weergegeven.

   of

   Klik op de plaatsing die u terug wilt rollen, dan **het pakket van de Terugdraaiing** in de hoger-juiste hoek van het scherm klikken.

   >[!IMPORTANT]
   >
   >De implementatie moet minder dan 24 uur hebben plaatsgevonden voordat u de toepassing terugdraait. Installaties die ouder zijn dan 24 uur kunnen niet worden teruggedraaid.

1. (Optioneel) In het gedeelte Voorvertoning terugdraaien kunt u de wijzigingen bekijken die optreden wanneer de implementatie wordt teruggedraaid.
1. Klik **Terugrol** in de hoger-juiste hoek van het scherm.
