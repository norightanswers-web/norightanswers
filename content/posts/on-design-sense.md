+++
date = '2025-09-09'
draft = false
title = 'On Design Sense'
summary = 'What it is and how designers use it to inform their decisions'
tags = ['craft']
+++

How does a game designer decide how to approach a mechanic or system? What leads them to the conclusions they draw? How do they form their thoughts and ideas about a feature or system into a tangible experience for the player?

They use their **Design Sense**.

Design Sense is a term I use to describe the way a game designer approaches their craft. It is the yardstick they hold up to measure the player experience. It informs their expectations of how a feature, system or mechanic works when they interact with it.

It is informed by their experiences, their preferences and tastes, their personal views and the goals they believe are important to achieve, both in the final product but also during development. It is a game designer's internal compass, and it is the most important tool a designer has. And, like the designer themself, it evolves with time and experience.

## Design Sense and the Vision

Many games have a stated **core vision**. This defines the **razor**(s) that are central to the experience and attempts to provide a common rallying point for the team to focus their approach to decision making, expected implementation of the fantasy and the player experience around.

So, how does your design sense work with the core vision? It starts by understanding what the game is, and what it is not. 

For example, if the game’s fantasy is to play as a private investigator, would it make sense to add a finishing move mechanic to combat? Probably not unless the PI also happens to enjoy fighting in cage matches.

Would it make sense to add a driving feature? Quite possibly \- stake-outs, tailing suspects and car chases are a part of the Private Investigator fantasy in a lot of media, after all. 

Consider, however, that driving can be a big, expensive feature depending on how in-depth you want it to be. There could be simpler, on-rails driving or trailing sections \- and it’s worth noting that doing stake-outs, tailing suspects and chases can all be done without an actual driving feature and all of the additional cost it incurs, instead occurring on foot.

Similarly, the finishing move mechanic might fit very well into your fantasy if your player character is meant to be in the mould of Sherlock Holmes who, even outside Hollywood portrayal, occasionally got into some fisticuffs and was said to practice “baritsu” (bartitsu).

In both of the examples above, I used my design sense to step through connected aspects of the fantasy, make lists of what may or may not fit, and explore those. While some of the ideas I generated might not work, for various reasons, they were pathways to finding interesting mechanics that fit the fantasy. This is how understanding what the game is intended to be, and what it is not intended to be, will inform the decisions you make during development and your justifications for those decisions.

## Design Sense Vs the Vision

There may be times when your design sense seems to clash with the vision. Where your particular approaches to solving problems never seem to hit the mark. This can be difficult and even frustrating. In these events it’s worth taking a moment to regroup and look at other features, which have aligned with the vision, and try to understand why. If possible, discuss it with another designer, they may be able to offer a different point of view or share ideas that help you align better with the vision.

One useful tactic for this can be ‘Yes and’ing. Even if you don’t immediately agree with a solution, try saying yes and expanding on the feature along similar lines, in your own way. It may not be the feature you expected it to be, but you might find something better too. It’s worthwhile to note that this does not give carte blanche to suggestions that break scope, but rather a way to find the core of the idea that can be worked into a shippable design.

## Design Sense in Action

Here is a scenario to consider, and some ideas on how to approach it. The approaches that resonate most with you will be those that agree most with your design sense.

During early production you’re tasked with figuring out how a specific, largely undefined feature will fit into the game. It is based on the core narrative conceit that the character can create objects they’ve seen before.   
Additionally, the moment-to-moment 3Cs gameplay is largely defined and implemented, and all of the buttons on the controller are already in use. How do we approach this challenge?

Given the defined situation, I suggest starting with the core narrative conceit. What does it say about the game? Does it set up an expectation you can take advantage of?

For this example, the conceit is that the character can create objects they’ve seen before. This is a fairly broad, open-ended task so there are many possible approaches, all with varying levels of complexity and player agency. 

The additional wrinkle that all the buttons on the controller are already used means that if we want to add an ability to let the player create objects, we need to find a way to do that.

**Note:** For the sake of brevity and remaining within a reasonable scope of discussion for the purposes of this article, I will intentionally omit or gloss over some details that would normally be important to the player’s experience, in the name of making a broader point. As an exercise for the reader, identify these aspects for yourself and explore how your own solutions might work within the confines of the problem space.

Here’s a few examples:

### The Everything Approach

We keep a list of every object in the game that the player has seen. In the game proper, this would be every prop that has passed through the view frustum of the player camera. 

