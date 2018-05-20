Developing a simulation of the board game Monopoly in R
The game Monopoly is played on a board with 40 squares.
Players begin the game on the GO square. On each turn, the player rolls two 6-sided dice. The sum of the
dice determines the number of squares they advance (in a clockwise direction) on that turn.
Without any further rules, we would expect players to visit each square with equal probability. However,
landing on G2J (go to jail), CC (community chest), and CH (chance) changes this distribution. When a
player lands on G2J, they must immediately move to the JAIL square.
At the beginning of the game, the CC and CH cards are shufed. When a player lands on CC or CH they
take a card from the top of the respective pile and, after following the instructions, it is returned to the
bottom of the pile. There are 16 cards in each pile, but for this assignment we are only concerned with cards
that order a movement. Any card not concerned with movement will be ignored and the player will remain
on the CC/CH square. The relevant cards are:

Community Chest (2/16)
1. Advance to GO
2. Go to JAIL

Chance (10/16)
1. Advance to GO
2. Go to JAIL
3. Go to C1
4. Go to E3
5. Go to H2
6. Go to R1
7. Go to next RR (railroad)
8. Go to next RR
9. Go to next UT (utility)
10. Go back 3 squares

In addition to G2J and CC/CH, if a player rolls doubles on three consecutive turns, they proceed directly to
jail. A “double” is a roll where the two dice are equal, such as rolling 2 fves or 2 sixes.
