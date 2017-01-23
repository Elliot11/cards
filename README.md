# Texas Holdem Hand Analyzer

## Description
The idea here is to develop a hand analyzer using Ruby and RSpec. The emphasis is on the test spec created with RSpec.

## Goal
I want to write a Ruby program that will allow me to create a hand analyzer like this:

```ruby
hand1 = Hand.new(Card.new('10', 'Clubs'), Card.new('10', 'Diamonds'))
hand2 = Hand.new(Card.new('3', 'Spades'), Card.new('3', 'Hearts'))
HandAnalyzer.show_odds(hand1, hand2) # hand1 => 80%, hand2 => 20%
```

The code above creates two hands (here, a lower pair of 3s vs. a higher pair of 10s). These odds are important to know in Texas Holdem. I want to calculate them either using a full simulation if possible, or just a random simulation of some portion of the possible cards, if the 1st possibility is too time-consuming.

## Development process
I am using test-driven development (TDD). I move forward by writing individual tests to get me closer to the goal described above.
