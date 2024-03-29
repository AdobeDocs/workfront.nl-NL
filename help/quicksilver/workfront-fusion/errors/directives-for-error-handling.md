---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Richtlijnen voor foutafhandeling in [!DNL Adobe Workfront Fusion]
description: In dit artikel worden instructies beschreven die u kunt gebruiken voor foutafhandeling in uw [!DNL Adobe Workfront Fusion] scenario's.
author: Becky
feature: Workfront Fusion
exl-id: dcf4f7e3-78d8-4eb4-9483-8a1c18b0e436
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '921'
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
   <p>Huidige vergunningsvereiste: Nee [!DNL Workfront Fusion] vergunningsvereiste.</p>
   <p>of</p>
   <p>Vereisten voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereisten: Als u de [!UICONTROL Select] of [!UICONTROL Prime] [!DNL Adobe Workfront] Abonnement, uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken. [!DNL Workfront Fusion] is opgenomen in de [!UICONTROL Ultimate] [!DNL Workfront] plannen.</p>
   <p>of</p>
   <p>Oudere productvereisten: Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Richtlijnen voor foutafhandeling

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Terugdraaien</p> <p> <img src="assets/rollback.png"> </p> </td> 
   <td> <p>De uitvoering van het scenario wordt onmiddellijk gestopt en een <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback" class="MCXref xref">Terugdraaien</a> de fase is begonnen op alle modules in een poging om hen allen aan hun aanvankelijke staat terug te keren. De volgende modules worden niet verwerkt.</p> <p>Met uitzondering van een aantal fouttypen wordt het scenario gedeactiveerd na het aantal opeenvolgende fouten dat is opgegeven onder Scenario-instellingen. Zie voor meer informatie <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#number" class="MCXref xref">Aantal opeenvolgende fouten</a>.</p> <p>De status van de uitvoering van het scenario wordt gemarkeerd als "fout."</p> <p>Opmerking: Dit is het standaardgedrag als geen route van de foutenmanager aan de module en in bijlage is <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">[!UICONTROL Allow storing incomplete executions]</a> instellen onder [!UICONTROL Scenario settings] is niet ingeschakeld.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Vastleggen</p> <p> <img src="assets/commit.png"> </p> </td> 
   <td> <p>De uitvoering van het scenario wordt onmiddellijk tegengehouden en een begaan fase is begonnen op alle modules. De volgende modules worden niet verwerkt.</p> <p>Alle onverwerkte bundels worden genegeerd.</p> <p>De status van de uitvoering van het scenario is gemarkeerd als "succes." Voor informatie over begaat fasen, zie <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit" class="MCXref xref">Vastleggen</a> in het artikel <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Uitvoering, cycli en fasen van scenario's in Adobe Workfront Fusion</a>.</p> </td> 
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
   <td> <p>De status van de uitvoering van het scenario wordt opgeslagen in de wachtrij met onvolledige uitvoeringen waar de fout handmatig kan worden opgelost. Zie voor meer informatie <a href="../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md" class="MCXref xref">Onvolledige uitvoeringen weergeven en oplossen in Adobe Workfront Fusion</a>. </p> <p>Er zijn echter enkele uitzonderingen. Zie voor meer informatie <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">Onvolledige uitvoeringen opslaan toestaan</a> in het artikel <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">Het deelvenster met scenario-instellingen in Adobe Workfront Fusion</a>.</p> <p>De volgende modules worden niet verwerkt.</p> <p>Als er onverwerkte bundels zijn, gaat de uitvoering van het scenario normaal voort.</p> <p>De status van de uitvoering van het scenario wordt gemarkeerd als "waarschuwing" wanneer de [!UICONTROL Automatically complete execution] is uitgeschakeld.</p> <p>Zie de <a href="#break" class="MCXref xref">[!UICONTROL Break]</a> voor nadere informatie.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Opnieuw</p> <p> <img src="assets/retry.png"> </p> </td> 
   <td> <p>In sommige gevallen zou het nuttig kunnen zijn om een falende module voor een paar tijden opnieuw uit te voeren wanneer er een kans is dat de reden voor de mislukking over tijd zou kunnen overgaan.</p> <p>Workfront Fusion biedt momenteel niet de instructie Retry, maar er kunnen verschillende oplossingen worden gebruikt om de functionaliteit ervan na te bootsen. Zie voor meer informatie <a href="../../workfront-fusion/errors/retry.md" class="MCXref xref">Foutafhandeling opnieuw uitvoeren in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* De foutafhandelingsinstructies kunnen momenteel niet worden gebruikt buiten een foutafhandelingsroute.
