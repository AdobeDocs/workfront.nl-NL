---
title: Metagegevenstoewijzing instellen
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Metagegevens zijn beschrijvende informatie die aan een document is gekoppeld. U kunt opstelling  [!DNL Adobe Workfront]  om meta-gegevens met documenten te omvatten die naar  [!DNL Workfront]  toepassingen worden verzonden.
author: Courtney, Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 7cf4787d-7cff-489e-bd5b-69db3ff09f6e
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '539'
ht-degree: 0%

---

# Metagegevenstoewijzing instellen

Metagegevens zijn beschrijvende informatie die aan een document is gekoppeld. U kunt [!DNL Adobe Workfront] zo instellen dat metagegevens worden opgenomen in documenten die naar [!DNL Workfront] -toepassingen worden verzonden.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table>
  <tr>
   <td>Adobe Workfront-pakket
   </td>
   <td> <p>Prime of Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr>
  <tr>
   <td>Adobe Workfront-licenties
   </td>
   <td><p>Standard</p>
   <p>Plan</p>
   </td>
  </tr>
   <tr>
   <td>Configuraties op toegangsniveau
   </td>
   <td>U moet een [!DNL Workfront] beheerder zijn.
   </td>
  </tr>
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Informatie over [!DNL Workfront] metagegevens

Metagegevens voor documenten in [!DNL Workfront] kunnen informatie bevatten zoals de verwante projectnaam, taakbeschrijving of Geplande voltooiingsdatum. Als [!DNL Workfront] beheerder kunt u [!DNL Workfront] zo configureren dat metagegevens worden opgenomen in documenten die vanuit [!DNL Workfront] naar de volgende [!DNL Workfront] -toepassingen worden verzonden:

* [!DNL Workfront DAM]

Voordat metagegevens met documenten kunnen worden verzonden, moet u eerst de metagegevens opgeven die u in het bestand wilt opnemen. U kunt elk veld toewijzen dat in [!DNL Workfront] wordt gebruikt. Als u de metagegevenstoewijzing hebt ingesteld, worden de toegewezen metagegevens opgenomen in alle documenten die naar een [!DNL Workfront] -toepassing zijn geüpload.

Wanneer een gebruiker een document van [!DNL Workfront] naar een [!DNL Workfront] -toepassing verzendt, worden de toegewezen metagegevens over het document overgedragen. Hoewel de versie van het document in de [!DNL Workfront] -toepassing is gekoppeld aan [!DNL Workfront] , worden wijzigingen die in de metagegevens van het document in [!DNL Workfront] zijn aangebracht, niet doorgevoerd in de metagegevens van het document in de [!DNL Workfront] -toepassing. Als een toegewezen veld in [!DNL Workfront] wordt gewijzigd, moet u een nieuwe versie van het document met de bijgewerkte metagegevens naar de [!DNL Workfront] -toepassing sturen.

>[!NOTE]
>
>U kunt metagegevens slechts in één richting toewijzen: van [!DNL Workfront] tot [!DNL Workfront DAM] . Metagegevens voor documenten die zijn gekoppeld aan [!DNL Workfront] van [!DNL Workfront DAM] kunnen niet worden overgebracht naar Workfront.

U kunt hetzelfde [!DNL Workfront] -veld toewijzen aan verschillende metagegevensvelden in [!DNL Workfront DAM] , maar u kunt in geen van deze toepassingen een metagegevensveld gebruiken voor meerdere metagegevensvelden van [!DNL Workfront] .

Als u meerdere [!DNL Workfront] -velden wilt configureren voor export naar één metagegevensveld in een [!DNL Workfront] -toepassing, maakt u eerst een berekend aangepast veld in [!DNL Workfront] om alle afzonderlijke aangepaste velden van een object weer te geven. Wijs vervolgens het berekende [!DNL Workfront] veld toe aan een metagegevensveld in de [!DNL Workfront] -toepassing. Voor meer informatie over berekende douanevelden, zie [ berekende gebieden aan een vorm ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) toevoegen.

Voordat u velden kunt toewijzen voor het toewijzen van metagegevens, moet u de toepassing inschakelen in [!DNL Workfront] . Voor meer informatie, zie [ documentintegratie ](../../administration-and-setup/configure-integrations/configure-document-integrations.md) vormen.

## [!DNL Workfront] configureren voor het verzenden van metagegevens

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op **[!UICONTROL Documents]** > **[!UICONTROL Metadata Mapping]** .

   ![ de afbeelding van Meta-gegevens ](assets/metadata-mapping.png)

1. Typ in het vak **[!UICONTROL Select Source Field for Mapping]** de naam van het Workfront-veld dat u wilt toewijzen aan [!DNL Workfront DAM] en selecteer het veld wanneer het in de lijst wordt weergegeven.
1. Selecteer in het vak **[!UICONTROL Select Target Field for Mapping]** het veld dat u wilt vullen met de gegevens in het geselecteerde [!DNL Workfront] -veld.

1. Klik op **[!UICONTROL Add Mapping]**.

   Het toegewezen veld wordt weergegeven in de toegewezen velden die onder aan de pagina worden vermeld.

1. Herhaal stap 5 en 6 totdat u alle gewenste [!DNL Workfront] -velden en de bijbehorende [!DNL Workfront DAM] -velden toevoegt.

## Toegewezen velden verwijderen

1. Meld u aan bij [!DNL Workfront] als de beheerder.

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op **[!UICONTROL Documents]** > **[!UICONTROL Metadata Mapping]** .

1. Selecteer in de lijst met toegewezen velden de velden die u uit de metagegevenstoewijzing wilt verwijderen.
1. Klik op **[!UICONTROL Delete]**.

   De toegewezen velden worden niet meer toegewezen. Wanneer een gebruiker nu een document verzendt van [!DNL Workfront] naar [!DNL Workfront DAM] , worden de metagegevens in de verwijderde velden niet samen met het document overgedragen.

   In een document dat is verzonden voordat u de toegewezen velden verwijdert, blijven de oorspronkelijke metagegevens behouden die ermee zijn verzonden, inclusief de metagegevens voor de verwijderde velden.
