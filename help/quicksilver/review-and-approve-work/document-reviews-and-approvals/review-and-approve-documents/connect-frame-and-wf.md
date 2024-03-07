---
product-area: projects
navigation-topic: approvals
title: Workfront en Frame.io verbinden
description: Workfront gebruikt Frame.io in het revisie- en goedkeuringsproces om mensen te ontmoeten waar ze willen werken. Het projectbeheer en goedkeuringsproces worden beheerd in Workfront en het controleproces wordt uitgevoerd in Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
source-git-commit: 2c1945cdc9f923ea7fdc750f69eeba2a026571ac
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 0%

---


# Workfront en Frame.io verbinden

>[!IMPORTANT]
>
>De inhoud van dit artikel verwijst naar de functionaliteit voor bijgewerkte documentgoedkeuring die alleen beschikbaar is voor specifieke accounts. Zie de artikelen in [Goedkeuring van werkzaamheden](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

Workfront gebruikt Frame.io in het revisie- en goedkeuringsproces om mensen te ontmoeten waar ze willen werken. Het projectbeheer en goedkeuringsproces worden beheerd in Workfront en het revisieproces wordt voltooid in Frame.io. U moet alle volgende secties voltooien om de integratie te voltooien:

* [Een Workfront-groep verbinden met een Frame.io-team](#connect-a-workfront-group-to-a-frameio-team)
* [Een Workfront-project maken en een verbonden groep toevoegen](#create-a-workfront-project-and-add-a-connected-group)



## Toegangsvereisten

* Uw organisatie moet handmatig zijn ingeschakeld om de in dit artikel beschreven functionaliteit te kunnen gebruiken. Zie voor meer informatie [Standaard Adobe Workfront- en Frame.io-integratie alfa: overzicht](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md).


## Een Workfront-groep verbinden met een Frame.io-team

We zijn in mei bezig deze functie actief te verbeteren voor algemene beschikbaarheid.

### Vereisten

* Maak een Frame.io-team om toe te wijzen aan een Workfront-groep.
* Zoek de API ontwikkelaarstoken voor het team. Zie voor meer informatie [Ontwikkeltokens](https://developer.frame.io/docs/getting-started/authentication#developer-tokens) op de Frame.io-ontwikkelaarssite.

### Een Workfront-groep verbinden met een Frame.io-team

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op **Groepen**.
1. Kies een bestaande groep of klik op **Groep maken**.
1. Klik in het linkerdeelvenster op **Verbinding maken met Frame.io**.
   ![](assets/connect-frame-group.png)
1. Voer het API-ontwikkelaarstoken in.
1. Klikken **Verbinding starten**.
1. (Voorwaardelijk) Als u de beheerder bent van meer dan één Frame.io-account, selecteert u de account die u wilt gebruiken.

## Een Workfront-project maken en een verbonden groep toevoegen

Nadat u een Groep van Workfront met een team Frame.io hebt verbonden, moet u een project met die verbonden groep tot stand brengen.

### Vereisten

* Er moet een Workfront-groep zijn verbonden met een Frame.io-team, zoals uitgelegd in de vorige sectie.

### Een Workfront-project maken en een verbonden groep toevoegen

{{step1-to-projects}}

1. Maak een geheel nieuw project of een sjabloon. Voor informatie over hoe te om een project tot stand te brengen, zie [Een project maken](/help/quicksilver/manage-work/projects/create-projects/create-project.md).

1. In het linkerpaneel, vind **Projectdetails**.

1. Zoek de **Groep** aan de rechterkant van het scherm en verwijder de standaardgroep.

1. Zoek de gewenste groep in het keuzemenu. Groepen die zijn verbonden met Frame.io geven het pictogram Frame.io weer.
   ![](assets/add-frame-group.png)

1. Breng andere wijzigingen in de projectconfiguratie aan.

1. Klikken **Wijzigingen opslaan**.

1. Ga door naar de volgende sectie.

### Voeg een taak toe en plaats de integratiestatus aan Actief

>[!NOTE]
>
>Subtaken worden momenteel niet gesteund in verbonden projecten Frame.io.


1. Creeer de taken u in Frame.io moet bevolken

1. Selecteer de taken die u nodig hebt en klik op **Bewerken**.

1. Naar de **Aangepaste Forms** en zoek het integratieformulier Frame.io.

   >[!IMPORTANT]
   >
   >Dit formulier wordt alleen weergegeven als er een verbonden Frame.io-groep is toegewezen in het gebied Projectdetails. Zie voor meer informatie [Een Workfront-project maken en een verbonden groep toevoegen](#create-a-workfront-project-and-add-a-connected-group) in dit artikel.


1. De optie **De integratiestatus van deze taak** selectievakje en kies **Actief**.
   ![](assets/frame-custom-form.png)

1. Klikken **Wijzigingen opslaan**. Er wordt een pictogram Frame.io weergegeven naast de projectnaam.

1. Wijs gebruikers of teams toe aan taken.

   >[!NOTE]
   >
   >De gebruikers of de teams die aan de taken worden toegevoegd worden ook toegevoegd aan het project Frame.io.

1. Upload om het even welke documenten of creatieve briefs in het gebied van de Documenten van het Project.

Het project is nog niet verbonden, moet u aan de volgende sectie verdergaan om de integratie te beëindigen.

### Het project inschakelen in Frame.io

1. De projectstatus wijzigen vanuit **Planning** tot **Huidig** of een aangepaste status die gelijk is aan de huidige status. Dit voltooit de integratie en produceert het project, de taken, en om het even welke documenten in Frame.io.

Het pictogram Frame.io naast de projectnaam wordt paars het signaleren van de integratie succesvol. De gebruikers ontvangen een e-mail uitnodigend hen aan het Frame.io project.

>[!IMPORTANT]
>
>Zodra het project voor Frame.io wordt aangesloten, worden de veranderingen die aan de projectgroep worden aangebracht niet weerspiegeld in Frame.io.


