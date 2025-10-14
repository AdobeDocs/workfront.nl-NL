---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Problemen oplossen - beschadigd interfacefont in proefdrukviewer op Mac
description: Problemen met beschadigd interfacefont oplossen in proefdrukviewer op Mac
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1e96720a-b967-4447-bd14-26fc6a502b25
source-git-commit: c3e15a052533d43065b50a9f56169b82f8dc3765
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 0%

---

# Problemen oplossen - beschadigd interfacefont in proefdrukviewer op Mac

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het zelfstandige product [!DNL Workfront Proof] . Voor informatie bij het proef binnen [!DNL Adobe Workfront], zie [&#x200B; het Bewijzen &#x200B;](../../../review-and-approve-work/proofing/proofing.md).

Als u ziet dat het interfacetype niet correct wordt weergegeven in de proefdrukviewer, kan dit worden veroorzaakt door een aantal problemen met de lettertypen op uw Mac-computer. Probeer de volgende oplossingen om het probleem op te lossen:

## Fontduplicaten verwijderen

Controleer of het systeem dubbele lettertypen bevat.

1. Sluit de browser die u gebruikt.
1. Open de toepassing Fontboek in de map Programma&#39;s.
1. Klik op **[!UICONTROL All Fonts]** (1).
1. Klik op **[!UICONTROL Edit]** > **[!UICONTROL Look for Enabled Duplicates]** .

1. Klik op **[!UICONTROL Yes]** om duplicaten op te lossen.
1. Als er een waarschuwing over beschadigde lettertypen wordt weergegeven, klikt u op **[!UICONTROL Yes]** .
1. Start de computer opnieuw op.
1. Voer de proefdruk opnieuw uit.

## De fontcache wissen

Soms worden de fontcache in Mac OS X beschadigd. Bijvoorbeeld wanneer een lettertype of een lettertypefamilie een aantal keren opnieuw wordt geïnstalleerd of wanneer een toepassing is bijgewerkt of opnieuw is geïnstalleerd. Naast de cachebestanden voor lettertypen van het besturingssysteem, hebben sommige toepassingen mogelijk een eigen fontcache. Als u deze cachebestanden voor lettertypen verwijdert, kan het probleem met verstoorde tekst worden opgelost.

Ten eerste moet u het lettertypeboek starten, het lettertype of de familie selecteren waarmee u problemen ondervindt en op de knop Verwijderen op het toetsenbord drukken. U kunt ook met de rechtermuisknop klikken en [!UICONTROL Remove Family] selecteren. Als u niet zeker weet welk lettertype of welke familie de problemen veroorzaakt, wilt u mogelijk eerst duplicaten verwijderen zoals hierboven beschreven.

De tweede stap is het wissen van de fontcache en er zijn verschillende manieren om dit te bereiken.

De eerste is eenvoudig in Veilige Wijze opnieuw op te starten door de sleutel van de Verschuiving onmiddellijk te houden wanneer u de laarzen bij opstarten hoort. Wanneer deze modus wordt geladen, wordt een voortgangsbalk weergegeven waarin het systeem verschillende controles en onderhoudsroutines uitvoert, waaronder het wissen van de fontcache.

De tweede benadering moet de Terminal gebruiken, die door het volgende bevel van binnen een administratieve rekening in werking te stellen kan worden gedaan: *sudo atsutil gegevensbestanden - verwijder*

>[!NOTE]
>
>Voor deze opdracht moet u uw wachtwoord invoeren. Dit wachtwoord wordt niet weergegeven wanneer u typt. We raden u aan overleg te plegen met uw IT-afdeling, omdat hiervoor beheerdersmachtigingen op uw computer nodig kunnen zijn.

Een andere manier is om een hulpprogramma voor fontcache, zoals FontNuke, te gebruiken en de cache te wissen met behulp van dit hulpprogramma.

Veel prepress- en illustratie-/ontwerpstudio&#39;s gebruiken ook Universal Type Server-software om licenties en distributie van lettertypen te beheren. Soms kan er een probleem optreden met de cache van Universal Type Server-lettertypen, waardoor de [!DNL Workfront Proof] -annotaties kunnen verdwijnen.

Als u wilt repareren, wist u het cachegeheugen voor Universal Type-serverlettertypen en start u de Universal Type-server opnieuw.

## Lettertypeconflict [!DNL Flash] herstellen

U hebt mogelijk geen toegang tot deze functionaliteit omdat deze wordt ondersteund door [!DNL Flash] , dat in de meeste omgevingen is vervangen.

De verouderde proefdrukviewer is gebaseerd op [!DNL Flash Player] en soms is er een lettertypeconflict tussen OS X en [!DNL Flash Player] mogelijk wanneer de tekst ontbreekt in de proefdrukviewer. Probeer het volgende:

1. Open Finder en open het tabblad **[!UICONTROL Go]** .
1. Druk op Option (⌥ Alt) om de map [!UICONTROL Library] in de vervolgkeuzelijst te openen.
1. Houd Option ingedrukt en klik op de map [!UICONTROL Library] .
1. Nadat de map [!UICONTROL Library] is geopend, gaat u naar de map [!UICONTROL Fonts] in de map.
1. Verplaats alle lettertypen in de map [!UICONTROL Fonts] naar een andere map, bijvoorbeeld op het bureaublad (maak geen andere map in de map Fonts).
1. Met deze handeling worden al uw aangepaste lettertypen verborgen. De standaardsysteemlettertypen worden dan nog steeds op hun eigen locatie opgeslagen.
1. Sluit [!DNL Safari] af en start het opnieuw.
1. Open de proefdruk opnieuw.

Uw lettertypen moeten nu worden weergegeven. Als u geen van de lettertypen nodig hebt die u uit de thuismap hebt verwijderd, kunt u deze veilig verwijderen. Als u dat niet doet, kopieert u de bestanden batchgewijs naar de map Bibliotheek/Fonts en ziet u welke oorzaak het probleem heeft.
