---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Workfront Proof SPF-records
description: Workfront Proof verzendt e-mailmeldingen naar uw revisoren via een Workfront Proof-e-mailadres, zoals notification@proofing.yourdomain.com. Om ervoor te zorgen dat de e-mailservers van uw ontvangers alle e-mailmeldingen van Workfront Proof vertrouwen, moet u een [!DNL Sender Policy] Het verslag van het kader (SPF) voor uw aangepaste domein dat met het wordt verbonden [!DNL Workfront Proof] account (bijvoorbeeld proofing.yourdomain.com).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 5295d451-2ad2-4835-9200-f10d4e6286a2
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# Workfront Proof SPF-records

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het standalone product [!DNL Workfront Proof]. Voor informatie over proefdrukken binnen [!DNL Adobe Workfront], zie [Proofing](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] stuurt e-mailmeldingen naar uw controleurs vanuit een [!DNL Workfront Proof] e-mailadres, bijvoorbeeld notification@proofing.yourdomain.com. Om ervoor te zorgen dat de e-mailservers van uw ontvangers alle [!DNL Workfront Proof] e-mailmeldingen, moet u een [!UICONTROL Sender Policy Framework] (SPF) record voor uw aangepaste domein dat is verbonden met het [!DNL Workfront Proof] account (bijvoorbeeld **proofing.yourdomain.com**).

Om opstelling een SPF verslag, zult u het SPF verslag moeten omvatten dat voor ons primair domein wordt gebruikt.

1. Voeg een **[!UICONTROL DNS TXT]** vermelding voor uw domein met de volgende waarde:

   `v=spf1 a:mx.proofhq.com -all`

   Uw e-mailbeheerder of IT-personeel kan u helpen dit in te stellen.

   >[!TIP]
   >
   >U kunt het gratis gereedschap gebruiken op [[!DNL https://mxtoolbox.com/spf.aspx]](https://mxtoolbox.com/spf.aspx) ter beoordeling [!DNL Workfront] SPF-records.
