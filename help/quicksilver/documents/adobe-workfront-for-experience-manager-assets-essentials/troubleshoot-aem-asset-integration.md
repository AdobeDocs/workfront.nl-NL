---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Problemen met de integratie met Adobe Experience Manager oplossen
description: 'Probleem: Assets wordt niet opgeslagen naar Adobe Experience Manager'
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: f7e31e20-01e3-462d-9020-005e155f0259
source-git-commit: abb021a6857f8016d4f8b6bcf99fe818e47faea6
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# Problemen met Adobe Experience Manager-integratie oplossen

## Probleem: Assets wordt niet opgeslagen naar Adobe Experience Manager

Wanneer een gebruiker een middel of een omslag selecteert om naar Experience Manager Assets uit te voeren en Uitgezocht klikt, sluit het selecteurenvenster maar de activa worden niet bewaard aan Experience Manager Assets. Er zijn in Workfront geen aanwijzingen dat de activa niet aan Experience Manager Assets zijn opgeslagen.

### Oorzaak

Dit kan gebeuren als gevolg van de lijst van gewenste personen in Adobe Cloud Manager. Als de lijst van gewenste personen van Cloud Manager van de Adobe voor een organisatie leeg is, dan zijn IP adressen niet beperkt, en Workfront kan tot de omslagen en de activa van de organisatie in Adobe Experience Manager toegang hebben. Nochtans, als zelfs één enkel IP adres aan de lijst van gewenste personen van Cloud Manager wordt toegevoegd, dan veronderstelt de lijst van gewenste personen dat om het even welk IP adres niet op de lijst wordt toegestaan. Daarom als de lijst van gewenste personen van Cloud Manager om het even welke IP adressen omvat, moeten de adressen van Workfront IP ook aan de lijst van gewenste personen worden toegevoegd om Workfront toe te laten om activa naar Experience Manager Assets te verzenden.

### Oplossing:

Voeg de Workfront IP adressen aan de lijst van gewenste personen van Cloud Manager van de Adobe toe.

* Voor instructies bij het toevoegen van IP adressen aan uw Adobe Cloud Manager, zie [ Inleiding aan IP Lijsten van gewenste personen ](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/using-cloud-manager/ip-allow-lists/introduction.html?lang=en) in de documentatie van Adobe Experience Manager.
* Voor een lijst van Workfront IP adressen om aan de lijst van gewenste personen toe te voegen, zie [ uw firewall ](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md) vormen.
