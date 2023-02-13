---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Problemen oplossen - beschadigd interfacefont in proefdrukviewer op Mac
description: 'Als u ziet dat het interfacetype niet correct wordt weergegeven in de proefdrukviewer, kan dit worden veroorzaakt door een aantal problemen met de lettertypen op uw Mac-computer. Probeer de volgende oplossingen om het probleem op te lossen: BEWERK ME.'
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1e96720a-b967-4447-bd14-26fc6a502b25
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '669'
ht-degree: 0%

---

# Problemen oplossen - beschadigd interfacefont in proefdrukviewer op Mac

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het standalone product [!DNL Workfront Proof]. Voor informatie over proefdrukken binnen [!DNL Adobe Workfront], zie [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Als u ziet dat het interfacetype niet correct wordt weergegeven in de proefdrukviewer, kan dit worden veroorzaakt door een aantal problemen met de lettertypen op uw Mac-computer. Probeer de volgende oplossingen om het probleem op te lossen:

## Fontduplicaten verwijderen

Controleer of het systeem dubbele lettertypen bevat.

1. Sluit de browser die u gebruikt.
1. Open de toepassing Fontboek in de map Programma&#39;s.
1. Klikken **[!UICONTROL All Fonts]** (1)
1. Klik op **[!UICONTROL Edit]** > **[!UICONTROL Look for Enabled Duplicates]**.

1. Klikken **[!UICONTROL Yes]** om duplicaten op te lossen.
1. Als er een waarschuwing over beschadigde lettertypen wordt weergegeven, klikt u op **[!UICONTROL Yes]**.
1. Start de computer opnieuw op.
1. Voer de proefdruk opnieuw uit.

## De fontcache wissen

Soms worden de fontcache in Mac OS X beschadigd. Bijvoorbeeld wanneer een lettertype of een lettertypefamilie een aantal keren opnieuw wordt geïnstalleerd of wanneer een toepassing is bijgewerkt of opnieuw is geïnstalleerd. Naast de cachebestanden voor lettertypen van het besturingssysteem, hebben sommige toepassingen mogelijk een eigen fontcache. Als u deze cachebestanden voor lettertypen verwijdert, kan het probleem met verstoorde tekst worden opgelost.

Ten eerste moet u het lettertypeboek starten, het lettertype of de familie selecteren waarmee u problemen ondervindt en op de knop Verwijderen op het toetsenbord drukken. U kunt ook met de rechtermuisknop klikken en [!UICONTROL Remove Family]. Als u niet zeker weet welk lettertype of welke familie de problemen veroorzaakt, wilt u mogelijk eerst duplicaten verwijderen zoals hierboven beschreven.

De tweede stap is het wissen van de fontcache en er zijn verschillende manieren om dit te bereiken.

De eerste is eenvoudig in Veilige Wijze opnieuw op te starten door de sleutel van de Verschuiving onmiddellijk te houden wanneer u de laarzen bij opstarten hoort. Wanneer deze modus wordt geladen, wordt een voortgangsbalk weergegeven waarin het systeem verschillende controles en onderhoudsroutines uitvoert, waaronder het wissen van de fontcache.

De tweede benadering is Terminal te gebruiken, die door het volgende bevel van binnen een administratieve rekening in werking te stellen kan worden gedaan: *sudo atsutil databases - remove*

>[!NOTE]
>
>Voor deze opdracht moet u uw wachtwoord invoeren. Dit wachtwoord wordt niet weergegeven wanneer u typt. We raden u aan overleg te plegen met uw IT-afdeling, omdat hiervoor beheerdersmachtigingen op uw computer nodig kunnen zijn.

Een andere manier is om een hulpprogramma voor fontcache, zoals FontNuke, te gebruiken en de cache te wissen met behulp van dit hulpprogramma.

Veel prepress- en illustratie-/ontwerpstudio&#39;s gebruiken ook Universal Type Server-software om licenties en distributie van lettertypen te beheren. Soms kan er een probleem optreden met de cache voor Universal Type Server-lettertypen, die de [!DNL Workfront Proof] annotaties die moeten verdwijnen.

Als u wilt repareren, wist u het cachegeheugen voor Universal Type-serverlettertypen en start u de Universal Type-server opnieuw.

## Repareren [!DNL Flash] lettertypeconflict

U hebt mogelijk geen toegang tot deze functionaliteit omdat deze wordt ondersteund door [!DNL Flash], die in de meeste omgevingen verouderd is.

De verouderde proefdrukviewer is gebaseerd op [!DNL Flash Player] en soms is er een lettertypeconflict tussen OS X en [!DNL Flash Player]. Probeer het volgende:

1. Open de Finder en open de **[!UICONTROL Go]** tab.
1. Druk op Option (⌥ Alt) om het dialoogvenster [!UICONTROL Library] in de vervolgkeuzelijst.
1. Houd Option ingedrukt en klik op de knop [!UICONTROL Library] map.
1. Na de [!UICONTROL Library] map wordt geopend, ga naar [!UICONTROL Fonts] in.
1. Alle fonts in het deelvenster [!UICONTROL Fonts] naar een andere map op uw bureaublad (maak geen andere map in de map Fonts).
1. Met deze handeling worden al uw aangepaste lettertypen verborgen. de standaardsysteemlettertypen moeten op hun aparte locatie worden opgeslagen.
1. Afsluiten en opnieuw starten [!DNL Safari].
1. Open de proefdruk opnieuw.

Uw lettertypen moeten nu worden weergegeven. Als u geen van de lettertypen nodig hebt die u uit de thuismap hebt verwijderd, kunt u deze veilig verwijderen. Als u dat niet doet, kopieert u de bestanden batchgewijs naar de map Bibliotheek/Fonts en ziet u welke oorzaak het probleem heeft.
