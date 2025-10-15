---
title: Projectfinanciën opnieuw berekenen
product-area: projects
navigation-topic: financials
description: De financiën worden berekend op een project aangezien de veranderingen in de uren voorkomen die voor het project worden geregistreerd of in de tarieven die worden gebruikt om kosten en opbrengst te berekenen.
author: Lisa
feature: Work Management
exl-id: 5a90c5a1-8b26-4b6f-b9ec-f446a2e94ff0
source-git-commit: 23a4d055871c9138818e70fa1cd936581dbd7552
workflow-type: tm+mt
source-wordcount: '1609'
ht-degree: 0%

---

# Projectfinanciën opnieuw berekenen

De financiën worden berekend op een project aangezien de veranderingen in de uren voorkomen die voor het project worden geregistreerd of in de tarieven die worden gebruikt om kosten en opbrengst te berekenen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td>Alle </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td>Toegang tot projecten en financiële gegevens bewerken</td> 
  </tr> 
  <tr> 
   <td>Objectmachtigingen</td> 
   <td>Machtigingen voor het project beheren met beheerdersmachtigingen</td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen bij het berekenen van de financiën in Adobe Workfront

De financiële middelen voor projecten worden als volgt berekend:

* U kunt kosten en opbrengsten op een project manueel opnieuw berekenen, door de optie van de Financiën van de Herberekening op een project te gebruiken.
* Daarnaast wordt door sommige handelingen een automatische herberekening gestart.

Wanneer het tarief van een gebruiker of een rol tijdens het leven van een project verandert, kan het volgende voorkomen:

* Wanneer de verandering wordt aangebracht, wordt het bijgewerkte tarief gebruikt vanaf dat punt op aangezien de uren worden geregistreerd en de financiële informatie wordt berekend. Het wijzigen van de snelheid heeft geen invloed op de manier waarop de gegevens zijn berekend voordat de wijziging is aangebracht. Voor alle bestaande geregistreerde uren, wordt het oude tarief gebruikt om financiële informatie te berekenen.
* U kunt Adobe Workfront dwingen om het nieuwe tarief voor alle uren terug te gebruiken die tot nu zijn geregistreerd, door de Recalculate optie van de Financiën te gebruiken. Dit dwingt Workfront alle eerder ingelogde uren, geplande kosten en inkomsten met terugwerkende kracht te herberekenen overeenkomstig de nieuwe tariefinformatie.

Het rapporttype Project (Financiële Gegevens) voert niet automatisch een herberekening van uw financiële gegevens uit. Als u de gegevens in dit rapporttype wilt bijwerken, moet u de financiën voor afzonderlijke projecten handmatig opnieuw berekenen.

>[!CAUTION]
>
>Voordat u de financiën voor een bepaald project handmatig opnieuw berekent, wilt u mogelijk alle financiële gegevens behouden die al zijn berekend op basis van een eerder percentage. We raden u aan de optie Financiën opnieuw berekenen alleen te gebruiken als u zeker weet dat u geen wijzigingen aanbrengt in bestaande gegevens of alleen als dergelijke wijzigingen gewenst zijn.

## Financiële gegevens behouden voor taken met bestaande uren {#preserve-financial-data-for-tasks-with-existing-hours}

Wanneer de financiële gegevens voor een project opnieuw worden berekend, herberekent Workfront met terugwerkende kracht alle eerder geregistreerde uren, geplande, werkelijke kosten en geplande en daadwerkelijke inkomsten, overeenkomstig om het even welke nieuwe of bijgewerkte financiële informatie.

