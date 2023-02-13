---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: "Voorbeeld van berekend aangepast veld: de manager van de maker van een uitgave weergeven op het aangepaste formulier voor de uitgave"
description: Met behulp van een berekend aangepast veld kunt u de naam van de beheerder van de maker van een uitgave weergeven op een aangepast formulier dat aan de uitgave is gekoppeld. Met dezelfde instructie kunt u vergelijkbare berekende velden maken voor projecten, problemen en andere objecten.
author: Nolan
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# Voorbeeld van berekend aangepast veld: Geef de manager van de maker van een uitgave weer op het aangepaste formulier voor de uitgave

Met behulp van een berekend aangepast veld kunt u de naam van de beheerder van de maker van een uitgave weergeven op een aangepast formulier dat aan de uitgave is gekoppeld. Met dezelfde instructie kunt u vergelijkbare berekende velden maken voor projecten, problemen en andere objecten.

>[!TIP]
>
>Voor meer informatie over extra voorbeelden van de douanetekstmodus van andere klanten, volgt [Rapportage tekstmodus](https://one.workfront.com/s/topic/0TO0z000000cdHmGAI/text-mode-reporting?tabset-21363=3) op onze communautaire site.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront-abonnement*</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront-licentie*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Configuraties op toegangsniveau*</td> 
   <td> <p>Administratieve toegang tot aangepaste formulieren<br>Voor informatie over het verlenen van administratieve toegang van het toegangsniveau, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gebruikers administratieve toegang verlenen tot bepaalde gebieden</a>.</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Objectmachtigingen</p> </td> 
   <td> <p>Contribute opent het object waaraan het formulier is gekoppeld met toegang tot het aangepaste formulier bewerken</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## De manager van de maker van een uitgave weergeven op het aangepaste formulier voor uitgave

In de volgende stappen wordt aangegeven hoe u een berekend veld kunt maken voor een aangepaste uitgave waarin u de naam kunt vastleggen van de manager van de gebruiker die de uitgave heeft gemaakt. Het proces is identiek wanneer u de naam van de manager van een gebruiker wilt vangen die een taak, een project, een portefeuille creeerde, bijvoorbeeld.

1. Maak een aangepast formulier voor uitgave en voeg er een berekend veld aan toe.

   Zie de volgende artikelen voor informatie over het maken van een aangepast formulier en het toevoegen van berekende velden aan dit formulier:

   * [Een aangepast formulier maken of bewerken](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)
   * [Berekende gegevens toevoegen aan een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)

1. Kopieer en plak de volgende code voor de tekstmodus in de **Berekening** veld van het aangepaste formulier:

   ```
   {owner}.{manager}.{name}
   ```

   >[!TIP]
   >
   >Berekeningen van aangepaste velden zijn hoofdlettergevoelig.

1. Klikken **Gereed** vervolgens **Opslaan + Sluiten**.

   De manager van de gebruiker die de kwestie creeerde toont op het berekende gebied wanneer de vorm die het gebied bevat aan een kwestie in bijlage is.
