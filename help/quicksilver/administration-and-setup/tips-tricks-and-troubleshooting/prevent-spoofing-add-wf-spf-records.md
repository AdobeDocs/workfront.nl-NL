---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Spoofberichten voorkomen en toevoegen [!DNL Adobe Workfront] SPF-records
description: Als gebruikers [!DNL Adobe Workfront] e-mailberichten, moet u toevoegen [!DNL Workfront] SPF registreert aan uw firewall. U moet met uw team van IT werken om verslagen toe te voegen SPF.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e93e3334-d72a-4f7b-9379-358f498c873b
source-git-commit: 8bcc2859b3b6ce7a264c8f234536a93b7761ab6b
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# Spoofberichten voorkomen en toevoegen [!DNL Adobe Workfront] SPF-records

## Probleem

Als gebruikers [!DNL Adobe Workfront] e-mailberichten, moet u toevoegen [!DNL Workfront] SPF registreert aan uw firewall. U moet met uw team van IT werken om verslagen toe te voegen SPF.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een [!DNL Workfront] beheerder. Zie voor meer informatie <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Oplossing

Als u reeds de IP adressen aan uw lijst van gewenste personen voor uw productiemilieu zoals die in wordt beschreven toevoegde [De lijst van gewenste personen van uw firewall configureren](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) en gebruikers ontvangen nog steeds geen e-mails:

1. Voeg het volgende SPF verslag aan uw firewall toe:

   *spf.workfront.com*

   Hiermee worden automatisch alle [!DNL Workfront] IP adressen aan uw lijst van gewenste personen op uw firewall en staat alle spamfilters (die verslagen gebruiken SPF) toe om te bevestigen [!DNL Workfront] servers als geldige afzenders voor uw domein.

   >[!NOTE]
   >
   > Een SPF-record is een TXT-record die deel uitmaakt van een DNS-streekbestand. Wij steunen niet het wijzigen van uw DNS streekdossier.

1. U moet specificeren welk type van SPF verslag moet worden gevormd. Dit zijn de geldige types van verslagen SPF:

   * all (https://dmarcian.com/spf-syntax-table/#all)
   * ip4 (https://dmarcian.com/spf-syntax-table/#ip4)
   * ip6 (https://dmarcian.com/spf-syntax-table/#ip6)
   * a (https://dmarcian.com/spf-syntax-table/#a)
   * mx (https://dmarcian.com/spf-syntax-table/#mx)
   * ptr (https://dmarcian.com/spf-syntax-table/#ptr)
   * exists (https://dmarcian.com/spf-syntax-table/#exists)
   * include (https://dmarcian.com/spf-syntax-table/#include)

   Bijvoorbeeld, &quot;v=spf1 a mx omvat: spf.workfront.com -all&quot;

Als u geen verslagen SPF aan uw firewall wegens bedrijfbeleid kunt toevoegen, gelieve met uw te werken [!DNL Workfront] Vertegenwoordiger van de steun.
