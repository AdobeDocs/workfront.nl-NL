---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Een canvasdashboard filteren
description: U kunt een filter op een dashboard van het Canvas toepassen nadat het is gecreeerd.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: 156e9d3f-49f6-4372-9749-c7124ff5baee
source-git-commit: c6458d777726092d74e8b031f5c14dfd58710e11
workflow-type: tm+mt
source-wordcount: '989'
ht-degree: 0%

---

# Een canvasdashboard filteren

>[!IMPORTANT]
>
>De functie Canvasdashboards is momenteel alleen beschikbaar voor gebruikers die deelnemen aan de bètafase. Onderdelen van het onderdeel zijn mogelijk niet compleet of werken niet zoals bedoeld in deze fase. Gelieve te dienen om het even welke terugkoppelen betreffende uw ervaring door de instructies in [&#x200B; te volgen verstrekt &#x200B;](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) sectie in het de bètaoverzichtsartikel van de dashboards van het Canvas.<br>
>Als u feedback hebt over een mogelijk probleem met een probleem of een technisch probleem, stuurt u een ticket naar Workfront Support. Voor meer informatie, zie [&#x200B; de Steun van de Klant van het Contact &#x200B;](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Deze bètaversie is niet beschikbaar op de volgende cloudproviders:
>
>* Je eigen sleutel voor Amazon Web Services
>* Azure
>* Google Cloud Platform


U kunt een filter op een dashboard van het Canvas toepassen dat herinneringen bevat. Een vraag werkt als filterbepaling die extra het filtreren criteria toepast zodat kunt u uw resultaten nog verder versmallen. Deze herinneringen kunnen worden gewijzigd telkens als u de filter toepast, toestaand u om de getoonde resultaten aan te passen zonder het moeten de belangrijkste filtercriteria van het dashboard of elk individueel rapport uitgeven.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-pakket</p></td> 
   <td> 
<p>Alle </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td> 
<p>Standard</p> 
<p>Plan</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuraties op toegangsniveau</p></td> 
   <td><p>Toegang tot rapporten, dashboards en kalenders bewerken</p>
  </td> 
  </tr> 
    </tr>  
        <tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td><p>Rechten voor het dashboard beheren</p>
  </td> 
  </tr> 
</tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Vereisten

U moet een dashboard maken voordat u het kunt filteren.

Voor meer informatie, zie [&#x200B; een Dashboard van het Canvas &#x200B;](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md) creëren.

## Een dashboard filteren

Voer de volgende stappen in de vermelde volgorde uit om een dashboard te filteren:

* [Deel 1: Een dashboardfilter maken](#part-1-create-a-dashboard-filter)
* [Deel 2: Een dashboardprompt maken](#part-2-define-a-dashboard-prompt)
* [Deel 3: Een dashboardprompt toepassen](#step-3-apply-a-dashboard-prompt)

>[!NOTE]
>
>Het dashboardfilter wordt toegepast op alle rapporten waarin dashboardfilters niet zijn uitgeschakeld.  U kunt individuele rapporten uitsluiten van het hebben van dashboard-vlakke filters die door het actiemenu voor elk rapport uit te breiden en **te selecteren onbruikbaar maken Filters** optie.


### Deel 1: Een dashboardfilter maken

Met een dashboardfilter, kunt u een gemeenschappelijke filter over alle rapporten toepassen die op een dashboard beschikbaar zijn zonder het moeten de filters voor elk individueel rapport wijzigen.

>[!NOTE]
>
>Deze filters kunnen alleen worden geconfigureerd door een gebruiker met beheertoegang tot het dashboard.


{{step1-to-dashboards}}

1. In het linkerpaneel, klik **de Dashboards van het Canvas**.

1. Op de **pagina van de Dashboards van het Canvas**, selecteer het dashboard u een filter op wilt toepassen.

1. In de upper-left hoek van de pagina van dashboarddetails, klik **Filters**. Het paneel Filters wordt geopend.

1. Selecteer **uitgeven filters**. Het **de filters van het dashboard** dialoogvakje opent.

1. (Optioneel) Volg onderstaande stappen om een regel toe te voegen:

   1. Selecteer **uitgeven** pictogram aan het recht van de regeldoos.

      ![&#x200B; geef pictogram &#x200B;](assets/edit-icon.png) uit

   1. Klik **toevoegen voorwaarde** en voeg dan de volgende informatie toe:
      * Selecteer een veld waarop u wilt filteren.
      * Selecteer een optie (of filtermodifier) om te bepalen aan welke voorwaarde het veld moet voldoen.

   1. (Facultatief) klik **toevoegen filtergroep** om een andere reeks het filtreren criteria toe te voegen. De standaardoperator tussen de sets is AND. Klik op de operator om deze te wijzigen in OR.

1. Ga aan [&#x200B; Deel 2 te werk: Creeer een dashboardherinnering &#x200B;](#part-2-define-a-dashboard-prompt).


### Deel 2: Een dashboardprompt definiëren

Met een dashboardprompt kunnen gebruikers extra aangepaste filters toepassen op rapporten die beschikbaar zijn op het dashboard.

>[!NOTE]
>
>De opties voor de dashboardprompt kunnen alleen worden geconfigureerd door een gebruiker met beheertoegang tot het dashboard.

1. Volg onderstaande stappen om een vraag toe te voegen:

   1. Selecteer **toevoegen herinnering**. Nieuwe velden worden rechts op het scherm weergegeven.

   1. Ga een etiket op het **in aanpassen etiket** gebied.

   1. Selecteer het veld waarop de vraag moet worden gebaseerd door de naam van het veld te typen en vervolgens te selecteren wanneer deze wordt weergegeven in de lijst. 

1. Volg onderstaande stappen om een aangepaste prompt toe te voegen:

   1. Selecteer **toevoegen douaneherinnering**. Nieuwe velden worden rechts op het scherm weergegeven.

   1. (Facultatief) ga een nieuw etiket op het **aanpassen etiket** gebied in. Door gebrek, wordt de etiket *Nieuwe douaneherinnering* toegewezen.

   1. Klik **toevoegen nieuwe optie**.

   1. Ga de snelle naam op het **gebied van de Waarde van de Optie 0&rbrace; in.**

   1. Klik **toevoegen voorwaarde** en specificeer dan het gebied u tegen en de bepaling wilt filtreren die bepaalt welk soort voorwaarde het gebied moet ontmoeten.

      >[!NOTE]
      >
      >De voorwaarde van een aangepaste prompt kan alleen worden bewerkt in de tekstmodus. Hierdoor kunnen meerdere voorwaarden op één veld worden toegepast.


   1. (Facultatief) klik **toevoegen filtergroep** om een andere reeks het filtreren criteria toe te voegen. De standaardoperator tussen de sets is AND. Klik op de operator om deze te wijzigen in OR.

1. Klik **sparen** om de filter op het dashboard toe te passen.

1. Ga aan [&#x200B; Deel 3 te werk: Pas een dashboardherinnering &#x200B;](#step-3-apply-a-dashboard-prompt) toe.

### Stap 3: Een dashboardprompt toepassen

Alle gebruikers met toegang tot een dashboard kunnen een dashboardherinnering op een Dashboard van het Canvas toepassen zodra de filter en de herinneringen zijn gecreeerd.

{{step1-to-dashboards}}

1. In het linkerpaneel, klik **de Dashboards van het Canvas**.

1. Op de **pagina van de Dashboards van het Canvas**, selecteer het dashboard u de herinnering wilt toepassen op.

1. In de upper-left hoek van de pagina van dashboarddetails, klik **Filters**. Het paneel Filters wordt geopend.

1. In **toon verslagen waar...** sectie, kies een voorwaarde voor één of alle getoonde herinneringen. De herinnering wordt toegepast en de toegepaste filters van het a **dashboard** markering verschijnt in de hoek van de rapportwidget.
   ![&#x200B; Uitgezochte voorwaarde &#x200B;](assets/prompts-list.png)

1. Klik het **Dichte** pictogram ![&#x200B; dicht pictogram &#x200B;](assets/close-icon.png) in de hoger-juiste hoek om het paneel te verbergen.


## Een dashboard filteren op valutatype

U kunt schakelen tussen verschillende valutatypen op dashboardniveau. Rapporten met valutavelden worden bijgewerkt met het geselecteerde valutatype.

>[!NOTE]
>
>De gebieden van de munteenheid kunnen op het rapportniveau worden gesloten. Als een valutaveld is vergrendeld, verandert het valutatype voor dat rapport niet wanneer u het valutatype voor het dashboard wijzigt.

Het valutatype voor het dashboard wijzigen,

1. Klik op het vervolgkeuzemenu Valuta in de rechterbovenhoek van de pagina met dashboarddetails.
1. Selecteer het gewenste valutatype in de lijst.

   ![&#x200B; daling van de veranderingsmunt neer &#x200B;](assets/filter-by-currency.png)
