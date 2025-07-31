title: Main
new-page: true
is-hand: true
max-cards: 3

[? if filling = 0 and has_flour = 0 : There are two major components to making dumplings - assembling the filling and assembling the skin. ?]

[? if filling_mixed = 1 and dumplings_made = 0 : The filling is already properly mixed, hopefully. ?]

[? if dumplings_made = 1 : Now, the only thing left to do is boil the dumplings, and eat. ?]

- @pantry
- @fridge
- #pinnedCard


@pantry
title: Pantry
card-image: img/pantry.jpg
is-deck: true
view-if: has_flour = 0 or filling_mixed = 0

- #pantry

@fridge
title: Fridge
card-image: img/fridge.jpg
is-deck: true
view-if: filling_mixed = 0

- #fridge
