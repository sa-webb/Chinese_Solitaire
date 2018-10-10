### Temporarily using as developer reference 

## TODO
# Clean dealing logic \\ One loop for 3 rows \\ Nested for remaining 4
# Verify Transfer Stack logic \\ Solitaire.java 442
# Insert Rules 
# Modify the menu \\ review instructions 
# Adjust the scores or rules 

## Random
# Add label or image to the face of cards 
# Add label or image to the back of the cards. 
# Possibly adjust the title location to more centered



## References 
https://github.com/jakewilson/solitaire/

# Line 107
https://github.com/jakewilson/solitaire/blob/master/src/Card.java


## Rules Reference 
https://politaire.com/help/chinese

There are 3 decks: 
Final 
Play - 
Deck - starts with original 52

## Original Dealing Logic 
for (int x = 0; x < NUM_PLAY_DECKS; x++)
		{
			
			Card c = deck.pop().setFaceup();
			playCardStack[x].putFirst(c);

			for (int y = x + 1; y < NUM_PLAY_DECKS; y++)
			{
				playCardStack[y].putFirst(c = deck.pop());
			}
		} 

