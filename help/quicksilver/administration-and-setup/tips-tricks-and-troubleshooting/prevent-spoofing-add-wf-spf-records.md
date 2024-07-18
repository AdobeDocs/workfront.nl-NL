---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Prevent spoofing en voeg  [!DNL Adobe Workfront]  SPF- verslagen toe
description: Als de gebruikers  [!DNL Adobe Workfront]  e-mailberichten niet ontvangen, moet u  [!DNL Workfront]  verslagen SPF aan uw firewall toevoegen. U moet met uw team van IT werken om verslagen toe te voegen SPF.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e93e3334-d72a-4f7b-9379-358f498c873b
source-git-commit: 8bcc2859b3b6ce7a264c8f234536a93b7761ab6b
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 0%

---

# Spoofsvorming voorkomen en [!DNL Adobe Workfront] SPF-records toevoegen

## Probleem

Als gebruikers geen e-mailmeldingen van [!DNL Adobe Workfront] ontvangen, moet u [!DNL Workfront] SPF-records toevoegen aan uw firewall. U moet met uw team van IT werken om verslagen toe te voegen SPF.

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
   <td> <p>U moet een [!DNL Workfront] beheerder zijn. Voor meer informatie, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref"> een gebruiker volledige administratieve toegang verlenen </a>.</p> <p><b> NOTA </b>: Als u nog geen toegang hebt, vraag uw [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] beheerder uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Oplossing

Als u reeds de IP adressen aan uw lijst van gewenste personen voor uw productiemilieu zoals die in [ wordt beschreven toevoegde vormt de lijst van gewenste personen van uw firewall ](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) en de gebruikers ontvangen nog geen e-mail:

1. Voeg het volgende SPF verslag aan uw firewall toe:

   *spf.workfront.com*

   Hierdoor worden automatisch alle [!DNL Workfront] IP-adressen aan de lijst van gewenste personen op uw firewall toegevoegd en kunnen alle spamfilters (die gebruikmaken van SPF-records) [!DNL Workfront] -servers valideren als geldige afzenders voor uw domein.

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

   Bijvoorbeeld &quot;v=spf1 a mx include: spf.workfront.com -all&quot;

Als u vanwege het bedrijfsbeleid geen SPF-records aan uw firewall kunt toevoegen, werkt u samen met uw [!DNL Workfront] ondersteuningsvertegenwoordiger.
