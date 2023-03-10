---
product-area: projects
navigation-topic: convert-issues
title: Een uitgave converteren naar een project in Adobe Workfront
description: Een uitgave converteren naar een project in Adobe Workfront
author: Alina
feature: Work Management
exl-id: e3ba15a3-6169-466c-9912-32a8afdcc68d
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '1292'
ht-degree: 0%

---

# Een uitgave converteren naar een project in Adobe Workfront

Als meer werk moet worden gedaan om een kwestie te voltooien nadat de kwestie wordt voorgelegd, kunt u de kwestie in een project omzetten.

U kunt een uitgave in een nieuw project omzetten of u kunt het in een project omzetten gebruikend een malplaatje. Dit artikel beschrijft beide manieren om kwesties in projecten om te zetten.

Voor algemene informatie over het converteren van problemen raadpleegt u [Overzicht van conversie van problemen in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot problemen, taken en projecten bewerken</p> <p>Toegang tot financiële gegevens bewerken om financiële informatie bij te werken voor een geconverteerde versie van de uitgave</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen weergeven voor de uitgave</p> <p>U krijgt beheermachtigingen voor het project nadat de uitgave is omgezet</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt.

## Een uitgave converteren naar een project

U kunt een kwestie in een leeg project omzetten of een kwestie omzetten in een project gebruikend een malplaatje.

1. Ga naar een project en klik op **[!UICONTROL Issues]** in het linkerdeelvenster.
1. Voer een van de volgende handelingen uit in de lijst met weergegeven problemen:

   * Als u een uitgave wilt omzetten in een leeg project, klikt u op de naam van de uitgave en klikt u op de knop **[!UICONTROL More]** menu ![](assets/more-icon.png) rechts van de naam van de uitgave klikt u op **[!UICONTROL Convert to a blank project]**.


      of

      Selecteer de uitgave in de lijst met uitgaven en klik op de knop **[!UICONTROL More]** menu ![](assets/more-icon.png) boven aan de lijst klikt u op **[!UICONTROL Convert to a blank project]**.

      >[!IMPORTANT]
      >
      >De Omzetten in een lege projectoptie toont slechts wanneer uw systeem of groepsbeheerder toeliet [!UICONTROL Allow users to create projects without using a template] voorkeur in [!UICONTROL Setup] gebied. Zie voor meer informatie [Projectvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).


      U moet taken aan het project manueel toevoegen of een malplaatje vastmaken aan het project nadat u de kwestie omzet.

      Ga verder met stap 3e hieronder.

      <!--
     Is this accurate?
     -->

      >[!TIP]
      >   
      >* Als de kwestie gebruikend een verzoekrij werd gecreeerd, erft het nieuwe project de Groep van de verzoekrij.
      >* Als de kwestie door het toe te voegen aan de sectie van Kwesties van het project werd gecreeerd, erft het nieuwe project de Groep als het project van de kwestie.


   * Voer een van de volgende handelingen uit om een uitgave om te zetten in een project met behulp van een sjabloon:

      * Klik op de naam van een uitgave en klik vervolgens op de knop [!UICONTROL **Meer**] menu ![](assets/more-icon.png) rechts van de naam van de uitgave

         ![](assets/issue-more-menu-expanded-with-convert-to-project-options-nwe-350x213.png)

         of

      * Selecteer de kwestie in de lijst van kwesties, in een rapport, of dashboard, klik **Meer** menu ![](assets/more-icon.png) boven aan de lijst klikt u op **Converteren naar project vanuit sjabloon** en typ de naam van een sjabloon in het dialoogvenster **Zoeksjabloon** klikt u vervolgens op de naam van de sjabloon wanneer deze in de lijst wordt weergegeven. Ga verder met stap 3.

         <!--      
        (is this accurate?)      
        -->
      >[!TIP]
      >
      >Als u sjablonen hebt toegevoegd aan de lijst Favorieten, kunt u de muis boven de knop [!UICONTROL **Favoriete sjablonen**] en klik op de sjabloon die u wilt gebruiken.

      Het vak Nieuw project van sjabloon wordt weergegeven.

      ![](assets/new-project-from-template-small-box-with-template-details-panel-nwe-350x279.png)

      >[!TIP]
      >
      >Als het probleem is gekoppeld aan een goedkeuringsproces of al is gekoppeld aan een oplossend object, geeft Workfront boven aan het vak Converteren naar project een waarschuwing weer om aan te geven dat de goedkeuring wordt verwijderd of dat het oplossende object tijdens de conversie wordt overschreven. Zie voor meer informatie [Overzicht van conversie van problemen in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).


1. (Voorwaardelijk) als u hebt geselecteerd om de uitgave in een project om te zetten gebruikend een malplaatje, ga met de volgende stappen verder:

   1. Bekijk de sjabloondetails rechts.

      De sjabloondetails bevatten onder meer de volgende informatie:

      * Sjabloonduur
      * Eigenaar van sjabloon
      * Het aantal taken op hoofdniveau dat de namen van de drie belangrijkste taken omvat
      * Het aantal taken in de sjabloon
      * De namen van de aangepaste sjabloonformulieren
   1. (Optioneel) Plaats de muisaanwijzer op de naam van een sjabloon en klik op het pictogram Favorieten ![](assets/favorites-icon-small.png) om het als favoriet voor toekomstig gebruik te merken.

      >[!TIP]
      >
      >Je kunt maximaal 40 Workfront-objecten als favorieten laten markeren. Dit omvat sjablonen en andere items.

   1. Klikken [!UICONTROL **Sjabloon gebruiken**] om een sjabloon te selecteren.

      De [!UICONTROL Convert to Project] wordt geopend.

      ![](assets/convert-to-project-from-template-large-project-box-nwe-350x291.png)

   1. Als een veld al in de sjabloon is ingevuld, wordt het veld vooraf ingevuld in het dialoogvenster [!UICONTROL Convert to project] doos. U kunt de vooraf ingevulde waarden bewerken zodat deze beter overeenkomen met uw project. Zie voor meer informatie [Projecten bewerken](../../../manage-work/projects/manage-projects/edit-projects.md).

      >[!TIP]
      >
      >* Uw systeem- of groepsbeheerder kan velden toevoegen aan of verwijderen uit de [!UICONTROL Convert to Project box] door de projectdetails in uw [!UICONTROL Layout Template].
      >
      >* Als u velden wilt bijwerken in het dialoogvenster [!UICONTROL Finance] in de [!UICONTROL Convert to Project] vak dat u moet hebben [!UICONTROL Edit] toegang tot [!UICONTROL Financial Data] in uw toegangsniveau. Als u [!UICONTROL View] toegang tot [!UICONTROL Financial Data] in uw toegangsniveau alle financiële informatie van de malplaatjeoverdrachten aan het nieuwe project en u kunt niet het uitgeven terwijl u de kwestie omzet. Zie voor meer informatie [Toegang tot financiële gegevens verlenen](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) en [Een sjabloon delen](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).


   1. (Optioneel en voorwaardelijk) Klik op [!UICONTROL **Opties**] in het linkerdeelvenster selecteert u een van de beschikbare opties:

      * [!UICONTROL **Behoud de oorspronkelijke kwestie en koppel zijn resolutie aan dit project**]

         Wanneer deze optie is uitgeschakeld, wordt de oorspronkelijke uitgave verwijderd.

         >[!NOTE]
         >
         >Gebruikers zonder toegang of machtigingen om problemen te verwijderen, kunnen de uitgave niet verwijderen omdat ze deze converteren, ongeacht de status van deze instelling. Voor informatie over toegang en toestemmingen tot kwesties, zie:
         >
         >* [Toegang verlenen tot kwesties](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
         > 
         >* [Een uitgave delen](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)


      * [!UICONTROL **(Gebruikersnaam) toegang verlenen tot dit project**]

         Als deze optie niet is geselecteerd, wordt de uitgave [!UICONTROL Primary Contact] heeft geen toegang tot de nieuwe taak.

         >[!NOTE]
         >
         >Welke opties hier beschikbaar zijn, is afhankelijk van de manier waarop de Workfront-beheerder deze voor iedereen in het systeem of voor uw groep heeft geconfigureerd. Zie voor meer informatie [Taak- en probleemvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
         >
         >
         >Of, als de top-level groepen in uw organisatie hen afzonderlijk vormden, hangen de beschikbare opties hier af van welke groep u voor het nieuwe project in stap 6 selecteerde. Zie voor meer informatie [Taak- en uitgavevoorkeuren voor een groep configureren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).
   1. Klikken [!UICONTROL **Aangepaste Forms**] en voer een van de volgende handelingen uit:

      * Bekijk de aangepaste formulieren die aan de sjabloon zijn gekoppeld. Zij zullen worden overgedragen naar het nieuwe project.
      * Controleer of alle vereiste velden geldige gegevens bevatten.
      * De aangepaste formulieren opnieuw rangschikken door deze te slepen ![](assets/drag-object-icon.png) waar je ze wilt.
      * Klik op de knop **x** rechts van een formulier dat u niet naar het project wilt overbrengen.
      * Indien nodig, breng de informatie van de douaneformulier van de kwestie aan het project over.

         >[!TIP]
         >
         >* Als een aangepast formulier voor meerdere objecten dat aan de uitgave is gekoppeld, is geconfigureerd voor gebruik met zowel uitgaven als projecten, blijft alle informatie die in het formulier is opgeslagen behouden wanneer u de conversie uitvoert.
         >
         >* Als u een sjabloon voor de conversie gebruikt en een aangepast formulier dat aan de sjabloon is gekoppeld, een aangepast veld bevat dat ook wordt gevonden in een aangepast formulier dat aan de uitgave is gekoppeld, wordt de veldwaarde van de uitgave gebruikt voor het nieuwe project. Als het aangepaste veld echter leeg is in de uitgave, wordt de waarde uit de sjabloon gebruikt.

   1. Klikken [!UICONTROL **Omzetten in project**].

      >[!TIP]
      >
      >Als u hebt besloten om de originele uitgave te verwijderen, is de kwestie nu een project.
      >   
      >of
      >  
      >Als u besloot om de oorspronkelijke uitgave te behouden, is de kwestie nu verbonden met het nieuwe project en het zal voltooien wanneer het project voltooit.
      >
      >Sommige probleemgebieden worden overgedragen naar het project. De meeste die gebieden in het malplaatje worden bepaald brengen automatisch naar het nieuwe gecreeerde project over als u hen in vorige stappen niet veranderde. Zie voor meer informatie [Overzicht van conversie van problemen in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).




1. (Optioneel) Stel desgewenst verdere projectdetails &#x200B; (eigenaar van project, projectdatums) en taken in.
1. Klikken [!UICONTROL **Omzetten in project**].

   De uitgave wordt nu omgezet in een project.

1. Klikken [!UICONTROL **Ga naar project**] binnen [!UICONTROL Success] in de rechterbovenhoek van de pagina. Hierdoor wordt de projectpagina geopend.
