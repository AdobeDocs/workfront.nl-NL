---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Een blauwdruk installeren
description: U kunt een blauwdruk installeren in de productieomgeving of in een Sandbox-omgeving.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 546e19ab-dc50-4d23-b5f6-31bde1c82b6a
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 0%

---

# Een blauwdruk installeren

U kunt een blauwdruk installeren in de productieomgeving of in een Sandbox-omgeving.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p> Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] licentie</strong></td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau</strong></td> 
   <td> <p>[!UICONTROL System administrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Waar moet ik een blauwdruk installeren? {#where-should-i-install-a-blueprint}

U kunt uw pakket installeren in een van de volgende omgevingen:

<table style="table-layout:auto">
        <tr>
        <td><strong>Productie</strong></td>
        <td>Productie is uw live omgeving.</td>
    </tr>
    <tr>
        <td><strong>Voorvertoning sandbox</strong></td>
        <td>De voorvertoning van de sandbox is een testomgeving die fungeert als replica van uw live omgeving en die elk weekend door Workfront wordt vernieuwd. Alle ondersteuningspakketten hebben toegang tot de voorvertoning van de sandbox. Voor meer informatie, zie <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md"> het [!DNL Adobe Workfront] Milieu van de Voorproef Sandbox </a>.</td>
    </tr>
    <tr>
        <td><strong>Sandbox 1 &amp; 2</strong></td>
        <td>De aangepaste vernieuwingssandbox is een aparte testomgeving die u handmatig kunt vernieuwen. Er zijn extra kosten voor het ophalen van de aangepaste vernieuwingssandbox. Voor meer informatie, zie <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md"> de [!DNL Adobe Workfront] Douane verfrist het milieu van Sandbox </a>.</td>
    </tr>
</table>

>[!TIP]
>
>We raden u aan de blauwdruk eerst in een sandboxomgeving te installeren. Op die manier kunt u de inhoud van de blauwdruk testen en controleren of deze geschikt is voor uw organisatie zonder wijzigingen aan te brengen in live-gegevens.

>[!NOTE]
>
>Bepaalde blauwdrukken kunnen alleen worden geïnstalleerd in de voorbeeldomgeving voor testdoeleinden. Als u toegang hebt tot inhoud met alleen voorvertoning in uw productieomgeving, Sandbox 1 of Sandbox 2, is de installatieknop niet actief en ziet u mogelijk een waarschuwingsbericht.\
>Ook is de mogelijkheid om naar een andere omgeving te schakelen beperkt wanneer u alleen inhoud met voorvertoning opent, zelfs als u in de voorvertoningsomgeving werkt.

## De blauwdruk installeren

1. Klik op het pictogram **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe] Workfront en klik vervolgens op **[!UICONTROL Blueprints]** .
1. Zoek de blauwdruk die u wilt installeren. U kunt filteren op het gebruiksgeval, het rijpingsniveau, de installatiestatus en aan de rechterkant typen.
1. (Optioneel) Klik op **[!UICONTROL Details]** voor meer informatie over de werking van de blauwdruk.
1. Klik op **[!UICONTROL Install]**.
1. Kies of u wilt installeren in uw productieomgeving of in een sandbox-omgeving.\
   Voor meer informatie, zie [ waar zou ik een blauwdruk moeten installeren?](#where-should-i-install-a-blueprint) in dit artikel.
1. Op de pagina [!UICONTROL Configure] kunt u een van de volgende handelingen uitvoeren:

   * Installeer de blauwdruk zoals deze is. Voor blauwdruktypes die geen configuratie vereisen, is dit de enige optie. Voor blauwdruktypes die configuratie nodig hebben, kunt u naar keuze verkiezen om de blauwdruk nu te installeren en het later te vormen. Klik op **[!UICONTROL Install as is]**.
   * Vorm de blauwdruk vóór installatie, voor blauwdrukken die configuratie vereisen. Maak uw configuratieselecties en klik op **[!UICONTROL Install blueprint]**\.

     Voor meer informatie, zie [ een blauwdruk ](../../administration-and-setup/blueprints/configure-template-package.md) vormen.
Wanneer de installatie is voltooid, wordt een bericht weergegeven met een lijst met specifieke objecten (zoals rollen, teams of groepen) die met succes zijn geïnstalleerd met de blauwdruk en alle objecten die niet zijn geïnstalleerd.

Na het installeren van de blauwdruk, zouden sommige extra acties kunnen nodig zijn om het volledig op te stellen. Voor informatie, zie [ Acties na het installeren van een blauwdruk ](../../administration-and-setup/blueprints/best-next-actions-after-install.md) te nemen.
