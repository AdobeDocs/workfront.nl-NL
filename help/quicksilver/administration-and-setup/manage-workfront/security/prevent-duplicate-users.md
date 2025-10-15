---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: Dubbele gebruikers voorkomen
description: Wanneer u een nieuwe gebruiker in Adobe Workfront maakt, kunt u geen e-mailadres meer gebruiken dat al door een andere gebruiker wordt gebruikt, zelfs als het e-mailadres per geval verschilt (bijvoorbeeld JohnDoe@example.com en johndoe@example.com). Als u zich wilt voorbereiden op toekomstige verificatieverbeteringen, moet u ervoor zorgen dat alle gebruikers een uniek e-mailadres hebben in een Workfront-exemplaar.
author: Becky, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 84d9a752-e894-42cf-9b40-375e35f02c97
source-git-commit: 6b2d93d2573d72e4390761038d8078f47d96d55e
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# Dubbele gebruikers voorkomen

Wanneer u een nieuwe gebruiker in Adobe Workfront maakt, kunt u geen e-mailadres meer gebruiken dat al door een andere gebruiker wordt gebruikt, zelfs als het e-mailadres per geval verschilt (bijvoorbeeld JohnDoe@example.com en johndoe@example.com). Als u zich wilt voorbereiden op toekomstige verificatieverbeteringen, moet u ervoor zorgen dat alle gebruikers een uniek e-mailadres hebben in een Workfront-exemplaar.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Standard</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Gebruikers met unieke e-mailadressen maken

Vanaf de release 2019.4 kunt u bij het maken van een nieuwe gebruiker in Workfront geen e-mailadres meer gebruiken dat al door een andere gebruiker wordt gebruikt, zelfs als het e-mailadres per geval verschilt. U kunt bijvoorbeeld niet één gebruiker maken met het e-mailadres JohnDoe@example.com als een andere gebruiker het e-mailadres johndoe@example.com heeft.

## E-mailadressen van bestaande gebruikers in uw Workfront-exemplaar bijwerken

Als Workfront-beheerder moet u bestaande gebruikers bijwerken die overeenkomstige e-mailadressen hebben die alleen per geval verschillen.
Dubbele e-mailadressen in een Workfront-exemplaar corrigeren:

1. Bekijk eventuele dubbele gebruikers en bepaal welke gebruiker niet langer nodig is.

   {{step-1-to-users}}

   1. In het **menu van de Filter**, uitgezochte **allen**.

   1. In het **menu van de Mening**, uitgezochte **Login van de Gebruiker**.

   1. In het **Groeperende** menu, uitgezochte **niets**.

   1. Pas de weergave Gebruikersaanmelding aan.

      1. Klik **Mening** > **aanpassen Mening**.

      1. Vervang de **identiteitskaart** kolom met de **E-mailE-mailAdres** kolom.

      1. Wijzig de naam van de weergave en sla deze op.

   1. Maak een nieuwe groep.

      1. Klik **Groepering** > **Nieuwe Groepering**.

      1. Klik **Schakelaar aan de Wijze van de Tekst** in de hoger-juiste hoek van de pagina.
      1. Plak de volgende code voor de tekstmodus:

         `group.0.linkedname=direct`
         `group.0.namekey=emailAddr`
         `group.0.valueexpression=LOWER({emailAddr})`
         `group.0.valueformat=string`
         `textmode=true`

   1. Wijzig de naam van de groep en sla deze op.

1. Voer een van de volgende handelingen uit:

   * (Voorkeursmethode) Voeg een +-adres toe aan het e-mailadres van de gebruiker voor elke extra account.

     Kies deze optie als één gebruiker in uw organisatie toegang tot meer dan 1 gebruikersaccount nodig heeft. Als het plus richten niet door uw e-mailleverancier wordt gesteund, moet u een afzonderlijke e-mailrekening voor elke Workfront rekening verstrekken.

     John Doe kan bijvoorbeeld één gebruikersaccount voor zijn account voor dagelijks gebruik hebben en één voor testdoeleinden:

      * johndoe@workfront.com
      * johndoe+reviewer@workfront.com

   * Wijzig het domein om een vals domein te gebruiken door de volgende tekst aan het e-mailadres toe te voegen:

     `.inactive`

     Jan Doe zou bijvoorbeeld de volgende domeinen kunnen hebben: (Deze moeten uniek zijn.)

      * johndoe@workfront.inactive
      * johndoe@workfront.inactive2

     U kunt zich niet meer aanmelden bij deze accounts omdat opnieuw instellen van het wachtwoord een geldig e-mailadres vereist. Deze accounts zijn alleen toegankelijk met de functie Aanmelden als.

   * Onbenodigde gebruikers verwijderen

     >[!IMPORTANT]
     >
     >Kies deze optie alleen voor accounts die per ongeluk zijn gemaakt of voor testaccounts. Deze optie wordt meestal alleen uitgevoerd voor accounts met een verkeerde aanmelding of een verkeerde aanmelding. Rekeningen die regelmatig zijn gebruikt, mogen nooit worden verwijderd.

Als u gebruikers hebt in een Workfront-exemplaar met overeenkomende e-mailadressen die alleen per geval verschillen, neemt Workfront contact met u op met aanvullende informatie en een tijdlijn wanneer deze moeten worden bijgewerkt.
