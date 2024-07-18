---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Het oplossen van problemen -  [!DNL Workfront Proof]  het proef kijker
description: Als de inhoud van uw proefdrukken niet wordt geladen en u alleen een lege proefdrukviewer kunt zien, is dit zeer waarschijnlijk omdat deze actie lokaal wordt geblokkeerd.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ce463565-d21e-4dbc-8de8-78bcbf16fb2c
source-git-commit: 39fdf5c2c2114a82c48f515c4a9f088596394045
workflow-type: tm+mt
source-wordcount: '951'
ht-degree: 0%

---

# Problemen oplossen - [!DNL Workfront Proof] de viewer controleren

<!-- Audited: 01/2024 -->

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het zelfstandige product [!DNL Workfront Proof] . Voor informatie bij het proef binnen [!DNL Adobe Workfront], zie [ het Bewijzen ](../../../review-and-approve-work/proofing/proofing.md).

Als de inhoud van uw proefdrukken niet wordt geladen en u alleen een lege proefdrukviewer kunt zien, is dit zeer waarschijnlijk omdat deze actie lokaal wordt geblokkeerd. Probeer hieronder de mogelijke oplossingen.

## Zorg ervoor dat de browserversie <!--and [!DNL Flash Player]--> up-to-date is

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

Ga in uw browser naar [!UICONTROL Menu] en zoek de optie [!UICONTROL About] (in sommige gevallen is dit zichtbaar onder een [!UICONTROL Help] -menu). In het pop-upvenster [!UICONTROL About] vindt u informatie over de huidige browserversie en ook een optie voor het bijwerken/controleren op updates.

Bijvoorbeeld in Chrome:

![ browser van Chrome versie ](assets/proofview-3.png)

Wanneer de meest recente browserversie is geïnstalleerd, probeert u de proefdruk opnieuw te openen en te controleren of het probleem is opgelost.

<!--

## Ensure Your Local [!DNL Flash] Storage is Available

Our [!DNL Workfront Proof] Viewer is based on Flash, and we store some data about the proofs (i.e., comments, proof tiles, [!DNL Workfront Proof] Viewer settings) on your computer using [!DNL Flash Player]. If the [!DNL Workfront Proof] Viewer opens, but there is no content inside you will want to make sure that the Flash Storage is available on your machine and that [!DNL Workfront Proof] is allowed to use it.

If there is some storage allocated, but you're working with the bigger proofs with multiple pages and comments try to increase the [!DNL Flash] Storage and re-load your proof.

-->

## Identificeer waar het probleem is

* Worden de proefdrukken geopend in een andere browser?
* Als u dagelijks één browser gebruikt en u problemen hebt met het bekijken van de proeven daar, probeer om het zelfde bewijs in een verschillende browser op uw computer te openen. U doet dit door de proefdrukkoppeling van de URL-balk van uw hoofdbrowser te kopiëren en deze in een andere browser te plakken. Als de proefdruk daar wordt geopend, herzie uw hoofdbrowser configuratie, stop-ins, en uitbreidingen aangezien deze zouden kunnen storen.
* We hebben geen voorkeursbrowser, maar als er prestatieproblemen optreden in uw huidige browser, raden we u aan over te schakelen op een andere browser.
* Worden de proefdrukken geopend op een andere computer op uw locatie?
Als de proefdruk niet wordt geopend in een browser op uw computer, probeert u deze dan op een andere computer op uw locatie en/of buiten uw locatie te openen. Hierdoor kunt u bepalen of een probleem zich op uw specifieke computer voordoet of dat het probleem zich in uw lokale netwerk bevindt.
Als uw beveiligingsniveau hoger is, kunnen de verbindingen met [!DNL Workfront Proof] worden geblokkeerd door:

   * Uw lokale AV-software
   * Uw oplossing voor netwerkbeveiliging
   * DNS-, firewall- of proxyconfiguratie
   * Dit zijn de instellingen die buiten onze controle liggen. Er zijn verschillende beveiligingsoplossingen beschikbaar en we kunnen niet zien welke in uw netwerk zijn geïmplementeerd en welke verbindingen met [!DNL Workfront Proof] blokkeren. Het is ook niet aan [!DNL Workfront Proof] om te beslissen over uw interne veiligheidsconfiguratie. Als u problemen hebt met het openen van de proefdrukken op de veelvoudige machines in uw plaats/netwerk, zouden wij u adviseren in contact met uw team van IT zodat konden zij de netwerkmontages controleren en [!DNL Workfront Proof] machtigen of toevoegen aan de lijst van gewenste personen, indien nodig.

