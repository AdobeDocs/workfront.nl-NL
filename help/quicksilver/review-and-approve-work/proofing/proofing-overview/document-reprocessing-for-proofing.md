---
product-area: documents
navigation-topic: proofing-overview
title: Documentverwerking voor proefdrukken
description: Wanneer u een document (DOCX, PDF, XLSX, AI) voor proef indient, verwerkt Adobe Workfront het opnieuw zodat het in de het proefdrukken kijker zonder de softwaretoepassing kan tonen u gebruikte om het tot stand te brengen.
author: Courtney
feature: Digital Content and Documents
exl-id: e577fa71-4828-4fc2-93a2-0eddbb5ad2ad
source-git-commit: 332c744ab9b760268620461ed2cb2551caf383cf
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 0%

---

# Documentverwerking voor proefdrukken

Wanneer u een document (DOCX, PDF, XLSX, AI) voor proef indient, verwerkt Adobe Workfront het opnieuw zodat het in de het proefdrukken kijker zonder de softwaretoepassing kan tonen u gebruikte om het tot stand te brengen. 

Elke pagina van uw document wordt als een miniatuurafbeelding weergegeven in de conceptviewer. Wanneer u op een miniatuur klikt, kunt u met 100%, 200% en 400% inzoomen op een bitmapversie van die pagina. Voor proefdrukken met een hoogte of breedte van meer dan 800 mm bedraagt het maximale zoomniveau 200%.

De kleuren in het document worden weergegeven in sRGB met kleurconversie uit de meest recente Adobe-bibliotheek. De proefdrukviewer ondersteunt ICC-profielen (International Color Consortium) die in het document zijn ingesloten.

Alle lettertypetekst wordt in de bijbehorende laag geëxtraheerd zolang u de juiste bestandsextensie gebruikt wanneer u het document naar het systeem uploadt. Tekst die als afbeeldingen of curven is opgenomen, wordt niet weergegeven.

>[!NOTE]
>
>Workfront ondersteunt momenteel documenten die maximaal 2000 pagina&#39;s bevatten. Dit geldt ook voor gecombineerde proefdrukken. Voor meer informatie, zie [&#x200B; tot een multi-paginaproef &#x200B;](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md) leiden.

## Algemene tips

* Omdat PDF-bestanden het meest gestandaardiseerd en betrouwbaar zijn, raden we u aan documenten om te zetten in deze indeling voordat u ze uploadt.
* Gebruik de meest recente versie van uw software om uw originele documenten te maken.
* Als u niet zeker weet welke instellingen u moet gebruiken bij het opslaan of exporteren van uw documenten in de toepassing waarin u deze hebt gemaakt, gebruikt u de standaardinstellingen. 
* Zorg ervoor dat u alle lettertypen die u in een document in het document gebruikt, insluit. Als u aangepaste lettertypen gebruikt, worden deze lettertypen in uw document alleen weergegeven op de computers waarop ze zijn geïnstalleerd. Omdat aangepaste lettertypen echter niet zijn opgenomen in het proefdruksysteem, kunnen er geen aangepaste lettertypen worden gebruikt bij het genereren van het bestand, zelfs niet wanneer deze zijn ingesloten.
* Plaats indien mogelijk alle tekstelementen in de bovenste lagen van het ontwerp. Op deze manier zorgt u ervoor dat de tekst kan worden uitgepakt en geselecteerd in het gereedschap Tekstannotatie.
* Plaats alle afbeeldingen en elementen van uw document erin. Als u deze koppelt vanuit externe bronnen, zoals een ander bestand op uw computer, worden ze niet weergegeven in de proefdruk die u maakt.
* Maak uw document met de aanbevolen standaarden voor het type en optimaliseer het voordat u het uploadt. Hierdoor wordt het document met succes geopend in de proefdrukviewer en in alle andere toepassingen en platforms.
* Voer in uw ontwerpsoftware de &quot;preflight&quot;-opties uit om te zien of er waarschuwingen worden gegenereerd in uw document. Deze opties zijn in de meeste toepassingen beschikbaar als uitvoervoorbeeld, afdrukproductie, enzovoort. Raadpleeg de documentatie bij de toepassing voor meer informatie.
* Zorg ervoor dat de kleurinstellingen in het hele document consistent zijn.
* Als uw document is beveiligd tegen handelingen zoals het kopiëren van bestanden, is het mogelijk dat de inhoud van het document niet kan worden geopend met het gereedschap Proofing.

## Procestijden

Doorgaans duurt de verwerking enkele seconden per pagina. Nochtans, kunnen diverse factoren dit, zoals netwerkverkeer/bandbreedte, lokale verbindingssnelheden, en internationale verbindingssnelheden (voor gebruikers buiten de V.S.) verlengen. Het volgende kan ook van invloed zijn op de verwerkingstijd:

* Voor statische documenten en afbeeldingen: aantal pagina&#39;s, afmetingen van pagina&#39;s, tekstvolume, complexiteit van afbeeldingen en objecten (elementen zoals meerdere vectorelementen, lagen, transparanties).
* Voor video&#39;s: lange duur, grote afmetingen en gebruikte codecs.
* Voor webvastleggingen: laadtijden en afmetingen van de pagina.

## Processtappen

Verzendbestanden bevatten enkele of alle volgende stappen:

1. **Verzending**. Wanneer u een document naar het systeem uploadt, gebruikt u de Nieuwe proefdrukpagina of een API (Application Programming Interface). 
1. **Rij**. Tijdens zware verkeersperioden, kan Workfront bijdragen in de rij moeten plaatsen om te voorkomen dat het systeem wordt overbelast. De meeste proefdrukken besteden slechts een paar seconden in een rij. 
1. **verwerking.** De bestanden bereiken de verwerkingscomputers volgens het inhoudstype. We gebruiken verschillende gereedschappen voor het verwerken van videoproeven, webvastleggingen, statische afbeeldingen en documenten. Bij ZIP-containers (Rich Media Containers) en interactieve webopnameverzendingen is geen verwerking vereist.
