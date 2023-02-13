---
product-area: documents;system-administration;setup
navigation-topic: manage-proofs-within-workfront
title: Toegang- en abonnementsinstellingen configureren voor een proefdruk
description: U kunt bepaalde toegangs en abonnementsmontages voor individuele proefdrukken vormen, zoals of om gebruikers te vereisen login en of om gebruikers toe te staan om op de proef in te tekenen. U kunt toegang- en abonnementsinstellingen instellen voor een proefdruk terwijl u deze maakt, of u kunt deze instellingen instellen voor een proefdruk die al in Workfront bestaat.
author: Courtney
feature: Digital Content and Documents
exl-id: f242887b-d768-4d56-b530-a1ac6294b2d4
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '949'
ht-degree: 0%

---

# Toegang- en abonnementsinstellingen configureren voor een proefdruk

U kunt bepaalde toegangs en abonnementsmontages voor individuele proefdrukken vormen, zoals of om gebruikers te vereisen login en of om gebruikers toe te staan om op de proef in te tekenen. U kunt toegang- en abonnementsinstellingen instellen voor een proefdruk terwijl u deze maakt, of u kunt deze instellingen instellen voor een proefdruk die al in Workfront bestaat.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Huidig plan: Pro of hoger</p> <p>of</p> <p>Ouder plan: Premium</p> <p>Voor meer informatie over het proefdrukken van toegang met de verschillende plannen, zie <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Toegang tot proefdrukfunctionaliteit in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Huidig plan: Werken of plannen</p> <p>Ouder plan: Willekeurig (proefdrukken moet zijn ingeschakeld voor de gebruiker)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bewijs van machtigingsprofiel </td> 
   <td>Manager of hoger</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot documenten bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met de beheerder van de Workfront of Workfront-proefdrukken als u wilt weten welk plan, welke rol of welk proefdrukprofiel u hebt.

## Toegang- en abonnementsinstellingen configureren tijdens het maken van een proefdruk

Als u toegang- en abonnementsinstellingen wilt instellen voor een proefdruk terwijl u deze maakt:

1. Ga naar het project, de taak, of de kwestie waar u het proef wilt, dan klik **Documenten** sectie.
1. Klikken **Nieuwe toevoegen** in de rechterbovenhoek.
1. Naar de **Proefinstellingen** in de rechterbenedenhoek van het dialoogvenster **Nieuwe proefdruk** pagina.

1. Configureer de volgende instellingen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Delen van proefdrukken via openbare URL of insluitcode toestaan</strong> </td> 
      <td>Als deze optie is geselecteerd, kan de proefdruk worden gedeeld via een openbare URL of insluitcode.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Abonneren op proefdrukken via openbare URL of insluitcode toestaan</strong> </td> 
      <td>Als deze optie is geselecteerd, kunnen personen die niet expliciet aan de proefdruk zijn toegevoegd, zich op de proefdruk abonneren. De persoon die zich op de proef abonneert, krijgt de rol en e-mail die u in de volgende montages bepaalt:
       <ul>
        <li><p><strong>Abonnementenrol:</strong> De standaardproefdrukrol die wordt toegewezen aan alle revisoren die zich op de proefdruk abonneren. </p><p>Belangrijk: Indien <strong>Delen toestaan met</strong> is ingesteld op een andere waarde dan <strong>Iedereen</strong> in de instellingen voor Workfront-proefdrukken werkt het abonnement alleen voor personen binnen de organisatie. Zie voor meer informatie <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Proefinstellingen configureren in Workfront Proof</a>.</p></li>
        <li><strong>Instellingen voor e-mailwaarschuwingen voor abonnees:</strong> De standaard e-mailwaarschuwing die wordt toegewezen aan alle revisoren die zich op de proefdruk abonneren.</li>
       </ul><p>
        <ul>
         <li><strong>Bewijs van toegang via e-mailkoppeling vereist voor:</strong> Configureer of de abonnee een e-mail ontvangt met een koppeling naar de proefdruk. U kunt <strong>Geen e-mail</strong> (E-mailkoppeling is niet vereist voor toegang tot de proefdruk), <strong>Alleen e-mail met verificatie-kennisgeving</strong> (de abonnee ontvangt een koppeling naar de proefdruk via e-mail zonder verificatie), of <strong>E-mails over validatie en proefdrukken</strong> (de abonnee ontvangt een koppeling naar de proefdruk via e-mail en moet op de koppeling klikken om toegang te krijgen tot een proefdruk. Deze optie heeft tot doel ervoor te zorgen dat de persoon een correct e-mailadres heeft ingevoerd waartoe hij toegang heeft).</li>
        </ul><p>Opmerking:  Als de proefdrukken de Geautomatiseerde Werkstroom in bijlage hebben alle abonnementen zullen bevestigingse-mail aan de bewijseigenaars produceren, zodat kunnen zij beslissen welk stadium de persoon aan zou moeten worden toegevoegd.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Blijf uw proefdruk maken.