>
>   Zie voor meer informatie [Fouthandlerroute](../../workfront-fusion/errors/error-handling.md#error) in het artikel [Foutafhandeling in Adobe Workfront Fusion](../../workfront-fusion/errors/error-handling.md).
>* [!DNL Workfront Fusion] biedt momenteel geen module van de Borg aan die u zou toelaten om (werpen) fouten gemakkelijk te produceren, hoewel een alternerende actie kan worden gebruikt om zijn functionaliteit te simuleren.
>
>   Zie voor meer informatie [Oplossing voor Throw](../../workfront-fusion/errors/throw.md#workaround-for-throw) in het artikel [Foutafhandeling genereren in Adobe Workfront Fusion](../../workfront-fusion/errors/throw.md).

## Break {#break}

Wanneer een fout door [!DNL Break] instructie, wordt een record gemaakt in de map Onvolledige uitvoeringen. Dit verslag slaat de staat van de scenariouitvoering, samen met gegevens van de vroegere modules op. De record verwijst naar de module waar de fout is opgetreden en bevat informatie over de gegevens die de module als invoer heeft ontvangen. Voor elke bundel gegevens die de fout veroorzaakt, wordt een afzonderlijke verslag gecreeerd.

Zie voor meer informatie [Onvolledige uitvoeringen weergeven en oplossen in Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### Fouten die voortvloeien uit de Break-richtlijn oplossen

U kunt de fout handmatig oplossen door het scenario (indien nodig) bij te werken en één keer uit te voeren.

U kunt het scenario ook vormen om een onvolledige uitvoering automatisch te verwerken door het scenario opnieuw uit te voeren. Om de module te vormen om onvolledige uitvoeringen te verwerken:

1. Schakel in de module Onderbreken de optie [!UICONTROL **Automatisch uitvoering voltooien**] optie.
1. In de **Aantal pogingen** veld, typt of wijst het maximumaantal pogingen toe dat u wilt dat de module de uitvoering opnieuw probeert

   Dit getal moet tussen 1 en 100 liggen.
1. In de **Interval tussen pogingen** Voer het aantal minuten in tussen elke poging om opnieuw te proberen of wijs het aantal minuten in.

Als deze optie is ingeschakeld, wordt bij een fout de onvolledige uitvoering opgehaald (na de tijd die in het dialoogvenster [!UICONTROL Interval between attempts] (veld) en uitgevoerd met de oorspronkelijke invoergegevens. Dit zal herhalen tot de uitvoering van de module zonder een fout voltooit of tot het Aantal gespecificeerde pogingen wordt bereikt.

>[!NOTE]
>
>Als de aanvankelijke poging opnieuw probeert ontbreekt, stijgt het interval tussen opnieuw probeert exponentieel elke andere poging.


Als &quot;Automatisch volledige uitvoering&quot; is ingeschakeld, wordt de uitvoering van het scenario gemarkeerd als &quot;Succes&quot; omdat de fouthandler voor automatisch opnieuw proberen van het einde de kwestie automatisch afhandelt. In dit geval ontvangen gebruikers geen e-mail over de mislukte uitvoering.

Wanneer &quot;Automatisch volledige uitvoering&quot; is uitgeschakeld, wordt de uitvoering gemarkeerd als &quot;Waarschuwing&quot;.

Er zijn sommige uitzonderingen op uitvoeringen die onder Onvolledige Uitvoeringen worden opgeslagen, en met sommige foutentypes, is auto-retry van een scenario uitvoering niet mogelijk.

Zie voor meer informatie [Onvolledige uitvoeringen opslaan toestaan](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) in het artikel [Het deelvenster met scenario-instellingen in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

Zie voor meer informatie [Geavanceerde foutafhandeling in Adobe Workfront Fusion](../../workfront-fusion/errors/advanced-error-handling.md).
