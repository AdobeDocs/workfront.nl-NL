---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Configureren [!DNL Workfront Proof] e-mails om spamfilters te voorkomen
description: "Het spamfilter van uw e-mailclient dient een belangrijk doel: bescherming tegen irritante en mogelijk kwaadaardige spammails. Maar als u niet de correcte montages in de spamfilter hebt, kan het u van het zien van het volgende belangrijke houden [!DNL Workfront Proof] e-mails: elektronische proefdrukken, nieuwsbrieven, en speciale mededelingen."
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1fce3d83-fdce-4ded-8e78-3468243a59e1
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 0%

---

# Configureren [!DNL Workfront Proof] e-mails om spamfilters te voorkomen

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het standalone product [!DNL Workfront Proof]. Voor informatie over proefdrukken binnen [!DNL Adobe Workfront], zie [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Het spamfilter van uw e-mailclient dient een belangrijk doel: bescherming tegen irritante en mogelijk kwaadaardige spammails. Maar als u niet de correcte montages in de spamfilter hebt, kan het u van het zien van het volgende belangrijke houden [!DNL Workfront Proof] e-mails: elektronische proefdrukken, nieuwsbrieven, en speciale mededelingen.

Om ervoor te zorgen dat uw [!DNL Workfront Proof] e-mails worden altijd naar uw Postvak IN gerouteerd in plaats van naar uw spammap. Voeg het volgende toe aan de lijst van gewenste personen:

* [!DNL Workfront Proof] mailserver: **[!DNL mx.proofhq.com]**
* [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; e-mailadressen (bijvoorbeeld notification@proofhq.com)

Voor meer informatie over URLs om aan uw lijst van gewenste personen toe te voegen, zie [De lijst van gewenste personen van uw firewall configureren](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) in het artikel [De lijst van gewenste personen van uw firewall configureren](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## [!DNL Workfront Proof] &quot;[!UICONTROL from]E-mailadressen

Afhankelijk van het type e-mailclient moet u mogelijk toevoegen [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; e-mailadressen naar een van de volgende opties om te voorkomen dat het spamfilter in de toekomst uw e-mails naar uw spammap stuurt:

* Uw lijst van contactpersonen
* Uw [!UICONTROL Safe Senders] list
* Een filter dat u maakt om e-mails van deze adressen naar uw Postvak IN te sturen

Mogelijk moet u ook bestaande [!DNL Workfront Proof] e-mailberichten uit uw spammap en controleer of een van de &quot;[!UICONTROL from]&quot;-adressen staan op de lijst met geblokkeerde adressen. Deze Help-pagina bevat de lijst met [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; adressen en toont hoe te om hen aan het spamfilter in de volgende e-mailcliënten toe te voegen:

* [!DNL Gmail]
* [!DNL Microsoft Outlook 2003 - 2007]
* [!DNL Windows Live Hotmail]
* [!DNL Yahoo Mail]
* [!DNL Aol]

>[!NOTE]
>
>Raadpleeg de Help van uw e-mailclient als u vragen hebt over een hier beschreven procedure.

Zie voor meer informatie [Spaminstellingen configureren voor algemene e-mailclients](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-spam-settings-clients.md).

## De [!DNL Workfront Proof] &quot;[!UICONTROL from]E-mailadressen die u wilt kopiëren

Om ervoor te zorgen dat uw [!DNL Workfront Proof] e-mailberichten bereiken uw Postvak IN. U moet twee e-mails toevoegen [!DNL Workfront Proof] e-mailadressen afzonderlijk naar het spamfilter van uw e-mailclient:

* Het algemene steunadres, [!DNL support@proofhq.com], waarvan [!DNL Workfront Proof] verzendt vele e-mailmededelingen
* Een meldingsadres waarvan [!DNL Workfront Proof] stuurt een e-mail met een proefdrukbericht naar de maker van de proefdruk en de controleurs met links naar de proefdrukproef. Dit kan een algemeen adres, notification@support.proofhq.com, of een specifiek adres zijn als u een aangepast subdomein of een wit etiketdomein hebt.

Toevoegen [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot;-adressen naar het filter van uw e-mailclient:

1. De algemene versie kopiëren [!DNL Workfront Proof] support &quot;[!UICONTROL from]&quot; E-mailadres (support@proofhq.com) en plak het in het veld dat voor uw e-mailclient is aangegeven.
1. Kopieer de juiste van de volgende [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; E-mailadressen en plak deze afzonderlijk in het veld dat voor uw e-mailclient is aangegeven:

   * notification@support.proofhq.com als u GEEN aangepast subdomein of een wit labeldomein hebt
   * notification@yoursubdomain.proofhq.com als u een aangepast subdomein hebt; substitueer uw subdomeinnaam in dit adres
   * notification@yoursubdomain.yourdomain.com als u een wit labeldomein hebt; substitueer uw subdomeinnaam en domeinnaam in dit adres

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See the relevant section below for your email client to find out where to paste in these two Workfront Proof "[!UICONTROL from]" addresses.</p>
-->