* Zijn de verbindingen met [!DNL Workfront Proof] toegestaan in uw netwerk?
In de Proefweergave laden we de tegels - fragmenten van de pagina&#39;s. Als deze inhoud aan uw uiteinde niet correct wordt geladen, worden sommige verbindingen met [!DNL Workfront Proof] mogelijk geblokkeerd in uw netwerk. U zult ervoor willen zorgen dat alle verbindingen en alle inhoud van *.proofhq.com aan de lijst van gewenste personen wordt toegevoegd. Uw IT-team moet hierbij kunnen helpen.

## Insteekmodules controleren

Als uw browser bijgewerkt is en uw netwerk de verbindingen met [!DNL Workfront Proof] niet blokkeert, kan er iets in uw browser zijn die het bekijken van de proefdrukken beïnvloedt. Er zijn vaak meerdere plug-ins en extensies beschikbaar in uw browser. Sommige van deze plug-ins kunnen problemen veroorzaken of een conflict veroorzaken met andere plug-ins.

De beste praktijken moeten alle onbekende toe:voegen-ons verwijderen en slechts degenen houden die u gebruikt en die u vertrouwt. Elke browser moet u opties bieden om de plug-ins en extensies te controleren, te wijzigen of te verwijderen. We gebruiken JavaScript om de viewer van [!DNL Workfront Proof] te laden, zodat u vooral de plug-ins wilt bekijken die dat kunnen beïnvloeden.

Als er om het even welke bepaalde toe:voegen-op interfereert met het laden van de proeven, kunt u proberen controlerend de details in de console van browser.

![ Browser console ](assets/proofview-4.png)

In de meeste nieuwere browsers zijn er enkele extra tools voor ontwikkelaars beschikbaar die kunnen worden gebruikt voor geavanceerdere probleemoplossing.

Als u problemen hebt met het bekijken van de proefdrukken:

* Open de browserconsole en laad de proefdruk opnieuw.
* Controleer of de console waarschuwingen of berichten bevat. Deze details kunnen helpen identificeren wat de worteloorzaak van de kwesties is.
* Laat uw IT-team de resultaten analyseren. Zij moeten advies kunnen geven en kunnen helpen het lokale probleem op te lossen.
* Deel de resultaten met ons ondersteuningsteam. We zullen graag hulp bieden.

## Instellingen voor gemengde inhoud controleren

Alle verbindingen met [!DNL Workfront Proof] zijn via HTTPS. In de [!DNL Workfront Proof] Viewer worden de tegels echter via HTTP geladen en worden de gegevens met de tokens beveiligd. Dit leidt tot Gemengde Inhoud die sommige browsers of veiligheidsoplossingen (door gebrek of door handconfiguratie) kunnen blokkeren.

Als dit de reden is waarom de proeven niet op uw computer openen (u zou de relevante alarm in de console van browser moeten kunnen zien), dergelijke verbindingen voor [!DNL Workfront Proof] goedkeuren of uw montages wijzigen om passieve gemengde inhoud op uw machine toe te staan. De gemengde inhoud kan door uw browser, software AV, of netwerkconfiguratie worden geblokkeerd om de nauwkeurige oorzaak te bepalen. U moet contact opnemen met uw IT-team/netwerkbeheerders. Ze moeten ook de gemengde inhoud op uw computer kunnen inschakelen.


