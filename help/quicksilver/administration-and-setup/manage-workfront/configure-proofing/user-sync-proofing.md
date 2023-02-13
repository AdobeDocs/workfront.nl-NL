---
user-type: administrator
content-type: reference;overview
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Gebruikerssynchronisatie tussen Adobe Workfront en Workfront Proof
description: Gebruikersgegevens worden gesynchroniseerd van Adobe Workfront naar Workfront Proof; wordt niet gesynchroniseerd van Workfront Proof naar Workfront. Daarom moet u deze wijzigingen altijd aanbrengen in Workfront wanneer u gebruikers maakt of wijzigt. U kunt geen wijzigingen aanbrengen aan gebruikers in de Workfront-proefdruk.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 4c88a249-b156-45c9-a44c-32f906bfa8a2
source-git-commit: b310e36c9eb148db631e7a3552a35dcccc652d60
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Gebruikerssynchronisatie tussen Adobe Workfront en Workfront Proof

Gebruikersgegevens worden gesynchroniseerd van Adobe Workfront naar Workfront Proof; wordt niet gesynchroniseerd van Workfront Proof naar Workfront. Daarom moet u deze wijzigingen altijd aanbrengen in Workfront wanneer u gebruikers maakt of wijzigt. U kunt geen wijzigingen aanbrengen aan gebruikers in de Workfront-proefdruk.

In de volgende secties vindt u informatie over gebruikerssynchronisatie van Workfront naar Workfront Proof:

## Informatie die wordt gesynchroniseerd

Workfront synchroniseert de volgende gebruikersgegevens met Workfront Proof:

* Naam (de voor- en achternaam van de gebruiker)
* E-mailadres

## Wanneer synchronisatie plaatsvindt

Gebruikersgegevens worden in de volgende omstandigheden gesynchroniseerd van Workfront naar Workfront Proof:

* Gebruikersgegevens worden bijgewerkt in Workfront
* Een gebruiker is gemaakt in Workfront

Afhankelijk van het feit of een gebruiker met hetzelfde e-mailadres aanwezig is in de Workfront Proof, wordt een van de volgende twee handelingen uitgevoerd:

* **Als er geen gebruiker met een overeenkomende e-mail bestaat in Workfront Proof en**

   * **Proofing is ingeschakeld voor de gebruiker:** De gebruiker wordt gemaakt als een gebruiker in Workfront Proof.
   * **Proofing is niet ingeschakeld voor de gebruiker:** De gebruiker wordt aangemaakt als contactpersoon in Workfront Proof.

* **Als er een gebruiker met een overeenkomende e-mailadres bestaat in Workfront Proof:** Proofing is ingeschakeld voor die gebruiker in Workfront (als deze nog niet was ingeschakeld) en informatie wordt gesynchroniseerd tussen de twee gebruikers.

   Zie voor meer informatie [De proefdruktoegang van een gebruiker configureren](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md) in [De proefdruktoegang van een gebruiker configureren](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md).

   >[!IMPORTANT]
   >
   >Wanneer een gebruiker met een overeenkomende e-mail in zijn of andere testomgeving aanwezig is, maakt Workfront een e-mailadres voor een alias door de account-id van de gebruiker als achtervoegsel toe te voegen aan de e-mail. Bijvoorbeeld: *username+accountid@domain.com*. Gebruikers ontvangen nog steeds proefdrukken als er een e-mailalias wordt gemaakt.
