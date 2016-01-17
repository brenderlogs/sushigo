sushigo
===============

Use the command line to play with a friend or the computer. Currently the game is only one round, with no puddings, and the hand size is set to six so that the minimax computer can explore the game tree without taking all day. Moreover, the first move is made with full knowledge of all cards in both players' hands.

Future work: More game tree pruning and increased hand size, closed hands on the first move, implement puddings and multiple rounds.

Playing is fairly simple, just type the name of the card you would like to take from your hand and place on your table. To use a chopsticks card on your table, type `Swap for C and D`, where C and D are the names of the cards in your hand you would like to swap with the chopsticks. The cards are played onto your table in the order you listed them in (this is important with wasabi).

Here's a sample game.

```
>>> execfile('sushigo.py')

SushiGo!

1. Human vs Human, 2. Human vs Robot: 2


p1's hand: ['DoubleMaki', 'Sashimi', 'TripleMaki', 'Chopsticks', 'SalmonNigiri', 'TripleMaki']

p1's table: []

p2's hand: ['SquidNigiri', 'SalmonNigiri', 'EggNigiri', 'Dumpling', 'Dumpling', 'SquidNigiri']

p2's table: []

p1's play: Chopsticks
p2's play: SquidNigiri


p1's hand: ['SalmonNigiri', 'EggNigiri', 'Dumpling', 'Dumpling', 'SquidNigiri']

p1's table: ['Chopsticks']

p2's hand: ['DoubleMaki', 'Sashimi', 'TripleMaki', 'SalmonNigiri', 'TripleMaki']

p2's table: ['SquidNigiri']

p1's play: Swap for SquidNigiri and SalmonNigiri
p2's play: TripleMaki


p1's hand: ['DoubleMaki', 'Sashimi', 'SalmonNigiri', 'TripleMaki']

p1's table: ['SquidNigiri', 'SalmonNigiri']

p2's hand: ['EggNigiri', 'Dumpling', 'Dumpling', 'Chopsticks']

p2's table: ['SquidNigiri', 'TripleMaki']

p1's play: SalmonNigiri
p2's play: Chopsticks


p1's hand: ['EggNigiri', 'Dumpling', 'Dumpling']

p1's table: ['SquidNigiri', 'SalmonNigiri', 'SalmonNigiri']

p2's hand: ['DoubleMaki', 'Sashimi', 'TripleMaki']

p2's table: ['SquidNigiri', 'TripleMaki', 'Chopsticks']

p1's play: Dumpling
p2's play: Swap for DoubleMaki and TripleMaki


p1's hand: ['Sashimi', 'Chopsticks']

p1's table: ['SquidNigiri', 'SalmonNigiri', 'SalmonNigiri', 'Dumpling']

p2's hand: ['EggNigiri', 'Dumpling']

p2's table: ['SquidNigiri', 'TripleMaki', 'DoubleMaki', 'TripleMaki']

p1's play: Sashimi
p2's play: Dumpling


p1's hand: ['EggNigiri']

p1's table: ['SquidNigiri', 'SalmonNigiri', 'SalmonNigiri', 'Dumpling', 'Sashimi']

p2's hand: ['Chopsticks']

p2's table: ['SquidNigiri', 'TripleMaki', 'DoubleMaki', 'TripleMaki', 'Dumpling']

p1's play: EggNigiri
p2's play: Chopsticks


p1's table: ['SquidNigiri', 'SalmonNigiri', 'SalmonNigiri', 'Dumpling', 'Sashimi', 'EggNigiri']

p2's table: ['SquidNigiri', 'TripleMaki', 'DoubleMaki', 'TripleMaki', 'Dumpling', 'Chopsticks']

p2 wins by 1
```
