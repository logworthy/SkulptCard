SkulptCard
==========

## Background

I'm involved in the [Mathematicians in Schools](http://www.mathematiciansinschools.edu.au/) program, 
and have been trying to introduce a class of 5th-grade kids to some of the basics of computer science.

I built this game to help out with that.

## The Game

The game is designed to be run locally (I don't have internet access at the school), so just clone the
repository and open **game.html** in a browser.  It has been tested on the latest versions of Firefox and Chromium.

15 cards are selected at random from a standard deck.  They are sorted face down by suit (spades, clubs, diamonds, hearts) 
and then by rank with the lowest card on the left.  

One of these cards is chosen at random for the player to guess.  The player must flip cards until they
find the chosen card.  

Once the chosen card has been found, clicking it advances the player to the next round and
the setup is refreshed.

## Design

This game was designed to help kids assess the merits of different strategies (algorithms) for finding the chosen card.

In particular, it can always be solved in 4 moves or less using a binary-search strategy.  However, a probabilistic
strategy (e.g. we know that high hearts are likely to be to the right of the deal)
will usually do better across most deals.

I'd hoped to eventually include a python element that would allow me to demonstrate different strategies for choosing
in code (and potentially allow the kids to code their own), 
hence the inclusion of [skulpt](https://github.com/skulpt/skulpt).

## Teaching

If you're looking for advice on how to incorporate this in the classroom you should probably ask 
[an actual teacher](http://blog.mrmeyer.com/).

I split the kids into two groups and had them play against each other (5 rounds each) on a projector.
They enjoyed it and pretty quickly gravitated towards the probabilistic strategy that I mention above.

Getting them to articulate *why* that's a good strategy, when it would work well/poorly and what sort of other strategies
they might try is my next challenge.

## Cards Licence

This project uses GPL card images sourced from [this page](http://freeware.esoterica.free.fr/html/freecards.html).

The following text appears on the source page:

>Authors: Original deck, (C) Oxymoron.
>.....The modified deck ([this download](http://freeware.esoterica.free.fr/html/adls/cmagedeck.zip)), (C) Katzmiff 2002
>
>Regular 52 playing cards plus two Jokers, upright & reversed Aces, one cardback. (59 images in all). This is the regular deck used in [CardMage](http://freeware-esoterica.narod.ru/cmfiles/cardmage.html).
>Size: 71 x 96 pixels.
>
>Licence for this deck is of course GPL and may be modified under the terms of the licence.
