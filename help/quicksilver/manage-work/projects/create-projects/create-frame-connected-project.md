---
product-area: projects
navigation-topic: create-projects
title: Een project maken dat is verbonden met Frame.io
description: Een project is een grote eenheid werk in Adobe Workfront. U kunt geheel nieuwe projecten maken, een sjabloon gebruiken of uitgaven of taken omzetten in projecten.
author: Courtney
feature: Work Management
hide: true
hidefromtoc: true
exl-id: 230d8e62-a3c9-4e38-9b26-5ba1c4f56391
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# Een project maken dat is verbonden met Frame.io

Dankzij de integratie van Workfront en Frame.io kunt u in Workfront projecten maken die zijn gespiegeld in Frame.io, zodat u deze projecten probleemloos kunt beoordelen en goedkeuren.

Wanneer een Workfront-project is verbonden met Frame.io, kunt u

* **wijs Gebruikers Frame.io aan taken** toe: De toegelaten gebruikers Frame.io worden op de hoogte gebracht per e-mail wanneer zij aan een taak van Workfront worden toegewezen, signalerend daar werk is te voltooien.
* **Deel het project met Gebruikers Frame.io**: Wanneer een project met toegelaten gebruikers wordt gedeeld Frame.io, hebben zij toegang tot het project binnen zowel Workfront als Frame.io.
* **Aandeel creatieve materialen met Frame.io**: De coördinatoren van het project kunnen instructies en materialen van Workfront rechtstreeks naar de creatieve gebruiker in Frame.io verzenden gebruikend een unidirectionele projectomslag van de synchronisatieproject. [!BADGE  Binnenkort ]{type=Informative}
* **de taakvooruitgang van het Spoor**: De Creatieven kunnen gebeëindigd activa verzenden en taken volledig-allen merken zonder Frame.io te verlaten.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

>[!IMPORTANT]
>
>Deze functionaliteit is alleen beschikbaar voor organisaties die zijn aangemeld bij de [!DNL Adobe Admin Console] .

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Standaard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot projecten bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Wanneer u een project creeert, ontvangt u automatisch Manage toestemmingen aan het project.</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

* De standaard Frame.io-account instellen in het Workfront-instellingengebied
* Gebruikers van Frame.io inschakelen in het Workfront-gebruikersprofiel

Voor meer informatie over de eerste vereisten hierboven, zie [  [!DNL Workfront]  vormen en  [!DNL Frame.io]  integratie ](/help/quicksilver/administration-and-setup/configure-integrations/configure-wf-and-frame.md).


## Een nieuwe projectsjabloon maken

Wanneer u een nieuwe sjabloon maakt, kunt u de informatie voor alle taken en voor uw toekomstige projectinstellingen invoeren. Deze informatie zal dan aan om het even welk project overbrengen dat u van het malplaatje creeert.

De projecten in Frame.io worden georganiseerd door teams, die met de groepen van Workfront worden verbonden. Wij adviseren gebruikend een projectmalplaatje om verbonden projecten tot stand te brengen omdat u de projectgroep kunt eerder plaatsen.

Als u verkiest om het project van kras tot stand te brengen, voegt Workfront automatisch de Standaard projectgroep toe en het spiegelproject Frame.io wordt gecreeerd onder dat standaardteam in Frame.io.

>[!NOTE]
>
>Het bijwerken van de groep na de verwezenlijking van het project verandert niet het team Frame.io.


### Creeer het malplaatje en specificeer de projectgroep

{{step1-to-templates}}

1. Klik **Nieuw Malplaatje**.
1. Typ een naam voor uw malplaatje, dan druk **binnengaan** om de naam te bewaren.
1. In het linkerpaneel, klik **Details van het Malplaatje**.
1. In de **sectie van de associatie van het Malplaatje**, zorg ervoor om een groep te specificeren. Als u geen groep toevoegt, wordt de standaardprojectgroep toegevoegd en het project in Frame.io wordt gecreeerd onder het overeenkomstige standaardteam in Frame.io.

Ga door naar de volgende sectie.

![ de groep van het Malplaatje ](assets/template-group.png)

### Taken toevoegen en gebruikers toewijzen die geschikt zijn voor Frame.io

1. In het linkerpaneel, klik **de Taken van het Malplaatje**.
1. Klik **Begin Toevoegend de Taken van het Malplaatje** om taken aan uw malplaatje snel toe te voegen. U kunt aanvullende instellingen later configureren.

   of

   Klik **Nieuwe Taak van het Malplaatje** om één taak tegelijkertijd toe te voegen en extra montages te vormen.
   ![ voegt taken aan malplaatje ](assets/add-tasks-to-template.png) toe
1. Voeg een taaknaam toe.
1. In het **gebied van Taken**, wijs gebruikers of teams toe. Als u een Frame.io toegelaten gebruiker, of individueel of in een team toewijst, worden zij samenwerkingstoegang tot het Frame.io- project verleend en over de taak in het Frame.io- project via e-mail op de hoogte gebracht. Van die e-mail, kunnen zij zich bij het project Frame.io aansluiten en beginnen met werken.
1. Herhaal stap 1 en 2 zo nodig.

Ga door naar de volgende sectie.

### Aanvullende sjabloondetails configureren

