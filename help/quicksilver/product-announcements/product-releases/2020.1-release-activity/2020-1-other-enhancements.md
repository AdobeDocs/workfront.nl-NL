---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: 2020.1 Andere verbeteringen
description: Deze pagina bevat een beschrijving van alle verbeteringen die zijn aangebracht in algemene gebieden van Workfront met de release 2020.1. Deze verbeteringen zijn momenteel beschikbaar in de voorvertoningsomgeving en worden eind maart of begin april 2020 beschikbaar gesteld in de productieomgeving.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a716590c-c833-458a-a138-9bc0723e5896
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# 2020.1 Andere verbeteringen

Deze pagina bevat een beschrijving van alle verbeteringen die zijn aangebracht in algemene gebieden van Workfront met de release 2020.1. Deze verbeteringen zijn momenteel beschikbaar in de voorvertoningsomgeving en worden eind maart of begin april 2020 beschikbaar gesteld in de productieomgeving.

Voor een lijst van alle veranderingen beschikbaar met de versie 2020.1, zie [ overzicht van de versie 2020.1 ](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md).

## Wijziging vereist voor het toevoegen van proefdrukken aan de lijst van gewenste personen

>[!NOTE]
>
>Deze functie is verwijderd uit de release van 2020.1. Het zal op een later tijdstip beschikbaar worden gesteld.

Het proefdrukdomein verandert van from proofhq.com in workfront.com.

Als uw firewall of mailserver zo is geconfigureerd dat alleen bepaalde leveranciers toegang krijgen, moet u de volgende aanvullende URL toevoegen aan uw lijst van gewenste personen om ervoor te zorgen dat gebruikers in uw organisatie proofs kunnen weergeven in Workfront in zowel de viewer voor proef in de browser als de viewer voor proef in het bureaublad:

&#42; .workfront.com

Ook &#42; proofhq.com URL wordt vereist.

Voor meer informatie over het bijwerken van uw lijst van gewenste personen, zie [ de lijst van gewenste personen van uw firewall ](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) vormen.

>[!NOTE]
>
>Deze update is alleen van toepassing op proefdrukken in Workfront. Deze update is niet van toepassing wanneer u de zelfstandige Workfront Proof-toepassing gebruikt.

## Workfront cookie gedrag bijgewerkt om compatibiliteit met Chrome te behouden

Om de compatibiliteit met een komende Google Chrome-update (Chrome v80) te behouden, hebben we het Workfront-platform bijgewerkt om ervoor te zorgen dat cookies correct worden verzonden met aanvragen.

Deze Chrome-update wijzigt de standaardwaarde van het Cookie-kenmerk SameSite. Als u wilt testen hoe uw Workfront-instantie zich gedraagt na de Google Chrome-update, past u de markeringen in Chrome aan en schakelt u de volgende opties in:

* &quot;SameSite, standaard cookies&quot;
* &quot;Cookies zonder SameSite moeten veilig zijn&quot;

## Workfront synchroniseert opmerkingen met Jira

De Workfront for Jira-integratie synchroniseert nu uw Workfront-opmerkingen naar de native commentaarstream van Jira.

Eerder was het mogelijk om opmerkingen van Jira naar Workfront te synchroniseren, maar niet van Workfront naar Jira.

Voor meer informatie, zie [ Adobe Workfront voor Jira ](../../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md) vormen.

## De Flash Portfolio Optimizer is verwijderd

Wij hebben de capaciteit verwijderd om tussen het nieuwe en erfenis (gebaseerd op Flash) Portfolio Optimizer van de Klassieke milieu van Workfront voor alle klanten te schakelen. De verouderde functie Portfolio optimaliseren is een verouderde functie en de nieuwe gereedschappen bieden vandaag dezelfde functionaliteit.

Ga voor meer informatie over de functie voor het optimaliseren van portfolio naar https://experience.workfront.com/s/article/Understanding-the-Portfolio-Optimizer-356650079

Voor informatie over afgekeurde op Flash-gebaseerde hulpmiddelen in Workfront zie [ Vervanging van op Flash-gebaseerde hulpmiddelen in Adobe Workfront ](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md).
