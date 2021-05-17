# Walkthrough / Guide

## Event Logic

Each event with another character has 5 potential 'scenes'.  Scenes are like 'bases' from middle school: first base, second base, third base, home, extra.  The number of scenes the player will be able to see depends on the 'event score', which uses a point system calculated as follows:

    Score refers to either Erik or Kaitlin's relevant score towards the Target
    Target is the other person they are with (Kim, Alisha, Chris, Marcus)
    Partner refers to Erik for Kaitlin, and Kaitlin for Erik

- Rule 1: Score with Target > 0 = 1 point
- Rule 2: Score with Target > All Other Targets = 1 point
- Rule 3: Score with Target > Your Partner = 1 point
- Rule 4: Score with Partner <= 0 = 1 point
- Rule 5: Score with Partner < 0 = 1 point

The events are written like so:

    $event = getEventScore(char, target)
    if $event >= 1:
        # the two actors kiss
        if $event >= 2:
            # second base (tits)
            if $event >= 3:
                # third base (handjob/finger)
                if $event >= 4:
                    # sex
                    if $event >= 5:
                        # bonus (anal, exotic position, etc)
                    else:
                        # you stop after sex
                else:
                    # you stop after handjob/fingering
            else:
                # you stop after playing with her tits
        else:
            # you stop after kissing

For example, let's say Erik has the following relationship scores:

- Kaitlin: 1
- Kim: 2
- Alisha: 3

Given the above scores, if Erik goes on a date with Kim, the furthest he will get with her is second base (Rules 1 and 3 = 2 points).

If he went on a date with Alisha though, he would get to third base (Rules 1, 2 and 3 = 3 points).

Another example:

- Kaitlin: 0
- Kim: 2
- Alisha: 3

The player could get to third base with Kim (Rules 1, 3, 4 = 3 points), and have sex with Alisha (Rules 1, 2, 3, 4 = 4 points)

Now if Kaitlin had these scores:

- Erik: -1
- Chris: 1
- Marcus: 2 (this could be 50, it doesn't matter, as long as it's higher than Erik and Chris)

Kaitlin would get to see bonus sex scenes with Marcus (Rules 1-5 = 5 points) if they went on a date, and home base with Chris (Rules 1, 3, 4, 5 = 4 points).

## Avoiding NTR/Kaitlin's Events

If for whatever reason you wish to completely avoid Kaitlin's events, simply keep her score with Erik above 0.  They will still occur depending on the event score above, however the furthest she can get is third base (Rules 1-3).  You may still see the repercussions of these events, but she may lie about them.

For example, let's say Kaitlin comes back from town with Chris and the scores are as follows:

- Erik > Kaitlin: -1
- Kaitlin > Erik: 1

You would notice a hickie on her neck, though she would lie about it and say it's a rash or a bug bite.  If the Erik > Kaitlin score was 1 or higher, he would not even notice the hickie.

## Erik's Events

### With Kim

#### Day 1

- when dropping off the bags, "Take a closer look."
- during the bonfire game, "Shoplifted something."

#### Day 2

- after coffee, "Relax with Kim."
- at the beach, "Refuse."


### With Alisha

#### Day 1

- when she's showering, "Apologize for disturbing her."
- during the bonfire game, "Got a tattoo."

#### Day 2

- after coffee, "Go hiking with Alisha."
- in the storm shelter, "Comfort her."

## Kaitlin's Events

### With Chris

#### Day 1

- at the dock, "Just say hi."
- during the bonfire game, "Played strip poker."

#### Day 2

- on the rocky island, "See what Chris has in mind..."

### With Marcus

#### Day 1

- when day drinking, "Give Kim a hand."
- during the bonfire game, "Had sex at work."

#### Day 2

- on the rocky island, "Squeeze in front of him."
