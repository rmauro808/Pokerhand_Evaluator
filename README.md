# Poker Hand Evaluator

This is a Python program designed to evaluate poker hands and determine the best possible hand from a set of five cards. The program is capable of identifying all standard poker hands, including Royal Flush, Straight Flush, Four of a Kind, Full House, Flush, Straight, Three of a Kind, Two Pair, One Pair, and High Card.

Features
- Poker Hand Evaluation: The program evaluates a set of five cards and identifies the best poker hand.
- Card and Deck Management: Includes a `Card` class for representing individual cards and a `Deck` class for managing the deck of cards.
- Card Values and Suits: Supports the standard 52-card deck with suits (Hearts, Diamonds, Clubs, Spades) and values (2-10, Jack, Queen, King, Ace).
- Unit Tests: Contains unit tests to verify the correctness of the poker hand evaluation logic.
  


Code Explanation

Card Class
The `Card` class represents a single card in the deck. It includes two properties:
- `suit`: One of the four suits (Hearts, Diamonds, Clubs, Spades).wwwwwwwwwwww
- `value`: One of the card values (2-10, Jack, Queen, King, Ace).

Deck Class
The `Deck` class manages a full deck of 52 cards. It shuffles the deck upon initialization and has a `deal` method to draw a specific number of cards from the deck.

PokerHandEvaluator Class
This class contains the core logic for evaluating poker hands. The `evaluate_hand` method takes a list of `Card` objects and returns the best possible hand along with the ranking of the cards that make up the hand.

Unit Testswwwwwwwwwwwwwwww w

The unit tests are located in `test_hand_evaluator.py`. They test various scenarios, such as:
- Royal Flush
- One Pair
- Straight Flush

Example Hand Evaluation
For example, if you have the following cards:
```python
cards = [
    Card("Diamonds", "A"),
    Card("Hearts", "A"),
    Card("Clubs", "3"),
    Card("Spades", "4"),
    Card("Diamonds", "10")
]

```
The expected output would be:
```
("One Pair", [12, 12, 8, 2, 1])


