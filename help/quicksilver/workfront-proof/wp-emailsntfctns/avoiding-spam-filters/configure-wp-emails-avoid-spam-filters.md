---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Vorm  [!DNL Workfront Proof]  e-mails om spamfilters te vermijden
description: "Het spamfilter van uw e-mailclient dient een belangrijk doel: u beschermen tegen vervelende en mogelijk kwaadaardige e-mails met spam. Maar, als u niet de correcte montages in de spamfilter hebt, kan het u van het zien van de volgende belangrijke  [!DNL Workfront Proof]  e-mails houden: proef e-mailberichten, nieuwsbrieven, en speciale mededelingen."
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1fce3d83-fdce-4ded-8e78-3468243a59e1
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 0%

---

# E-mailberichten configureren om spamfilters te voorkomen[!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het zelfstandige product [!DNL Workfront Proof] . Voor informatie bij het proef binnen [!DNL Adobe Workfront], zie [ het Bewijzen ](../../../review-and-approve-work/proofing/proofing.md).

Het spamfilter van uw e-mailclient dient een belangrijk doel: u kunt beschermen tegen vervelende en mogelijk kwaadaardige spamberichten. Maar als u niet over de juiste instellingen in het spamfilter beschikt, kunt u de volgende belangrijke e-mails van [!DNL Workfront Proof] niet zien: proefdrukken van e-mailmeldingen, nieuwsbrieven en speciale communicatie.

Om ervoor te zorgen dat uw [!DNL Workfront Proof] e-mails altijd naar uw Postvak IN plaats van naar uw spammap worden gerouteerd, moet u het volgende aan de lijst van gewenste personen toevoegen:

* [!DNL Workfront Proof] mailserver: **[!DNL mx.proofhq.com]**
* [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; e-mailadressen (bijvoorbeeld notification@proofhq.com)

Voor meer informatie over URLs om aan uw lijst van gewenste personen toe te voegen, zie [ de lijst van gewenste personen van uw firewall ](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) in het artikel [ vormen de lijst van gewenste personen van uw firewall ](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot;-e-mailadressen

Afhankelijk van het type e-mailclient moet u mogelijk [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot;-e-mailadressen toevoegen aan een van de volgende opties om te voorkomen dat het spamfilter in de toekomst uw e-mailberichten naar uw spammap stuurt:

* Uw lijst van contactpersonen
* Uw lijst [!UICONTROL Safe Senders]
* Een filter dat u maakt om e-mails van deze adressen naar uw Postvak IN te sturen

Mogelijk moet u ook bestaande [!DNL Workfront Proof] e-mails uit uw spammap verwijderen en controleren of een van de &quot;[!UICONTROL from]&quot;-adressen voorkomt in de lijst met geblokkeerde adressen. Deze Help-pagina bevat de [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot;-adressen en laat zien hoe u deze aan het spamfilter kunt toevoegen in de volgende e-mailclients:

* [!DNL Gmail]
* [!DNL Microsoft Outlook 2003 - 2007]
* [!DNL Windows Live Hotmail]
* [!DNL Yahoo Mail]
* [!DNL Aol]

>[!NOTE]
>
>Raadpleeg de Help van uw e-mailclient als u vragen hebt over een hier beschreven procedure.

Voor meer informatie, zie [ spammontages voor gemeenschappelijke e-mailcliënten ](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-spam-settings-clients.md) vormen.

## De [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot;-e-mailadressen die moeten worden gekopieerd

Om ervoor te zorgen dat uw [!DNL Workfront Proof] e-mailadres uw Postvak IN bereikt, moet u twee [!DNL Workfront Proof] -e-mailadressen afzonderlijk aan het spamfilter van uw e-mailclient toevoegen:

* Het algemene ondersteuningsadres [!DNL support@proofhq.com] , waaruit [!DNL Workfront Proof] veel e-mailberichten verzendt
* Een meldingsadres waar [!DNL Workfront Proof] een e-mail met een proefdrukbericht stuurt naar de maker van de proef en de controleurs met koppelingen naar de proefdrukproef. Dit kan een algemeen adres, notification@support.proofhq.com, of een specifiek adres zijn als u een aangepast subdomein of een wit etiketdomein hebt.

Als u [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot;-adressen wilt toevoegen aan het filter van uw e-mailclient:

1. Kopieer het algemene e-mailadres ( [!UICONTROL from] ) voor [!DNL Workfront Proof] ondersteuning (support@proofhq.com) en plak het in het veld dat voor uw e-mailclient is aangegeven.
1. Kopieer de juiste e-mailadressen van [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; en plak deze AFZONDERLIJK in het veld dat voor uw e-mailclient is aangegeven:

   * notification@support.proofhq.com als u GEEN aangepast subdomein of een wit labeldomein hebt
   * notification@yoursubdomain.proofhq.com als u een aangepast subdomein hebt; vervang uw subdomeinnaam in dit adres
   * notification@yoursubdomain.yourdomain.com als u een wit etiketdomein hebt; vervang uw subdomeinnaam en domeinnaam in dit adres

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See the relevant section below for your email client to find out where to paste in these two Workfront Proof "[!UICONTROL from]" addresses.</p>
-->
