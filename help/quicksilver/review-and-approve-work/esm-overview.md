---
product-area: documents
navigation-topic: approvals
title: Overzicht van opslag in Adobe-bedrijven
description: Overzicht van opslag in Adobe-bedrijven
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 16c564a9-abd7-4b07-be3e-9c823f40177d
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: b3c8559ddac934cc41461f88503b2fa71abaf452
workflow-type: tm+mt
source-wordcount: '855'
ht-degree: 0%

---

# Overzicht van opslag in Adobe-bedrijven

Adobe Enterprise Storage is een op cloud gebaseerde opslagoplossing die fungeert als centrale opslagplaats voor bedrijfsmiddelen in Adobe. De integratie met Workfront en Frame.io is gebaseerd op Adobe Enterprise Storage, waardoor naadloze samenwerking en beheer van bedrijfsmiddelen tussen deze platforms mogelijk zijn.

Met deze opslagoptie wordt ook de weg vrijgemaakt voor toekomstige integratie van bedrijfsmiddelen met andere Adobe-producten, zoals Adobe Creative Cloud.

## Belangrijkste kenmerken

* **Verenigde opslaglaag**: Adobe Enterprise Storage fungeert als een back-end voor gedeelde opslag voor Workfront, Frame.io, Document Cloud en Creative Cloud. Dit maakt naadloze samenwerking en beheer van bedrijfsmiddelen op deze platforms mogelijk.

* **Inzet supply chain van de Inhoud**: Adobe Enterprise storage is een basisonderdeel voor Adobe Content Supply chain vision, waardoor teams hun bedrijfsmiddelen in uitvoering kunnen beheren zonder dat handmatige downloads of heruploads in verschillende Adobe-toepassingen nodig zijn.

* **gecentraliseerde toestemmingen en toegang**: Adobe Enterprise Storage ondersteunt toegangsbeheer op bedrijfsniveau, integratie met Adobe IMS (Identity Management System) voor veilige en schaalbare gebruikersrechten.

* **Van begin tot eind middelenzicht**: Assets dat is opgeslagen in Adobe Enterprise Storage kan direct worden opgezocht en beheerd in Workfront-, Frame.io- en Creative Cloud-apps, zodat u consistente metagegevens, versieringen en audittrails krijgt.

* **Integratie met overzicht en goedkeuringswerkschema&#39;s**: De bedrijfsopslag van Adobe maakt creatieve revisie en goedkeuringswerkschema&#39;s mogelijk door als bron van waarheid voor alle activa te dienen, die ervoor zorgen dat terugkoppelen en goedkeuringen centraal worden gevolgd.

* **Schaalbare opslag en quotabeheer**: Adobe Enterprise Storage biedt schaalbare opslagopties en uniforme quota&#39;s voor alle Adobe-producten.

## Integratie met workflows voor evaluatie en goedkeuring

De integratie van Workfront en Frame.io maakt gebruik van Adobe Enterprise Storage om een uniforme evaluatie- en goedkeuringservaring te bieden. Dankzij deze integratie kunnen projectcoördinatoren projecten beheren en werken plannen in Workfront, terwijl creatieve personen, marketers en belanghebbenden hun middelen in Frame.io kunnen beoordelen en goedkeuren. Dit zorgt ervoor dat alle belanghebbenden toegang hebben tot de meest recente versies van middelen en feedback op één locatie wordt gecentraliseerd.

Voor meer informatie over de integratie van Workfront en Frame.io, zie [ Verenigd overzicht van overzicht en goedkeuring ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).

## Verschillen tussen Adobe Enterprise-opslag en oudere Workfront-opslag

Bestaande Workfront-omgevingen beschikken over een combinatie van Adobe Enterprise Storage en oudere Workfront-opslag. Alle objecten die vóór de release van Adobe Enterprise Storage zijn gemaakt, maken gebruik van oudere Workfront-opslagsystemen.

Als u eenmaal Adobe Enterprise Storage in uw omgeving hebt ingeschakeld, kunt u zowel Adobe Enterprise Storage- als oudere Workfront-opslagprojecten maken.

>[!NOTE]
>
>Nieuwe netwerkomgevingen beschikken standaard over Adobe Enterprise Storage en hebben geen optie om oude Workfront-opslag te gebruiken.


### Documenten

