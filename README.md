// add your code here

bool valid = false;
for (int i = 0; i <= cards.Length - 5; i++) // loops through every card in "cards" array, stars at index 0 and ends at 95.
{
    if (cards[i + 1] == cards[i] + 1 && // checking if it goes up in +1 each time.
        cards[i + 2] == cards[i] + 2 &&
        cards[i + 3] == cards[i] + 3 &&
        cards[i + 4] == cards[i] + 4)
    {
        valid = true;
        gameWon = true; // if that condition is true it means 5 in a row have been validated so the game is won.
        break;
    }
}


// end of your code
