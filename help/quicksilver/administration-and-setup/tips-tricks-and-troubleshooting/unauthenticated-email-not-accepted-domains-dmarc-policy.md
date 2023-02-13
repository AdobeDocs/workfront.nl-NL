---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Wanneer een geverifieerde e-mail niet wordt geaccepteerd vanwege het DMARC-beleid van het domein
description: Als er een e-mail is verzonden door de [!DNL Workfront] Het systeem wordt niet geaccepteerd vanwege het DMARC-beleid van het domein. Uw e-mailbeheerder kan het probleem verhelpen door uw e-mailsysteem te configureren zodat alle e-mailberichten van workfront.com zijn toegestaan.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2443267a-dcc0-485b-be29-17539fb54188
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# Niet-geverifieerde e-mail wordt niet geaccepteerd vanwege het DMARC-beleid van het domein

## Probleem

[Testen] Ik heb de volgende e-mail met terugstuiterende informatie ontvangen:

550-5.7.1 Niet-geverifieerde e-mail van &quot;customer domain.com&quot; wordt niet geaccepteerd vanwege\
Het DMARC-beleid van het domein 550-5.7.1. Neem contact op met de beheerder van &quot;customer domain.com&quot;\
550-5.7.1 domein als dit een wettige post was. Ga naar\
550-5.7.1 [*https://support.google.com/mail/answer/2451690*](https://support.google.com/mail/answer/2451690) voor meer informatie over DMARC\
550 5.7.1 initiatief.

## Oplossing

DMARC is geconfigureerd in het e-mailsysteem van uw bedrijf en maakt geen deel uit van [!DNL Adobe Workfront]. Als u deze e-mail ontvangt, moet u contact opnemen met uw e-mailbeheerder.

Uw e-mailbeheerder moet uw e-mailsysteem zodanig configureren dat e-mail van noreply@workfront.com of bij voorkeur alle e-mailberichten van workfront.com is toegestaan/vertrouwd.

Zie voor meer informatie over DMARC [https://support.google.com/mail/answer/2451690.](https://support.google.com/mail/answer/2451690)
