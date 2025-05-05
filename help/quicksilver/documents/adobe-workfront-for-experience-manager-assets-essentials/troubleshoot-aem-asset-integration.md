---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Problemen met de integratie met Adobe Experience Manager oplossen
description: 'Probleem: Assets wordt niet opgeslagen naar Adobe Experience Manager'
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: f7e31e20-01e3-462d-9020-005e155f0259
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# Problemen met Adobe Experience Manager-integratie oplossen

## Probleem: Assets wordt niet opgeslagen naar Adobe Experience Manager

Wanneer een gebruiker een middel of een omslag selecteert om naar Experience Manager Assets uit te voeren en Uitgezocht klikt, sluit het selecteurenvenster maar de activa worden niet bewaard aan Experience Manager Assets. Er zijn in Workfront geen aanwijzingen dat de activa niet aan Experience Manager Assets zijn opgeslagen.

### Oorzaak

Dit kan door de lijst van gewenste personen in Adobe Cloud Manager gebeuren. Als de Adobe Cloud Manager-lijst van gewenste personen voor een organisatie leeg is, zijn IP-adressen niet beperkt en heeft Workfront toegang tot de mappen en middelen van de organisatie in Adobe Experience Manager. Nochtans, als zelfs één enkel IP adres aan de lijst van gewenste personen van Cloud Manager wordt toegevoegd, dan veronderstelt de lijst van gewenste personen dat om het even welk IP adres niet op de lijst wordt toegestaan. Daarom als de lijst van gewenste personen van Cloud Manager om het even welke IP adressen omvat, moeten de adressen van Workfront IP ook aan de lijst van gewenste personen worden toegevoegd om Workfront toe te laten om activa naar Experience Manager Assets te verzenden.

### Oplossing:

Voeg de Workfront IP adressen aan de lijst van gewenste personen van Cloud Manager van Adobe toe.

* Voor instructies bij het toevoegen van IP adressen aan uw Adobe Cloud Manager, zie [ Inleiding aan IP Lijsten van gewenste personen ](https://experienceleague.adobe.com/nl/docs/experience-manager-cloud-service/content/implementing/using-cloud-manager/ip-allow-lists/introduction) in de documentatie van Adobe Experience Manager.
* Voor een lijst van Workfront IP adressen om aan de lijst van gewenste personen toe te voegen, zie [ uw firewall ](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md) vormen.
