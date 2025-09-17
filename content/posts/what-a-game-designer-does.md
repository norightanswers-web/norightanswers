+++
date = '2025-09-09'
draft = false
title = 'What a Game Designer Does'
summary = 'A high level overview of what game designers do'
tags = ['craft']
+++

Often when someone says they want to be a game designer, they usually follow it with “I have a great idea for a game\!”. 

Now, there’s nothing wrong with that, but expecting to become a designer to execute on your personal vision for a game is a long path. Working professionally, you will very likely have to spend a number of years on projects where the vision comes from the Creative Director before reaching a point where you’re the one whose ideas are being made into reality. There are, of course, exceptions to this \- particularly if you’re working alone or in a small team where you can have more creative control or input, but even then there’s a lot more to the job.

So then, if a designer’s role isn’t just about having the next great idea, what is it? Let’s dig into that.

## Translating direction into systems and mechanics

As a designer, you’ll be receiving direction from someone above you. This will likely be a lead designer (some projects have only one, some have several) or in some cases a director. 

Depending on how the studio or project runs, you may be given \- or asked to produce a ‘one pager’ or a brief of some kind that roughly outlines what the high level experience or functionality should be \- or you may be tasked with creating this outline and getting it approved. From this, it will be your job to create a detailed breakdown and description of the feature and all of its components for the team to build. The form this takes will again depend on your studio, project and team. In some cases it may be a paragraph or point form list outlining how the system or feature works, while in others it may be an exhaustive breakdown of every aspect including art, audio, animation, AI behaviours, player-system interactions and every possible edge case with plans for mitigation.

## Prototyping

Depending when you join a project you may or may not have an active role in prototyping mechanics or features, and if you do, your part in that can vary from guiding programmers as they put a quick representation of the system together for review/approval, to scripting the system yourself. Getting familiar with a visual scripting tool like Unreal Blueprints and Unity Visual Scripting, or learning a scripting language such as LUA, Python or C\#[^1] is a valuable skill that not only lets a designer build towards a representation of the system they want directly, but it also lets you talk with more technical team members in a direct way and understand logic flow, both of which are highly beneficial.

It’s worth noting that at this stage you’re not looking to make something that’s perfect, polished or performant, just a representation of the thing you’re working towards. It will be rough and almost certainly need to be refined or rebuilt, but the goal here is to get something that’s playable and shows where the feature or mechanic is going so the team can see how it fits into the game as a whole and what changes are needed (this is can be referred to as the ‘intent’ of the feature).

## Presenting Features/Mechanics

Your studio or project may ask designers to give a presentation to the team in order to get approval or inform and build consensus for the feature in the team. Usually this is done with presentation software, like powerpoint, google slides or miro, and the content should be kept clean, clear and easy to understand. Reference material, concept art and animations can help convey the intended functionality of the feature.

This process can be helpful in clarifying your design, but it can also generate feedback from the team that should be taken into account if the feature is approved for development. While, as the designer, it will be your job to design and document the feature, your team will be helping to build it and their input should be considered accordingly.

## Creating & Maintaining Documentation

Another key responsibility for a designer is documentation.The form that it takes will, as always, depend on your studio, project or team. Word-processor documents, spreadsheets and visual diagrams are all common and can each serve different purposes depending on the feature, its complexity and the audience it is intended for.

The documentation you create won’t exist in a vacuum, though. You will receive feedback on your written design or prototype. As development progresses and other systems take shape, your feature and design may need to be adjusted, changed, redesigned or cut entirely from the game.

As this happens, keeping your documentation up to date, to ensure the team has a clear picture of what is expected and how the game will function, is an important task. Outdated documentation can be detrimental to both the project and team. 

## Following your features & Communicating with the Team

Documentation is a good reference, but communicating with the team about your feature is even more important, especially as not everyone will read the documentation. 

As your feature passes through implementation, it’s important to communicate with the people who are building it to ensure it matches the intended design. More than a few designers have fallen into the trap of believing what they want is clear, only to have a feature delivered and discover that some aspect was misunderstood or poorly communicated, resulting in additional work and/or missed deadlines. 

By talking with your team about your vision for the feature, and how it fits into the overall experience of the game, you can be sure you’re all on the same page. This also helps address issues as they come up \- sooner rather than later \- which may prevent the feature from being shipped in a state you’re not happy with, or cut entirely.

## Review & Iteration

Once your feature is in the game, you will spend time playing it to generate feedback on any changes that need to be made. That feedback could be asking for more tunable values, having bugs created for unintended behaviours in the feature, or praise and encouragement for a job well done. Never underestimate the power that positive feedback can have on your teammates. Making games is a long, difficult process, and celebrating a job well done or progress on a feature can make the journey easier and help buoy morale.

You will also receive feedback from the team on the feature as well. Most designers expect their lead and directors to provide the feedback, but it’s important to know that valuable feedback can come from anywhere. Getting the team involved in the feedback process not only gives them a feeling of ownership and importance, but it also gives you further insight into how your feature is working and is being perceived.

At this stage you may also begin having playtests. Getting the opinion of people outside your team can also help you understand where things are or aren’t working, how your feature fits into the rest of the game, and what players do or don’t understand about it. This can help highlight what players find too difficult or too easy and where they get lost or confused. This is just a small example as playtesting is a much larger topic than can be fully unpacked here, but it’s important to be aware of. 

All of this feedback is valuable. You may use it to tune the values that have been exposed in the tools for you directly, or you may provide it to the team in order to help drive change or gain consensus on what needs to be addressed.

Regardless of the feedback, spending time to understand the details of specific feedback, and why it was given, is valuable. Sometimes unrelated systems or events during gameplay can lead to a feature being misunderstood or perceived in a way you didn’t expect, and the fix then may or may not be in the feature being tested. How you address the feedback will be partially up to you, but it will also involve your team. Leads and directors will have final say on any mitigation that you or the team suggest.

## Polish

As the project nears completion, there is generally a period of time where the game is functional, playable from start to finish, and is mostly free of large, game breaking bugs. At this time features and mechanics will enter the polish phase where you may spend the extra time to iron out all the little kinks in the experience and make it as smooth as possible.

This is a time of negotiation. Development isn’t finished at this stage, but the technical teams will be working to stabilize the game in order to avoid crashes and bugs, but also optimize it to run as well as possible throughout. They will be sorting out framerate dips, lengthy load times and other performance hitches. 

At this point in time, designers will want their systems iterated on so the process of, for example, resolving that annoying two second delay between completing an interaction with a chest and getting to see the loot, will end up on a list of priorities. If you want it fixed you’ll need to advocate for it based on how important you feel it is when weighed against all the other changes you or other designers, leads and directors want made.

This is not an exhaustive description of what all game designers do, but rather an outline to help clarify what the role of a designer is and roughly what to expect. It’s worth noting that some designers are more specialized and focus on specific aspects such as AI, Combat or Systems, while others may be more generalized. As always, this depends on the studio, project or team.

[^1]:  While C\# is a full programming language in its own right, Unity, Godot and other engines use it as a scripting language.