In order to allow the player to create them, we overload a button with a hold or long press in order to summon a menu that they can choose the object from. In this case we’ll say that summoning a menu puts the player into a different gameplay context, which means the previously used buttons are free within the confines of the menu to be used to navigate the menu and select the object to summon. Alternatively we could re-use an existing input convention for navigating the UI for this menu, if one existed.

This is, undoubtedly, the most expensive option from both a development and player experience standpoint. It requires every object type in the game to be tracked as to whether you’ve seen it or not and it requires the player to be able to sort through them easily. It also requires all objects to have a use and for players to understand them. For a small game with only a few recurring objects this is less of a problem, but for a game made at scale that could have dozens or even hundreds of objects, this becomes a **combinatorial explosion** and requires a deep investment, across all disciplines, in the mechanic to make it worthwhile. This could also become a limiting factor in how many objects the game can have if the player needs to be able to create them all.  
It does, however, present an elegant approach to solving the issue of inputs.

### The Mechanical Approach

In data we tag objects and require the player to interact with them to learn how to create them. This introduces another new mechanic, though \- interacting with the objects. This could take a number of forms but for simplicity let’s say the player inspects the object. 

For inspecting an object, we could overload an existing button when looking at an object you can learn to summon. Overloading this input will allow a contextual interaction that players can learn, but will also require objects that can be inspected to not interfere with other aspects of gameplay, which may require additional metrics to be established for their placement.

For creating an object we could reuse the same button with a hold action on it to summon the object creation menu. If that isn’t possible, a **chorded input** could be a possibility.

It’s worth mentioning that this approach also means there’s the possibility that a player could simply **not** inspect and learn how to create objects. A common solution to the problem is that in order to advance you need to be able to create the object.

### The Restricted Approach

The list of objects a player can create is authored per-level to strongly restrict what they can create, and when. This means someone (probably you\!) needs to curate a list of selected objects that the player can create in each level. The input issue could be solved by having specific locations that visually hint which object the player can summon there, and then contextually overload a button to create the object.

This has the least player agency of the options but is also the most straightforward and easily understood option. Players will need to understand why the list of objects they can create changes from level to level, and the form that takes can vary \- perhaps it’s an expanding list that adds a few new objects in each level, that’s easily understood. Or it could be completely new or different objects in each level because the levels themselves are so different from one another that previous objects no longer make sense or serve a purpose in this environment.

### The Mix and Match Approach

The final approach I’ll describe here \- which is by no means the final option \- is one that is very well worth considering. By taking elements from each idea and combining them, you take the best pieces of each and make something that is potentially stronger than all the other options. It’s also an approach that is often taken in design out of necessity and compromise.

An example of mix and match would be:

* The long-press, new context menu (Everything)  
* The inspection mechanic from (Mechanical)  
* The limited number of learnable objects per level (Restricted)


Combining these aspects of each approach has now given us a feature that has a limited scope that the team could potentially produce and support, and allows us strong controls over which objects can be learned and used in each level.

So, how do you choose which approach is right? Well, spoilers, there are no right answers. It entirely depends on the direction, vision, pillars, scope of the project, what project leadership actually wants for the game and your own design sense.

You can, however, make it a little easier by looking at a few additional factors.

* What is the core gameplay of the game you’re making?   
* How does a given approach enhance or diminish the gameplay?   
* Is this solution in keeping with the themes and experiences in the game?  
* Is this really needed to deliver the desired experience?  
* Is the required effort worth the expected outcome?  
* Is this new or groundbreaking in some way? Does it need to be?

## Developing & Improving Your Design Sense

So, if design sense is so important, is it something you’re born with? Is it an innate sixth videogame sense that only a lucky few have? 

Well, no actually. It’s a skill that you develop. Here’s a few ways to do that:

**Play** games to see what ‘feels good’ to you and what doesn't. Analyze why you feel something does or doesn’t feel good and what you would have considered doing instead, while considering the rest of the game and what knock-on effects it would have. If you made those changes, would it be the same game?

**Explore** non-games media. Yes, you can develop your design sense by **not** playing games\! Reading books, watching films and playing tabletop games all contribute to your sense of what feels good in an experience. Remember, in games we are making **experiences** and if done well that will transcend the moment to moment and stick with players.

**Expand** the pool of experiences you have to draw on. Explore new activities like hiking, rock climbing, sailing, exploring unfamiliar cuisine, building furniture or metal working. Every human experience can teach us something about what we do and don’t like, and why. More importantly, they can change our minds as well. Always keep an open mind and be willing to consider your world view may be too narrow or you may have drawn the wrong conclusions.

Finally, and most importantly: **Be curious.**