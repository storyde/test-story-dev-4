title: Cooking

@filling
title: Filling
is-pinned-card: true
new-page: true
card-image: img/filling.jpg
view-if: filling > 2 and dumplings_made = 0 and filling_mixed = 0 and has_chives = 1
tags: pinnedCard

Do you want to finalize the filling? The current ingredients include:

[? if has_wood_ears = 1 : wood ears ?]

[? if has_vermicelli = 1 : vermicelli ?]

[? if has_chives = 1 : chives ?]

[? if has_eggs = 1 : eggs ?]

[? if has_spices = 1 : spices ?]

[? if has_shrimp = 1 : shrimp ?]

Are you missing anything?

- @more_filling: There's more to add.
- @no_more: Mix the filling.

@more_filling

Probably best to double-check to see if there's anything you've missed.

@no_more
on-arrival: filling_mixed = 1

There's nothing more to add, you hope.

"馅儿做完了 *The filling is made*," you say.


@dumplings
title: Make the dumplings.
view-if: filling_mixed = 1 and dumplings_made = 0
new-page: true
card-image: img/board.jpg
is-pinned-card: true
on-arrival: dumplings_made = 1
tags: pinnedCard

Now that the filling is done, the next step is to actually assemble the dumplings. This is usually a task for two people. When you made dumplings with Mom, in the brief moment of reconcilliation last year before you left home again, one of you would make the skins, and the other would assemble the dumplings.

Emily looks at you, and it seems like she has the same idea.

"Okay, so..."

- @make_skin: You make the skin, Emily assembles the dumplings.
- @assemble: Emily makes the skin, you assemble the dumplings.

@make_skin
on-arrival: em_assembles = 1

You'll roll out the dough, and Emily will assemble the dumplings.

"Um, I haven't done this in a while," she says. "Like, probably at least 10 years. So it might look bad. Sorry."

- @oh_why: "Oh, why?"
- @make_dough: Concentrate on making the dough.

@oh_why

"Oh, why?"

"After high school my parents said I should study instead of cooking." A pause. "I used to like cooking. Maybe a bit too much. My dad said that when I grew up I should find a wife who liked cooking, unlike my mom. So now if I'm going to be a good wife I have to learn how to cook better. Sorry. That was a joke."

- @heteronormative: "That's heteronormative as fuck."
- @dont_worry: "Don't worry, I like cooking!"
- @make_dough: Concentrate on making the dough.
- @make_dumplings: Concentrate on making the dumplings.

@heteronormative

"That's heteronormative as fuck," you say.

"Sorry. Yeah. You shouldn't be the only one cooking in this household, though..."

- @cook_more_together: "Maybe we should cook more together."
- @make_dough: Concentrate on making the dough.
- @make_dumplings: Concentrate on making the dumplings.

@dont_worry

"Don't worry, I like cooking," you say.

"You shouldn't have to be the only one cooking in this household, though!"

- @cook_more_together: "Maybe we should cook together more."
- @make_dough: Concentrate on making the dough.
- @make_dumplings: Concentrate on making the dumplings.

@cook_more_together

"Maybe we should cook together more," you suggest.

"Yeah, we should do something like this more often."

Unfortunately, your schedules and habits are such that you usually purchase ready-made food. Maybe that will change. It's difficult, though. Time and energy are against you.

- @make_dough
- @make_dumplings

@make_dough
view-if: em_assembles = 1
title: Concentrate on making the dough.

First, you kneed the dough, and stretch it out into a long cylinder, maybe a couple of inches in diameter. Next, with a knife, you cut off little pieces of the dough cylinder, maybe half an inch in thickness. Then, you press the cylinder with the palm of your hand, and then roll the piece of dough. You alternate pressing on the piece of dough back and forth with the rolling pin in your right hand, and then rotating it with the left hand. This way, you roll the piece of dough into an approximate circle.

Meanwhile, Emily assembles the dumplings. They're rather inexpertly assembled, laying flat on the side instead of sitting upright with a curve in the middle like Mom always made, but it's going to be fine. In the mouth, it will all taste the same. 

- @in_the_end

@assemble
on-arrival: you_assemble = 1

"Okay, I literally have no idea how to make the dough," Emily says. "The skin, I mean."

"You just, like, first roll the dough into a long cylinder, then you cut off small chunks, and then roll those small chunks of the cylinder into a flat circle with a rolling pin."

She stares at you, seemingly dumbfounded.

- @show_you: "I'll show you."

@show_you

