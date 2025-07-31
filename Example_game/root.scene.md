title: Root Scene
new-page: true
go-to: main if started = 1; start_menu if started = 0


@start_menu

= 饺子 (Dumplings)

- @start: Start game
- @credits: Credits


@start
on-arrival: started = 1
new-page: true

= 过新年

This Chinese New Year is different from all of the previous ones. Despite your family's various tribulations, Mom has always recalled you home for the occasion. This is the furthest you have been from "home", wherever that is.

- @step_back: Your name is Karen Zhao, or 赵秋怡, and you are...

@step_back

Your name is Karen Zhao, or 赵秋怡, or Zhao Qiuyi, and you are... a person, you suppose, or something like that. You're in your 20s. You were born in Changchun, Jilin Province, PRC, and you moved to America with your parents at a young age. And...

- @living_em: And you've been living with Emily for a while now.

@living_em

The two of you share a one-bedroom apartment in the city in which the two of you attend different postgraduate programs.

- @relationship: The two of you are in some sort of relationship.
- @dating: Wait, are you actually *dating*?
- @married: You're basically married already.

@relationship

Yes, you're in a relationship. Emily Chen is your girlfriend, and you are hers, or something like that. You've been together since sometime last year, since the early phase of the pandemic, or something like that.

- @dumplings: Does it really matter what you call it, though?

@dating

"Dating" would imply that the two of you engage on activities that can commonly be termed as "dates". Instead you just live together and eat together and sometimes share a bed and...

- @dumplings: Does it really matter what you call it, though?

@married
on-arrival: wife = 1

You live together and have an exclusive relationship and usually eat together and sometimes share a bed and sometimes share finances and one or both of you have made frequent references to being married despite your not-actually-married circumstances and...

- @dumplings: Does it really matter what you call it, though?

@dumplings

Well, whatever it is, the two of you have decided to make dumplings today. Mom gave you one of her recipes, and in the past week, you and Emily braved the long journey to an Asian market to acquire all the requisite ingredients.

As they say, today is the day.


@credits

Text and photographs by Autumn Chen. Very loosely adapted from a recipe my mother taught me. The recipe for the filling was actually for 韭菜盒子 (https://en.wikipedia.org/wiki/Jiucai_hezi), but I think it works for dumplings as well.

Made with DendryNexus.

- @start_menu: Back to menu
