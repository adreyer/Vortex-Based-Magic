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
* "Feels like" playing limited magic.

Requirements
_____________

The game is played with a shuffled pool of cards contaning spells and land as well as one of each basic land per player. This is basically a cube or booster packs shuffled with basic land, but we do not know the optimal mana curve or land ratio.

Classification of Cards
________________________

All cards are divided into the following sets for the purpose of this game.

a. red ones
b. instants and sorceries
c. ninth edition storm crows
d. overpowered ones
e. merfolk
f. those owned by the emperor
g. those not included in this classification

Before you play, a system for arbitrating inconsistency and incompleteness should be agreed on. If you come up with solutions that work, please fork this and send a pull request.

Zones
_______

We replace the library with two additional types of zones: packs and the shoe. The zones function in the same way as ordinary zones in Magic, except as follows:

*shoe*
  The shoe is a hidden zone containing cards that are not owned or controlled by any player. At the beginning of the game, it contains all cards in the game. When any effect other than a draw effect would affect a player's library, it instead affects the shoe. The shoe must be kept in a single face-down pile. No player can look at or change the order of the shoe unless an effect causes him or her to do so.

*packs*
  A pack is a zone containing cards temporarily owned by a single player. Additionally, a passed pack under no player's ownership resides in its own zone. At the beginning of the game, each player is dealt a pack of seven cards from the shoe, and the passed pack is dealt face-down. All packs are hidden zones. A player may arrange his or her pack in any convenient fashion and look at it as much as he or she wishes. A player can't look at the cards in another player's pack but may count those cards at any time. If a pack contains more than seven cards, then its owner randomly discards a card from that pack as a state-based action.

*passed pack*
  The passed pack is a pack that no player currently owns. It exists to make passing of packs an atomic operation and to ensure that each player drafts from different packs on subsequent turns. The passed pack is a hidden zone contianing cards that are not owned or controlled by any player.

*hand*
  A player's opening hand is assembled by four turns for each player, each turn consisting only of a draw step and a pass step. After these turns, each player adds three basic lands from outside the game to his or her hand. If a player would mulligan this hand, he or she instead does nothing. After each player has a hand of seven cards, play begins using normal turn structure.

Game Play
______________

*drawing*
    Whenever a rule or effect would cause a player to draw a card, that player instead drafts a card. Drafting consists of two steps: the replenish step and the pick step.

    a. replenish: the player adds the top card of the shoe to his or her pack until the pack contains exactly seven cards. If the shoe contains no cards, nothing happens in this step.
    b. pick: the player chooses one card from his or her pack and puts it in his or her hand. He or she becomes the owner of that card for the duration of the game. If there are no cards in his or her pack, all spells and effects currently on the stack are countered, the current turn ends immediately, and the player who failed to pick loses one life.

*pass step*
    In the end phase, after the cleanup step the player exchanges his or her pack for the pack in the passed pack zone. At this time, he or she loses ownership of the previous pack and gains ownership of the new pack. This step occurs as a state-based action.

*mulligan*
  During a player's upkeep, if his or her pack contains five or more basic lands, he or she may reveal that pack and exile all cards it contains. Until the end of the turn, that player must replenish to exactly five cards instead of seven.
