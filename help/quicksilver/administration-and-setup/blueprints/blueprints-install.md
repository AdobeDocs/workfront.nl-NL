---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Een blauwdruk installeren
description: U kunt een blauwdruk installeren in de productieomgeving of in een Sandbox-omgeving.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 546e19ab-dc50-4d23-b5f6-31bde1c82b6a
source-git-commit: 48de4553478fc42d88d81ea953440337f6684e50
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Een blauwdruk installeren

<!-- Audited: 5/2025 -->

U kunt een blauwdruk installeren in de productieomgeving of in een Sandbox-omgeving.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td>
   <p>Nieuw: Standaard</p>
   <p>of</p>
   <p>Huidig: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>U moet een [!DNL Workfront] beheerder zijn. </td> 
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
        <td>Productie is uw live omgeving.</td>
    </tr>
    <tr>
        <td><strong>Voorvertoning sandbox</strong></td>
        <td>De voorvertoning van de sandbox is een testomgeving die fungeert als replica van uw live omgeving en die elk weekend door Adobe Workfront wordt vernieuwd. Alle ondersteuningspakketten hebben toegang tot de voorvertoning van de sandbox. Voor meer informatie, zie <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md"> het [!DNL Adobe Workfront] Milieu van de Voorproef Sandbox </a>.</td>
    </tr>
    <tr>
        <td><strong>Sandbox 1 &amp; 2</strong></td>
        <td>De aangepaste vernieuwingssandbox is een aparte testomgeving die u handmatig kunt vernieuwen. Er zijn extra kosten voor het ophalen van de aangepaste vernieuwingssandbox. Voor meer informatie, zie <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md"> de [!DNL Adobe Workfront] Douane verfrist het milieu van Sandbox </a>.</td>
    </tr>
</table>

>[!TIP]
>
>We raden u aan de blauwdruk eerst in een Sandbox-omgeving te installeren. Op die manier kunt u de inhoud van de blauwdruk testen en controleren of deze geschikt is voor uw organisatie zonder wijzigingen aan te brengen in live-gegevens.

>[!NOTE]
>
>Bepaalde blauwdrukken kunnen alleen worden geïnstalleerd in de voorbeeldomgeving voor testdoeleinden. Als u toegang hebt tot inhoud met alleen voorvertoning in uw productieomgeving, Sandbox 1 of Sandbox 2, is de installatieknop niet actief en ziet u mogelijk een waarschuwingsbericht.\
>Bovendien is het omschakelingsvermogen van de omgeving beperkt wanneer u toegang krijgt tot inhoud die alleen in de voorvertoning kan worden weergegeven, zelfs als u zich in de voorvertoningsomgeving bevindt.

## De blauwdruk installeren

{{step1-to-blueprints}}

1. Zoek de blauwdruk die u wilt installeren. U kunt filteren op gebruik, rijpheidsniveau, installatiestatus en rechts op de pagina typen.
1. (Optioneel) Klik op **[!UICONTROL Details]** voor meer informatie over de werking van de blauwdruk.
1. Klik op **[!UICONTROL Install]**.
1. Kies of u wilt installeren in uw productieomgeving of in een sandbox-omgeving.\
   Voor meer informatie, zie [ waar zou ik een blauwdruk moeten installeren?](#where-should-i-install-a-blueprint) in dit artikel.
1. Op **vorm** pagina, kunt u verkiezen om één van het volgende te doen:

   * Installeer de blauwdruk zoals deze is. Voor blauwdruktypes die geen configuratie vereisen, is dit de enige optie. Voor blauwdruktypes die configuratie nodig hebben, kunt u naar keuze verkiezen om de blauwdruk nu te installeren en het later te vormen. Klik op **[!UICONTROL Install as is]**.
   * Vorm de blauwdruk vóór installatie, voor blauwdrukken die configuratie vereisen. Maak uw configuratieselecties, dan klik **[!UICONTROL Install blueprint]**.

     Voor meer informatie, zie [ een blauwdruk ](../../administration-and-setup/blueprints/configure-template-package.md) vormen.

   De installatie is voltooid en er wordt een bericht weergegeven met een lijst met specifieke objecten (zoals rollen, teams of groepen) die met succes zijn geïnstalleerd met de blauwdruk en alle objecten die niet zijn geïnstalleerd.

Na het installeren van de blauwdruk, zouden sommige extra acties kunnen nodig zijn om het volledig op te stellen. Voor informatie, zie [ Acties na het installeren van een blauwdruk ](../../administration-and-setup/blueprints/best-next-actions-after-install.md) te nemen.
