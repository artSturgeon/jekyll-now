---
layout: post
title: libGDX Jam Post-mortem
excerpt: A retrospective on my entry for the 2015/16 libGDX Jam
---

## The jam is now over, how did we do?

I was intending to post my dev log entries on [itch.io](http://itch.io/) and on this blog, but ended up just posting them on itch. So to start with here's a link to the [dev log](http://itch.io/jam/libgdxjam/topic/12178/arthur-scotts-devlog) I made during the game jam.

And here's a link to the actual [game page](http://houseofsturgeon.itch.io/space-sweeper).

And the rating page with my [results](http://itch.io/jam/libgdxjam/rate/50757).


Overall placing was **43 out of 83** entries. Highest ratings were innovation (30) and graphics (40), lowest was audio (53).

I'm pretty happy with the results, this was my first game jam, and Space Sweeper is pretty much my first finished arcade game. I'm also still finding my way around with Kotlin, and Ashley (Entity Component System).

Let's break it down!


## What went well?


* Using an ECS

    I struggled a little at first with where to put logic which touches more than one entity/system, but I think I'm starting to get the hang of it now. Being able to add/remove components and systems at runtime is really powerful, and much neater than the bunch of if statements I ended up with in [Nubbles](/nubbles)!

* Kotlin

    I like the Kotlin syntax, after using JavaScript/TypeScript for a while and then coming back to Java, Kotlin made the transition a little less painful. Higher order functions and Lambdas make things like list filtering and callbacks much neater. And no semi-colons!


## What didn't go so well?


* Kotlin

    While overall I do like Kotlin, it does have it's own idiosyncrasies. It seems to take the whole *'it might be Null!'* problem and turn it into a catastrophe. It may just be because I'm not used to some of the operators, but I still ended up having to deal manually with null pointer problems.

* IntelliJ

    When it works it's easily the best Java IDE I've used, but it seems to be really finicky about how it's set up. As I was traveling during the jam I used a few different computers, with slightly different setups. What worked fine on one computer, just wouldn't on another. I ended up using Eclipse for a while because it just worked with my Kotlin/Gradle setup, which is daft, as JetBrains developed Kotlin...


## What did we learn?
* Make a plan

    The temptation with something like a game jam is to jump straight in and start knocking out code, but that way madness lies. Better to sit down with a pencil and paper, sketch out some ideas, pick one, flesh it out on paper, before committing to any code creation. You need an idea of where you're going in a game jam, because you won't have time to pivot.

* Iteration is king

    Get something working end to end as soon as possible. Make something that's actually a game, i.e. has at least play/win/lose states. Then iterate on this, add in new features and ideas. This way if something doesn't get finished in time, you'll still be able to release something.

Source code is on [github](https://github.com/artSturgeon/spacesweeper) if you want to have a look. It isn't too bad but given it was a jam there are a few areas which got a bit clunky...

Overall the standard of entries was very high, and I'll be looking through some of the source code for other games to see what I can learn. Looking forward to entering again next year!

Thanks much,

art
