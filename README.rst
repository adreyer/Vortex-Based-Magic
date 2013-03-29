Vortex Based Magic
====================

Goals
________

* Immediate gratification.
* Casual play.
* As simple as possible.
* A magic format played from a shared pool of cards.
* Works with 2-5 players.
* Most games finish in under an hour.
* "Feels" like playing limited magic.

Requirements
_____________

The game is played with a shuffled pool of cards containg spells and land as well as one of each basic land per player. This is basically a cube or booster packs shuffled with basic land but we do not know the optimal makeup.

Classification of Cards
________________________

All cards are divided into the following sets for the purpose of this game.

a. red ones
b. instants and sorceries
c. ninth edition storm crows
d. overpowered ones
e. those owned by the emperor
f. those not included in this classification

Before you play a system for arbitrating inconsistency and incompleteness should be agreed on. If you come up with solutions that work please fork this and send a pull request.

Zones
_______

We replace the library with two additional zones, draw piles and the shoe. The zones are the same as ordinary magic except as follows.

*shoe*
  starts the game containing the randomized pool of cards for that game. This takes the place of the Library for all purposes except drawing

*draw piles(pack)*
  each player and the "passed pack" is dealt a seven card draw pile to start the game. a player may look at his or her draw pile at will.

*passed pack*
  This is a draw pile that no player currently controls. It exists merely to keep the passing of cards atomic.

*hand*
  a players hand starts with one of each the 5 basic lands.

Game Play
______________

The parts of a turn are the same with the following exceptions:

*draw phase* The draw phase is broken into two actions.

    a. replenishes, adds cards from the shoe to his or pack until the pack contains 7 cards. If the shoe is depleted nothing happens.
    b. picks, chooses one card from his or her pack and adds it to his or her hand. He or she becomes the owner of that card. If there are no cards to pick all spells and effects currently on the stack are canceled; the current turn ends; The player who failed to pick loses one life.

*pass step* 
    After the end step the player exchanges his or her pack for the pack in the passed pack zone.

Mechanics:
____________

*draw*
  whenever you would draw a card, replenish your pack, then pick.
*scry, fateseal, search, shuffle etc*
  effects that would use a library use the shoe instead.
*mulligan*
  if your pack contains 5 or more lands you may reveal it, exile it then replenish.
