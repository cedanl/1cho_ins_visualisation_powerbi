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

## Opdracht 2: 'How-to' overlay maken

![Callouts complete](https://github.com/user-attachments/assets/62b94b6b-188e-4b0d-8857-ab573f18ce53)

In order to make sure your organisation knows how to use your dashboards an information overlay might be a good idea. For the user this is a very easily accessible tool to use, without the need to read entire manuals or watch several videos with explanation.

Make sure that your dashboard is finalised before you start working on the overlay. Because otherwise you will have to change the overlay every time something changes position in your dashboard. This particular overlay is created in Microsoft PowerPoint, but any image editor will do. The rest of the How To will discuss the steps taken with PowerPoint.

First, make sure that your image editor has the same dimensions as dashboard (standard Power BI is 16:9). You should also make sure that you are getting the best resolution possible. Standard PowerPoint settings give the slide the following width and height:

![Standard powerpoint slide size](https://github.com/user-attachments/assets/42b9a1c3-2bf5-4aa7-99c3-cb5c419bf12f)

However, you should adjust this to the following width and height (if you are working with the standard 16:9 dimension in Power BI):

![Adjusted powerpoint slide size](https://github.com/user-attachments/assets/a985c64c-5076-4353-acc9-e38cb40470dc)

Go to ‘Design’ in the ribbon, then click on ‘Slide Size’, and finally on ‘Custom Slide Size’ in order to change this:

![Ribbon slide size](https://github.com/user-attachments/assets/06f6d88f-d4c2-4cb8-ba95-d25cd4caefe7)

Now take a screenshot of the report page for which you are designing the overlay and upload it in PowerPoint and ensure the screenshot covers the entire slide:

![Screenshot dashboard](https://github.com/user-attachments/assets/b5d04117-0d7a-419e-ac87-8b86a42e61a6)

Now insert a rectangle shape and make sure it covers the entire slide:

![Rectangle](https://github.com/user-attachments/assets/c516df2d-f850-41ef-a4ec-093ce9594279)

Give the rectangle the colour of your choice (I gave it the main theme colour) and make the shape transparent (I use 80% transparency):

![Buttons fill aanpassen](https://github.com/user-attachments/assets/748acf51-c21c-44ea-8eb6-57fe1d2d0126)

![Transparancy](https://github.com/user-attachments/assets/f02d0f9b-bdbe-4fa4-9b5f-486f1b28dce6)

Now you can add some comments that you want your user to see. In my example we are using callouts, but you can do whatever you see fit to give as input to your users:

![Callouts](https://github.com/user-attachments/assets/b9a675f5-bac8-435f-9ef7-002ab3c46df6)

After adding some comments your overlay might look something like this:

![Callouts complete](https://github.com/user-attachments/assets/c19a3f49-e2a9-4a5b-9218-f314bc33eb66)

Now for the final part you will need to make sure that the transparency remains intact. Therefore, you cannot use the normal save function that PowerPoint provides. Instead, select any of your shapes and go to ‘Shape Format’ in the ribbon and then click on ‘Selection Pane’:

![Selection Pane](https://github.com/user-attachments/assets/d984fa0e-1efd-4be7-a025-2633acbd2e93)

Now in the selection ensure to select all objects except the screenshot of your dashboard (or delete the screenshot of your dashboard, but still select all other objects!):

![Select all](https://github.com/user-attachments/assets/efddb0c1-237c-4d4b-ad84-bfeb1687c61d)

Now right click, ‘save as’ and choose .png as type of picture.

Now you have an overlay that can be used in Power BI! The way this overlay is used in Power BI is by the means of bookmarks. I would recommend giving this page a view in order to get help with using bookmarks: https://learn.microsoft.com/en-us/power-bi/create-reports/desktop-bookmarks?tabs=powerbi-desktop. However, here is also a quick overview of using this particular type of bookmark as an overlay.

In your Power BI dashboard go to ‘Insert’ and click on ‘Image’, now select your created overlay:

![Insert image overlay](https://github.com/user-attachments/assets/93b861bf-833f-4b16-8ba6-51ed5c80324e)

Now make sure the overlay covers the edges:

![Edges overlay powerBI](https://github.com/user-attachments/assets/a619d364-cf38-4fdd-a890-70675bd6f968)

Now for the creation of bookmarks, go to ‘View’ in the ribbon and then click on ‘Bookmarks’:

![Bookmark selection](https://github.com/user-attachments/assets/ec9c2fbc-7767-4885-be8b-59b42a156f4a)

Now select your overlay (only your overlay) and click on ‘Add’ in the bookmark menu:

![add bookmark](https://github.com/user-attachments/assets/c282479b-d27b-46a6-9824-ccf81322a4f9)

Select your created bookmark in the bookmark menu and deselect ‘Data’ and select ‘Selected visuals’:

![Selection bookmark visuals](https://github.com/user-attachments/assets/b2fa723f-fa1a-4262-9894-606753768b27)

This will be the bookmark that will make your overlay visible to the users. However, we do not want the overlay to be visible constantly. Therefore, we will need a bookmark that makes sure your overlay is invisible for your users, a default state.

In the ‘View’ ribbon also select ‘Selection’. This will show you all of the different elements in your dashboard. The elements will get standard names from Power BI (the overlay will be named picture), I would suggest renaming the elements so you know what you are selecting:

![Selection powerBI](https://github.com/user-attachments/assets/683f1b98-bc9c-477f-88d7-f99be678b601)

Now select your overlay element and click on the little eye icon next to it in the ‘Selection’ menu, after that the element will become invisible but also immediately unselected, reselect the overlay element in the ‘Selection’ menu:

![Make invisible](https://github.com/user-attachments/assets/2eb22084-8f70-44f4-ab1b-00b0cc62e833)

Now add another bookmark by again pressing ‘Add’ in the ‘Bookmark’ menu:

![Bookmark add again](https://github.com/user-attachments/assets/f2f699f5-ca53-4197-a621-9adfe29a9cfb)

Select your second created bookmark in the bookmark menu and deselect ‘Data’ and select ‘Selected visuals’ just as before:

![Selection bookmark visuals](https://github.com/user-attachments/assets/335c7312-41aa-4f82-bf15-148bef2543de)

Now you have created the two states of your overlay, visible and invisible. Now you want to make sure that people can access both states. You will need a button or another element like a picture which you can click to access the bookmarks.

After you have created whatever you want to use to access the bookmark click on that element, go to ‘Action’ in the Format pane and click on Type ‘Bookmark’ and select your first created bookmark:

![Button selection](https://github.com/user-attachments/assets/99aa0c4f-f8c2-4b3e-b42f-ae442d494149)

Hold Ctrl and left-click on your button and you should then get the transparent overlay to pop-up. Now you want to make sure that if your user clicks anywhere the overlay becomes invisible again. Luckily the overlay itself is clickable and covers the entire screen. So select the overlay, go to ‘Action’ in the Format image pane and click on Type ‘Bookmark’ and select your second bookmark (the one that makes the overlay invisible):

![invisible maken](https://github.com/user-attachments/assets/045ef1c2-5391-4f47-9bd5-17328f97bfd5)

Now hold Ctrl and left-click on the overlay and you should go back to your default dashboard view.

One thing to note is that your overlay should always be the top element in your dashboard. Just make sure that the overlay is always the top-item in the selection pane, the ordering here shows which elements are in front of others, with the top one being the element most in front.

## Opdracht 3: 'How-to' video maken en als tooltip gebruiken

## Opdracht 4: Maak zelf een 'animated' button

