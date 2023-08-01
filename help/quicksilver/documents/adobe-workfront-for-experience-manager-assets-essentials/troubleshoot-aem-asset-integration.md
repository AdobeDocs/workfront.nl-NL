---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Problemen met de integratie met Adobe Experience Manager oplossen
description: Sluit uw werk aan op uw inhoud in Experience Manager Assets Essentials - BEWERK ME.
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
source-git-commit: e4bf79b8c5d53870aec6d415510acccb53a5c7f6
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# Problemen met Adobe Experience Manager-integratie oplossen

## Probleem: middelen worden niet opgeslagen naar Adobe Experience Manager

Wanneer een gebruiker een middel of een omslag selecteert om naar Experience Manager Assets uit te voeren en Uitgezocht klikt, sluit het selecteurenvenster maar de activa worden niet bewaard aan Experience Manager Assets. Er zijn in Workfront geen aanwijzingen dat de activa niet aan Experience Manager Assets zijn opgeslagen.

### Oorzaak

Dit kan gebeuren vanwege de lijst van gewenste personen in Adobe Cloud Manager. Als de Adobe Cloud Manager-lijst van gewenste personen voor een organisatie leeg is, zijn de IP-adressen niet beperkt en heeft Workfront toegang tot de mappen en middelen van de organisatie in Adobe Experience Manager. Nochtans, als zelfs één enkel IP adres aan de lijst van gewenste personen van de Manager van de Wolk wordt toegevoegd, dan veronderstelt de lijst van gewenste personen dat om het even welk IP adres niet op de lijst wordt toegestaan. Daarom als de lijst van gewenste personen van de Manager van de Wolk om het even welke IP adressen omvat, moeten de adressen van Workfront IP ook aan de lijst van gewenste personen worden toegevoegd om Workfront toe te laten om activa naar Experience Manager Assets te verzenden.

### Oplossing:

Voeg de Workfront IP-adressen toe aan de lijst van gewenste personen Adobe Cloud Manager.

* Ga voor instructies over het toevoegen van IP-adressen aan uw Adobe Cloud Manager naar [Inleiding aan IP Lijsten van gewenste personen](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/using-cloud-manager/ip-allow-lists/introduction.html?lang=en) in de documentatie van Adobe Experience Manager.
* Voor een lijst van Workfront IP adressen om aan de lijst van gewenste personen toe te voegen, zie [Uw firewall configureren](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md).