#### Nieuw gebied Documenten

Het nieuwe gebied van Documenten is een verenigd documentengebied dat voor de opslag van de onderneming van Adobe wordt herontworpen.

Deze bijgewerkte interface vereenvoudigt navigatie, verbetert duidelijkheid, en maakt het voor teams gemakkelijker om overzichten en goedkeuringen in één verenigde milieu te beheren. Voor meer informatie, zie het [ het gebiedsoverzicht van Documenten ](/help/quicksilver/documents/managing-documents/documents-area.md).

#### Nieuw machtigingsmodel document

>[!IMPORTANT]
>
>In Adobe Enterprise Storage werken documentmachtigingen anders dan in oudere Workfront-opslagsystemen. Documenten nemen machtigingen over van het project, de taak of de uitgave waaraan zij zijn gekoppeld.

Documenten kunnen niet afzonderlijk worden gedeeld. In plaats daarvan genereert het systeem automatisch een map voor elke taak of uitgave en neemt het de machtigingen over van de taak of uitgave. Alle documenten die naar de taak of uitgave zijn geüpload, worden in die gegenereerde map opgeslagen.

Voor meer informatie over het nieuwe model van de documenttoestemming, zie {de toestemmingen van Objecten en overzicht van het toegangsniveau voor het model van de ondernemingsopslag van Adobe ](/help/quicksilver/review-and-approve-work/esm-access-permissions.md).[

##### Gekoppelde objecten op mappen

Op projectniveau, tonen de systeem-geproduceerde omslagen een verbonden voorwerp. De map krijgt automatisch dezelfde naam als de taak of uitgave waartoe deze behoort. Met gekoppelde mappen weet het systeem op welke taak of welke uitgave de map moet worden weergegeven.

Voor meer informatie, zie [ hoe de toestemmingen van het document ](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work) werken.

## Workfront-objecten

In de onderstaande tabel worden de functies van Adobe Enterprise Storage en oudere Workfront-opslag voor Workfront-objecten vergeleken.

Workfront-objecten omvatten portfolio&#39;s, programma&#39;s, projecten, sjablonen, taken en uitgaven.

| Adobe Enterprise-opslag | Legacy Workfront-opslag |
|---|---|
| <ul><li>Gebruikt Adobe Enterprise Storage</li><li>Geïntegreerd met Frame.io</li><li>Gebruikt de nieuwe ervaring bij Documenten</li><li>Handhaaft strikte naamgevingsconventies</li><li>Direct delen van document is niet beschikbaar</li><li>Documenten zijn beschikbaar in andere Adobe-producten, zoals Frame.io en Creative Cloud</li></ul> | <ul><li>Gebruikt Workfront-opslag</li><li>Gebruikt de proefdrukviewer</li><li>Ondersteunt het delen van afzonderlijke documenten</li></ul> |

### Objecten verplaatsen, kopiëren en omzetten

U kunt Workfront-objecten verplaatsen, kopiëren en omzetten tussen soortgelijke opslagmodellen. U kunt bijvoorbeeld een taak verplaatsen van een Adobe Enterprise Storage-project naar een ander Adobe Enterprise Storage-project. U kunt een taak niet verplaatsen van een Adobe Enterprise Storage-project naar een ouder Workfront-opslagproject.

Deze acties zijn beschikbaar in het menu Meer voor een taak of kwestie. Elke actie eerbiedigt documentintegriteit, toestemmingsovererving, en de regels van de ondernemingsopslag van Adobe.

## Opslag in Adobe Enterprise

Bestaande klanten kunnen Adobe Enterprise Storage in hun omgeving inschakelen bij contractvernieuwing. Voor meer informatie over het toelaten van de ondernemingsopslag van Adobe, zie [ de ondernemingsopslag van Adobe voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md) toelaten.

>[!NOTE]
>
>Nieuwe klanten hebben standaard Adobe Enterprise Storage ingeschakeld en hebben niet de mogelijkheid om oude Workfront-opslag te gebruiken.



## Overwegingen

* Workfront is mogelijk niet meer synchroon met Frame.io of Creative Cloud, zoals een middel dat in Workfront wordt verwijderd maar nog steeds in Frame.io wordt weergegeven. Neem contact op met de Workfront-ondersteuning om uw omgeving te laten synchroniseren.


