*****************************README******************************

Variables:
Rows:No of rows
Columns:No of Columns
total:total no of tiles=rows*columns
No_of_mines:No_of_mines
mines[no_of_mines]:Location of mines
arr[rows+2][columns+2]:1 if location has a mine else 0
	2 extra rows and 2 extra columns have been added to remove 	particular processing for corner elements
count_open:No of open mines
flagged_as_mines: No of tiles flagged as mines by users
flagged_correct:No of mines flagged correct by users
cheats:No of cheats used


When a user leftclicks,the program first checks if the tile is a
mine. If it is,the program calls the game_over() function which displays all the mines and removes the click attributes of all buttons.
If the clicked tile is not a mine,it displays the no on the tile & checks if it is a 0.If it is a 0,it changes the colour to orange and checks it neighbours for all 0's

When a user right clicks,it changes colour to black,and increases number of flagged_as_mines by 1. If a correct mine is flagged,flagged_correct increases by 1.

When a user left clicks ,its background simply toggles between yellow and no colour.

On pressing validate,flagged_as_mines is compared with flagged_correct and respons is generated.

On pressing cheat,a mine is displayed which has not been flagged or displayed as a cheat before.All its neighbours whih are not mines are also displayed

On pressing resize,a new board is created

On pressing reset,a new random board with same dimensions is created


****************************************************************