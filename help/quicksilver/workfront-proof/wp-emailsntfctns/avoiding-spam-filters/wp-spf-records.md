---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Workfront Proof SPF-records
description: Workfront Proof stuurt e-mailmeldingen naar uw revisoren via een Workfront Proof-e-mailadres, zoals notification@proofing.yourdomain.com. Om ervoor te zorgen dat de e-mailservers van uw ontvangers alle e-mailberichten van Workfront Proof vertrouwen, moet u opstelling a  [!DNL Sender Policy]  het verslag van het Kader (SPF) voor uw aangepast domein dat met de  [!DNL Workfront Proof]  wordt verbonden rekening (bijvoorbeeld, proofing.yourdomain.com).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 5295d451-2ad2-4835-9200-f10d4e6286a2
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---

# Workfront Proof SPF-records

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het zelfstandige product [!DNL Workfront Proof] . Voor informatie bij het proef binnen [!DNL Adobe Workfront], zie [&#x200B; het Bewijzen &#x200B;](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] verzendt e-mailmeldingen naar uw revisoren via een [!DNL Workfront Proof] -e-mailadres, zoals notification@proofing.yourdomain.com. Om ervoor te zorgen dat de e-mailservers van uw ontvangers alle [!DNL Workfront Proof] e-mailberichten vertrouwen, moet u opstelling een [!UICONTROL Sender Policy Framework] (SPF) verslag voor uw aangepast domein dat met de [!DNL Workfront Proof] rekening wordt verbonden (bijvoorbeeld, **proofing.yourdomain.com**).

Om opstelling een SPF verslag, zult u het SPF verslag moeten omvatten dat voor ons primair domein wordt gebruikt.

1. Voeg een **[!UICONTROL DNS TXT]** -item voor uw domein toe met de volgende waarde:

   `v=spf1 a:mx.proofhq.com -all`

   Uw e-mailbeheerder of IT-personeel kan u helpen dit in te stellen.

   >[!TIP]
   >
   >U kunt het vrije hulpmiddel bij [[!DNL https://mxtoolbox.com/spf.aspx] gebruiken &#x200B;](https://mxtoolbox.com/spf.aspx) om [!DNL Workfront] verslagen van SPF te herzien.
