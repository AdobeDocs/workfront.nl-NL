---
product-area: projects
navigation-topic: create-projects
title: Een project maken dat is verbonden met Frame.io
description: Een project is een grote eenheid werk in Adobe Workfront. U kunt geheel nieuwe projecten maken, een sjabloon gebruiken of uitgaven of taken omzetten in projecten.
author: Courtney
feature: Work Management
source-git-commit: 089173acb8fecd920ca096c5bf9c6ee61910c20b
workflow-type: tm+mt
source-wordcount: '1158'
ht-degree: 0%

---


# Een project maken dat is verbonden met Frame.io

Dankzij de integratie van Workfront en Frame.io kunt u in Workfront projecten maken die zijn gespiegeld in Frame.io, zodat u deze projecten probleemloos kunt beoordelen en goedkeuren.

Wanneer een Workfront-project is verbonden met Frame.io, kunt u

* **Frame.io-gebruikers toewijzen aan taken**: Gebruikers met Frame.io-functionaliteit worden via e-mail op de hoogte gesteld wanneer zij aan een Workfront-taak zijn toegewezen. Hierbij wordt aangegeven dat er werk moet worden voltooid.
* **Deel het project met Gebruikers Frame.io**: Wanneer een project met Frame.io toegelaten gebruikers wordt gedeeld, hebben zij toegang tot het project binnen zowel Workfront als Frame.io.
* **Creatieve materialen delen met Frame.io**: Projectcoördinatoren kunnen instructies en materialen van Workfront rechtstreeks naar de creatieve gebruiker in Frame.io verzenden via een eenrichtingsprojectmap voor synchronisatie. [!BADGE Binnenkort beschikbaar]{type=Informative}
* **Taakvoortgang volgen**: Creatieve personen kunnen voltooide middelen en markeringstaken volledig verzenden, dus zonder Frame.io te verlaten.

## Toegangsvereisten

>[!IMPORTANT]
>
>Deze functionaliteit is alleen beschikbaar voor organisaties die aan de [!DNL Adobe Admin Console].

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

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Vereisten

* De standaard Frame.io-account instellen in het Workfront-instellingengebied
* Gebruikers van Frame.io inschakelen in het Workfront-gebruikersprofiel

Zie voor meer informatie over de bovenstaande voorwaarden [Vorm [!DNL Workfront] en [!DNL Frame.io] integratie](/help/quicksilver/administration-and-setup/configure-integrations/configure-wf-and-frame.md).


## Een nieuwe projectsjabloon maken

Wanneer u een nieuwe sjabloon maakt, kunt u de informatie voor alle taken en voor uw toekomstige projectinstellingen invoeren. Deze informatie zal dan aan om het even welk project overbrengen dat u van het malplaatje creeert.

De projecten in Frame.io worden georganiseerd door teams, die met de groepen van Workfront worden verbonden. Wij adviseren gebruikend een projectmalplaatje om verbonden projecten tot stand te brengen omdat u de projectgroep kunt eerder plaatsen.

Als u verkiest om het project van kras tot stand te brengen, voegt Workfront automatisch de Standaard projectgroep toe en het spiegelproject Frame.io wordt gecreeerd onder dat standaardteam in Frame.io.

>[!NOTE]
>
>Het bijwerken van de groep na de verwezenlijking van het project verandert niet het team Frame.io.


### Creeer het malplaatje en specificeer de projectgroep

{{step1-to-templates}}

1. Klikken **Nieuwe sjabloon**.
1. Typ een naam voor de sjabloon en druk op **Enter** om de naam op te slaan.
1. Klik in het linkerdeelvenster op **Sjabloondetails**.
1. In de **Sjabloonkoppeling** , moet u een groep opgeven. Als u geen groep toevoegt, wordt de standaardprojectgroep toegevoegd en het project in Frame.io wordt gecreeerd onder het overeenkomstige standaardteam in Frame.io.

Ga door naar de volgende sectie.

![](assets/template-group.png)

### Taken toevoegen en gebruikers toewijzen die geschikt zijn voor Frame.io

1. Klik in het linkerdeelvenster op **Sjabloontaken**.
1. Klikken **Sjabloontaken toevoegen starten** om snel taken aan uw sjabloon toe te voegen. U kunt aanvullende instellingen later configureren.

   of

   Klikken **Nieuwe sjabloontaak** om één taak tegelijkertijd toe te voegen en extra montages te vormen.
   ![](assets/add-tasks-to-template.png)
