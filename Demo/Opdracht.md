# Opdrachten voor Demo

Voor deze demonstratie zijn enkele opdrachten voorbereid. Alle benodigde files voor deze opdrachten zijn in deze repository te vinden. Download allereerst de bestanden die in de map 'download' staan van de Demo. Zet deze bestanden in dezelfde map. Open vervolgens '1cHO inschrijvingen instelling demo.pbix'. Dit bestand is een kopie van het '1cHO inschrijvingen instelling.pbix' bestand met een extra 'Opdracht pagina'. Tijdens deze demonstratie wordt er met name op deze 'Opdracht pagina' gewerkt.

## Opdracht 1: Parameters aanpassen

In de instellingrapportage zijn enkele parameters ingesteld. Deze parameters zorgen voor specifieke instellingen in de visualisaties, maar ook voor bewerkingen in de powerQuery achter het dashboard. De belangrijkste zijn de filepath en de naam instellingsbestand parameters. Hiermee zorg je ervoor dat de powerquery de bestanden gaat ophalen met de juiste naam en vanaf de juiste locatie.

![Pic 1 parameters](https://github.com/user-attachments/assets/7e41ba39-cdae-4b5f-b1ec-ea22c26e7ace)


Pas de filepath parameter aan naar het filepath waar je jouw bestanden hebt staan. De naam parameter hoeft voor deze demo niet aangepast te worden.

![Pic 2 filepath](https://github.com/user-attachments/assets/9356df9f-b877-4b11-82dd-c0d9441cb341)


Daarnaast hebben we ook de 3 nationaliteitsparameters. Deze zorgen ervoor dat je in de visualisaties een overzicht krijgt van de gekozen nationaliteiten in de volgorde zoals ze zijn opgegeven in de parameter. Er worden in de visualisaties ook nog EER en non-EER getoond, de gekozen nationaliteiten in de parameters worden in deze twee groepen niet meegenomen.

Pas de nationaliteiten aan naar nationaliteiten waar jullie interesse in hebben (zie bestand dec_nationaliteitscode voor de codes die gebruikt worden voor de nationaliteiten) en klik op refresh.

![Pic 3  nationaliteiten](https://github.com/user-attachments/assets/ee33ef2f-d664-4bc5-9fe5-39d21f5bb141)

## Opdracht 2: 'Help' overlay maken

![Callouts complete](https://github.com/user-attachments/assets/62b94b6b-188e-4b0d-8857-ab573f18ce53)

Zoals net getoond kan een 'help' overlay de gebruikers helpen met het gebruik van het dashboard. Als je deze overlay voor eigen dashboards wilt maken is het belangrijk om ervoor te zorgen dat je dashboard af is voordat je aan de overlay begint. Dit zodat er geen items meer van plaats veranderen nadat je er in je overlay naar verwijst op een specifieke locatie.

Voor deze opdracht wordt gebruik gemaakt van microsoft PowerPoint. Andere afbeelding editors kunnen gebruikt worden, maar aangezien Power BI ook binnen het microsoft pakket valt is het handig om binnen de microsoft producten te blijven.

Ten eerste, zorg ervoor dat je afbeelding editor dezelfde dimensies heeft als het dashboard (standard Power BI is (16:9). Zorg er ook voor dat je de beste resolutie mogelijk krijgt. Met de standaard instellingen van PowerPoint krijg je de volgende breedte en hoogte:

![Standard powerpoint slide size](https://github.com/user-attachments/assets/42b9a1c3-2bf5-4aa7-99c3-cb5c419bf12f)

Pas de breedte en hoogte in PowerPoint aan naar het volgende:

![Adjusted powerpoint slide size](https://github.com/user-attachments/assets/a985c64c-5076-4353-acc9-e38cb40470dc)

Ga naar 'Design' in de 'ribbon' en klik op 'Slide Size' en ten slotte op 'Custom Slide Size':

![Ribbon slide size](https://github.com/user-attachments/assets/06f6d88f-d4c2-4cb8-ba95-d25cd4caefe7)

Neem nu een screenshot van de 'Opdracht pagina' en upload deze in PowerPoint. Zorg ervoor dat het screenshot de hele slide bedekt: 

![Screenshot dashboard](https://github.com/user-attachments/assets/b5d04117-0d7a-419e-ac87-8b86a42e61a6)

Voeg een rechthoek vorm in en zorg dat deze de hele slide bedekt:

![Rectangle](https://github.com/user-attachments/assets/c516df2d-f850-41ef-a4ec-093ce9594279)

Geef deze rechthoek de kleur van je dashboard (#F4D74B in dit geval) en make de rechthoek doorzichtig (80% transparency):

![Buttons fill aanpassen](https://github.com/user-attachments/assets/748acf51-c21c-44ea-8eb6-57fe1d2d0126)

![Transparancy](https://github.com/user-attachments/assets/f02d0f9b-bdbe-4fa4-9b5f-486f1b28dce6)

Voeg nu comments toe die je wilt dat de gebruiker ziet. In het voorbeeld gebruiken we 'callouts', maar je kunt zelf bedenken wat je graag zou willen meegeven aan de gebruikers:

![Callouts](https://github.com/user-attachments/assets/b9a675f5-bac8-435f-9ef7-002ab3c46df6)

Na de comments ziet de overlay er ongeveer zo uit:

![Callouts complete](https://github.com/user-attachments/assets/c19a3f49-e2a9-4a5b-9218-f314bc33eb66)

Ten slotte is het belangrijk om de 'transparency' te behouden. In PowerPoint kun je daarom niet de normale 'save' functie gebruiken. Kies een van de objecten die je hebt toegevoegd en ga naar 'Shape Format' in de 'ribbon' en klik op 'Selection Pane':

![Selection Pane](https://github.com/user-attachments/assets/d984fa0e-1efd-4be7-a025-2633acbd2e93)

In dit selectie menu kies je alle objecten behalve het screenshot van je dashboard. Je kunt ook het screenshot verwijderen, maar ook in dat geval moeten de andere objecten alsnog geselecteerd worden:

![Select all](https://github.com/user-attachments/assets/efddb0c1-237c-4d4b-ad84-bfeb1687c61d)

Nu rechtermuisklik en 'save as' en kies .png als filetype van je afbeelding.

Nu kan de overlay gebruikt worden in Power BI. Deze overlay wordt in Power BI gebruikt door middel van bookmarks. Als je nog niet bekend bent met bookmarks is hier een handige informatie pagina: https://learn.microsoft.com/en-us/power-bi/create-reports/desktop-bookmarks?tabs=powerbi-desktop. Voor de opdracht zijn de stappen hieronder verder uitgelegd.

Op de 'Opdracht pagina' ga je naar 'Insert' en klik op 'Image', selecteer nu je zojuist gemaakte overlay:

![Insert image overlay](https://github.com/user-attachments/assets/93b861bf-833f-4b16-8ba6-51ed5c80324e)

Zorg ervoor dat de overlay je dashboard bedekt:

![Edges overlay powerBI](https://github.com/user-attachments/assets/a619d364-cf38-4fdd-a890-70675bd6f968)

Om een bookmark toe te voegen ga je naar 'View' in de 'ribbon' en klik op 'Bookmarks':

![Bookmark selection](https://github.com/user-attachments/assets/ec9c2fbc-7767-4885-be8b-59b42a156f4a)

Selecteer nu je overlay (en alleen je overlay) en klik op 'Add' in hte bookmark menu:

![add bookmark](https://github.com/user-attachments/assets/c282479b-d27b-46a6-9824-ccf81322a4f9)

Selecteer je gemaakte bookmark in het bookmark menu en deselecteer 'Data' en selecteer 'Selected visuals':

![Selection bookmark visuals](https://github.com/user-attachments/assets/b2fa723f-fa1a-4262-9894-606753768b27)

De zojuist gemaakte bookmark zorgt ervoor dat de overlay zichtbaar wordt voor de gebruikers. Er moet nu ook nog een bookmark gemaakt worden die ervoor zorgt dat de overlay onzichtbaar wordt voor de gebruikers.

Selecteer in de 'View' ribbon ook 'Selection'. Dit toont de verschillende elementen in je dashboard. De elementen krijgen standaard namen van power BI (de overlay heet bijvoorbeeld 'picture'). Echter, voor werkbaarheid is het een goed idee om deze elementen te noemen naar wat ze vertegenwoordigen:

![Selection powerBI](https://github.com/user-attachments/assets/683f1b98-bc9c-477f-88d7-f99be678b601)

Selecteer nu je overlay element en klik op het kleine oog icoontje ernaast in het 'Selection' menu. Hierna wordt je element onzichtbaar en ook meteen gedeselecteerd. Selecteer het overlay element nogmaals in het 'Selection' menu:

![Make invisible](https://github.com/user-attachments/assets/2eb22084-8f70-44f4-ab1b-00b0cc62e833)

Voeg wederom een bookmark toe door op 'Add' te klikken in het bookmark menu:

![Bookmark add again](https://github.com/user-attachments/assets/f2f699f5-ca53-4197-a621-9adfe29a9cfb)

Selecteer je tweede gemaakte bookmark in het bookmark menu en deselecteer 'Data' en selecteer 'Selected visuals' zoals een paar stappen eerder:

![Selection bookmark visuals](https://github.com/user-attachments/assets/335c7312-41aa-4f82-bf15-148bef2543de)

Nu zijn de twee staten van je overlay gemaakt, zichtbaar en onzichtbaar. Nu moet er nog voor gezorgd worden dat men toegang heeft to beide staten. In de opdracht is er al een button gemaakt (Help button) waaraan een actie toegevoegd kan worden om de overlay zichtbaar te maken.

Klik op het 'Help button' element, ga naar actie, klik op type 'Bookmark' en selecteer je eerst gemaakte bookmark:

![Button selection](https://github.com/user-attachments/assets/99aa0c4f-f8c2-4b3e-b42f-ae442d494149)

Houd Ctrl ingedrukt en linksklik op de button. Nu zou de transparante overlay als pop-up moeten verschijnen. Vervolgens wil je ervoor zorgen dat de gebruiker waar dan ook kan klikken om de overlay weer onzichtbaar te maken. Gelukkig is de overlay zelf klikbaar en bedekt deze de hele pagina. Selecteer nu de overlay, ga naar 'Action' in het Format image pane en clik op type 'Bookmark' en selecteer je tweede gemaakte bookmark (de bookmark waardoor je overlay onzichtbaar wordt):

![invisible maken](https://github.com/user-attachments/assets/045ef1c2-5391-4f47-9bd5-17328f97bfd5)

Houd wederom Ctrl ingedrukt en linkermuisklik op de overlay en nu ga je terug naar de default weergave van je dashboard.

Zorg er altijd voor de je 'help' overlay het bovenste element is in je dashboard. Dit kun je doen door in de selection pane de overlay altijd als bovenste element in het rijtje te hebben. De volgorde in de selection pane bepaald welke elementen voor andere staan.

## Opdracht 3a: 'How-to' video als tooltip gebruiken

Om het de gebruikers nog makkelijker te maken kun je ook gebruik maken van een 'how to' video. Deze wil je vervolgens dan als een hover over pop-up laten zien. Om dit voor elkaar te krijgen kun je gebruik maken van tooltips. In het dashboard lijkt het alsof een button een tooltip heeft, echter power BI heeft deze functie nog niet. In werkelijkheid is er een andere visual gemaakt waar tooltips wel mogelijk zijn en deze over de 'vraagteken' button heen gezet:

![Pic 4 How to](https://github.com/user-attachments/assets/5f24ab97-770d-4b10-91bf-c8350a2d80b5)

Om dit voor elkaar te krijgen is er eerst een dummy measure gemaakt zonder echte data. Ga naar de 'Home' ribbon en selecteer 'New measure':

![Pic 5 Measure](https://github.com/user-attachments/assets/5ae143cd-65bc-4bfb-ad0a-b6441c89e443)

Geef deze measure een waarde van 'blank':

![Pic 6 Dummy measure](https://github.com/user-attachments/assets/e3edf27d-83e1-46c9-b930-9e7948aa137e)

Voeg nu een 'Card' visual toe in het rapport en zet deze over de 'vraagteken' button heen in het rapport:

![Pic 7 Card visual](https://github.com/user-attachments/assets/e9ef1cd7-da92-417e-97b4-11f4691514b4)

De 'Card' visual heeft nog een waarde nodig voordat deze actief is, geef de visual de waarde 'Dummy Measure':

![Pic 8 card visual vullen](https://github.com/user-attachments/assets/690c9a7b-1731-424c-b0e7-1cd1798abf5c)

Vervolgens moet er niks van de 'Card' zichtbaar zijn. Ga daarom in het 'Visualisations' menu naar de Callout value en Category label en stel ze als volgt in:

![Pic 9 waardes card](https://github.com/user-attachments/assets/774d9c0f-c5bc-469c-bbbf-43af8b7abab9)

Tenslotte moet er nog een tooltip aan toegevoegd worden. In de opdracht is al een tooltip pagina gemaakt met een video. Voor nu wordt er gebruik gemaakt van deze pagina, echter verderop in de opdracht wordt uitgelegd hoe deze video gemaakt is en de custom tooltip pagina.

Ga in het 'Visualisations' menu naar 'General' en deselecteer 'Header icons' en selecteer 'Tooltips' Kies bij tooltips voor type 'Report page' en page 'TT gif' (de al gemaakte tooltip pagina met video):

![Pic 10 tooltip kiezen](https://github.com/user-attachments/assets/68b37a00-e889-41d4-b12a-e8713b06cc05)

Als er nu over de 'vraagteken' button heen gehovered wordt krijg je het filmpje te zien!

## Opdracht 3b: 'How-to' video maken

Om een 'how-to' video te maken is er gebruik gemaakt van het programma ScreenToGif (https://www.screentogif.com/). Echter, ieder screenrecording programma kan gebruikt worden hiervoor.

## Opdracht 4: Maak zelf een 'animated' button

De laatste opdracht is om zelf een geanimeerde button te maken. Ook een handigheidje dat gebruikt kan worden om wat extra’s toe te voegen aan de rapportages. Let op! Hierdoor kan het rapport al snel overweldigend uitzien, maar wanneer met mate gebruikt kun je hier extra aandacht leggen op bepaalde aspecten van je rapport of bijvoorbeeld duidelijk maken dat de button interactief is.

![image](https://github.com/user-attachments/assets/ae384757-c948-4e85-8014-83c4297c084b)

In de opdracht wordt de bewegende pijl gemaakt:

![Pic 11 pijlk](https://github.com/user-attachments/assets/a7148dab-a108-4cef-8bd3-2f437cc4ce9c)

Om deze te maken is wederom gebruik gemaakt van PowerPoint.

Zorg ervoor dat de slide volledig leeg is en voeg daarna een 'kromme pijl' toe. Ga naar de 'Insert' ribbon en klik op 'Icons', zoek vervolgens naar 'arrow' en selecteer de 'kromme pijl':

![Pic 12 icons kiezen](https://github.com/user-attachments/assets/d785d254-1475-4098-9143-192d7bdacc83)

Pas de grootte en de orientatie van de pijl aan:

![pic 13 orientatie pijl](https://github.com/user-attachments/assets/1545a024-2016-4575-9801-832500cbcfb5)

Geef de achterkant van de slide dezelfde kleur als het dashboard. Ga naar de 'Design' ribbon, kies vervolgens 'Format Background' en selecteer de juiste kleur (#F4D74B):

![pic 14 kleur achtergrond](https://github.com/user-attachments/assets/d3bf5c42-8a27-4e7c-9fec-277f078eaa59)

Vervolgens wordt de animatie toegevoegd aan de pijl. Dit kan door de pijl te selecteren dan naar de 'Animations' ribbon te gaan en, kies 'Custom Path' en vervolgens op 'Add Animation' te klikken:

![Pic 15 add animation](https://github.com/user-attachments/assets/d84a9f16-5042-4c00-9996-cc4711d4a021)