"I'll show you," you say, and you demonstrate how you would roll out the dough. First, you kneed the dough, and stretch it out into a long cylinder, maybe a couple of inches in diameter. Next, with a knife, you cut off little pieces of the dough cylinder, maybe half an inch in thickness. Then, you press the cylinder with the palm of your hand, and then roll the piece of dough. You alternate pressing on the piece of dough back and forth with the rolling pin in your right hand, and then rotating it with the left hand. This way, you roll the piece of dough into an approximate circle.

"I think I can do it," Emily says after watching you. "Sorry, I'm really bad at this. I haven't helped make dumplings in, like, probably at least 10 years."

- @oh_why: "Oh, why?"
- @make_dumplings: Concentrate on making the dumplings.

@make_dumplings
view-if: you_assemble = 1
title: Concentrate on making the dumplings.

While Emily makes the skins (slower than you would make), you assemble the dumplings. With the skin in your left hand, you take a glob of filling with chopsticks and plop them down in the middle. Then, you fold the centers together along the diameter of the skin, and then, with the crook between your thumb and index finger, you fold in the skin on either side of the center. The sign of an expert is making a dumpling that can stand up, and you do so.

- @in_the_end


@in_the_end
title: Enough dumplings are assembled to make one pot.

After enough dumplings are assembled to make more than one pot (around 20 or so), the two of you decide to take a break.


@boil
title: Boil the dumplings.
view-if: dumplings_made = 1
new-page: true
card-image: img/dumplings.jpg
is-pinned-card: true
on-arrival: dumplings_boiled = 1
tags: pinnedCard

Finally, you can boil the dumplings. You fill a pot with water, and then boil it on the stovetop. After it is boiling, you add in the dumplings. After the water boils again, you add in an extra cup of cold water.

It is extremely crucial that you add in the extra cup of water, for reasons unknown.

- @third_time: After the water boils for the third time, it is done.

@third_time
on-arrival: dumplings_made = 12
go-to: em_worried if em_helped <= 0

After the water boils for the third time, and the dumplings are floating in the top of the water, that is when they should be fully cooked.

- @try_them: Try them!!!

@em_worried

"Sorry, I feel like I didn't help much," Emily says.

- @its_okay_dumplings
- @its_okay_dough
- @dishes


@its_okay_dumplings
view-if: em_assembles
title: "It's okay! You helped assemble the dumplings!"

"It's okay! You helped assemble the dumplings!"

"But like, you did everything else..."

- @try_dumplings

@its_okay_dough
view-if: you_assemble
title: "It's okay! You helped make the dough!"

"It's okay! You helped make the dough!"

"But like, you did everything else..."

- @try_dumplings

@dishes
title: "You can do the dishes afterwards."

"You can do the dishes afterwards."

"Yeah, of course, but also..."

- @try_dumplings

@try_dumplings
title: "Let's just try the dumplings first, okay?"
go-to: try_them

"Let's just try the dumplings, okay?"

"Okay..." She nods. "But next time, I want to do more to help."

@try_them
title: Try them!!!

You plate some of the dumplings. You and Emily each get chopsticks and take a bite.

- @dumplings_good
- @dumplings_bad

@dumplings_good
title: They're pretty good!
on-arrival: dumpling_quality = 1
view-if: has_spices = 1 and has_eggs = 1

The dumplings are actually pretty good, perhaps surprisingly! The flavor profile is balanced despite the slapdash ingredient mixing.

You and Emily look at each other, coming to the same conclusion. She smiles, and you smile in turn.

"We should, like..." Emily begins-

"Increase our frequency of home-cooked Chinese meals?"

"Yeah, that."

- @endgame: Next time...

@dumplings_bad
title: They... need some improvement.
on-arrival: dumpling_quality = -1
view-if: has_spices = 0 or has_eggs = 0 or has_chives = 0

You and Emily look at each other, coming to the same conclusion. It isn't *bad*-tasting, but it's missing something. There is a balance or texture that is missing.

- @no_spices
- @no_eggs

@no_spices
view-if: has_spices = 0
title: "Oh no, I forgot to add the spices!"

"Oh no, I forgot to add the spices! I didn't even add the soy sauce or salt."

"That's why it tastes so bland... I should have noticed. I should have said something. Sorry."

- @endgame: There's always next time...

@no_eggs
view-if: has_eggs = 0
title: "Oh no, I forgot to add the eggs!"

"Oh no, I forgot to add the eggs!"

[? if has_shrimp = 1 : "At least there's shrimp, for the protein?" ?]

[? if has_shrimp = 1 : "Yeah... sorry about that." ?]

"It's fine. I didn't know either. I should have said something. Sorry."

- @endgame: There's always next time...

@endgame
game-over: true
