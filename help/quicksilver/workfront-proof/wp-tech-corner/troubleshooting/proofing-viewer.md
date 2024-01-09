---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Problemen oplossen - [!DNL Workfront Proof] proefdrukviewer
description: Als de inhoud van uw proefdrukken niet wordt geladen en u alleen een lege proefdrukviewer kunt zien, is dit zeer waarschijnlijk omdat deze actie lokaal wordt geblokkeerd.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ce463565-d21e-4dbc-8de8-78bcbf16fb2c
source-git-commit: 238b675b15b189c622692c1ba9babab5e82bfe09
workflow-type: tm+mt
source-wordcount: '951'
ht-degree: 0%

---

# Problemen oplossen - [!DNL Workfront Proof] proefdrukviewer

<!-- Audited: 01/2024 -->

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het standalone product [!DNL Workfront Proof]. Voor informatie over proefdrukken binnen [!DNL Adobe Workfront], zie [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Als de inhoud van uw proefdrukken niet wordt geladen en u alleen een lege proefdrukviewer kunt zien, is dit zeer waarschijnlijk omdat deze actie lokaal wordt geblokkeerd. Probeer hieronder de mogelijke oplossingen.

## De browser controleren <!--and [!DNL Flash Player]--> is bijgewerkt

Alle ontwikkelaars werken constant aan hun toepassingen en zij geven regelmatig nieuwe eigenschappen en moeilijke situaties voor hun producten vrij. Dit moet gebruikerservaring verbeteren en veiligheidsniveau handhaven zodat is het de beste praktijken om slechts de nieuwste versies te gebruiken. Dit helpt ook conflicten tussen de toepassingen te voorkomen.

<!--
### [!DNL Flash Player] Plugin Version

To check your current [!DNL Flash Player] version visit the [[!DNL Adobe] website](http://www.adobe.com/software/flash/about/).

![ProofView_2.png](assets/proofview-2-350x199.png)

If your version number differs from the one listed for your platform go to the [[!DNL Flash Player] download page](http://get.adobe.com/flashplayer/otherversions/) and get the latest version.

Please note: we do recommend using the original [!DNL Adobe] plugin, so if your browser uses a built-in solution deactivate it and install the [!DNL Adobe] solution.
-->

### Browserversie

Meestal werken de meeste browsers automatisch bij, maar als u problemen ondervindt, is het de moeite waard om te controleren welke versie u gebruikt en een update uit te voeren, indien nodig.

Ga in uw browser naar [!UICONTROL Menu] en zoek de [!UICONTROL About] optie (in sommige gevallen kan dit zichtbaar zijn onder een [!UICONTROL Help] ). In de [!UICONTROL About] in het pop-upvenster vindt u informatie over de huidige browserversie en ook een optie om bij te werken of te controleren op updates.

Bijvoorbeeld in Chrome:

![Browserversie van Chrome](assets/proofview-3.png)

Wanneer de meest recente browserversie is geïnstalleerd, probeert u de proefdruk opnieuw te openen en te controleren of het probleem is opgelost.

<!--
## Ensure Your Local [!DNL Flash] Storage is Available

Our [!DNL Workfront Proof] Viewer is based on Flash, and we store some data about the proofs (i.e., comments, proof tiles, [!DNL Workfront Proof] Viewer settings) on your computer using [!DNL Flash Player]. If the [!DNL Workfront Proof] Viewer opens, but there is no content inside you will want to make sure that the Flash Storage is available on your machine and that [!DNL Workfront Proof] is allowed to use it.

If there is some storage allocated, but you're working with the bigger proofs with multiple pages and comments try to increase the [!DNL Flash] Storage and re-load your proof.

Please see [Problems With Viewing Proofs - [!DNL Flash] Shared Objects Explained](../../../workfront-proof/wp-tech-corner/troubleshooting/view-proof-flash-shared-object.md) for the detailed instructions.
-->

## Identificeer waar het probleem is

* Worden de proefdrukken geopend in een andere browser?
* Als u dagelijks één browser gebruikt en u problemen hebt met het bekijken van de proeven daar, probeer om het zelfde bewijs in een verschillende browser op uw computer te openen. U doet dit door de proefdrukkoppeling van de URL-balk van uw hoofdbrowser te kopiëren en deze in een andere browser te plakken. Als de proefdruk daar wordt geopend, herzie uw hoofdbrowser configuratie, stop-ins, en uitbreidingen aangezien deze zouden kunnen storen.
* We hebben geen voorkeursbrowser, maar als er prestatieproblemen optreden in uw huidige browser, raden we u aan over te schakelen op een andere browser.
* Worden de proefdrukken geopend op een andere computer op uw locatie?
Als de proefdruk niet wordt geopend in een browser op uw computer, probeert u deze dan op een andere computer op uw locatie en/of buiten uw locatie te openen. Hierdoor kunt u bepalen of een probleem zich op uw specifieke computer voordoet of dat het probleem zich in uw lokale netwerk bevindt.
Als uw veiligheidsniveau hoger is, uw verbindingen aan [!DNL Workfront Proof] kan worden geblokkeerd door:

   * Uw lokale AV-software
   * Uw oplossing voor netwerkbeveiliging
   * DNS-, firewall- of proxyconfiguratie
   * Dit zijn de instellingen die buiten onze controle liggen. Er zijn diverse beschikbare veiligheidsoplossingen en wij kunnen niet zien welke in uw netwerk worden uitgevoerd en welke verbindingen kunnen blokkeren aan [!DNL Workfront Proof]. Het is ook niet aan [!DNL Workfront Proof] om uw interne veiligheidsconfiguratie te beslissen. Als u problemen hebt met het openen van de proefdrukken op de veelvoudige machines in uw plaats/netwerk, zouden wij u adviseren in contact met uw team van IT zodat konden zij de netwerkmontages controleren en machtigen of toevoegen [!DNL Workfront Proof] in de lijst van gewenste personen, indien nodig.

* Zijn de verbindingen met [!DNL Workfront Proof] toegestaan in uw netwerk?
In de Proefweergave laden we de tegels - fragmenten van de pagina&#39;s. Als deze inhoud aan uw uiteinde niet correct wordt geladen, kan het zijn dat sommige verbindingen met [!DNL Workfront Proof] worden geblokkeerd in uw netwerk. U zult ervoor willen zorgen dat alle verbindingen en alle inhoud van *.proofhq.com aan de lijst van gewenste personen wordt toegevoegd. Uw IT-team moet hierbij kunnen helpen.

## Insteekmodules controleren

Als uw browser bijgewerkt is en uw netwerk blokkeert niet de verbindingen aan [!DNL Workfront Proof]kan er iets in uw browser zijn dat invloed heeft op het weergeven van de proefdrukken. Er zijn vaak meerdere plug-ins en extensies beschikbaar in uw browser. Sommige van deze plug-ins kunnen problemen veroorzaken of een conflict veroorzaken met andere plug-ins.

De beste praktijken moeten alle onbekende toe:voegen-ons verwijderen en slechts degenen houden die u gebruikt en die u vertrouwt. Elke browser moet u opties bieden om de plug-ins en extensies te controleren, te wijzigen of te verwijderen. We gebruiken JavaScript om de [!DNL Workfront Proof] de viewer, zodat u vooral de plug-ins wilt bekijken die dat kunnen beïnvloeden.

Als er om het even welke bepaalde toe:voegen-op interfereert met het laden van de proeven, kunt u proberen controlerend de details in de console van browser.

![Browserconsole](assets/proofview-4.png)

In de meeste nieuwere browsers zijn er enkele extra tools voor ontwikkelaars beschikbaar die kunnen worden gebruikt voor geavanceerdere probleemoplossing.

Als u problemen hebt met het bekijken van de proefdrukken:

* Open de browserconsole en laad de proefdruk opnieuw.
* Controleer of de console waarschuwingen of berichten bevat. Deze details kunnen helpen identificeren wat de worteloorzaak van de kwesties is.
* Laat uw IT-team de resultaten analyseren. Zij moeten advies kunnen geven en kunnen helpen het lokale probleem op te lossen.
* Deel de resultaten met ons ondersteuningsteam. We zullen graag hulp bieden.

## Instellingen voor gemengde inhoud controleren

Alle verbindingen met [!DNL Workfront Proof] zijn via HTTPS. In de [!DNL Workfront Proof] Viewer we laden de tegels via HTTP en de gegevens worden beveiligd met de tokens. Dit leidt tot Gemengde Inhoud die sommige browsers of veiligheidsoplossingen (door gebrek of door handconfiguratie) kunnen blokkeren.

Als dit de reden is waarom de proeven niet op uw computer openen (u zou de relevante alarm in de console van browser moeten kunnen zien), dergelijke verbindingen voor toestaan [!DNL Workfront Proof] of wijzig de instellingen om passief gemengde inhoud op uw computer toe te staan. De gemengde inhoud kan door uw browser, software AV, of netwerkconfiguratie worden geblokkeerd om de nauwkeurige oorzaak te bepalen. U moet contact opnemen met uw IT-team/netwerkbeheerders. Ze moeten ook de gemengde inhoud op uw computer kunnen inschakelen.


