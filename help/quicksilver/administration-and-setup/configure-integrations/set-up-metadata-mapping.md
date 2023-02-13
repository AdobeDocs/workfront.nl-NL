---
title: Metagegevenstoewijzing instellen
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Metagegevens zijn beschrijvende informatie die aan een document is gekoppeld. U kunt instellen [!DNL Adobe Workfront] om metagegevens op te nemen met documenten die zijn verzonden naar [!DNL Workfront] toepassingen.
author: Caroline
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 7cf4787d-7cff-489e-bd5b-69db3ff09f6e
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# Metagegevenstoewijzing instellen

Metagegevens zijn beschrijvende informatie die aan een document is gekoppeld. U kunt instellen [!DNL Adobe Workfront] om metagegevens op te nemen met documenten die zijn verzonden naar [!DNL Workfront] toepassingen.

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
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een [!DNL Workfront] beheerder. Zie voor meer informatie <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Info [!DNL Workfront] metagegevens

Metagegevens voor documenten in [!DNL Workfront] kan informatie bevatten zoals de verwante projectnaam, taakbeschrijving of Geplande voltooiingsdatum. Als [!DNL Workfront] beheerder, kunt u vormen [!DNL Workfront] om metagegevens op te nemen met documenten die zijn verzonden van [!DNL Workfront] aan het volgende [!DNL Workfront] toepassingen:

* [!DNL Workfront DAM]

Voordat metagegevens met documenten kunnen worden verzonden, moet u eerst de metagegevens opgeven die u in het bestand wilt opnemen. U kunt elk veld toewijzen dat wordt gebruikt in [!DNL Workfront]. Nadat u metagegevenstoewijzing hebt ingesteld, worden alle documenten geüpload naar een [!DNL Workfront] de toegewezen metagegevens worden in de toepassing opgenomen.

Wanneer een gebruiker een document verzendt van [!DNL Workfront] een [!DNL Workfront] , worden toegewezen metagegevens over het document overgedragen. Terwijl de versie van het document in [!DNL Workfront] toepassing is gekoppeld aan [!DNL Workfront]wijzigingen aangebracht in de metagegevens van het document in [!DNL Workfront] niet worden weerspiegeld in de metagegevens van het document in het dialoogvenster [!DNL Workfront] toepassing. Als een toegewezen veld in [!DNL Workfront] is gewijzigd, moet u een nieuwe versie van het document met de bijgewerkte metagegevens naar de [!DNL Workfront] toepassing.

>[!NOTE]
>
>U kunt metagegevens slechts in één richting toewijzen: van [!DNL Workfront] tot [!DNL Workfront DAM]. Metagegevens voor documenten die zijn gekoppeld aan [!DNL Workfront] van [!DNL Workfront DAM] kan niet worden overgedragen naar Workfront.

U kunt hetzelfde toewijzen [!DNL Workfront] veld naar verschillende metagegevensvelden in [!DNL Workfront DAM], maar u kunt in geen van deze toepassingen voor meerdere toepassingen een metagegevensveld gebruiken [!DNL Workfront] metagegevensvelden.

Meerdere configureren [!DNL Workfront] velden die u wilt exporteren naar één metagegevensveld in een [!DNL Workfront] eerst een berekend aangepast veld maken in [!DNL Workfront] om alle afzonderlijke aangepaste velden van een object weer te geven. Wijs vervolgens de berekende waarden toe [!DNL Workfront] veld naar een metagegevensveld in [!DNL Workfront] toepassing. Zie voor meer informatie over berekende aangepaste velden [Berekende gegevens toevoegen aan een aangepast formulier](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

Voordat u velden kunt toewijzen voor het toewijzen van metagegevens, moet u de toepassing inschakelen in [!DNL Workfront]. Zie voor meer informatie [Documentintegratie configureren](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Configureren [!DNL Workfront] om metagegevens te verzenden

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **[!UICONTROL Documents]** > **[!UICONTROL Metadata Mapping]**.

   ![](assets/metadata-mapping.png)

1. In de **[!UICONTROL Select Source Field for Mapping]** typt u de naam van het Workfront-veld waarnaar u wilt toewijzen [!DNL Workfront DAM]en selecteert u de optie wanneer deze in de lijst wordt weergegeven.
1. In de **[!UICONTROL Select Target Field for Mapping]** selecteert u het veld dat u wilt vullen met de gegevens in het geselecteerde veld [!DNL Workfront] veld.

1. Klik op **[!UICONTROL Add Mapping]**.

   Het toegewezen veld wordt weergegeven in de toegewezen velden die onder aan de pagina worden vermeld.

1. Herhaal stap 5 en 6 totdat u alle gewenste stappen toevoegt [!DNL Workfront] velden en bijbehorende [!DNL Workfront DAM] velden.

## Toegewezen velden verwijderen

1. Aanmelden bij [!DNL Workfront] als de beheerder.
1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **[!UICONTROL Documents]** > **[!UICONTROL Metadata Mapping]**.

1. Selecteer in de lijst met toegewezen velden de velden die u uit de metagegevenstoewijzing wilt verwijderen.
1. Klik op **[!UICONTROL Delete]**.

   De toegewezen velden worden niet meer toegewezen. Nu wanneer een gebruiker een document verzendt van [!DNL Workfront] tot [!DNL Workfront DAM], worden de metagegevens in de verwijderde velden niet samen met het document overgedragen.

   In een document dat is verzonden voordat u de toegewezen velden verwijdert, blijven de oorspronkelijke metagegevens behouden die ermee zijn verzonden, inclusief de metagegevens voor de verwijderde velden.
