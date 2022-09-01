# AllCardsOnDeckCS

PEDAC TIME

Data:

52 Cards in a deck
4 suits
13 "ranks" per suit

52 Cards include:

Hearts:
"Ace of Hearts" ,
"2 of Hearts" ,
"3 of Hearts" ,
"4 of Hearts" ,
"5 of Hearts" ,
"6 of Hearts" ,
"7 of Hearts" ,
"8 or Hearts" ,
"9 of Hearts" ,
"10 of Hearts" ,
"Jack of Hearts" ,
"Queen of Hearts" ,
"King of Hearts" ,

Spades:
"Ace of Spades" ,
"2 of Spades" ,
"3 of Spades" ,
"4 of Spades" ,
"5 of Spades" ,
"6 of Spades" ,
"7 of Spades" ,
"8 or Spades" ,
"9 of Spades" ,
"10 of Spades" ,
"Jack of Spades" ,
"Queen of Spades" ,
"King of Spades" ,

Clubs:
"Ace of Clubs" ,
"2 of Clubs" ,
"3 of Clubs" ,
"4 of Clubs" ,
"5 of Clubs" ,
"6 of Clubs" ,
"7 of Clubs" ,
"8 or Clubs" ,
"9 of Clubs" ,
"10 of Clubs" ,
"Jack of Clubs" ,
"Queen of Clubs" ,
"King of Clubs" ,

Diamonds:
"Ace of Diamonds" ,
"2 of Diamonds" ,
"3 of Diamonds" ,
"4 of Diamonds" ,
"5 of Diamonds" ,
"6 of Diamonds" ,
"7 of Diamonds" ,
"8 of Diamonds" ,
"9 of Diamonds" ,
"10 of Diamonds" ,
"Jack of Diamonds" ,
"Queen of Diamonds" ,
"King of Diamonds" ,

Problem:

Take a deck created from these cards and shuffle it using the Fisher-Yates algorithm. That entails swapping the string on the last index -- in this case 51 -- with a string on a randomly chosen index before it. You progress your way down the indexes until you reach the first one, index 0. After shuffling completes, present the two strings at Index 0 and 1.

Algorithm:

- Make a list of strings name "deck" with the 52 cards
- Make a LOOP to shuffle
  - "total" index = length of the deck - 1
  - rightIndex = last index (moving down the indexes)
  - leftIndex = RANDOM string to be swapped with rightIndex
    - 0 < leftIndex > rightIndex
  - var leftCard = value of Index[randomly chosen] (left)
  - var rightCard = value of Index[last Index not swapped] (right)
  - SWAP with
  - deck[leftIndex] = rightCard
  - deck[rightIndex] = leftCard <---- Somehow this swaps them...
- LOOP back up to beginning and repeat until rightIndex = 1
  - Print message $"Shuffling complete! Your cards are {rightCard} and {leftCard}"
