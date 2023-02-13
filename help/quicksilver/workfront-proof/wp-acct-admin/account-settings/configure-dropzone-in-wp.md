---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: De dropzone configureren in [!DNL Workfront Proof]
description: Als [!DNL Workfront Proof] beheerder, kunt u de montages van Dropzone van uw gebruikers plaatsen bekijken en uitgeven. Zie Dropzone voor informatie over Dropzone.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: c5c0c7ac-f829-401d-a27c-9581856a7cec
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---

# De dropzone configureren in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het standalone product [!DNL Workfront Proof]. Voor informatie over proefdrukken binnen [!DNL Adobe Workfront], zie [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Als [!DNL Workfront Proof] beheerder, kunt u de montages van Dropzone van uw gebruikers plaatsen bekijken en uitgeven. Voor informatie over Dropzone raadpleegt u [Dropzone](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md).

1. Klikken **[!UICONTROL Settings]** > **[!UICONTROL Account Settings]** en open vervolgens de **[!UICONTROL Dropzone]** tab.

1. Breng een van de volgende wijzigingen aan in het dialoogvenster **[!UICONTROL Dropzone details]** sectie:

   * **[!UICONTROL Web Dropzone]**: Schakel Dropzone in of uit.
   * **[!UICONTROL Web Dropzone URL]**: De URL die u in uw browser moet invoeren om proefdrukken via de Dropzone te verzenden.
   * **[!UICONTROL Email Dropzone]**: Schakel de Dropzone voor e-mail in of uit.

      >[!NOTE]
      >
      >E-mailen naar dropzones wordt niet meer ondersteund.

   * **[!UICONTROL Dropzone Owner]**: Stel de eigenaar van de dropzone in of bewerk deze. Dit is de persoon die op de hoogte wordt gesteld van nieuwe inzendingen bij de Dropzone. Om als eigenaar Dropzone te worden geplaatst, moet de gebruiker een Supervisor, Admin, het Factureren Admin, of de maker van de rekening zijn. Zie voor meer informatie [Profielen met proefmachtigingen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * **[!UICONTROL Default role for creators]**: Alle verzenders worden als standaardinstelling toegevoegd aan de proefdruk.
   * **[!UICONTROL Email notification for all creators]**: Stel hier de voorkeur voor e-mailwaarschuwingen in voor makers van proefdrukken (respondenten). Zie [Instellingen voor e-mailmeldingen configureren in [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md) voor informatie over de verschillende beschikbare waarschuwingsinstellingen.

   * **[!UICONTROL New version function]**: Schakel de functie Nieuwe versie in en uit op de dropzone. Dit geeft of verwijdert de capaciteit voor mensen om nieuwe versies van proeven via Dropzone voor te leggen.
   * **[!UICONTROL Delete draft proofs after (days)]**: Geef het aantal dagen op waarna een conceptbewijs wordt verwijderd. De proefdrukken blijven in een ontwerpstatus als de Dropzone-verzending niet is voltooid nadat het bestand naar de Dropzone is geüpload.
   * **[!UICONTROL Hide reviewer role]**: Het veld revisorrol verbergen wanneer u personen toevoegt aan de dropzone.
   * **[!UICONTROL Send proof message on activation]**: Configureren [!DNL Workfront Proof] de controleurs automatisch een e-mailbericht sturen wanneer een proefdruk wordt geactiveerd.
   * **[!UICONTROL Activate proof on submission]**: Configureren [!DNL Workfront Proof] om proefdrukken automatisch te activeren bij verzending (zodat deze niet handmatig hoeven te worden geactiveerd).

   * Als een proefdruk uit de Dropzone wordt verplaatst (bijvoorbeeld naar een andere map in uw account), zijn de Dropzone-instellingen niet meer van toepassing op de proefdruk. Dit is met name van belang voor instellingen voor e-mailwaarschuwingen.

1. Breng wijzigingen aan in het dialoogvenster **[!UICONTROL Dropzone fields]** sectie om op te geven welke velden worden weergegeven in het dialoogvenster [!UICONTROL Proof details] sectie van de Dropzone-verzendpagina wanneer proefdrukken via de Dropzone worden ingediend.
1. In de **[!UICONTROL Permitted domains]** in, geeft u domeinen op die u wilt toestaan om de Dropzone te gebruiken.

   * U kunt op **[!UICONTROL Add domain]** om een domein toe te voegen. Wanneer u de domeindetails hebt toegevoegd, klikt u op **[!UICONTROL Save]**.

   * U kunt **[!UICONTROL Edit]** en **[!UICONTROL Delete]** bestaande domeinen die u eerder hebt toegevoegd.

1. Onder **[!UICONTROL People to notify]** geeft u de personen op die u samen met de eigenaar van de dropzone op de hoogte wilt brengen wanneer nieuwe proefdrukken bij de dropzone worden ingediend [Dropzone](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/dropzone.md)

   * Klikken **[!UICONTROL Add people]** voert u de gegevens van de ontvanger in en klikt u op **[!UICONTROL Save]**.

   * **[!UICONTROL Delete]** personen die u eerder hebt toegevoegd.
