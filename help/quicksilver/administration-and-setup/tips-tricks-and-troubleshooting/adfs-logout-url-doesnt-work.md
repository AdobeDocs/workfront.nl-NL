---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ADFS-aanmeldings-URL werkt niet
description: De op deze pagina beschreven procedure is alleen van toepassing op organisaties die nog niet aan boord van de Adobe Admin Console zijn.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4d868625-e976-47b4-9e80-f1eca84a2768
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# ADFS-aanmeldings-URL werkt niet

>[!IMPORTANT]
>
>De op deze pagina beschreven procedure is alleen van toepassing op organisaties die nog niet zijn aangemeld bij de [!UICONTROL Adobe Admin Console].
>
>Als uw organisatie is aangemeld bij de [!UICONTROL Adobe Admin Console], zie [verschillen in toediening op basis van Platforms ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## Probleem

Wanneer u de URL voor afmelden met ADFS (https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0) gebruikt, ontvangt u een berichtpagina met de fout: &quot;Er is een probleem opgetreden bij het openen van de site. Blader opnieuw naar de site.&quot;

Als het probleem zich blijft voordoen, neemt u contact op met de beheerder van deze site en geeft u het volgende referentienummer om het probleem te identificeren: **57092dfc-751a-4915-8e6a-b4c5d413f8c6**

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront] licentie</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een [!DNL Workfront] beheerder. Zie voor meer informatie <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Oplossing

1. Ga in uw ADFS-beheerserver naar **[!UICONTROL Trust Relationships]** > **[!UICONTROL Relying Party Trusts]** > `<your party trust>` eigenschappen.

1. Onder de **[!UICONTROL Endpoints]** tabblad, klikt u op **[!UICONTROL Add]**.

1. **[!UICONTROL Endpoint Type]** = SAML Logout, Binding = POST, URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0

   U kunt een reactie-URL instellen als u deze wilt doorsturen naar een andere pagina. Maar wij adviseren de plaats ADFS omdat het waarschuwt dat u wordt geregistreerd, maar u zou uw browser moeten nog sluiten.
