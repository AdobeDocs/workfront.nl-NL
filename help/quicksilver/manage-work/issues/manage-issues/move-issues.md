---
product-area: projects
navigation-topic: manage-issues
title: Problemen verplaatsen
description: U kunt kwesties tussen projecten en taken bewegen.
author: Alina
feature: Work Management
exl-id: 8ab9be3e-0412-43d9-ad1e-75c43613fa82
source-git-commit: 6c82c585376b41cff0e57b253b6a214fb00309de
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 0%

---

# Problemen verplaatsen

U kunt kwesties tussen de volgende voorwerpen bewegen:

* Van een project naar een ander project
* Van een taak aan een andere taak in het zelfde project of in een ander project
* Van een taak aan het project of aan een ander project
* Van een project aan een taak in het zelfde project of een taak in een ander project

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Aanvraag of hoger</p> <p>Controleer of u een hogere licentie hebt om problemen te verplaatsen in de sectie Issues van een project.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot problemen bewerken</p> <p>De mening of hogere toegang tot Projecten en Taken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over toegang tot kwesties in uw Niveau van de Toegang, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Toegang verlenen tot kwesties</a>. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor het probleem beheren</p> <p>Contribute-machtigingen voor het item waarnaar u het probleem verplaatst met de mogelijkheid om problemen toe te voegen.</p> <p> Voor informatie over het verlenen van machtigingen voor uitgaven raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Een uitgave delen </a></p> <p>Voor informatie over het aanvragen van aanvullende machtigingen raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt.

## Overwegingen bij het verplaatsen van problemen

Overweeg het volgende wanneer het bewegen van kwesties die documenten bevatten of met een verzoekrij worden geassocieerd:

* **Wanneer een kwestie met een verzoekrij wordt geassocieerd:** Wanneer u een uitgave naar een ander voorwerp verplaatst en de kwestie met een verzoekrij wordt geassocieerd, wordt de verplaatste kwestie niet meer geassocieerd met de originele rij de eerste kwestie voortkwam uit.
* **Wanneer een document aan de uitgave wordt vastgemaakt:** Als u een uitgave naar een ander object verplaatst en er een document aan gekoppeld is, gaan het document, de versies en proefdrukken ook naar de nieuwe uitgave. Eventuele goedkeuringen die aan het document zijn gekoppeld, worden niet verplaatst.
* **Wanneer een uitgave aan een document of een omslag wordt verbonden:** Wanneer u een uitgave verplaatst waarvoor documenten of mappen zijn gekoppeld aan een externe service zoals Google Drive, worden de koppelingen naar de documenten samen met het probleem verplaatst.

## Uitgaven in een lijst verplaatsen

U kunt een of meerdere problemen verplaatsen vanuit een lijst met problemen of vanuit een probleemrapport.

1. Ga naar het project dat de kwestie of de kwesties bevat die u wilt bewegen.

   of

   Ga naar een probleemrapport.

1. Als u hebt geselecteerd om naar een project te gaan, klikt u op **Problemen** in het linkerdeelvenster.
1. Selecteer de kwestie of de kwesties die u wilt bewegen en klik **Het menu Meer** boven aan de lijst met uitgaven klikt u op **Verplaatsen naar**.

   ![](assets/copy-and-move-to-links-for-issue-in-a-list-nwe-350x119.png)

1. Doorgaan met het verplaatsen van het probleem, zoals beschreven in de sectie [Eén probleem verplaatsen](#move-a-single-issue) beginnen met Stap 2.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: ensure step stays accurate)
   </MadCap:conditionalText>
   -->

## Eén probleem verplaatsen {#move-a-single-issue}

U kunt één probleem verplaatsen wanneer u het bekijkt.

### Eén probleem verplaatsen in de voorvertoningsomgeving

1. Ga naar een probleem dat u wilt kopiëren, klik op de knop **Meer** menu ![](assets/more-icon.png)rechts van de naam van de uitgave selecteert u **Verplaatsen** naar.

   ![](assets/nwe-move-at-issue-level-highlighted-350x579.png)

   De **Probleem verplaatsen** wordt weergegeven.

   ![](assets/move-issue-box-nwe-350x280.png)

1. In de **Doelproject selecteren** de naam van het project opgeven waarin u de problemen wilt verplaatsen. De naam van het huidige project toont door gebrek.

   >[!TIP]
   >
   >Er worden slechts 100 projecten weergegeven in de lijst.

1. (Voorwaardelijk) Klik **aanvraagtoegang** als u geen toegang hebt om kwesties naar het project te verplaatsen.
1. (Voorwaardelijk) blijf de kwestie op het geselecteerde bestemmingsproject bewegen zonder toegang te vragen als u toegang hebt om kwesties aan één van de taken op het bestemmingsproject toe te voegen.

   ![](assets/move-issue-request-access-from-project-nwe-350x118.png)

   >[!TIP]
   >
   >De gelijkaardige berichten tonen als het geselecteerde project in afwachting van goedkeuring, voltooid, of dood is, wanneer de beheerder van Workfront het toevoegen van kwesties aan deze projecten verhindert. Zie voor meer informatie [Projectvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Optioneel) In het dialoogvenster **Opties** Schakel een van de items uit die in de onderstaande tabel worden vermeld om deze te verwijderen uit de verplaatste uitgave. Alle opties zijn standaard geselecteerd.

   >[!IMPORTANT]
   >
   >Als u de selectie van items in de lijst Opties opheft, gaan er gegevens verloren. Informatie uit de bestaande uitgave wordt verwijderd en kan niet worden hersteld.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Alles selecteren</td> 
      <td>Schakel deze optie uit als u alle informatie uit de uitgave wilt verwijderen wanneer u deze naar de nieuwe locatie verplaatst. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Toewijzingen</td> 
      <td>Verwijdert gebruikers, baanrollen, of teams die aan de kwestie worden toegewezen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Voortgang</td> 
      <td>Hiermee verwijdert u het eventuele percentage van de uitgave dat is voltooid. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>Documenten</p></td> 
      <td> <p>Hiermee verwijdert u alle gegevens op het documenttabblad, inclusief documentversies, gekoppelde documenten en mappen.

   <b>OPMERKING</b>

   Als u ervoor kiest om de documenten niet samen met de uitgave te laten verplaatsen, worden de documenten verwijderd en gedurende 30 dagen in de prullenbak geplaatst. Een beheerder kan deze herstellen en ze worden hersteld bij het verplaatste probleem.

   Als de uitgave wordt geschrapt nadat het wordt bewogen, zullen de herstelde documenten in het gebied van Documenten van de gebruikerspagina van de beheerder worden geplaatst die hen herstelt.
   <br> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Machtigingen</td> 
      <td>Hiermee verwijdert u de entiteiten waarmee de uitgave wordt gedeeld. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Updates</td> 
      <td>Hiermee verwijdert u opmerkingen uit de sectie Updates van de uitgave.</td> 
     </tr> 
    </tbody> 
   </table>


1. (Optioneel) In het dialoogvenster **Taak selecteren** selecteert u de taak waar u de uitgave wilt plaatsen.
1. Klikken **Probleem verplaatsen** of **Problemen verplaatsen**, als u meerdere uitgaven in een lijst hebt geselecteerd.

   De verplaatste kwesties worden toegevoegd aan het gespecificeerde project.




