---
title: Veelgestelde vragen over SOAP API
description: Veelgestelde vragen over SOAP API
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
role: Developer
exl-id: fcf89bd6-0e07-42a7-9ae3-9a1309e51946
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '805'
ht-degree: 0%

---

# Veelgestelde vragen over SOAP API

## Hoe maak ik mijn eerste bestandsproefdruk?

Het neemt drie eenvoudige stappen:

**Stap 1**: Upload het dossier aan Workfront Proof door het via een verzoek van Post te verzenden aan  [ https://soap.proofhq.com/upload.php ](https://soap.proofhq.com/upload.php). Wij zullen u de dossier knoeiboel terugkeren - dit is zeer belangrijk! Op dit moment ziet u niets in uw account. U hebt ons het bestand alleen maar gestuurd, maar u hebt ons niet verteld wat u ermee moet doen.

**Stap 2**: Als u nog geen identiteitskaart van de Zitting hebt, verkrijg door doLogin () te gebruiken of getSessionID () methodes. Gebruik de eerste methode om u aan te melden met gebruik van het e-mailadres en wachtwoord van de gebruiker of de tweede methode als u het e-mailadres en de verificatietoken van de gebruiker hebt.

**Stap 3:** nu is het tijd om uw bewijs tot stand te brengen. Gebruik de methode createProof() en verzend ons ten minste de vereiste velden (er zijn momenteel slechts 5). Zorg ervoor dat u de parameter Hash instelt op de bestandshash die tijdens &quot;Stap 1&quot; wordt geretourneerd, zodat u kunt bepalen welk bestand moet worden gebruikt wanneer u een proefdruk maakt.

Als u zich nu aanmeldt bij uw account, wordt de proefdruk weergegeven.

## Hoe maak ik mijn eerste proefdruk van webmomentopnamen?

Het neemt twee eenvoudige stappen:

**Stap 1**: Als u nog geen identiteitskaart van de Zitting hebt, verkrijg door doLogin () te gebruiken of getSessionID () methodes. Gebruik de eerste methode om u aan te melden met gebruik van het e-mailadres en wachtwoord van de gebruiker of de tweede methode als u het e-mailadres en de verificatietoken van de gebruiker hebt.

**Stap 2:**Nu is het tijd om uw bewijs tot stand te brengen. Gebruik de methode createProof() en verzend ons ten minste de vereiste velden (er zijn momenteel slechts 5). Zorg ervoor dat u de Hash-parameter instelt op &#39;web&#39; en de SourceName-parameter als de URL van de webpagina die u wilt vastleggen.

Als u zich nu aanmeldt bij uw account, wordt de proefdruk weergegeven.

## Wat is het verschil tussen een bewijs en een versie?

In Workfront Proof-versies worden weergegeven als één proefdruk. Als u op een specifieke versie in de webinterface klikt, worden de details van die versie weergegeven. In werkelijkheid, is elke versie een afzonderlijk bewijs en het Web UI toont deze samen.

Vanuit het perspectief van de API is elke versie een afzonderlijke proefdruk en zijn de proefdrukken gekoppeld door hun id&#39;s.

**createProof ()** zal altijd **versie 1** van de proef creëren. Laten we bijvoorbeeld aannemen dat de id die voor dit bewijs &quot;100&quot; is geretourneerd, is.

Wanneer het gebruiken van **createProofVersion ()** verzendt altijd in identiteitskaart van de vorige versie. Als wij **versie 2** op proef &quot;100&quot;willen creëren, gaan wij **in &quot;100&quot;voor de parameter ParentFileID** over. Dit vertelt het systeem dat deze proef versie 2 van de reeks zou moeten zijn. De methode retourneert een unieke bewijs-id, bijvoorbeeld &#39;101&#39;.

Als een derde versie i.e. **versie 3** wordt vereist, zult u **createProofVersion ()** opnieuw roepen en dit keer **gaat in &quot;101&quot;voor ParentFileID** over die de verbonden lijst van versies zal verzekeren behoorlijk wordt gecreeerd.

## Moet ik een nieuwe identiteitskaart van de Zitting vóór elke vraag verkrijgen?

Het is belangrijk om erop te wijzen dat elke identiteitskaart van de Zitting hoofdzakelijk een gebruiker is die de acties uitvoert. 

U te hoeven om geen nieuwe identiteitskaart van de Zitting vóór elke vraag aan API te verkrijgen en het zal 24 uren geldig blijven. De vervaltijd stelt telkens opnieuw in wanneer u een vraag aan API maakt.

## Wat is een bewijs/persoonlijke URL?

**Team/Openbaar**: Elke proefversie heeft een uniek Team (Openbaar) URL. Als deze optie is ingeschakeld, wordt de proefdruk geopend in de modus Alleen-lezen. U kunt het Team URL verkrijgen gebruikend [ getProofURL () ](https://api.proofhq.com/home/proofs/getproofurl.html) methode.

**Persoonlijk**: Persoonlijke URL is uniek voor elke recensent en proefdrukversie. Als een proefset drie versies bevat en een revisor in alle versies aanwezig is, heeft de controleur drie unieke persoonlijke URL&#39;s. Een persoonlijke URL opent de proefversie met de reeds geïdentificeerde controleur en moet daarom veilig worden gehouden en niet worden gedeeld. Persoonlijke URLs kan worden verkregen door [ te roepen getProofReviewers () ](https://api.proofhq.com/home/proofs/getproofreviewers.html) methode en dan herhalend over elk  [ SOAPRecepientObject ](https://api.proofhq.com/home/objects/soaprecipientobject.html) en het krijgen van de parameter &quot;proof_url&quot;.

## >Hoe kan ik aangepaste parameters opnemen bij het openen van het minibewijs?

Met de miniproefdruk kunt u het proefdrukgereedschap in uw eigen pagina insluiten. Een &quot;verwijzer&quot;parameter kan als deel van miniproef worden omvat om een omleiding URL te verstrekken wanneer een gebruiker op de dichte knoop in de miniproef klikt. U kunt een willekeurig aantal aangepaste parameters opnemen als onderdeel van deze omleidings-URL door deze toe te voegen met het escape-teken &#39;&amp;&#39;, bijvoorbeeld %26.

Bijvoorbeeld de miniproef-URL
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com&customparam1=somevalue&customparam2=` moet worden gecodeerd als 
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com%26customparam1=somevalue%26customparam2=` om de aangepaste parameters door te geven.

## Hoe te om een Cliënt van de Dienst van het Web van Java tot stand te brengen?

[ Deze video ](https://screencast.com/t/xsSNrqs5b) toont hoe u een cliënt van de Dienst van het Web van Java kunt tot stand brengen gebruikend Eclipse en de definitie van Workfront Proof WSDL.

