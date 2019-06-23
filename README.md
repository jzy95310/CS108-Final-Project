# CS108-Final-Project
Team Members: 
Ziyang Jiang (zij004), Haotian Sun (htsun), Xinyu Wang (xwang7), Yumeng Yue (yuey3), Sizhuo Zhang (sizhuo)

## Extensions:

###	Editor:<br/>

>A.	Error checking<br/>
>>a.	Update its name in scripts of all shapes immediately after a change to the name of a page/shape<br/>
>>b.	Prohibit the user from using Script/Cut Shape/Copy Shape/EditText/Set Property/Delete Shape functionalities (wherever a shape     object is required) when no shape is currently selected and display warning message via a toast<br/>
>>c.	Ignore the request of creating a new shape/page when a shape/page with the proposed name already exists<br/>
>>d.	Decline the request when the user is trying to delete current starting page and display warning message via a toast<br/>
>>e.	Prohibit the user from creating a game with a name that already exists and prompt the user to give a different name<br/>

>B.	Undo functionality for a series of actions all the way back to the very beginning state<br/>
>>a.	Undo support for basic changes to shapes:moving, renaming, changing the script,etc<br/>
>>b.	Undo support for adding/deleting/cutting/copying/pasting shapes<br/>
>>c.	Undo support for adding/deleting/renaming pages<br/>
>>d.	Display the exact undo operation performed via a toast<br/>

>C.	Support Cut/Copy/Paste shapes functionalities even across pages<br/>

>D.	Allow the user to use image bounds or the original proportion of the image to scale the size of a shape<br/>

>E.	Support deleting a specific game or emptying all games in the database<br/>

>F.	Autoname new games with incrementing numbers when the user does not give a name for the new game<br/>

>G.	Allow the user to set different font types (bold, italic) for a text shape<br/>

### Player: <br/>

>A.	In the game player, shapes shrink to the size of 200*200 automatically to fit into the possession area after entering it, and will recover to their original sizes immediately after going back to a page. 
>B.	Support displaying text shapes of different font types (bold, italic)
>C.	Save the current state of a game in the game player to the database and let the user to resume playing it later
>D.	Allow the user to choose a background image from preloaded images including logos of all 30 NBA teams

## Notes: <br/>

* Script clauses with the same “trigger” will be concatenated into one clause, and all the actions in those clauses will be executed instead of being ignored.<br/>
* The pasted shape will be pasted at a fixed location.<br/>
* All the input capital letters will be convert to lowercase.<br/>
* Delete current page will jump to start page immediately.<br/>
* The shape size of text will only be controlled by the font size in “Set Property”.<br/>
* The shape size of image will not be affected by the font size in “Set Property”.<br/>
* In editor, all the images will be placed in the possession area with size 100*100 and with constant space between them.<br/>
* The name of a game can only contain letters, digits and ‘_’.<br/>
* When using the feature of proportional scaling, the width and height of the shape are only determined by the new width.<br/>
* The editor does not have background because we want users to have a clean page for editing.<br/>
* When multiple shapes overlap, those modified later will be on top of shapes modified earlier and only the top one will be selected when the user click on the overlapping area.<br/>