Workfront beschikt over robuuste mogelijkheden voor projectbeheer. Wij adviseren gebruikend [ projectmalplaatjes ](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md) artikel uitgeven om de volgende gebieden van het malplaatje te vormen:

* Overzicht
* Financiën
* Aangepaste Forms
* Projectinstellingen
* Instellingen voor taken
* Instellingen van uitgave
* Toegang

### Een project maken op basis van de sjabloon

Nadat u een sjabloon hebt gemaakt, kunt u dit gebruiken om projecten te maken.

{{step1-to-projects}}

1. Klik **Nieuw Project van Malplaatje**.
1. Typ in het zoekvak de naam van de gewenste sjabloon.
1. Selecteer de malplaatjenaam, dan klik **malplaatje van het Gebruik**.
   ![ vind uw malplaatje ](assets/find-your-template.png)
1. Pas om het even welke projectmontages aan zoals nodig, dan klik **creeer project**.
1. In het linkerpaneel, klik **Documenten**.
1. Gebruik de one-way sync map om creatieve materialen automatisch te delen met Frame.io. [!BADGE  Binnenkort ]{type=Informative}

   >[!NOTE]
   >
   >Deze functie is momenteel in ontwikkeling. Als u informatie met gebruikers in Frame.io wilt delen, uploadt u de bestanden naar het tabblad Document. Wanneer de status van het project op Huidig wordt geplaatst, duwen die dossiers automatisch aan Frame.io.

1. In de projectheader, verander het project van **Planning** aan **Huidige**.

Nadat het project is gemaakt en ontwerpers voltooide middelen uploaden, kunt u een revisie- en goedkeuringswerkstroom toewijzen aan het element in Workfront. Voor meer informatie, zie [ een documentoverzicht of goedkeuringsverzoek ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md) creëren. <!-- name may need to change -->

## Een geheel nieuw project maken

Desgewenst kunt u een geheel nieuw project maken.

>[!IMPORTANT]
>
>* De projecten in Frame.io worden georganiseerd door teams, die met de groepen van Workfront worden verbonden. Wij adviseren gebruikend een projectmalplaatje om verbonden projecten tot stand te brengen omdat u de projectgroep kunt eerder plaatsen.
>
>
>* Als u verkiest om het project van kras tot stand te brengen, voegt Workfront automatisch de Standaard projectgroep toe en het spiegelproject Frame.io wordt gecreeerd onder dat standaardteam in Frame.io.
>
>Het bijwerken van de groep na de verwezenlijking van het project verandert niet het team Frame.io.

### Het project maken

{{step1-to-projects}}

1. Klik **Nieuw Project**.
1. Typ een naam voor uw project, dan druk **binnengaan** om de naam te bewaren.

Ga door naar de volgende sectie.

### Taken toevoegen en gebruikers toewijzen die geschikt zijn voor Frame.io

1. In het linkerpaneel, klik **Taken**.
1. Klik **Begin Toevoegend Taken** om taken aan uw project snel toe te voegen. U kunt aanvullende instellingen later configureren.

   of

   Klik **Nieuwe Taak** om één taak tegelijkertijd toe te voegen en extra montages te vormen.
   ![ Nieuwe taak ](assets/add-project-tasks.png)
1. Voeg een taaknaam toe.
1. In het **gebied van Taken**, wijs gebruikers of teams toe. Als u een Frame.io toegelaten gebruiker, of individueel of in een team toewijst, worden zij samenwerkingstoegang tot het Frame.io- project verleend en over de taak in het Frame.io- project via e-mail op de hoogte gebracht. Van die e-mail, kunnen zij zich bij het project Frame.io aansluiten en beginnen met werken.
1. Herhaal stap 1 en 2 zo nodig.

Ga door naar de volgende sectie.

### Creatieve materialen uploaden

1. In het linkerpaneel, klik **Documenten**.
1. Gebruik de one-way sync map om creatieve materialen automatisch te delen met Frame.io. [!BADGE  Binnenkort ]{type=Informative}

   >[!NOTE]
   >
   >Deze functie is momenteel in ontwikkeling. Als u informatie met gebruikers in Frame.io wilt delen, uploadt u de bestanden naar het tabblad Document. Wanneer de status van het project op Huidig wordt geplaatst, duwen die dossiers automatisch aan Frame.io

Ga door naar de volgende sectie.

### Aanvullende projectdetails configureren

Workfront beschikt over robuuste mogelijkheden voor projectbeheer. Wij adviseren gebruikend [ projecten ](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md) artikel uitgeven om de volgende gebieden van het project te vormen:

* Overzicht
* Financiën
* Aangepaste Forms
* Projectinstellingen
* Instellingen voor taken
* Instellingen van uitgave
* Toegang

### Het project instellen op huidig

1. In de projectkopbal, verander het project van Planning in Huidig.
Nadat het project is gemaakt en ontwerpers voltooide middelen uploaden, kunt u een revisie- en goedkeuringswerkstroom toewijzen aan het element in Workfront.

Nadat het project is gemaakt en ontwerpers voltooide middelen uploaden, kunt u een revisie- en goedkeuringswerkstroom toewijzen aan het element in Workfront.

Voor meer informatie, zie [ een documentoverzicht of goedkeuringsverzoek ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md) creëren. <!-- name may need to change -->
