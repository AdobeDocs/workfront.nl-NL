---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Power BI-hulpprogramma kan geen verbinding maken met het opgegeven wachtwoord
description: Wanneer u zich probeert aan te melden bij Data Connect vanuit uw Power BI-hulpprogramma, ontvangt u een aanmeldingsfout.
author: Courtney
feature: Reports and Dashboards
source-git-commit: 40050915153af6e1f70024461e193fb536d74e35
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---


# Power BI kan geen verbinding maken met het opgegeven wachtwoord

## Probleem

Wanneer u zich probeert aan te melden bij Data Connect vanuit uw Power BI-hulpprogramma, wordt de volgende fout weergegeven:

`Cannot connect from BI tool with provided password`

## Oorzaak

Bij het maken van de JDBC-verbinding geeft Workfront een tijdelijk wachtwoord op voor Data Connect.

Voordat u Data Connect kunt openen via Power BI, moet u zich eerst aanmelden met de opgegeven verbindingsgegevens, het tijdelijke wachtwoord bijwerken en vervolgens doorgaan met uw aanmelding.


## Oplossing

Stel het verbindingswachtwoord in Workfront opnieuw in en maak vervolgens een nieuw wachtwoord met de koppeling in het dialoogvenster Verbinding bewerken.

### Verbindingswachtwoord in Workfront opnieuw instellen

1. Ga naar Workfront > Setup > System > Data Connect.
1. De verbinding zoeken en openen vanuit de lijst.
1. Onder **het Wachtwoord van de Verbinding van het Terugstellen**, controleer de doos om te bevestigen dat u het wachtwoord wilt terugstellen.
1. Klik **het Wachtwoord van de Verbinding van het Terugstellen**.
   ![ teruggestelde verbindingswachtwoord ](assets/reset-password.png)
1. Ga verder met de onderstaande sectie.

### Een nieuw wachtwoord voor de verbinding maken

1. Kopieer de URL en plak deze in een nieuw browsertabblad.
1. Kopieer in Workfront de naam van de verbindingsgebruiker en het standaardwachtwoord naar het nieuwe browsertabblad.
   ![ exemplaar URL en standaardwachtwoord ](assets/link-password.png)
1. Klik **binnen Teken**.
1. Ga een nieuw wachtwoord in, dan klik **voorleggen**.
1. Ga naar de Power BI-tool en meld u aan met het nieuwe wachtwoord.

