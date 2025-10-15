---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ADFS-aanmeldings-URL werkt niet
description: De op deze pagina beschreven procedure is alleen van toepassing op organisaties die nog niet aan boord van de Adobe Admin Console zijn.
author: Becky, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4d868625-e976-47b4-9e80-f1eca84a2768
source-git-commit: fb555df123701c62e9a0f2d451ad6dcd16586595
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 1%

---

# ADFS-aanmeldings-URL werkt niet

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>De procedure die op deze pagina wordt beschreven, is alleen van toepassing op organisaties die nog niet zijn aangemeld bij de [!UICONTROL Adobe Admin Console] .
>
>Als uw organisatie aan [!UICONTROL Adobe Admin Console] is bezet, zie [&#x200B; Op platform-gebaseerde beleidsverschillen ([!DNL Adobe Workfront]/ [!DNL Adobe Business Platform]) &#x200B;](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## Probleem

Wanneer u de URL voor afmelden met ADFS (https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0) gebruikt, ontvangt u een berichtpagina met de fout: &quot;Er is een probleem opgetreden bij het openen van de site. Blader opnieuw naar de site.&quot;

Als het probleem voortduurt, contacteer de beheerder van deze plaats en verstrek het volgende verwijzingsaantal om het probleem te identificeren: **57092dfc-751a-4915-8e6a-b4c5d413f8c6**

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront] -pakket</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront] -licentie</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>[!UICONTROL System Administrator]</td>  
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Oplossing

1. Ga in uw ADFS-beheerserver naar **[!UICONTROL Trust Relationships]** > **[!UICONTROL Relying Party Trusts]** > `<your party trust>` -eigenschappen.

1. Klik onder het tabblad **[!UICONTROL Endpoints]** op **[!UICONTROL Add]** .

1. **[!UICONTROL Endpoint Type]** = SAML Logout, Binding = POST, URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0

   U kunt een reactie-URL instellen als u deze wilt doorsturen naar een andere pagina. Maar wij adviseren de plaats ADFS omdat het waarschuwt dat u wordt geregistreerd, maar u zou uw browser moeten nog sluiten.
