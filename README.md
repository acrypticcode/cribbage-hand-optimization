# Cribbage Hand Optimization
Author: Curran Flanders

Start Date: 07/28/2024

## Description
Program to advise which cards to discard in cribbage to obtain highest-scoring hand

## Rules of cribbage
Cribbage is a card game in which two players compete to reach a score of 121 points before their opponent. During a round, each player is dealt 6 cards and chooses two to "throw" or remove from their hands. These thrown cards are combined to form the "crib" so that each player has four cards in their hand and there are four cards in the crib. After players choose which cards to throw, the deck is cut and a card from the deck is turned over. It is treated as a part of both players' hands and the crib for the purposes of scoring. Each hand is scored for several possible card combinations including pairs of cards with the same rank, runs of cards with adjacent ranks, and cards whose values sum to exactly 15. The crib is scored in the same way, and its points are awarded to the dealer. Players also score points during a pegging phase in every round, where the players play cards one at a time and score points based on combinations of their own and their opponenents cards that have been played.

See the full rules of cribbage here: [bicyclecards.com/how-to-play/cribbage/](https://bicyclecards.com/how-to-play/cribbage/)

## Approach
There are three ways in which players can score points: by scoring their own hand, by scoring the crib as the dealer, and during the pegging round. The information the program is given is the cards in the players hand and the cards that have not yet been revealed and discarded (i.e. they are either in the deck or the opponenent's hand). There are fifteen possible combinations of two cards the player can discard from their six-card hand. Each of these possible pairs of discards is given a score for each of the three ways the player can score points, representing the average point differential obtained compared to their opponent assuming their opponent is also playing optimally. These three scores are then summed and the pair is matched with the highest total score is recommended to the player for discard.

## Progess
Allowed user to optimize cribbage hand considering only the personal scoring of their hand and not the score of the cards the crib or the score from the pegging round. The next step is likely to be accounting for the cards in the crib. This will involve the determination of optimal strategies using game theory.
