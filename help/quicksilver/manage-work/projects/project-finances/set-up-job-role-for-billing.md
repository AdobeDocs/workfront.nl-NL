---
content-type: overview
product-area: projects
navigation-topic: financials
title: Een taakrol instellen voor facturering
description: Met Workfront kunt u een gebruiker met een andere taakrol dan zijn primaire functie factureren. Dit is handig wanneer iemand tijdelijk werk verricht dat met een ander tarief moet worden gefactureerd.
author: Lisa
feature: Work Management
source-git-commit: d92908d358ca53ae9d443fd76556e3e8b273e3cb
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 0%

---

# Een taakrol instellen voor facturering

{{highlighted-preview-article-level}}

Met Workfront kunt u een gebruiker met een andere taakrol dan zijn primaire functie factureren. Dit is handig wanneer iemand tijdelijk werk verricht dat met een ander tarief moet worden gefactureerd.

U kunt een Rol van de Baan voor het Factureren op twee manieren toewijzen:

* Op projectniveau: gebruik dit wanneer de persoon onder dezelfde taakrol voor het volledige project zou moeten worden gefactureerd.
* Op toewijzingsniveau: gebruik deze optie wanneer u specifieke taken anders wilt factureren.

>[!NOTE]
>
>* Een functie voor facturering is alleen van toepassing op personen (gebruikers). Het is niet van toepassing op algemene functies of plaatsaanduidingen voor taken.
>* Het toevoegen van een Rol van de Baan voor het Factureren beïnvloedt slechts het factureringstarief, niet kosten.
>* Facturering op taakniveau heeft altijd voorrang op facturering op projectniveau.

Voor meer informatie, zie [&#x200B; Overzicht van opbrengst en kostenhiërarchie &#x200B;](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) en [&#x200B; creeer geavanceerde taken &#x200B;](/help/quicksilver/manage-work/tasks/assign-tasks/create-advanced-assignments.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td> Toegang tot betaalkaarten bewerken</td> 
  </tr> 
  <tr> 
   <td>Objectmachtigingen</td> 
   <td>Rechten voor het project beheren </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Wijs een Rol van de Baan voor het Factureren op het projectniveau toe

Wanneer u een baanrol voor het factureren van een project creeert:

* De factureringsrol is op alle taken en taken binnen het project voor die gebruiker van toepassing.
* Facturering gebruikt het het factureringspercentage van de geselecteerde baanrol, maar de kosten volgen nog de primaire rol van de gebruiker.

Om een baanrol voor het factureren op het projectniveau toe te wijzen:

1. Open een project.
1. Klik **Middel voor het Factureren** in het linkerpaneel.
1. Selecteer de **rol van de Baan voor het factureren** lusje als het niet reeds wordt getoond.
1. Klik **toevoegen > toevoegt baanrol voor het factureren**.
1. Op **voeg baanrol voor het factureren** doos toe, selecteer de **Gebruiker**.
1. Selecteer de **rol van de Baan** als baanrol voor het factureren voor deze gebruiker op dit project te gebruiken.
1. (Facultatief) klik **toevoegt baanrol** om efficiënte data voor de baanrol voor het factureren te bepalen. Ga het **Begin** en **Eind** data voor de baanrol in.

[Functie toevoegen voor facturering op projectniveau](assets/jrfb-project-level.png)

1. Klik **toevoegt baanrol** opnieuw om extra het factureren rollen voor verschillende tijdsperioden te specificeren.
1. Klik **sparen**.

### Voorbeeld op projectniveau

>[!BEGINSHADEBOX]

John&#39;s belangrijkste functie is Designer 1. Het project vereist een Senior Designer, en John vult in.

U zou de Rol van de Baan voor het Factureren aan **Hogere Designer** op het projectniveau plaatsen.

Resultaat

* Factureringsinkomsten zijn de hoogste Designer-rente
* Kostprijs is de Designer 1-kostenvoet (John&#39;s werkelijke kostenpercentage)

>[!ENDSHADEBOX]

## Een taakrol toewijzen voor facturering op toewijzingsniveau

Wanneer u een baanrol voor het factureren op een taak toevoegt, treedt het plaatsen een project-vlakke het facturerings rol voor slechts die specifieke taak met voeten.

Om een baanrol voor het factureren op het taakniveau toe te wijzen:

1. Open een project en zoek de taak.
1. Ga naar de van de taak **Geavanceerde Taken**.

   Voor informatie, zie [&#x200B; Geavanceerde taken &#x200B;](/help/quicksilver/manage-work/tasks/assign-tasks/create-advanced-assignments.md) creëren.

1. Voor het net van de taaktaak, bepaal de plaats van de kolom **rol van de Baan voor het factureren**.
1. Selecteer een taakrol voor elke toewijzing waar u verschillende facturering wilt.

   >[!NOTE]
   >
   >Als een baanrol voor het factureren op het projectniveau werd toegewezen, verschijnt het op de taak. U kunt op de **rol van de Baan voor het factureren** gebied klikken en een andere baanrol selecteren voor de taak te gebruiken.
   >Het informatiepictogram geeft een melding of een taakrol voor facturering is gedefinieerd op het project of het toewijzingsniveau.

   ![&#x200B; rol van de Baan voor het factureren op een taak &#x200B;](assets/jrfb-assignment-level.png)

### Voorbeeld op toewijzingsniveau

>[!BEGINSHADEBOX]

John&#39;s belangrijkste functie is Designer 1. Op projectniveau wordt hij gefactureerd als Senior Designer, maar er is één speciale taak waarvoor een factureringspercentage van Principal Designer vereist is.

U zou de Rol van de Baan voor Facturering aan Hoofd Designer op die taak slechts plaatsen.

Resultaat

* Al John&#39;s andere taken schrijven als Senior Designer aan
* Deze ene taak factureert als Opdrachtgever Designer
* Kosten blijven Designer 1

>[!ENDSHADEBOX]
