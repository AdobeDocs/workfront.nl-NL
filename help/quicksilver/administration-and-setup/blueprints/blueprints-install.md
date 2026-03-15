---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Een blauwdruk installeren
description: U kunt een blauwdruk in uw Productiemilieu of een milieu installeren Sandbox.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 546e19ab-dc50-4d23-b5f6-31bde1c82b6a
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 0%

---

# Een blauwdruk installeren

<!-- Audited: 5/2025 -->

U kunt een blauwdruk in uw Productiemilieu of een milieu installeren Sandbox.

## Toegangsvereisten

+++ Vouw uit om de toegangsvereisten voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>Workfront-beheerder</td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Waar moet ik een blauwdruk installeren? {#where-should-i-install-a-blueprint}

U kunt uw pakket installeren in een van de volgende omgevingen:

<table style="table-layout:auto">
        <tr>
        <td><strong>Productie</strong></td>
        <td>Productie is je live omgeving.</td>
    </tr>
    <tr>
        <td><strong>Voorvertoning sandbox</strong></td>
        <td>Sandbox Preview is een testomgeving die fungeert als replica van uw live omgeving en die elk weekend wordt vernieuwd door Adobe Workfront. Alle ondersteuningspakketten hebben toegang tot de voorvertoning in de sandbox. Voor meer informatie, zie <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md"> het [!DNL Adobe Workfront] Milieu van de Voorproef Sandbox </a>.</td>
    </tr>
    <tr>
        <td><strong>Sandbox 1 en 2</strong></td>
        <td>De aangepaste sandbox Vernieuwen is een aparte testomgeving die u handmatig vernieuwt. Er zijn extra kosten voor het ophalen van de aangepaste sandbox Vernieuwen. Voor meer informatie, zie <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md"> de [!DNL Adobe Workfront] Douane verfrist het milieu van Sandbox </a>.</td>
    </tr>
</table>

>[!TIP]
>
>We raden u aan de blauwdruk eerst in een Sandbox-omgeving te installeren. Zo kunt u de inhoud van de blauwdruk testen en ervoor zorgen dat deze geschikt is voor uw organisatie zonder wijzigingen aan te brengen in live-gegevens.

>[!NOTE]
>
>Bepaalde blauwdrukken kunnen alleen worden geïnstalleerd in de voorvertoningsomgeving voor testdoeleinden. Als u toegang krijgt tot inhoud met alleen voorvertoning in uw Productieomgeving, Sandbox 1 of Sandbox 2, is de installatieknop niet actief en ziet u mogelijk een waarschuwingsbericht.\
>Bovendien is de omgevingsmogelijkheid beperkt wanneer u alleen Voorvertoning-inhoud opent, zelfs wanneer u zich in de voorvertoningsomgeving bevindt.

## De blauwdruk installeren

{{step1-to-blueprints}}

1. Zoek de blauwdruk die u wilt installeren. U kunt filteren op gebruiksscenario, volwassenheidsniveau, installatiestatus en aan de rechterkant van de pagina typen.
1. (Optioneel) Klik op **[!UICONTROL Details]** om te leren hoe de blauwdruk werkt.
1. Klik op **[!UICONTROL Install]**.
1. Kies of u wilt installeren in uw productieomgeving of in een sandbox-omgeving.\
   Voor meer informatie, zie [ waar zou ik een blauwdruk moeten installeren?](#where-should-i-install-a-blueprint) in dit artikel.
1. Op **vorm** pagina, kunt u verkiezen om één van het volgende te doen:

   * Installeer de blauwdruk zoals deze is. Voor typen blauwdrukken waarvoor geen configuratie nodig is, is dit de enige optie. Voor blauwdruktypen die moeten worden geconfigureerd, kunt u desgewenst de blauwdruk nu installeren en later configureren. Klik op **[!UICONTROL Install as is]**.
   * Configureer de blauwdruk voor de installatie voor blauwdrukken die moeten worden geconfigureerd. Maak uw configuratieselecties en klik vervolgens op **[!UICONTROL Install blueprint]** .

     Voor meer informatie, zie [ een blauwdruk ](../../administration-and-setup/blueprints/configure-template-package.md) vormen.

   De installatie is voltooid en er wordt een bericht weergegeven met een lijst met specifieke objecten (zoals rollen, teams of groepen) die zijn geïnstalleerd met de blauwdruk en alle objecten die niet zijn geïnstalleerd.

Na het installeren van de blauwdruk, zouden sommige extra acties kunnen nodig zijn om het volledig op te stellen. Voor informatie, zie [ te nemen Acties na het installeren van een blauwdruk ](../../administration-and-setup/blueprints/best-next-actions-after-install.md).
