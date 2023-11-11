---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Problemen oplossen - [!DNL Workfront Proof] proefdrukviewer
description: Als de inhoud van uw proefdrukken niet wordt geladen en u alleen een lege proefdrukviewer kunt zien, is dit zeer waarschijnlijk omdat deze actie lokaal wordt geblokkeerd. Probeer hieronder de mogelijke oplossingen.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ce463565-d21e-4dbc-8de8-78bcbf16fb2c
source-git-commit: 20fcf4dd07c1058559533501f7e297d78c43a70b
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 0%

---

# Problemen oplossen - [!DNL Workfront Proof] proefdrukviewer

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het standalone product [!DNL Workfront Proof]. Voor informatie over proefdrukken binnen [!DNL Adobe Workfront], zie [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Als de inhoud van uw proefdrukken niet wordt geladen en u alleen een lege proefdrukviewer kunt zien, is dit zeer waarschijnlijk omdat deze actie lokaal wordt geblokkeerd. Probeer hieronder de mogelijke oplossingen.

## Zorg voor uw browser en [!DNL Flash Player] Versies zijn bijgewerkt

Alle ontwikkelaars werken constant aan hun toepassingen en zij geven regelmatig nieuwe eigenschappen en moeilijke situaties voor hun producten vrij. Dit moet gebruikerservaring verbeteren en veiligheidsniveau handhaven zodat is het de beste praktijken om slechts de nieuwste versies te gebruiken. Dit helpt ook conflicten tussen de toepassingen te voorkomen.

<!--
### [!DNL Flash Player] Plugin Version

To check your current [!DNL Flash Player] version visit the [[!DNL Adobe] website](http://www.adobe.com/software/flash/about/).

![ProofView_2.png](assets/proofview-2-350x199.png)

If your version number differs from the one listed for your platform go to the [[!DNL Flash Player] download page](http://get.adobe.com/flashplayer/otherversions/) and get the latest version.

Please note: we do recommend using the original [!DNL Adobe] plugin, so if your browser uses a built-in solution deactivate it and install the [!DNL Adobe] solution.
-->

### Browserversie

Tegenwoordig worden de meeste browsers automatisch bijgewerkt, maar als u problemen ondervindt, is het de moeite waard om te controleren welke versie u gebruikt en update uit te voeren, indien nodig.

Ga in uw browser naar [!UICONTROL Menu] en zoek de [!UICONTROL About] optie (in sommige gevallen kan dit zichtbaar zijn onder [!UICONTROL Help] ). In de [!UICONTROL About] pop-up zult u informatie over de huidige browser versie en ook een optie vinden om bij te werken/voor updates te controleren.

Zie Chrome:

![Proefweergave_3.png](assets/proofview-3-350x206.png)

Als je beschikt over de nieuwste [!DNL Flash Player] Klik op de geïnstalleerde plug-in en browserversie om de proefdruk opnieuw te openen en na te gaan of het probleem is opgelost.

## Zorg ervoor dat uw lokale [!DNL Flash] Opslag is beschikbaar

Ons [!DNL Workfront Proof] De viewer is gebaseerd op de Flash en we slaan gegevens op over de proefdrukken (opmerkingen, proeftegels, proefdrukken, [!DNL Workfront Proof] Viewer-instellingen) op uw computer met [!DNL Flash Player]. Als de [!DNL Workfront Proof] De viewer wordt geopend, maar er is geen inhoud in de viewer. Zorg ervoor dat de Flash Storage beschikbaar is op uw computer en dat [!DNL Workfront Proof] mag het gebruiken.

Als er wat opslagruimte is toegewezen, maar u werkt met grotere proefdrukken met meerdere pagina&#39;s en opmerkingen, probeert u de [!DNL Flash] Bewaar en laad uw proefdruk opnieuw.

Zie onze [Problemen met het bekijken van proefdrukken - [!DNL Flash] Gedeelde objecten beschreven](../../../workfront-proof/wp-tech-corner/troubleshooting/view-proof-flash-shared-object.md) voor de gedetailleerde instructies.

## Identificeer waar het probleem is

* Worden de proefdrukken geopend in een andere browser?
* Als u dagelijks één browser gebruikt en u problemen hebt met het bekijken van de proefdrukken, probeert u dezelfde proefdruk te openen in een andere browser op uw computer. Als u dit wilt doen, kopieert u de proefdrukkoppeling van de URL-balk van uw hoofdbrowser en plakt u deze in een andere browser. Als de proefdruk daar goed opent, herzie uw belangrijkste browser configuratie, stop-ins en uitbreidingen aangezien deze zich kunnen mengen.
* We hebben geen voorkeursbrowser, maar als er prestatieproblemen optreden in uw huidige browser, raden we u aan over te schakelen op een andere browser.
* Worden de proefdrukken geopend op een andere computer op uw locatie?
Als de proefdruk niet wordt geopend in een browser op uw computer, probeert u deze te openen op een andere computer op uw locatie en/of buiten uw locatie. Dit zal u toestaan om te bepalen als een kwestie aan uw bepaalde machine of als het iets in uw lokaal netwerk is te wijten.
Als uw beveiligingsniveau hoger is, kunt u uw verbindingen met [!DNL Workfront Proof] kan worden geblokkeerd door:

   * Uw lokale AV-software
   * Uw oplossing voor netwerkbeveiliging
   * DNS-, firewall- of proxyconfiguratie
   * Dit zijn de instellingen die buiten onze controle liggen. Er zijn diverse beschikbare veiligheidsoplossingen en wij kunnen niet zien welke in uw netwerk worden uitgevoerd en welke verbindingen kunnen blokkeren aan [!DNL Workfront Proof]. Het is ook niet aan [!DNL Workfront Proof] om uw interne veiligheidsconfiguratie te beslissen. Als u problemen hebt met het openen van de proefdrukken op de meerdere computers in uw locatie/netwerk, raden wij u aan contact op te nemen met uw IT-team zodat zij de netwerkinstellingen kunnen controleren en de [!DNL Workfront Proof] in de lijst van gewenste personen, indien nodig.

* Zijn de verbindingen met [!DNL Workfront Proof] toegestaan in uw netwerk?
In de Proefweergave laden we de tegels - fragmenten van de pagina&#39;s. Als deze inhoud aan uw uiteinde niet goed wordt geladen, kan het zijn dat sommige verbindingen met [!DNL Workfront Proof] worden geblokkeerd in uw netwerk. U zult ervoor willen zorgen dat alle verbindingen en alle inhoud van *.proofhq.com aan de lijst van gewenste personen wordt toegevoegd. Uw IT-team moet hierbij kunnen helpen.

## Insteekmodules controleren

Als uw browser en [!DNL Flash Player] de insteekmodule is bijgewerkt en uw netwerk blokkeert niet de verbindingen aan [!DNL Workfront Proof] er kan iets in uw browser zijn dat het bekijken van de proefdrukken beïnvloedt. Er zijn momenteel meerdere plug-ins en extensies beschikbaar in uw browser. Sommige van deze plug-ins veroorzaken een conflict of veroorzaken een conflict met andere plug-ins.

De beste praktijken moeten alle onbekende toe:voegen-ons verwijderen en slechts degenen houden die u gebruikt en die u vertrouwt. Elke browser moet u opties bieden om de plug-ins en extensies te controleren, te wijzigen of te verwijderen. Ons [!DNL Workfront Proof] Viewer is gebaseerd op [!DNL Flash] en gebruiken JavaScript om de viewer te laden, zodat u vooral de insteekmodules wilt raadplegen die deze kunnen beïnvloeden.

Als er om het even welke bepaalde toe:voegen-op interfereert met het laden van de proeven kunt u proberen de details in de console van browser te controleren.

![Proefweergave_4.png](assets/proofview-4-350x57.png)

In de meeste nieuwere browsers zijn er enkele extra tools voor ontwikkelaars beschikbaar die kunnen worden gebruikt voor geavanceerdere probleemoplossing.

Als u problemen hebt met het bekijken van de proefdrukken:

* Open de browserconsole en laad de proefdruk opnieuw.
* Controleer of de console waarschuwingen of berichten bevat. Deze details kunnen helpen identificeren wat de worteloorzaak van de kwesties is.
* Laat uw IT-team de resultaten analyseren. Zij moeten advies kunnen geven en kunnen helpen het lokale probleem op te lossen.
* Deel de resultaten met ons ondersteuningsteam. We zullen graag hulp bieden.


## Instellingen voor gemengde inhoud controleren

Alle verbindingen met [!DNL Workfront Proof] zijn via HTTPS. In de [!DNL Workfront Proof] Viewer we laden de tegels via HTTP en de gegevens worden beveiligd met de tokens. Dit leidt tot Gemengde Inhoud die sommige browsers of veiligheidsoplossingen (door gebrek of volgens handconfiguratie) kunnen blokkeren.

Als dit de reden is waarom de proeven niet op uw computer openen (u zou de relevante alarm in de console van browser moeten kunnen zien) dergelijke verbindingen voor machtigen [!DNL Workfront Proof] of wijzig de instellingen om passief gemengde inhoud op uw computer toe te staan. De gemengde inhoud kan door uw browser, AV software, netwerkconfiguratie enz. worden geblokkeerd - om de nauwkeurige oorzaak te bepalen gelieve in contact met uw team/netwerkbeheerders van IT te krijgen. Ze moeten ook de gemengde inhoud op uw computer kunnen inschakelen.


