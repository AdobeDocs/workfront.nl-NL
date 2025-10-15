---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Afzonderlijke onderliggende objecten herstellen
description: In dit artikel wordt beschreven hoe u hulp kunt krijgen bij het herstellen van afzonderlijke onderliggende objecten die minder dan 30 dagen geleden zijn verwijderd uit uw Adobe Workfront Production- of Preview-omgeving.
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: e2e4fbb7-5433-4d88-8e36-d82f4cc8a194
source-git-commit: 156341072c291b5c03432da399a509d9772b73ea
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 0%

---

# Afzonderlijke onderliggende objecten herstellen

In dit artikel wordt beschreven hoe u hulp kunt krijgen bij het herstellen van afzonderlijke onderliggende objecten die minder dan 30 dagen geleden zijn verwijderd uit uw Adobe Workfront Production- of Preview-omgeving.

Een beheerder van Workfront kan projecten, taken, kwesties, en documenten in elke instantie van Workfront herstellen, zoals die in [ wordt beschreven herstelt geschrapte punten ](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md). Maar alleen het Workfront-databaseteam kan objecten zoals taken, uitgaven, documenten, aangepaste formulieren, uren en notities, onafhankelijk van het bovenliggende object herstellen.

Gegevens uit uw live omgeving zijn maximaal 7 dagen beschikbaar in de voorvertoningssandbox. Dit betekent dat u de standalone gegevens van het milieu van de Sandbox van de Voorproef kunt uitvoeren gebruikend de volgende methodes:

* Kick-start
* Een rapport maken en de resultaten exporteren

Voor meer informatie over het uitvoeren van gegevens van Workfront, zie [ Gegevens van de Uitvoer ](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

U kunt de geëxporteerde gegevens op de volgende manieren importeren:

* Handmatig als u geëxporteerde rapporten gebruikt
* Als u Kick-Starts in bulk gebruikt

  Voor meer informatie over het invoeren van gegevens in Workfront die Kick-Begint gebruiken, zie [ Gegevens van de Invoer in Adobe Workfront gebruikend een Kick-Begin malplaatje ](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

De omgeving van de zandbak van de Voorproef wordt verfrist tijdens onze onderhoudsvensters tijdens het weekend.

Voor meer informatie over de vensters van onderhoud voor het milieu van de Sandbox van de Voorproef, zie [ de de statusplaats van Adobe ](https://status.adobe.com).

>[!IMPORTANT]
>
>Documenten vormen een uitzondering op deze herstelmethoden. U kunt ze handmatig downloaden vanuit de voorvertoningsomgeving en ze opnieuw uploaden naar de productieomgeving. Als u documenten bulksgewijs wilt downloaden en uploaden, moet u Workfront om gegevensherstel vragen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td>Systeembeheerder</td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Informatie nodig voor het terugzetten van gegevens

Zodra u hebt bepaald dat een geschrapt voorwerp door ons Team van het Gegevensbestand moet worden hersteld, verzamel zo veel informatie aangezien u over het hebt. De volgende informatie wordt vereist voor onze gegevensbestandbeheerders om het voorwerp te vinden en in werking te stellen herstelt:

* Objectnaam
* Objecttype (taak, probleem, project, enz.)
* Geschatte datum en tijdstip van verwijdering
* ObjectGUID (indien mogelijk)

  Verwijs naar de volgende informatie wanneer het bepalen van GUID van een voorwerp:

   * GUID kan worden gevonden door van e-mailberichten van verwijzingen te voorzien die door met het voorwerp (taken aan, commentaren op, enz.) worden teweeggebracht
   * Voorbeeld van een GUID die aan het eind van een URL wordt gevonden: `yourdomain.my.workfront.com/issue/view?ID=568bfa96011220154c8ca4c4e691556b`

Als u deze informatie hebt verzameld of hulp nodig hebt, belt u ons klantenondersteuningsteam op bij 844-306-HELP(4357) of stuurt u een ticket online.

## Gegevensherstelproces

1. Nadat ons klantenondersteuningsteam uw informatie ontvangt, zullen zij het aan ons Team van de Steun van de Klant doorverwijzen.
1. Ons klantenondersteuningsteam zal contact opnemen met ons databaseteam.
1. Zodra het Team van het Gegevensbestand een kans heeft gehad om de gegevens te herzien die worden hersteld, kan een nauwkeurigere schatting voor ETA worden verstrekt. Een terugzetbewerking duurt doorgaans drie dagen, maar kan langer duren, afhankelijk van het type en het volume van de gegevens die worden teruggezet.
1. Het team van het Gegevensbestand zal de informatie aan uw milieu van de Sandbox van de Voorproef herstellen waar u de kans zult hebben om de herstelde gegevens te herzien. Ons klantenondersteuningsteam zal u laten weten wanneer de gegevens in de zandbak van de Voorproef kunnen worden gevonden.
1. Als u tevreden bent met de terugzetbewerking in de sandbox, laat u het ondersteuningsteam van de klant hiervan op de hoogte en neemt u contact op met ons databaseteam om hen te laten weten dat zij de gegevens kunnen terugzetten in uw productieomgeving.
1. U hebt de kans om de herstelde gegevens te controleren voordat het verzoek wordt gesloten.
