+++
date = '2025-10-24'
draft = false
title = 'Design Docs: Goals and the Player Experience'
summary = 'Defining what a features does vs how the player feels when interacting with it.'
tags = ['craft']
+++

Every studio, team and designer has their own way of approaching game design documentation. Some are very formalized and prescriptive, while others are more free-form. Nearly all design documentation contains a list of goals \- things the feature is expected to do in the game \- but much like the documents themselves, their format varies wildly. Some are highly specific while others are nebulous. This can make interpreting how a feature should be implemented, and when it is achieving all of its goals, fraught with potential error and confusion.

To resolve this, we can break the goals into two lists \- one we’ll still call Goals, and another we’ll call Player Experience. Each list can have multiple line items that describe the feature in their own way.

## Goals

These are statements that define how a feature works *mechanically* and what it *does*. They’re a list of succinct, deliverable statements, clearly written so they can be checked off. If a goal written for a feature says the feature does something, that’s exactly what it does. If it’s not doing that in the game, it’s either not implemented or not working as expected.

Example:

* When the player collects a power-up, their strength is increased by 50

## Player Experience

These are statements that define how the player should *feel* when they interact with a feature. As each player’s experience is subjective, they can be harder to gauge when they’ve been met, but are critically important to the player’s perception of their gameplay experience.

Example:

* When the player collects a power-up, they feel more powerful

## Why Separate Them?

This breakdown of each type of statement into its own category allows us to treat them differently \- in both expectation and evaluation. Often goals are easier to achieve, but player experience statements take longer to satisfy because they don’t describe something mechanical, but rather how the player feels. 

Consider the examples given in both sections above; they seem to say what could be read as the same thing, but are meaningfully different. 

In the goals section we clearly state that something mechanical about the game has changed \- in this case the player’s strength attribute. Reading that you might say, “Oh, they’re more powerful” but that depends on how the strength attribute is implemented in the game and how the player perceives or interacts with it \- it could be an attribute the player hasn’t invested in or that their gameplay style doesn’t leverage \- but that isn’t important for the goal \- only that the strength attribute has changed.

In contrast, the player experience section doesn’t define any values but instead describes how we want the player to feel. This could be achieved in many possible ways \- by increasing the player’s strength attribute, making them briefly invulnerable, increasing how high they jump or altering how much damage enemies take while the power-up is in effect. This has much more latitude to achieve the *feeling* we want the player to have.

Now, this isn’t to say that one type of statement is superior to the other, but rather that they’re different tools. The ideal design document will use both to describe how to achieve the intended end product. Taking the above statements together we can use the player experience to define the sort of experience we want the player to have, and the goals to document how we will achieve that.

Here’s the power-up feature example again, using both types of statements together:

**Goals**

* When the player collects a power-up, for `[10]` seconds:   
  * `[Strength]` is increased by `[50]`  
  * They are invulnerable to damage

**Player Experience**

* When the player collects a power-up:
  * They feel more powerful  
  * They want to collect more power-ups

**Tip:** Use square brackets, or some other indicator, to define tunable values. This allows the person doing the implementation to know which values you need exposed in data.

By combining both types of statements we can clearly delineate the problem spaces for *how* the feature works versus the way the player is expected to *feel* when they interact with it. This makes evaluating the feature and tackling specifically identified problems much more straight-forward as development progresses.