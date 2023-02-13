---
product-area: projects
navigation-topic: manage-issues
title: Uitgaven kopiëren
description: U kunt een uitgave of een verzoek kopiëren en hen op het zelfde of een ander project opslaan. U kunt een kwestie van een taak aan een ander project ook kopiëren.
author: Alina
feature: Work Management
exl-id: a28adc22-825f-401e-9ed2-efddaa297b8d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 0%

---

# Uitgaven kopiëren

U kunt een uitgave of een verzoek kopiëren en hen op het zelfde of een ander project opslaan. U kunt een kwestie van een taak aan een ander project ook kopiëren.

U kunt uitgaven van de volgende voorwerpen kopiëren:

* Van een project aan het zelfde project (dupliceer het op het zelfde project)
* Van een taak naar dezelfde taak (dupliceren als deze zich op dezelfde taak bevindt)
* Van een project naar een ander project
* Van een taak tot een project

>[!TIP]
>
>&quot;Issues&quot; en &quot;request&quot; worden door elkaar gebruikt in Workfront. U kunt kwesties over zowel projecten als taken registreren om op onvoorzien werk te wijzen dat moet worden gericht. U kunt verzoeken ook voorleggen die als kwesties op een project worden geregistreerd dat als Rij van het Verzoek wordt aangewezen.

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
   <td> <p>Aanvraag of hoger</p> <p>U kunt een licentie voor het kopiëren van een uitgave controleren of verhogen in de sectie Issues van een project.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Toegangsniveau*</td> 
   <td> <p>Toegang tot problemen bewerken</p> <p>De mening of hogere toegang tot Projecten en Taken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over toegang tot kwesties in uw Niveau van de Toegang, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Toegang verlenen tot kwesties</a>. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor het probleem beheren</p> <p>Contribute-machtigingen voor het item waarnaar u het probleem kopieert, met de mogelijkheid om problemen toe te voegen.</p> <p> Voor informatie over het verlenen van machtigingen voor uitgaven raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Een uitgave delen </a></p> <p>Voor informatie over het aanvragen van aanvullende machtigingen raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Overwegingen voor problemen die samenhangen met documenten of aanvraagwachtrijen

Overweeg het volgende wanneer het kopiëren van kwesties die documenten bevatten of met een verzoekrij worden geassocieerd:

* **Wanneer een kwestie met een verzoekrij wordt geassocieerd:** Wanneer u een uitgave naar een ander voorwerp kopieert en de kwestie met een verzoekrij wordt geassocieerd, wordt de gekopieerde kwestie niet meer geassocieerd met de originele rij de eerste kwestie voortkwam uit.
* **Wanneer een document aan de uitgave wordt vastgemaakt:** Wanneer u een uitgave naar een ander voorwerp kopieert en de kwestie heeft een document aan het in bijlage, het document en zijn versies zich ook aan de nieuwe kwestie bewegen. Proefdrukken of goedkeuringen die aan het document zijn gekoppeld, worden niet verplaatst.
* **Wanneer een uitgave aan een document of een omslag wordt verbonden:** Wanneer u een uitgave kopieert waarin documenten of mappen zijn gekoppeld aan een externe service zoals Google Drive, worden de koppelingen naar de documenten overgebracht naar de gekopieerde uitgave. 

## Uitgaven kopiëren in een lijst

U kunt een of meerdere uitgaven kopiëren uit een lijst met problemen of uit een uitgiftenrapport.

1. Ga naar het project dat de kwestie of de kwesties bevat die u wilt kopiëren.

   of

   Ga naar een probleemrapport.

1. Als u hebt geselecteerd om naar een project te gaan, klikt u op **Problemen** in het linkerdeelvenster.
1. Selecteer de uitgave of de kwesties die u wilt kopiëren en klik **Het menu Meer** boven aan de lijst met uitgaven klikt u op **Kopiëren naar**.

   ![](assets/copy-issue-in-list-nwe-350x169.png)

1. Doorgaan met het kopiëren van het probleem, zoals beschreven in de sectie [Eén uitgave kopiëren](#copy-a-single-issue) beginnen met Stap 2.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE:&nbsp;ensure step number stays accurate)
   </MadCap:conditionalText>
   -->

## Eén uitgave kopiëren {#copy-a-single-issue}

U kunt één uitgave kopiëren wanneer het bekijken.

1. Ga naar een kwestie die u wilt kopiëren, dan klik **Meer** menu ![](assets/more-icon.png) rechts van de naam van de uitgave, **Kopiëren** naar.

   ![](assets/nwe-copy-at-issue-level-highlighted-350x580.png)

   De **Probleem kopiëren** wordt weergegeven.

   ![](assets/copy-issue-box-nwe-350x285.png)

1. In de **Doelproject selecteren** de naam van het project op waar u de uitgaven wilt kopiëren. De naam van het huidige project toont door gebrek.

   >[!TIP]
   >
   >Er worden slechts 100 projecten weergegeven in de lijst.

1. (Voorwaardelijk) Klik **aanvraagtoegang** als u geen toegang hebt om kwesties aan het project te kopiëren.
1. (Voorwaardelijk) blijf de kwestie aan het geselecteerde bestemmingsproject kopiëren zonder toegang te vragen als u toegang hebt om kwesties aan één van de taken op het bestemmingsproject toe te voegen.

   ![](assets/copy-issue-request-access-from-project-nwe-350x125.png)

   >[!TIP]
   >
   >De gelijkaardige berichten tonen als het geselecteerde project in afwachting van goedkeuring, voltooid, of dood is, wanneer de beheerder van Workfront het toevoegen van kwesties aan deze projecten verhindert. Zie voor meer informatie [Projectvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Optioneel) In het dialoogvenster **Opties** Schakel een van de items uit die in de onderstaande tabel worden vermeld, uit als u deze uit de nieuwe uitgave wilt verwijderen. Alle opties zijn standaard geselecteerd.

   >[!NOTE]
   Dit is alleen van invloed op de gekopieerde problemen, niet op de oorspronkelijke problemen.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Toewijzingen</td> 
      <td>Verwijdert gebruikers, baanrollen, of teams die aan de kwestie worden toegewezen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Voortgang</td> 
      <td>Hiermee verwijdert u het eventuele percentage van de uitgave dat is voltooid. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documenten</td> 
      <td><span style="line-height: 1.5;">Hiermee verwijdert u alle gegevens op het documenttabblad, inclusief documentversies, gekoppelde documenten en mappen.</span> <br>Standaard kunnen proefdrukken en goedkeuringen van documenten niet naar een andere uitgave worden gekopieerd.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Machtigingen</td> 
      <td>Hiermee verwijdert u de entiteiten waarmee de uitgave wordt gedeeld. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Updates</td> 
      <td>Hiermee verwijdert u opmerkingen uit de sectie Updates van de uitgave.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aangepaste gegevens</td> 
      <td>Hiermee verwijdert u de informatie uit het aangepaste formulier over de uitgave en de informatie over de aangepaste formulieren die zijn gekoppeld aan de documenten die bij de uitgave zijn gevoegd, als deze ook met de uitgave zijn gekopieerd. De aangepaste formulieren blijven bij de formulieren en documenten horen, maar de informatie over de formulieren gaat niet over op de nieuwe uitgave. </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optioneel) In het dialoogvenster **Taak selecteren** selecteert u de taak waar u de uitgave wilt plaatsen.
1. Klikken **Uitgave kopiëren** of **Uitgaven kopiëren** als u meerdere uitgaven in een lijst hebt geselecteerd.

   De gekopieerde problemen worden toegevoegd aan het opgegeven project.

 
