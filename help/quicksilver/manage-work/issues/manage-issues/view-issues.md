---
product-area: projects
navigation-topic: manage-issues
title: Problemen weergeven
description: U kunt kwesties bekijken die met een project, een taak, of een herhaling worden geassocieerd.
author: Alina
feature: Work Management
exl-id: b6791c8f-b356-4235-8b0e-952e29a88952
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1038'
ht-degree: 0%

---

# Problemen weergeven

U kunt kwesties bekijken die met een project, een taak, of een herhaling worden geassocieerd.

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
   <td> <p>Aanvraag of hoger</p> <p>Controleer of u een hogere licentie hebt om problemen weer te geven in de sectie Issues van een project.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot problemen bekijken</p> <p>De mening of hogere toegang tot Projecten en Taken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over toegang tot kwesties in uw Niveau van de Toegang, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Toegang verlenen tot kwesties</a>. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen weergeven voor de uitgave</p> <p> Voor informatie over het verlenen van machtigingen voor uitgaven raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Een uitgave delen </a></p> <p>Voor informatie over het aanvragen van aanvullende machtigingen raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Problemen weergeven die zijn gebaseerd op status

Om kwesties over een project, een taak, of een herhaling te bekijken:

1. Open een project, een taak, of een herhaling die kwesties bevat, dan klik **Problemen** in het linkerdeelvenster.

1. Als u alle, geopende of afgesloten problemen wilt weergeven, klikt u op een van de onderstaande filters in het menu **Filter** vervolgkeuzemenu.

>[!TIP]
>
>De lijst met filters varieert afhankelijk van wat uw systeem of groepsbeheerder heeft geselecteerd om in de lijst weer te geven.

