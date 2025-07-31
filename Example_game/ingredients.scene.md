title: Ingredients


@flour
title: Flour
is-card: true
new-page: true
card-image: img/flour.jpg
tags: pantry
max-visits: 1
on-arrival: has_flour = 1

Of course, the flour is past the expiration date.

"Do you think it's still good past the expiration date?" you ask. "It's only a few months."

"Hold on, let's look this up..." Emily takes out her phone. "The New York Times says that white flour can probably be used no matter its age. Apparently it can last for years, even. So it's probably fine."

"That's a relief..."

- @make_dough: Make the dough.

@make_dough

The recipe calls for 4 cups of flour, 1 1/2 cups of water, and 1 tsp of oil. So, you mix all that into the bowl, and stir with a fork.

"I can stir it," Emily says, watching over your shoulder.

- @em_stir: Let Emily handle this.
- @stir_yourself: You can stir it yourself.

@em_stir
on-arrival: em_helped += 1

You hand Emily the fork and let her stir the dough.


@stir_yourself

"It's already basically good," you reply.


@wood-ears
title: 木耳 (Wood ears)
is-card: true
new-page: true
card-image: img/wood_ears.jpg
tags: pantry
max-visits: 1
on-arrival: has_wood_ears += 1; filling += 1
view-if: filling_mixed = 0

The recipe calls for "some" 木耳, an unspecified quantity.

Wood ears (木耳) are some kind of black dried fungi. You're supposed to soak them in water, and once they're soft again, chop them up and add them to the filling.


@vermicelli
title: 粉丝 (Vermicelli)
is-card: true
new-page: true
card-image: img/vermicelli.jpg
tags: pantry
max-visits: 1
on-arrival: has_vermicelli += 1; filling += 1
view-if: filling_mixed = 0

The recipe calls for "some" 粉丝, an unspecified quantity. Most of the quantities are unspecified.

粉丝 (vermicelli) are thin noodle-like sticks made from mung bean flour (and corn starch, according to the ingredients). You're supposed to soak them in warm water until they're soft, then chop them up finely and add to the filling.


@chives
title: 韭菜 (Chives)
is-card: true
new-page: true
card-image: img/chives.jpg
tags: fridge
max-visits: 1
on-arrival: has_chives += 1; filling += 1
view-if: filling_mixed = 0

The recipe calls for about 1/2 lb chives. You do not weigh your chives, but it seems approximately correct. Mom does not weigh her ingredients either.

Chives (韭菜) are the primary components of the filling. Chives are a grassy vegetable, a little garlic-y or something like that? Anyway, you're supposed to chop them up finely (you can never chop as finely as mom did).

"There are a lot of chives. Can I help cut some of them?" Emily asks.

- @em_chives: Let Emily handle some of the 韭菜.
- @chives_2: Chop them all yourself.

@em_chives
on-arrival: em_helped += 1

You give Emily the knife and let her handle the vegetables. She cuts them about as well as you do.

"Sorry, this is like, really thick," she says.

@chives_2

"It's okay, I can do it myself," you say, and finish chopping the rest of the vegetables.

"Oh, okay..."


@eggs
title: Eggs
is-card: true
new-page: true
card-image: img/eggs_1.jpg
tags: fridge
max-visits: 1
on-arrival: has_eggs += 1; filling += 1
view-if: filling_mixed = 0

The recipe calls for 4 eggs, cooked.

Eggs have probably the most involved preparation step of any of the ingredients here. You have to cook the eggs first, scramble them, before adding them into the filling mix. That involves cracking the eggs, beating them, turning on the stovetop, adding some oil to the pan, adding the eggs into the pan, stirring them until they solidify, and then, finally, you will have some scrambled eggs.

- @ask_em_scramble: Ask Emily if she can make the scrambled eggs.
- @scramble_yourself: Cook the eggs yourself.

@ask_em_scramble
on-arrival: em_helped += 1; em_eggs = 1

"Um, Em, can you make the 炒鸡蛋? The, um, scrambled eggs?" You catch yourself speaking Chinese more when cooking. Something about it feels natural. Emily speaks much less Chinese; she was born in America.

Emily smiles. "Sure, it's probably the one thing I can make..."

She seems to be rather good at this. While she cooks the eggs, you can work on the rest of the recipe.


@scramble_yourself

For some reason, you feel as if you have to do all of this yourself. So you crack four eggs into a bowl, stir them with chopsticks until they are a uniform yellow, and then proceed to turn on the stovetop, add oil to the pan, and cook.

"I could have helped," says Emily. "Sorry..."

- @its_okay: "It's okay! I wanted to do this..."

@its_okay

"It's okay! I wanted to do this..."

Emily catches your gaze for a moment. "Uh, okay then."


@spices
title: Spices and oils
is-card: true
new-page: true
card-image: img/spices.jpg
tags: pantry
max-visits: 1
on-arrival: has_spices += 1; filling += 1
view-if: filling > 1 and filling_mixed = 0

The recipe calls for olive oil (extremely not traditionally Chinese, but whatever), sesame oil, a little soy sauce (not too much), salt, and white pepper powder. The quantities are not given for any of these ingredents, so you add enough to the pot until it looks approximately right.


@shrimp
title: Shrimp
is-card: true
new-page: true
card-image: img/shrimp.jpg
tags: fridge
max-visits: 1
view-if: filling_mixed = 0

The recipe calls for approximately 1/4 lb of chopped shrimp.

There is a package of frozen shrimp in the fridge, which is a few months expired. But, frozen products never go bad, right?

- @vegetarian: "Oh, um, you can't eat this, right, Em?"

@vegetarian

"Oh, um, you can't eat this, right, Em?"

She shrugs. "I mean, I'm not that strict... I don't know, I haven't looked up the carbon footprint of aquaculture recently. Do you think it's necessary?"

- @add_shrimp: Add the shrimp
- @no_shrimp: Don't add the shrimp.

@add_shrimp
on-arrival: has_shrimp = 1; filling += 1

You chop up the shrimp and add it into the filling bowl. "I suppose the recipe says we should... You know, my mom said that this is a 素的 recipe. Like, somehow shrimp isn't an animal."

"It's fine," Emily says. "I can eat shrimp, if it's something you like."


@no_shrimp

"Let's not add it," you say. Emily nods.
