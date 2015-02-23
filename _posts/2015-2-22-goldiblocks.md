---
layout: post
title: Goldiblocks and the Three Bear-rays
---


Once upon a time, there was a little girl named Goldiblocks. 

``` ruby
goldie = Girl.new
goldie.name = "Goldiblocks"
```

She went for a walk somehwere no little girls should ever go...the forest. Pretty soon, she stumbled upon a house. While most people would have just walked away, little Miss Goldiblocks just had to see what was inside.

``` ruby
home = House.new
```

...But the door was locked. Goldiblocks kocked and knocked, but nobody answered. So she decided to take measures into her own hands.

``` ruby
goldie.pick_lock(home)

home.guests 
=> ["Goldiblocks]
```

Goldiblocks then enters the kitchen, starving as usual, looking to eat someone else's food.

``` ruby
home.porridges
=> ['hot', 'cold', 'just right']

goldie.eat_porridge(home.porridges)
This porridge is too damn hot!
This one's freezing cold!
Awwwwwwwwww yeaaaaaaaaaa. That's the one.

home.porridges
=> ['hot', 'cold', nil]
```

After she was done stuffing her face, Goldiblocks realized how exhausing all that work was. She went to go park herself in a chair for a bit.

``` ruby
home.chairs
=> ['big', 'medium', 'small']

goldie.sit_down(home.chairs)
This chair is big enough for a bear.
Another huge-ass chair.
This one is actually oka.....Ah, crap.

home.chairs
=> ['big', 'medium', nil]
```

This was a great sign to take it easy on the porridge next time.

Deciding that she still needed to rest her spoiled little self, Goldiblocks made her way into the bedrooms.

``` ruby
home.beds
=> ['hard', 'soft', 'perfect']

goldie.lay_down(home.beds)
This bed is hard as a rock.
Too...soft...can't.....get....out....
I feel like I'm floating!

goldie.conscious
=>false
```

The homeowners finally arrive. And yup, they're frickin' bears.

``` ruby
papa = Bear.new
mama = Bear.new
baby = Bear.new
```

They walked inside their home after a lovely visit to their local church with all of their bear neighbors, when they noticed something was wrong. Someone was messing with their stuff. As you might expect...

``` ruby
papa.come_home_to_looted_house
papa.mood
=>'pissed'
```

The bears search around for the person who broke into their home, when...

``` ruby
papa.find_intruder(goldie)
You're going down, Goldiblocks!!!

goldie.escape_attempt(home)
Goldiblocks looks around for the nearest escape.
She finds a window and makes a break for it!

``` ruby
papa.stop_escape(goldie)
```

Random Outcome 1:

``` ruby
papa.just_missed(goldie)
Papa barely misses and allows Goldiblocks to get away.
Goldiblocks runs away in the forest, never to be seen by the bear family again. 
Hopefully Goldiblocks stops eating other people's porridge.
```

Random Outcome 2:

``` ruby
papa.size
=> 'massive'
papa.size
=>'huge'

papa.administer_justice(goldie)
Bite to the face!
Goldiblocks has committed her last B&E."
The last thing she hears is "No porridge will EVER BE our porridge."

goldie.alive
=>false
```


