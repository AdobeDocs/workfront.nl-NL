---
title: Toegang verlenen aan gebruikers
description: Als Adobe Workfront-beheerder kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot andere gebruikers in Workfront te definiëren.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5e87cad4-4a5d-4cb2-848f-7c97ff11d0e8
source-git-commit: 3c5bcb85080a882a8b69bffcd01563a0479f98a5
workflow-type: tm+mt
source-wordcount: '768'
ht-degree: 0%

---


# Toegang verlenen aan gebruikers

Als Adobe Workfront-beheerder kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot andere gebruikers in Workfront te definiëren, zoals wordt uitgelegd in [Overzicht van toegangsniveaus](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Toegang tot gebruikers configureren

U kunt beheren welke informatie gebruikers voor andere gebruikers kunnen bekijken en uitgeven gebruikend een standaardtoegangsniveau of een niveau van de douanetoegang dat u creeert. Gebruikers met het standaardabonnement en de werkvergunningen kunnen de contactinformatie van andere gebruikers bekijken. Een van de volgende gebruikers kan andere gebruikers maken en bewerken:

* Een Workfront-beheerder.

  Zie voor meer informatie [Volledige administratieve toegang verlenen aan een gebruiker](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

* Een gebruiker met een standaardplanvergunning die ook toegang tot gebruikers heeft, zoals die in dit artikel wordt verklaard.

  De gebruikers die beperkt zijn om slechts gebruikers van hun bedrijf of het primaire bedrijf te zien hebben toegang om slechts de gebruikers uit te geven zij kunnen zien. Zie voor meer informatie [Aangepaste toegangsniveaus maken of wijzigen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Een gebruiker met een standaardplanvergunning die ook als manager van een andere gebruiker wordt gespecificeerd.

  De gebruikers die Edit toegang tot gebruikers in hun toegangsniveau worden verleend kunnen gebruikers beheren die aan hen rapporteren. Voor informatie over het beheren van een gebruiker raadpleegt u [Het organigram weergeven](../../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

* Een gebruiker met een standaardlicentie voor abonnementen die een gebruiker heeft gemaakt, kan de gemaakte gebruiker deactiveren, verwijderen of bewerken. Voor informatie over het maken van nieuwe gebruikers raadpleegt u [Gebruikers toevoegen](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## De toegang van gebruikers tot het bewerken van gebruikers configureren met behulp van een aangepast toegangsniveau

1. Beginnen met het maken of bewerken van het toegangsniveau, zoals wordt uitgelegd in [Aangepaste toegangsniveaus maken of wijzigen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. U wijzigt als volgt de mogelijkheid voor gebruikers met een abonnement- of werkvergunning om de profielen van andere gebruikers weer te geven:

   1. Klik op het tandwielpictogram ![](assets/gear-icon-settings.png) op de **Weergave** rechts van **Gebruikers**.

   1. Uitschakelen **Contactgegevens weergeven** Klik vervolgens op de X om het dialoogvenster **Uw instellingen nauwkeurig afstellen** doos.

1. Als u de mogelijkheid wilt wijzigen dat gebruikers met een abonnement toegang krijgen tot andere gebruikers, klikt u op het tandwielpictogram ![](assets/gear-icon-settings.png) op de **Bewerken** rechts van **Gebruikers** Selecteer vervolgens de mogelijkheden die u wilt bieden:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Maken</strong> </td> 
      <td> <p>Hiermee kunnen gebruikers gebruikers maken.<br>Deze optie is standaard ingeschakeld.</p> 
      &lt;!—
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Zorg ervoor dat deze wijziging wordt aangebracht voordat u de 2 opmerkingen ongedaan maakt. Op 3/29 zegt het document-req dat dit afhankelijk is van onderzoeksresultaten.</p>

       &lt;p>&lt;b>OPMERKING&lt;/b>: dit is niet beschikbaar als uw organisatie is aangemeld bij de Adobe Admin Console. Zie uw netwerk of beheerder van IT als u meer informatie nodig hebt.&lt;/p>
       —>  &lt;/td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>Verwijderen</strong> </td> 
      <td> <p> Hiermee kunnen gebruikers de gebruikers verwijderen die ze zelf hebben gemaakt.<br>Deze optie is standaard ingeschakeld.</p> <p><b>OPMERKING</b>: Dit is niet beschikbaar als uw organisatie is aangemeld bij de Adobe Admin Console. Zie uw netwerk of beheerder van IT als u meer informatie nodig hebt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Gebruikersbeheerder (alle gebruikers)</strong> </td> 
      <td> <p>Hiermee kunnen gebruikers het volgende doen voor alle gebruikers in Workfront:</p> 
       <ul> 
        <li>De gebruiker bewerken, verwijderen of deactiveren</li> 
        <li>Aanmelden als gebruiker</li> 
        <li>Het wachtwoord van de gebruiker opnieuw instellen</li> 
       </ul> <p>Deze optie is standaard uitgeschakeld.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Gebruikersbeheerder (Groepgebruikers)</strong> </td> 
      <td> <p>Hiermee kunnen gebruikers het volgende doen voor elke gebruiker in een groep die ze beheren: 
        <ul>
         <li><p>De gebruiker bewerken, verwijderen of deactiveren</p></li>
         <li>Aanmelden als gebruiker</li>
         <li><p>Het wachtwoord van de gebruiker opnieuw instellen</p><p><b>OPMERKING</b>: Een groepsbeheerder kan zich niet aanmelden als of het wachtwoord van een Workfront-beheerder herstellen.</p></li>
        </ul><p>Deze optie is standaard uitgeschakeld.</p></p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Als u groepbeheerders geen toegang tot alle leden van de groepen wilt verlenen die zij beheren, maak beide hierboven opties van Admin van de Gebruiker onbruikbaar. De beheerders van de groep zullen nog tot groepsleden kunnen toegang hebben die zij aan Workfront toevoegen, of die aan hen in Workfront rapporteren.

1. (Optioneel) Als u de toegangsinstellingen wilt configureren voor andere objecten en gebieden in het toegangsniveau waaraan u werkt, gaat u verder met een van de artikelen in [Toegang tot Adobe Workfront configureren](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), zoals [Toegang verlenen tot taken](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) en [Toegang tot financiële gegevens verlenen](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Klik op **Opslaan**.

## Toegang tot gebruikers per licentietype

Zie de sectie voor informatie over wat gebruikers op elk toegangsniveau kunnen doen met gebruikers [Gebruikers](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#users) in het artikel [Beschikbare functionaliteit voor elk objecttype](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