## Toegang- en abonnementsinstellingen configureren voor een bestaande proefdruk

U kunt als volgt toegangs- en abonnementsinstellingen instellen voor een proefdruk die al in Workfront bestaat:

1. Selecteer in het gebied Documenten het document met de proefdruk waarvoor u instellingen wilt configureren en klik vervolgens op **Documentdetails**.
1. Klik in het linkerdeelvenster op **Instellingen van viewer proefdrukken**.
1. Configureer de volgende instellingen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Delen van proefdrukken via openbare URL of insluitcode toestaan</strong><strong>e</strong> </td> 
      <td>Als deze optie is geselecteerd, kan de proefdruk worden gedeeld via een openbare URL of insluitcode.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Abonneren op proefdrukken via openbare URL of insluitcode toestaan</strong> </td> 
      <td>Als deze optie is geselecteerd, kunnen personen die niet expliciet aan de proefdruk zijn toegevoegd, zich op de proefdruk abonneren. De persoon die zich op de proef abonneert, krijgt de rol en e-mail die u in de volgende montages bepaalt:
       <ul>
        <li><p><strong>Abonnementenrol:</strong> De standaardproefdrukrol die wordt toegewezen aan alle revisoren die zich op de proefdruk abonneren. </p><p>Belangrijk: Indien <strong>Delen toestaan met</strong> is ingesteld op een andere waarde dan <strong>Iedereen</strong> in de instellingen voor Workfront-proefdrukken werkt het abonnement alleen voor personen binnen de organisatie. Zie voor meer informatie <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Proefinstellingen configureren in Workfront Proof</a>.</p></li>
        <li><strong>Instellingen voor e-mailwaarschuwingen voor abonnees:</strong> De standaard e-mailwaarschuwing die wordt toegewezen aan alle revisoren die zich op de proefdruk abonneren.</li>
       </ul><p>
        <ul>
         <li><strong>Bewijs van toegang via e-mailkoppeling vereist voor:</strong> Configureer of de abonnee een e-mail ontvangt met een koppeling naar de proefdruk. U kunt <strong>Geen e-mail</strong> (E-mailkoppeling is niet vereist voor toegang tot de proefdruk), <strong>Alleen e-mail met verificatie-kennisgeving</strong> (de abonnee ontvangt een koppeling naar de proefdruk via e-mail zonder verificatie), of <strong>E-mails over validatie en proefdrukken</strong> (de abonnee ontvangt een koppeling naar de proefdruk via e-mail en moet op de koppeling klikken om toegang te krijgen tot een proefdruk. Deze optie heeft tot doel ervoor te zorgen dat de persoon een correct e-mailadres heeft ingevoerd waartoe hij toegang heeft).</li>
        </ul><p>Opmerking:  Als de proefdrukken de Geautomatiseerde Werkstroom in bijlage hebben alle abonnementen zullen bevestigingse-mail aan de bewijseigenaars produceren, zodat kunnen zij beslissen welk stadium de persoon aan zou moeten worden toegevoegd.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **Opslaan**.
