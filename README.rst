Goal
________

* Immediate gratification.
* Casual play.
* A magic format played from a shared pool of cards.
* Works with 2-5 players.
* Most games finish in under an hour.
* "Feels" like playing limited magic.

Requirements
_____________

The game is played with a shuffled pool of cards containg spells and land as well as one of each basic land per player. This is basically a cube or booster packs shuffled with basic land but we do not know the optimal makeup.

Classification of Cards
________________________

All available cards are classified by the following sets for the purpose of this game.

* red cards.
* instants and sorceries.
* those cards owned by the emperor.
* those that are not included in this classification.

Before you play a system for arbitrating inconsistency and incompleteness should be agreed on. If you come up with solutions that work please fork this and send a pull request.

Zones
_______

We replace the library with two additional zones, draw piles and the shoe. The zones are the same as ordinary magic except as follows.

*shoe*
  starts the game containing the randomized pool of cards for that game. The size of the shoe is not defined. This takes the place of the Library for all purposes except drawing

*draw piles(pack)*
  each player and the "passed draw pile" is dealt a seven card draw pile to start the game. a player may look at his or her draw pile at will.

*passed draw pile*
  This is a draw pile that no player currently controls. It exists merely to keep the passing of cards atomic.

*hand*
  a players hand starts with one of each the 5 basic lands.

Game Play
______________

during each turn a player:

1. untaps
2. draw phase: the draw phase is broken into two actions.

    a. replenishes, adds cards from the shoe to his or pack until the pack contains 7 cards.
    b. picks, chooses one card from his or her pack and adds it to his or her hand. He or she becomes the owner of that card.

3. main phase
4. combat phase
5. second main phase
6. end step
7. pass step the player exchanges his or her pack for the pack in the passed pack zone.

Mechanics:
____________

*draw*
  whenever you would draw a card, replenish your pack, then pick.
*scry, fateseal, search, shuffle etc*
  effects that would use a library use the shoe instead.
*mulligan* 
  if your pack contains 5 or more lands you may reveal it, exile it then replenish.

Termination
_____________

* the game ends when all but one or fewer players has lost or at least one player has won.
* if the shoe is depleted replenish effects are ignored.
* if a player cannot pick a card all players lose one life.
* If after after all players have taken a turn the gamestate does not change due to any effects those effects are ignored for the rest of the game.(because this game is going to terminate).