* [&#x200B; Behoud de Ontvangsten van het Project &#x200B;](#preserve-project-revenue)
* [Projectkosten behouden](#preserve-project-cost)

### Ontvangsten van project behouden  {#preserve-project-revenue}

De inkomstenpercentages kunnen tijdens de levensduur van een project veranderen.

Voor meer informatie over het factureren van tarieven en opbrengst, zie het artikel [&#x200B; Overzicht van het Factureren en de Ontvangsten &#x200B;](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

De belastingtarieven kunnen op de volgende niveaus veranderen:

* Het systeemniveau (voor functies)\
  Voor meer informatie over het creëren van baanrollen met het factureren van tarieven op het systeemniveau, zie het artikel [&#x200B; baanrollen &#x200B;](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md) creëren en beheren.

* Het gebruikersniveau\
  Voor meer informatie over het veranderen van de het facturerings tariefinformatie over gebruikers, zie het artikel [&#x200B; uitgeven het profiel van een gebruiker &#x200B;](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Het niveau van het Bedrijf (voor baanrollen)\
  Voor meer informatie, zie [&#x200B; het factureren van de baanrol van de Opheffing tarieven op het bedrijfsniveau &#x200B;](../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

* Het projectniveau (voor functies)\
  Voor meer informatie over het met voeten treden van baanroltarieven op het projectniveau, zie het artikel [&#x200B; Overzicht van het met voeten treden van de Factureringsriten van de Rol van de Taak en het berekenen van Inkomsten op een project &#x200B;](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

Bijvoorbeeld, verandert het het facturerings tarief van een gebruiker tijdens een project van $50 in $75 per uur en u wilt alle bestaande gegevens aan het oude tarief ($50 en uur) worden berekend. Wanneer de projectfinanciën echter opnieuw worden berekend, worden de inkomsten van taken die al over bestaande financiële gegevens beschikken aangepast aan de nieuwe factureringsgraad (van $75 per uur).

* [&#x200B; Behoud de Inkomsten van het Project door een het Factureren Verslag &#x200B;](#preserve-project-revenue-by-creating-a-billing-record) te creëren
* [De Ontvangsten van het Project van het behoud door veelvoudige het Tarief met voeten te treden](#preserve-project-revenue-by-using-multiple-billing-rate-overrides)

#### Projectinkomsten behouden door een factureringsrecord te maken {#preserve-project-revenue-by-creating-a-billing-record}

Wanneer de factureringstarieven op om het even welk hierboven vermeld niveau veranderen, kunt u bestaande die reeds op het project is berekend bewaren door te vermijden om de handmatige optie van de Herberekening van Financiën te gebruiken of door de tijd te sluiten die op het project wordt geregistreerd en berekend gebruikend het oude tarief in een het facturerings verslag met een status van Facturering.

Wanneer u geen financiën op het project opnieuw berekent of wanneer u de uren sluit die in een factureringsverslag worden geregistreerd, zullen de uren na de tariefveranderingen na het tarief worden geregistreerd met het nieuwe tarief berekenen, en de uren die vóór de veranderingen van het kostentarief worden geregistreerd blijven berekend bij het oude tarief.

Voor meer informatie over het creëren van het factureren verslagen, zie het artikel [&#x200B; het factureren verslagen &#x200B;](../../../manage-work/projects/project-finances/create-billing-records.md) creëren.

#### De Ontvangsten van het Project van het behoud door veelvoudige het Tarief met voeten te treden {#preserve-project-revenue-by-using-multiple-billing-rate-overrides}

Wanneer de factureringstarieven voor baanrollen op het projectniveau veranderen, kunt u bestaande opbrengst behouden die reeds op het project is berekend door veelvoudige het facturerings tariefoverschrijvingen te gebruiken die binnen een gespecificeerd tijdkader worden gesloten.

Voor meer informatie over het gebruiken van veelvoudige het factureren tariefoverschrijvingen, zie het artikel [&#x200B; Overzicht van het met voeten treden van de FactureringsRates van de Rol van de Taak en het berekenen van Inkomsten op een project &#x200B;](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

>[!NOTE]
>
>Dit is alleen van toepassing op de factureringstarieven voor de rol die op projectniveau worden gewijzigd.

### Projectkosten behouden {#preserve-project-cost}

De kostentarieven kunnen op de volgende niveaus veranderen:

* Systeemniveau (voor functies)\
  Voor meer informatie over het creëren van baanrollen met kostentarieven op het systeemniveau, zie het artikel [&#x200B; creëren en baanrollen beheren &#x200B;](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Gebruikersniveau\
  Voor meer informatie over het veranderen van de informatie van het kostentarief over gebruikers, zie het artikel [&#x200B; uitgeven het profiel van een gebruiker &#x200B;](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Wanneer de factureringstarieven op om het even welk hierboven vermeld niveau veranderen, kunt u bestaande die kosten bewaren die reeds op het project zijn berekend door de tijd te sluiten die op het project wordt geregistreerd en die aan het oude tarief wordt berekend in een facturerings verslag met een status van Factureerde. Voor meer informatie over het creëren van het factureren verslagen, zie het artikel [&#x200B; het factureren verslagen &#x200B;](../../../manage-work/projects/project-finances/create-billing-records.md) creëren.

U kunt ook vermijden gebruikend de handmatige Recalculate optie van Financiën, als u geen het facturerings verslag wilt tot stand brengen, zoals die in de sectie [&#x200B; wordt beschreven manueel financiën voor een project &#x200B;](#manually-recalculate-finances-for-a-project) in dit artikel herberekenen.

Wanneer u geen financiën op het project opnieuw berekent of wanneer u de uren sluit die in een factureringsverslag worden geregistreerd, zullen de uren na de tariefveranderingen na het tarief worden geregistreerd met het nieuwe tarief berekenen, en de uren die vóór de veranderingen van het kostentarief worden geregistreerd blijven berekend bij het oude tarief.

## De financiën van een project handmatig opnieuw berekenen {#manually-recalculate-finances-for-a-project}

Als uw tarieven tijdens de levensduur van een project veranderen en u uw kosten en opbrengstberekeningen de nieuwe tarieven wilt weerspiegelen, moet u de financiën op het project manueel opnieuw berekenen.

>[!NOTE]
>
>U kunt opbrengstwaarden van het bijwerken verhinderen om op de nieuwe tarieven te wijzen wanneer u manueel financiën herberekent door de stappen in de sectie [&#x200B; financiële gegevens voor taken met bestaande uren &#x200B;](#preserve-financial-data-for-tasks-with-existing-hours) van dit artikel te volgen. Kostenwaarden worden altijd bijgewerkt om de nieuwe tarieven weer te geven wanneer u de financiën handmatig herberekent voor een project.

U kunt de financiën van projecten in Workfront van de projectpagina of van een projectlijst of rapport herberekenen.

U kunt de financiën opnieuw berekenen terwijl u ze bulksgewijs bewerkt. Voor informatie, zie [&#x200B; financiën in bulk &#x200B;](#manually-recalculate-finances-in-bulk) sectie in dit artikel manueel opnieuw berekenen.

1. Ga naar het project waar u financiën wilt opnieuw berekenen en **Meer** pictogram ![&#x200B; klikken Meer menu &#x200B;](assets/qs-more-icon-on-an-object.png) rechts van de projectnaam.

   ![&#x200B; het niveau van het Project meer dropdown &#x200B;](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   of

   Ga naar een projectlijst of een rapport en selecteer één of verscheidene projecten, dan klik **Meer** pictogram ![&#x200B; Meer menu &#x200B;](assets/qs-more-icon-on-an-object.png) bij de bovenkant van de lijst.

   ![&#x200B; herberekenen uitdrukkingen &#x200B;](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >Afhankelijk van de complexiteit van uw projecten raden we u aan geen groot aantal projecten te selecteren wanneer u de financiën in bulk herberekent voor optimale prestaties. Sommige dingen die een project te complex zouden kunnen maken zouden veelvoudige gebiedsdelen of taken of een groot aantal douanevelden kunnen zijn.

1. Klik **opnieuw berekenen Financiën**.

   Alle geplande kosten en inkomsten van het project worden opnieuw berekend met nieuwe informatie.

   U zou een bevestiging bij de bovenkant van browser moeten ontvangen dat de financiën van het project met succes zijn herberekend.
Bestaande kostenwaarden en sommige inkomstenwaarden die niet vergrendeld zijn, worden bijgewerkt om de nieuwe tarieven weer te geven.

## De financiën handmatig opnieuw bulksgewijs berekenen{#manually-recalculate-finances-in-bulk}

U kunt de financiën van verschillende projecten handmatig opnieuw berekenen door ze bulksgewijs te bewerken. Hierdoor worden de inkomsten van de projecten met terugwerkende kracht opnieuw berekend.

>[!IMPORTANT]
>
>U kunt opbrengstwaarden van het bijwerken verhinderen om op de nieuwe tarieven te wijzen wanneer u manueel financiën herberekent door de stappen in de sectie [&#x200B; financiële gegevens voor taken met bestaande uren &#x200B;](#preserve-financial-data-for-tasks-with-existing-hours) van dit artikel te volgen. Kostenwaarden worden altijd bijgewerkt om de nieuwe tarieven weer te geven wanneer u de financiën voor projecten handmatig herberekent.

De financiering van verschillende projecten handmatig herberekenen:

1. Ga naar een lijst met projecten.
1. Selecteer verscheidene projecten in de lijst, dan klik het **Meer** pictogram ![&#x200B; Meer menu &#x200B;](assets/qs-more-icon-on-an-object.png) bij de bovenkant van de lijst.

   ![&#x200B; herberekenen uitdrukkingen &#x200B;](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >Afhankelijk van de complexiteit van uw projecten raden we u aan geen groot aantal projecten te selecteren wanneer u deze in bulk bewerkt, zodat u optimale prestaties krijgt. Sommige dingen die een project te complex zouden kunnen maken zouden veelvoudige gebiedsdelen of taken of een groot aantal douanevelden kunnen zijn.

1. Klik **opnieuw berekenen Financiën**.

   Alle geplande kosten en ontvangsten voor de geselecteerde projecten worden opnieuw berekend met nieuwe informatie.

   U zou een bevestiging bij de bovenkant van browser moeten ontvangen dat de financiën van de projecten met succes zijn herberekend.

## Acties die een automatische herberekening van de financiën in gang zetten

De volgende acties leiden tot de financiële herberekening van projecten in Workfront:

* Taakstatus wijzigen
* Een taak met uren verplaatsen naar een ander project
* De projectstatus wijzigen van Voltooid in een actieve status

>[!NOTE]
>
>Wanneer u de projectstatus wijzigt, worden alleen de geplande waarden opnieuw berekend.

U kunt financiën ook manueel onder **opnieuw berekenen Meer** menu ![&#x200B; Meer menu &#x200B;](assets/qs-more-menu.png) op het projectniveau, door **te klikken herberekent Financiën**.
