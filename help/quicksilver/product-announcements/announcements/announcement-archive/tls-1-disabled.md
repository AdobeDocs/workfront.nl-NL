---
content-type: reference
navigation-topic: announcements
title: TLS 1.2 is vereist in Adobe Workfront
description: Om optimale beveiliging te bieden, eist Adobe Workfront dat alle browserverbindingen en API-integratie die afhankelijk zijn van TLS 1.0 of eerder, worden geüpgraded naar het gebruik van TLS 1.2. In de voorvertoningsomgeving is TLS 1.0 al uitgeschakeld.
author: Luke
feature: Product Announcements
exl-id: 153668ae-0647-47fd-9153-ce45cd8c54ee
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# TLS 1.2 is vereist in Adobe Workfront

Om optimale beveiliging te bieden, eist Adobe Workfront dat alle browserverbindingen en API-integratie die afhankelijk zijn van TLS 1.0 of eerder, worden geüpgraded naar het gebruik van TLS 1.2. In de voorvertoningsomgeving is TLS 1.0 al uitgeschakeld.

Workfront heeft in maart 2018 officieel de steun voor TLS 1.0 beëindigd. Alle integratie waarbij TLS 1.0 werd gebruikt, verliep vanaf 9 januari 2019 niet meer.  TLS 1.1 wordt in het vierde kwartaal van 2019 uitgeschakeld.

De volgende secties verstrekken meer detail over deze belangrijke mijlpalen, evenals hoe u voor deze verbetering in uw organisatie kunt voorbereidingen treffen:

## Workfront beëindigt de officiële ondersteuning van TLS 1.0 (5 maart 2018)

Workfront heeft in maart 2018 de officiële ondersteuning voor TLS 1.0 beëindigd.

Browserverbindingen en API-integratie die gebruikmaken van TLS 1.0 zijn nog steeds operationeel, maar Workfront lost problemen in de Workfront-toepassing die betrekking hebben op TLS 1.0 niet op.

## Workfront-integratie met TLS 1.0 uitgeschakeld (9 januari 2019)

Op 9 januari 2019 moeten alle Workfront-browserverbindingen en API-integraties die gebruikmaken van TLS 1.0 worden bijgewerkt om TLS 1.1 of hoger te kunnen gebruiken. Browserverbindingen en API-integratie die verder gebruikmaken van TLS 1.0 (binnenkomende of uitgaande verbindingen), kunnen na deze tijd niet meer communiceren met de Workfront-toepassing. 

## TLS 1.1 uit te schakelen in het vierde kwartaal van 2019

In de productieomgeving werd TLS 1.1 op 21 oktober 2019 uitgeschakeld. Na deze tijd werken alle integraties met TLS 1.1 niet meer.

Deze wijziging treedt in werking op 7 augustus in de omgeving van de voorvertoning en de sandbox om organisaties te helpen zich voor te bereiden op het uitschakelen.

## Voorbereiden op de TLS-upgrade

* [Bij toegang tot Workfront via de browser](#when-accessing-workfront-via-the-browser)
* [Wanneer u verbinding maakt met Workfront via de API](#when-connecting-to-workfront-via-the-api)

### Bij toegang tot Workfront via de browser {#when-accessing-workfront-via-the-browser}

Zorg ervoor dat gebruikers in uw organisatie Workfront openen via een ondersteunde browser. (Voor informatie over ondersteunde browsers raadpleegt u [Adobe Workfront-browservereisten](../../../workfront-basics/workfront-browser-requirements.md).)

Alle browsers die door Workfront worden ondersteund, zijn compatibel met TLS 1.2.

### Wanneer u verbinding maakt met Workfront via de API {#when-connecting-to-workfront-via-the-api}

Als u toepassingen van derden via de API (zowel binnenkomend als uitgaand) integreert in Workfront, moet u ervoor zorgen dat TLS 1.2 (en de TLS 1.2-coderingsprotocollen) in uw integratie is ingeschakeld.
