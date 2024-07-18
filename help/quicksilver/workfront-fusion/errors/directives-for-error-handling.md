---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Richtlijnen voor foutafhandeling in  [!DNL Adobe Workfront Fusion]
description: Dit artikel beschrijft richtlijnen die u voor fout behandeling in uw  [!DNL Adobe Workfront Fusion]  scenario's kunt gebruiken.
author: Becky
feature: Workfront Fusion
exl-id: dcf4f7e3-78d8-4eb4-9483-8a1c18b0e436
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 0%

---

# Richtlijnen voor foutafhandeling in [!DNL Adobe Workfront Fusion]

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] of hoger</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] licentie**</td> 
   <td>
   <p>Huidige licentievereiste: geen [!DNL Workfront Fusion] licentievereiste.</p>
   <p>of</p>
   <p>Vereiste voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en integratie] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereiste: als u het [!UICONTROL Select] - of [!UICONTROL Prime] [!DNL Adobe Workfront] -abonnement hebt, moet uw organisatie [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken. [!DNL Workfront Fusion] wordt opgenomen in het [!UICONTROL Ultimate] [!DNL Workfront] -abonnement.</p>
   <p>of</p>
   <p>Vereiste verouderd product: uw organisatie moet [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met de [!DNL Workfront] -beheerder als u wilt weten welk abonnement, licentietype of toegang u hebt.

Voor informatie over [!DNL Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Richtlijnen voor foutafhandeling

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Terugdraaien</p> <p> <img src="assets/rollback.png"> </p> </td> 
   <td> <p>De uitvoering van het scenario wordt onmiddellijk tegengehouden en de fase van het Terugschroeven van prijzen van de a <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback" class="MCXref xref"> </a> is begonnen op alle modules in een poging om hen allen aan hun aanvankelijke staat terug te keren. De volgende modules worden niet verwerkt.</p> <p>Met uitzondering van een aantal fouttypen wordt het scenario gedeactiveerd na het aantal opeenvolgende fouten dat is opgegeven onder Scenario-instellingen. Voor meer informatie, zie <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#number" class="MCXref xref"> Aantal opeenvolgende fouten </a>.</p> <p>De status van de uitvoering van het scenario wordt gemarkeerd als "fout."</p> <p>Opmerking: dit is het standaardgedrag als er geen fouthandlerroute aan de module is gekoppeld en de instelling <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">[!UICONTROL Allow storing incomplete executions]</a> onder [!UICONTROL Scenario settings] niet wordt gecontroleerd.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Vastleggen</p> <p> <img src="assets/commit.png"> </p> </td> 
   <td> <p>De uitvoering van het scenario wordt onmiddellijk tegengehouden en een begaan fase is begonnen op alle modules. De volgende modules worden niet verwerkt.</p> <p>Alle onverwerkte bundels worden genegeerd.</p> <p>De status van de uitvoering van het scenario is gemarkeerd als "succes." Voor informatie over begaat fasen, zie </a> Vastleggen <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit" class="MCXref xref"> in de uitvoering van het artikel <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref"> Scenario, cycli, en fasen in de Fusie van Adobe Workfront </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Hervatten</p> <p> <img src="assets/resume.png"> </p> </td> 
   <td> <p>Er wordt een vervangend uitvoerbestand opgegeven en geleverd aan de module die een fout aantreft.</p> <p>De volgende modules worden verwerkt.</p> <p>De status van de uitvoering van het scenario is gemarkeerd als "succes."</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Negeren</p> <p> <img src="assets/ignore.png"> </p> </td> 
   <td> <p>De fout wordt genegeerd en de verdere modules worden niet verwerkt.</p> <p>Als er onverwerkte bundels zijn, gaat de uitvoering van het scenario normaal voort.</p> <p>De status van de uitvoering van het scenario is gemarkeerd als "succes."</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Break</p> <p> <img src="assets/break.png"> </p> </td> 
   <td> <p>De status van de uitvoering van het scenario wordt opgeslagen in de wachtrij met onvolledige uitvoeringen waar de fout handmatig kan worden opgelost. Voor meer informatie, zie <a href="../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md" class="MCXref xref"> Mening en los onvolledige uitvoeringen in de Fusie van Adobe Workfront </a> op. </p> <p>Er zijn echter enkele uitzonderingen. Voor meer informatie, zie <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref"> toestaan het opslaan van onvolledige uitvoeringen </a> in het artikel <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref"> het paneel van scenario-montages in de Fusie van Adobe Workfront </a>.</p> <p>De volgende modules worden niet verwerkt.</p> <p>Als er onverwerkte bundels zijn, gaat de uitvoering van het scenario normaal voort.</p> <p>De status van de uitvoering van het scenario wordt gemarkeerd als "waarschuwing" wanneer de optie [!UICONTROL Automatically complete execution] is uitgeschakeld.</p> <p>Zie de sectie <a href="#break" class="MCXref xref">[!UICONTROL Break]</a> hieronder voor meer informatie.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Opnieuw</p> <p> <img src="assets/retry.png"> </p> </td> 
   <td> <p>In sommige gevallen zou het nuttig kunnen zijn om een falende module voor een paar tijden opnieuw uit te voeren wanneer er een kans is dat de reden voor de mislukking over tijd zou kunnen overgaan.</p> <p>Workfront Fusion biedt momenteel niet de instructie Retry, maar er kunnen verschillende oplossingen worden gebruikt om de functionaliteit ervan na te bootsen. Voor meer informatie, zie <a href="../../workfront-fusion/errors/retry.md" class="MCXref xref"> fout behandeling in de Fusie van Adobe Workfront </a> opnieuw proberen.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* De foutafhandelingsinstructies kunnen momenteel niet worden gebruikt buiten een foutafhandelingsroute.
>
>   Voor meer informatie, zie [ de managerroute van de Fout ](../../workfront-fusion/errors/error-handling.md#error) in het artikel [ de behandeling van de Fout in de Fusie van Adobe Workfront ](../../workfront-fusion/errors/error-handling.md).
>* [!DNL Workfront Fusion] biedt momenteel geen module Throw die u in staat zou stellen om gemakkelijk voorwaardelijke fouten te genereren (genereren), hoewel een tijdelijke oplossing kan worden gebruikt om de functionaliteit ervan na te bootsen.
>
>   Voor meer informatie, zie [ Oplossing voor Borg ](../../workfront-fusion/errors/throw.md#workaround-for-throw) in het artikel [ fout behandeling van de Borg in de Fusie van Adobe Workfront ](../../workfront-fusion/errors/throw.md).

## Break {#break}

Wanneer een fout wordt afgehandeld door de instructie [!DNL Break] , wordt een record gemaakt in de map Onvolledige uitvoeringen. Dit verslag slaat de staat van de scenariouitvoering, samen met gegevens van de vroegere modules op. De record verwijst naar de module waar de fout is opgetreden en bevat informatie over de gegevens die de module als invoer heeft ontvangen. Voor elke bundel gegevens die de fout veroorzaakt, wordt een afzonderlijke verslag gecreeerd.

Voor meer informatie, zie [ Mening en los onvolledige uitvoeringen in de Fusie van Adobe Workfront ](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) op.

### Fouten die voortvloeien uit de Break-richtlijn oplossen

U kunt de fout handmatig oplossen door het scenario (indien nodig) bij te werken en één keer uit te voeren.

U kunt het scenario ook vormen om een onvolledige uitvoering automatisch te verwerken door het scenario opnieuw uit te voeren. Om de module te vormen om onvolledige uitvoeringen te verwerken:

1. Binnen de module van het Sluiten, laat [!UICONTROL **automatisch volledige uitvoerings**] optie toe.
1. Op het **Aantal pogingen** gebied, ga of kaart het maximumaantal pogingen in dat u de module wilt de uitvoering opnieuw proberen

   Dit getal moet tussen 1 en 100 liggen.
1. In het **Interval tussen pogingen** gebied, ga of kaart het aantal notulen tussen elke poging opnieuw in.

Als deze optie is ingeschakeld en er een fout optreedt, wordt de onvolledige uitvoering opgehaald (na de in het veld [!UICONTROL Interval between attempts] opgegeven tijd) en uitgevoerd met de oorspronkelijke invoergegevens. Dit zal herhalen tot de uitvoering van de module zonder een fout voltooit of tot het Aantal gespecificeerde pogingen wordt bereikt.

>[!NOTE]
>
>Als de aanvankelijke poging opnieuw probeert ontbreekt, stijgt het interval tussen opnieuw probeert exponentieel elke andere poging.


Als &quot;Automatisch volledige uitvoering&quot; is ingeschakeld, wordt de uitvoering van het scenario gemarkeerd als &quot;Succes&quot; omdat de fouthandler voor automatisch opnieuw proberen van het einde de kwestie automatisch afhandelt. In dit geval ontvangen gebruikers geen e-mail over de mislukte uitvoering.

Wanneer &quot;Automatisch volledige uitvoering&quot; is uitgeschakeld, wordt de uitvoering gemarkeerd als &quot;Waarschuwing&quot;.

Er zijn sommige uitzonderingen op uitvoeringen die onder Onvolledige Uitvoeringen worden opgeslagen, en met sommige foutentypes, is auto-retry van een scenario uitvoering niet mogelijk.

Voor meer informatie, zie [ toestaan het opslaan van onvolledige uitvoeringen ](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) in het artikel [ het paneel van scenario-montages in de Fusie van Adobe Workfront ](../../workfront-fusion/scenarios/scenario-settings-panel.md).

Voor extra informatie, zie [ Geavanceerde fout behandeling in de Fusie van Adobe Workfront ](../../workfront-fusion/errors/advanced-error-handling.md).
