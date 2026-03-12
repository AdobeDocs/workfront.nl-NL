---
product-area: documents
navigation-topic: approvals
title: Overzicht van opslag in Adobe-bedrijven
description: Overzicht van opslag in Adobe-bedrijven
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 16c564a9-abd7-4b07-be3e-9c823f40177d
source-git-commit: 97c351ca38a8b6075634b2f755f2330562bc8b52
workflow-type: tm+mt
source-wordcount: '809'
ht-degree: 0%

---

# Overzicht van opslag in Adobe-bedrijven

Adobe Enterprise Storage is een op cloud gebaseerde opslagoplossing die fungeert als centrale opslagplaats voor bedrijfsmiddelen in Adobe. De integratie met Workfront en Frame.io is gebaseerd op Adobe Enterprise Storage, waardoor naadloze samenwerking en beheer van bedrijfsmiddelen tussen deze platforms mogelijk zijn.

Met deze opslagoptie wordt ook de weg vrijgemaakt voor toekomstige integratie van bedrijfsmiddelen met andere Adobe-producten, zoals Adobe Creative Cloud.

## Belangrijkste kenmerken

* **Verenigde opslaglaag**: De ondernemingsopslag van Adobe doet dienst als gedeeld opslagsteun voor Workfront, Frame.io, Document Cloud, en Creative Cloud. Dit maakt naadloze samenwerking en beheer van bedrijfsmiddelen op deze platforms mogelijk.

* **Inschakelen van supply chain van de Inhoud**: De ondernemingsopslag van Adobe is een basiscomponent voor de visie van Supply chain van de Inhoud van Adobe, toestaand teams om werk-in-vooruitgang activa zonder de behoefte aan handmatige downloads of herupload in diverse toepassingen van Adobe te beheren.

* **Gecentraliseerde toestemmingen en toegang**: De ondernemingsopslag van Adobe steunt onderneming-vlakke toegangscontroles, die met het Systeem van Adobe IMS (Identity Management) voor veilige en scalable gebruikerstoestemmingen integreren.

* **Van begin tot eind middelenzicht**: Assets die in de ondernemingsopslag van Adobe wordt opgeslagen kan in Workfront, Frame.io, en Creative Cloud apps worden gevestigd en worden beheerd, die verenigbare meta-gegevens, versioning, en controletrails verstrekken.

* **Integratie met overzicht en goedkeuringswerkschema&#39;s**: De ondernemingsopslag van Adobe laat creatieve overzicht en goedkeuringswerkschema&#39;s toe door als bron van waarheid voor alle activa te dienen, die ervoor zorgen dat terugkoppelt en goedkeuringen centraal worden gevolgd.

* **Schaalbare opslag en quotabeheer**: De ondernemingsopslag van Adobe biedt scalable opslagopties en verenigde quota het volgen over de producten van Adobe aan.

## Integratie met workflows voor evaluatie en goedkeuring

De integratie van Workfront en Frame.io maakt gebruik van Adobe Enterprise Storage om een uniforme evaluatie- en goedkeuringservaring te bieden. Dankzij deze integratie kunnen projectcoördinatoren projecten beheren en werken plannen in Workfront, terwijl creatieve personen, marketers en belanghebbenden hun middelen in Frame.io kunnen beoordelen en goedkeuren. Dit zorgt ervoor dat alle belanghebbenden toegang hebben tot de meest recente versies van middelen en feedback op één locatie wordt gecentraliseerd.

Voor meer informatie over de integratie Workfront en Frame.io, zie [&#x200B; Frame.io integratieoverzicht &#x200B;](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/frame-int-overview.md).

## Verschillen tussen Adobe Enterprise-opslag en oudere Workfront-opslag

Bestaande Workfront-omgevingen beschikken over een combinatie van Adobe Enterprise Storage en oudere Workfront-opslag. Alle objecten die vóór de release van Adobe Enterprise Storage zijn gemaakt, maken gebruik van oudere Workfront-opslagsystemen.

Als u eenmaal Adobe Enterprise Storage in uw omgeving hebt ingeschakeld, kunt u zowel Adobe Enterprise Storage- als oudere Workfront-opslagprojecten maken.

>[!NOTE]
>
>Nieuwe netwerkomgevingen beschikken standaard over Adobe Enterprise Storage en hebben geen optie om oude Workfront-opslag te gebruiken.


### Documenten

#### Nieuw documentgebied

Het nieuwe documentengebied is een uniform documentgebied dat opnieuw is ontworpen voor Adobe Enterprise Storage.

Deze bijgewerkte interface vereenvoudigt navigatie, verbetert duidelijkheid, en maakt het voor teams gemakkelijker om overzichten en goedkeuringen in één verenigde milieu te beheren. Voor meer informatie, zie het [&#x200B; het gebiedsoverzicht van Documenten &#x200B;](/help/quicksilver/documents/managing-documents/documents-area.md).

#### Nieuw machtigingsmodel document

>[!IMPORTANT]
>
>In Adobe Enterprise Storage werken documentmachtigingen anders dan in oudere Workfront-opslagsystemen. De documenten erven toestemmingen van het project, de taak, of uitgeven zij met verbonden zijn.

Documenten kunnen niet afzonderlijk worden gedeeld. In plaats daarvan genereert het systeem automatisch een map voor elke taak of uitgave en neemt het de machtigingen over van de taak of uitgave. Alle documenten die naar de taak of uitgave zijn geüpload, worden in die gegenereerde map opgeslagen.

Voor meer informatie over het nieuwe model van de documenttoestemming, zie &lbrace;de toestemmingen van Objecten en overzicht van het toegangsniveau voor het model van de ondernemingsopslag van Adobe [.](/help/quicksilver/review-and-approve-work/esm-access-permissions.md)

##### Gekoppelde objecten op mappen

Op projectniveau, tonen de systeem-geproduceerde omslagen een verbonden voorwerp. De map krijgt automatisch dezelfde naam als de taak of uitgave waartoe deze behoort. Met gekoppelde mappen weet het systeem op welke taak of welke uitgave de map moet worden weergegeven.

Voor meer informatie, zie [&#x200B; hoe de toestemmingen van het document &#x200B;](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work) werken.

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

Bestaande klanten kunnen Adobe Enterprise Storage in hun omgeving inschakelen bij contractvernieuwing. Voor meer informatie over het toelaten van de ondernemingsopslag van Adobe, zie [&#x200B; de ondernemingsopslag van Adobe voor uw organisatie &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md) toelaten.

>[!NOTE]
>
>Nieuwe klanten hebben standaard Adobe Enterprise Storage ingeschakeld en hebben niet de mogelijkheid om oude Workfront-opslag te gebruiken.






