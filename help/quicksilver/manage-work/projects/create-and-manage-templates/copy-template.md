---
product-area: templates
navigation-topic: templates-navigation-topic
title: Een projectsjabloon kopiëren
description: Naast het creëren van een projectmalplaatje van kras, kunt u bestaande ook kopiëren en het wijzigen.
author: Alina
feature: Work Management
exl-id: b2e0878b-8245-4e01-819d-c3746f553d95
source-git-commit: 0d968a3f398c2e7dc4154cd5a16acf35ca7c86f5
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---

# Een projectsjabloon kopiëren

<!--Audited: 5/2025-->

Naast het maken van een geheel nieuwe projectsjabloon kunt u ook een bestaande sjabloon kopiëren en wijzigen in Adobe Workfront.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td><p>Nieuw: Standaard</p> 
   <p>Huidig: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot sjablonen bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen voor een sjabloon weergeven of vergroten</p>  </td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen bij het kopiëren van sjablonen

De volgende items worden altijd van een bestaande sjabloon naar een nieuwe gekopieerd:

* Sjabloontaken
* Standaardinformatie sjabloontaak (standaardgoedkeuringsproces taak, standaard aangepaste Forms)
* Aangepaste formulieren
* Risico&#39;s
* Informatie over wachtrijinstellingen
* Portfolio en Programma
* Goedkeuringen
* Documenten
* De dagen van de oorspronkelijke sjabloontaken worden overgedragen naar de nieuwe sjabloon. U moet de dag van het Begin of van de Voltooiing van het malplaatje (afhankelijk van zijn Wijze van het Programma) veranderen om de dagen op de malplaatjetaken bij te werken, indien nodig.

De volgende items worden nooit van een bestaande sjabloon naar een nieuwe gekopieerd:

* Factureringstarieven
* Opmerkingen van gebruikers

## Een sjabloon kopiëren


<!--ensure steps and casing on the fields and buttons is accurate with unshim-->

1. Ga naar de sjabloon die u wilt kopiëren.
1. Klik het **Meer** menu ![ Meer pictogram ](assets/qs-more-icon-on-an-object.png) aan het recht van de malplaatjenaam in de kopbal, dan klik **Exemplaar**.

   Het **vakje van het Malplaatje van het Exemplaar** opent.

   <!--![Copy template box](assets/copy-template-box.png)-->

1. Specificeer een naam voor het malplaatje op het **Nieuwe gebied van de Naam van het Malplaatje**.

   Standaard is de nieuwe naam `Copy of Original template name` .

1. Selecteer **gebruikerstaken van het Behouden op taken en malplaatje** optie, als u alle taak en malplaatjetoewijzingen van het originele malplaatje aan het nieuwe malplaatje wilt dragen. De taaktoewijzingen van het malplaatje, en de Eigenaar en Sponsor van het Malplaatje worden overgebracht naar het gekopieerde malplaatje.
1. Klik **sparen** om een exemplaar van het malplaatje tot stand te brengen.

   De nieuwe sjabloon wordt weergegeven in de sjabloonlijst in het gedeelte Sjabloon van Workfront.
