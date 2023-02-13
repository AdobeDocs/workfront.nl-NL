---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Gebruikers met een proefdruklicentie weergeven in Adobe Workfront
description: U kunt op een van de volgende manieren bekijken welke gebruikers in Adobe Workfront momenteel de optie "Gebruiker kan proefdrukken genereren" hebben ingeschakeld.
author: Courtney
feature: Digital Content and Documents
exl-id: 4d45ecd9-4348-43a4-9fa7-090b996b4695
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---

# Gebruikers met een proefdruklicentie weergeven in Adobe Workfront

U kunt op een van de volgende manieren bekijken welke gebruikers in Adobe Workfront momenteel de optie &quot;Gebruiker kan proefdrukken genereren&quot; hebben ingeschakeld.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Ouder plan: Selecteren of Premium</p> <p>Voor meer informatie over het proefdrukken van toegang met de verschillende plannen, zie <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Toegang tot proefdrukfunctionaliteit in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toegang bewerken tot:</p> 
    <ul> 
     <li> <p>Rapporten, dashboards en kalenders maken</p> </li> 
     <li> <p>Filters, weergaven en groepen maken</p> </li> 
    </ul> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met de beheerder van de Workfront of Workfront-proefdrukken als u wilt weten welk plan, welke rol of welk proefdrukprofiel u hebt.

## Een gebruikersrapport maken

U kunt een gebruikersrapport maken om te bekijken welke gebruikers proefdrukken kunnen genereren:

1. Navigeren naar **Rapportage** gebied.
1. Klik op de knop **Nieuw rapport** vervolgkeuzemenu en vervolgens op **Gebruikersrapport**.

1. Op de **Filters** tabblad, klikt u op **Filterregel toevoegen**.

1. Vouw in het beschikbare veld de **Gebruiker** en klik vervolgens op **Bevat proeflicentie**.

1. Selecteren **Gelijk** > **Waar**.

   ![report_prooflicenses.png](assets/report-prooflicenses-350x135.png)

1. Klikken **Opslaan en sluiten**.

   In het rapport worden alle gebruikers in Workfront weergegeven waaraan een testlicentie is toegewezen.

## De weergave Personen bijwerken

U kunt een nieuwe kolom in de weergave Personen toevoegen om te bekijken welke gebruikers proefdrukken kunnen genereren:

1. Ga naar de **Mensen** gebied.
1. Klik op de knop **Mensen** tab.
1. In de **Weergave** Voer een van de volgende handelingen uit in het keuzemenu:

   * Als u deze informatie aan een bestaande weergave wilt toevoegen, selecteert u de weergave die u wilt aanpassen en klikt u op **Weergave aanpassen**.
   * Als u deze gegevens aan een nieuwe weergave wilt toevoegen, klikt u op **Nieuwe weergave**.

1. Klikken **Kolom toevoegen**.
1. Vouw in het beschikbare veld de **Gebruiker** en klik vervolgens op **Bevat proeflicentie**.

1. Klikken **Gereed** en klik vervolgens op **Weergave opslaan** of **Opslaan als nieuwe weergave**.

   De weergave wordt weergegeven **Waar** of **Onwaar** afhankelijk van de vraag of de gebruiker een bewijs van bevoegdheid heeft toegewezen aan hen.
