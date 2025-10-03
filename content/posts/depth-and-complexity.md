+++
date = '2025-10-03'
draft = true
title = 'Depth and Complexity'
summary = 'Defining and understanding each so you can use them effectively.'
tags = ['craft']
+++

There are few terms in game development so often confused, conflated and misunderstood as depth and complexity. It’s not uncommon to see it framed as “depth vs complexity” as though they exist on a sliding scale with depth at one end and complexity the other.

The truth is that depth and complexity are separate scales of their own. You can have high or low depth and high or low complexity within the same game because they are not intrinsically tied together. Increasing complexity does not diminish depth, just as decreasing depth does not enhance complexity.

## Depth

Depth is a one-to-many relationship; a single action that has a variety of outcomes in gameplay with consistent, predictable results. It uses a limited number of first order actions, however each action has contextual outcomes. 

Let’s take the example of the crafting grid in Minecraft. It’s a single mechanic that allows you to use multiple ingredients with it in order to create contextual outcomes. What you get out depends on what you put in. The crafting grid is limited in size and forms the most basic layer of crafting in the game. The crafting table extends on this formula. It expands on the crafting grid and allows for more ingredients to be used in order to create more advanced tools and objects. 

In both cases the only action the player has is adding or removing ingredients to and from the grid. Once the player arranges the ingredients in the grid into a valid recipe, they can remove the created item, consuming the ingredients.

Characteristics of Depth:

* One-to-many relationship  
* Few first order actions  
* Each action has contextual outcomes

## Complexity

Complexity arises through a many-to-one relationship or many one-to-one relationships. It is notable in that it presents a much larger palette of first order actions for players to understand.

Returning to the example of crafting in Minecraft, the recipes used to create objects on the crafting table add complexity to the mechanic. With nine slots in the grid and every inventory item in the game able to be placed on any slot, but having only one correct recipe to create a particular object, we have many one-to-one relationships. If you include the variations of tools and objects made with different materials we now have a many-to-one relationship for each outcome.

Characteristics of Complexity

* Many-to-one or many one-to-one relationships  
* Many first order actions  
* Each action has an outcome, but isn't guaranteed to be contextual

## Cognitive Load

Every piece of information we ask players to retain, process and act on increases their cognitive load. Purely from a systems standpoint, each connection between actions and outcomes increases the player’s cognitive load by virtue of needing to understand these relationships and how they will be impacted by them. When you add all of the other elements of the game into the mix there can be a lot for players to take in while playing.

While both depth and complexity add to the player’s cognitive mode, complexity increases it considerably more. Understanding how much you’re asking a player to remember while playing is vitally important. Requiring players to remember and understand too many interactions between systems builds fatigue. Over time, that fatigue compounds and can cause the player to disengage from the experience, pushing them out of the game.

It is generally a good practice to use complexity sparingly, intentionally and introduce it slowly in order to give players time to absorb it and acclimate to it. As always however, the approach you choose needs to suit the purposes of the experience you intend to create.

## A Case for Complexity

Consider that sometimes you want something to be complex. Systems that are intentionally difficult to conceptualize or master. They can be meant to simulate a situation or even to intentionally overwhelm the player as part of the experience. 

Returning to the example of Minecraft, the recipe book could have been added much earlier in development, however the original intention was to need to experiment in order to learn how to make objects. This complexity in having obscured recipes added another layer of mystery and learning to the game, which still remains, however has been mitigated by the recipe book.

As another example, look at an aeroplane’s control panel. There are many \- sometimes dozens \- of dials, buttons, switches and indicators that each do something. Flying an aeroplane is a complicated activity by its very nature, so if you want to truly simulate that activity in an immersive way, it will naturally be complex.