1. Voeg een taaknaam toe.
1. In de **Toewijzingen** , wijst u gebruikers of teams toe. Als u een Frame.io toegelaten gebruiker, of individueel of in een team toewijst, worden zij samenwerkingstoegang tot het Frame.io- project verleend en over de taak in het Frame.io- project via e-mail op de hoogte gebracht. Van die e-mail, kunnen zij zich bij het project Frame.io aansluiten en beginnen met werken.
1. Herhaal stap 1 en 2 zo nodig.

Ga door naar de volgende sectie.

### Aanvullende sjabloondetails configureren

Workfront beschikt over robuuste mogelijkheden voor projectbeheer. We raden u aan de [Projectsjablonen bewerken](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md) artikel om de volgende gebieden van het malplaatje te vormen:

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

1. Klikken **Nieuw project van sjabloon**.
1. Typ in het zoekvak de naam van de gewenste sjabloon.
1. Selecteer de sjabloonnaam en klik op **Sjabloon gebruiken**.
   ![](assets/find-your-template.png)
1. Pas zo nodig om het even welke projectmontages aan, dan klik **Project maken**.
1. Klik in het linkerdeelvenster op **Documenten**.
1. Gebruik de one-way sync map om creatieve materialen automatisch te delen met Frame.io. [!BADGE Binnenkort beschikbaar]{type=Informative}

   >[!NOTE]
   >
   >Deze functie is momenteel in ontwikkeling. Als u informatie met gebruikers in Frame.io wilt delen, uploadt u de bestanden naar het tabblad Document. Wanneer de status van het project op Huidig wordt geplaatst, duwen die dossiers automatisch aan Frame.io.

1. In de projectheader, verander het project van **Planning** tot **Huidig**.

Nadat het project is gemaakt en ontwerpers voltooide middelen uploaden, kunt u een revisie- en goedkeuringswerkstroom toewijzen aan het element in Workfront. Zie voor meer informatie [Een documentrevisie of goedkeuringsaanvraag maken](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md). <!-- name may need to change -->

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

1. Klikken **Nieuw project**.
1. Typ een naam voor uw project en druk op **Enter** om de naam op te slaan.

Ga door naar de volgende sectie.

### Taken toevoegen en gebruikers toewijzen die geschikt zijn voor Frame.io

1. Klik in het linkerdeelvenster op **Taken**.
1. Klikken **Taken toevoegen starten** om snel taken aan uw project toe te voegen. U kunt aanvullende instellingen later configureren.

   of

   Klikken **Nieuwe taak** om één taak tegelijkertijd toe te voegen en extra montages te vormen.
   ![](assets/add-project-tasks.png)
1. Voeg een taaknaam toe.
1. In de **Toewijzingen** , wijst u gebruikers of teams toe. Als u een Frame.io toegelaten gebruiker, of individueel of in een team toewijst, worden zij samenwerkingstoegang tot het Frame.io- project verleend en over de taak in het Frame.io- project via e-mail op de hoogte gebracht. Van die e-mail, kunnen zij zich bij het project Frame.io aansluiten en beginnen met werken.
1. Herhaal stap 1 en 2 zo nodig.

Ga door naar de volgende sectie.

### Creatieve materialen uploaden

1. Klik in het linkerdeelvenster op **Documenten**.
1. Gebruik de one-way sync map om creatieve materialen automatisch te delen met Frame.io. [!BADGE Binnenkort beschikbaar]{type=Informative}

   >[!NOTE]
   >
   >Deze functie is momenteel in ontwikkeling. Als u informatie met gebruikers in Frame.io wilt delen, uploadt u de bestanden naar het tabblad Document. Wanneer de status van het project op Huidig wordt geplaatst, duwen die dossiers automatisch aan Frame.io

Ga door naar de volgende sectie.

### Aanvullende projectdetails configureren

Workfront beschikt over robuuste mogelijkheden voor projectbeheer. We raden u aan de [Projecten bewerken](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md) artikel om de volgende gebieden van het project te vormen:

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

Zie voor meer informatie [Een documentrevisie of goedkeuringsaanvraag maken](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md). <!-- name may need to change -->