* **Openen:** Hier worden de geopende problemen weergegeven.

   Dit geldt ook voor objecten die zijn gekoppeld aan een object Resolving en objecten in de status Gesloten - In afwachting van goedkeuring.

   Voor informatie over het oplossen van voorwerpen, zie [Overzicht van Oplossende en Oplosbare objecten](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

* **Voltooid:** Hiermee geeft u alle problemen weer die een werkelijke voltooiingsdatum hebben.
* **Alles** Hiermee geeft u alle problemen weer.

## Informatie over problemen begrijpen

U kunt informatie over een kwestie bekijken wanneer u tot het toegang hebt.

Ga als volgt te werk om een uitgave te openen en informatie hierover weer te geven:

1. Open een project, een taak, of een herhaling die kwesties bevat, dan klik **Problemen** in het linkerdeelvenster.
1. Van de **Filter** selecteert u het filter om de problemen weer te geven die u wilt bekijken.

   Selecteer een van de volgende opties:

   * Open
   * Voltooid
   * Alles

1. Klik op de naam van een uitgave.

   Wanneer u beheerdersmachtigingen voor de uitgave hebt, kunt u elk bewerkbaar veld in de uitgave bewerken en goedkeuringen, uren of documenten aan de uitgave toevoegen.

1. Klik in het linkerdeelvenster op een van de volgende opties om meer informatie over het probleem weer te geven:

* **Updates**: U kunt de volgende handelingen uitvoeren:

   * Opmerking over de kwestie of antwoord op een bestaande opmerking.
   * Logtijd.
   * Wijzig de status van de uitgave.

      Ga voor meer informatie over het bijwerken van werkzaamheden in Workfront naar [Werk bijwerken](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* **Documenten**: Voeg documenten toe aan de uitgave. Ga voor meer informatie over het toevoegen van documenten aan Workfront naar [Documenten vanuit uw bestandssysteem toevoegen aan Adobe Workfront](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

* **Probleemdetails**: Deze koppeling uitvouwen om de **Overzicht** en **Aangepaste Forms** gebieden.

   Als u beheerdersmachtigingen voor de uitgave en bewerkingsrechten voor het aangepaste formulier hebt, kunt u hier enkele gegevens bewerken.

   De volgende velden weergeven of bewerken in het dialoogvenster **Overzicht** gebied:

   * **Naam**
   * **Pad**: de weg waardoor de kwestie aan het project werd geregistreerd.

      Als een kwestie als verzoek in een verzoekrij werd voorgelegd, zijn de namen van het project, de Groep van het Onderwerp, en het Onderwerp van de Rij hier vermeld. Dit veld kan niet worden bewerkt.

      Zie voor meer informatie over het verzenden van aanvragen [Adobe Workfront-aanvragen maken en verzenden](../../../manage-work/requests/create-requests/create-submit-requests.md).

   * **Beschrijving**
   * **URL**: elk webadres dat met de uitgave verband houdt.
   * **Prioriteit**: een visuele vlag die u toestaat om kwesties voorrang te geven.
   * **Ernst**: een visuele markering die aangeeft hoe ernstig het in het probleem beschreven probleem is.
   * **Primaire contactpersoon**: De standaard primaire contactpersoon is de gebruiker die de uitgave heeft gemaakt. Dit veld kan worden bewerkt.
   * **Geplande uren**: geeft aan hoeveel tijd iemand nodig heeft om de uitgave te voltooien. De standaardwaarde is 8 uur. Dit veld kan worden bewerkt.
   * **Werkelijke uren**: geeft de hoeveelheid tijd weer die nodig was om de uitgave te voltooien. Dit is de daadwerkelijke tijd dat iemand voor de kwestie registreert.
   * **Geplande begindatum**: de datum waarop de uitgifte van start gaat. De standaardwaarde is de datum en de tijd waarop de uitgave is gemaakt.
   * **Werkelijke begindatum**: de datum en het tijdstip waarop de status van de uitgave is gewijzigd in In uitvoering.
   * **Geplande afsluitdatum**: de datum waarop de uitgifte volgens plan zal worden voltooid.
   * **Werkelijke afsluitdatum**: de datum waarop de afgifte daadwerkelijk is voltooid. Dit veld wordt automatisch ingevuld wanneer de status van de uitgave verandert in Gesloten of Opgelost, of kan handmatig worden bewerkt.
   * **Werkelijke kosten**: de kosten op basis van de werkelijk aantal uren dat op de uitgave is aangemeld. Dit veld kan niet worden bewerkt. De Ware Kosten van een kwestie worden berekend gebaseerd op de volgende formule, waar het Tarief van de Kosten van de Gebruiker de kostentarief verbonden aan de gebruiker die de tijd aan de kwestie registreert:

      Feitelijke kosten van uitgave = aantal uren geregistreerd * Kostenpercentage van gebruiker

   * **Ingevoerd door**: dit is de gebruiker die de uitgave heeft gemaakt . Dit veld kan niet worden bewerkt.
   * **Laatst bijgewerkt op**: Dit is de gebruiker die een veld over de uitgave voor het laatst heeft bijgewerkt. Dit veld kan niet worden bewerkt.

      In de **Aangepaste Forms** in, kunt u een of meer aangepaste formulieren selecteren die u aan de uitgave wilt koppelen.

* **Uren**: Hiermee wordt een lijst met uurwaarden van de uitgave weergegeven.
* **Goedkeuringen:** Hiermee geeft u de goedkeuringspaden weer die aan de uitgave zijn gekoppeld.

   Zie voor meer informatie over het koppelen van goedkeuringen aan een probleem de [Een goedkeuringsproces koppelen aan een tijdelijk onderdeel](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md#associating-the-approval-process-with-an-object) sectie in [Een goedkeuringsproces voor werkitems maken](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Weergeven welke projecten en taken problemen hebben

U kunt pictogrammen toevoegen in de weergave van een project of taakrapport of lijst om aan te geven of er problemen aan zijn gekoppeld. Het toevoegen van pictogrammen aan de mening van een rapport of een lijst is gelijkaardig voor projecten en taken.

Om pictogrammen toe te voegen die tonen of een project kwesties in een projectrapport heeft:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront.
1. Klikken **Rapportage** > **Nieuw rapport** > **Projectrapport**.
1. In de **Tonen in deze kolom** veld, beginnen met typen **Statuspictogrammen** en selecteert u deze wanneer deze in de lijst wordt weergegeven.

1. Klikken **Opslaan + Sluiten** .

   De uitgiftepictogrammen worden weergegeven op de projecten die problemen hebben in het dialoogvenster **Statuspictogrammen** kolom.

   ![project_list_with_issue_icon.png](assets/project-list-with-issue-icon-350x132.png)
