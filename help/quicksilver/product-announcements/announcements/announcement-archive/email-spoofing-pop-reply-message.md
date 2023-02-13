---
content-type: reference
navigation-topic: announcements
title: E-mailspoofing en antwoordverwijdering
description: We brengen twee wijzigingen aan in de manier waarop Adobe Workfront e-mail verzendt en ontvangt met de release van 20.3 (gepland augustus 2020).
author: Luke
feature: Product Announcements
exl-id: 9110f04d-b7a9-428b-928c-c4eb746fec3f
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# E-mailwoordenboek en POP-reactie

We brengen twee wijzigingen aan in de manier waarop Adobe Workfront e-mail verzendt en ontvangt met de release van 20.3 (gepland augustus 2020).

## Uitgaande e-mail van Workfront

Om ervoor te zorgen dat e-mails met succes worden geleverd, elimineren we spoofing van e-mailberichten, die vaak als spam worden gelabeld (zie E-mailspoofing). Alle e-mailberichten van Workfront worden verzonden van notifications@my.workfront.com, inclusief zowel automatische waarschuwingen als gebruikerscommunicatie. Een voorbeeld-e-mail van Joan Harris ziet er zo uit in het gebied van uw e-mail:

![](assets/noreply.png)

*We raden u aan contact op te nemen met uw IT-team* om ervoor te zorgen dat e-mail van notifications@my.workfront.com niet wordt geblokkeerd voor inkomende e-mail naar uw systeem. U kunt ook naar [De lijst van gewenste personen van uw firewall configureren](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) voor details over welke IP ons verkeer en e-mail komt.

## Binnenkomende e-mailantwoorden op meldingen (POP-antwoord)

Met bepaalde e-mailberichten kunnen gebruikers via e-mail reageren en het antwoord laten kopiëren naar Workfront als reactie op opmerkingen in het Workfront-systeem. Systeembeheerders in Workfront hebben van oudsher kunnen kiezen tussen het leveren van hun eigen POP-e-mailserver voor het ontvangen van deze reacties of het gebruik van het ingebouwde Workfront-antwoordsysteem. De aangepaste keuze voor de POP-e-mailserver wordt verwijderd met de release 20.3. Alle accounts die zijn geconfigureerd om een aangepaste server te gebruiken, worden automatisch overgezet om het native Workfront-antwoordsysteem voor e-mail te gebruiken. Er is geen actie vereist voor systeembeheerders of andere Workfront-gebruikers.

E-mailberichten die rechtstreeks afkomstig zijn van het Workfront Proof-systeem worden niet gewijzigd. Je blijft deze e-mailberichten ontvangen zoals je in het verleden hebt gedaan.

Neem contact op met de [Workfront-ondersteuningsteam](https://one.workfront.com/s/support?language=en_US).
