---
user-type: administrator
content-type: reference;overview
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Gebruikerssynchronisatie tussen Adobe Workfront en Workfront Proof
description: Gebruikersgegevens worden gesynchroniseerd van Adobe Workfront naar Workfront Proof; ze worden niet gesynchroniseerd van Workfront Proof naar Workfront. Daarom moet u deze wijzigingen altijd aanbrengen in Workfront wanneer u gebruikers maakt of wijzigt. U kunt geen wijzigingen aanbrengen in gebruikers in Workfront Proof.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 4c88a249-b156-45c9-a44c-32f906bfa8a2
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Gebruikerssynchronisatie tussen Adobe Workfront en Workfront Proof

Gebruikersgegevens worden gesynchroniseerd van Adobe Workfront naar Workfront Proof; ze worden niet gesynchroniseerd van Workfront Proof naar Workfront. Daarom moet u deze wijzigingen altijd aanbrengen in Workfront wanneer u gebruikers maakt of wijzigt. U kunt geen wijzigingen aanbrengen in gebruikers in Workfront Proof.

In de volgende secties vindt u informatie over gebruikerssynchronisatie van Workfront naar Workfront Proof:

## Informatie die wordt gesynchroniseerd

Workfront synchroniseert de volgende gebruikersgegevens met Workfront Proof:

* Naam (de voor- en achternaam van de gebruiker)
* E-mailadres

## Wanneer synchronisatie plaatsvindt

Gebruikersgegevens worden in de volgende omstandigheden gesynchroniseerd van Workfront naar Workfront Proof:

* Gebruikersgegevens worden bijgewerkt in Workfront
* Een gebruiker is gemaakt in Workfront

Afhankelijk van het feit of een gebruiker met hetzelfde e-mailadres bestaat in Workfront Proof, wordt een van de volgende twee handelingen uitgevoerd:

* **als geen gebruiker met een passende e-mail bestaat in Workfront Proof en**

   * **het Bewijzen wordt toegelaten voor de gebruiker:** de gebruiker wordt gecreeerd als Gebruiker in Workfront Proof.
   * **het Bewijzen wordt niet toegelaten voor de gebruiker:** de gebruiker wordt gecreeerd als Contact in Workfront Proof.

* **als een gebruiker met een passende e-mail in Workfront Proof bestaat:** het Bewijzen wordt toegelaten voor die gebruiker in Workfront (als het niet reeds) werd toegelaten en de informatie wordt gesynchroniseerd tussen de twee gebruikers.

  Voor meer informatie, zie [&#x200B; de het proefdrukken van een gebruiker toegang &#x200B;](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md) in [&#x200B; vormen de het proefdrukken van een gebruiker toegang &#x200B;](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md).

  >[!IMPORTANT]
  >
  >Wanneer een gebruiker met een overeenkomende e-mail in zijn of andere testomgeving aanwezig is, maakt Workfront een e-mailadres voor een alias door de account-id van de gebruiker als achtervoegsel toe te voegen aan de e-mail. Bijvoorbeeld, *username+accountid@domain.com*. Gebruikers ontvangen nog steeds proefdrukken als er een e-mailalias wordt gemaakt.
