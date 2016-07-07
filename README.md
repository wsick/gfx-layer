# gfx-layer
Proposal for a layered graphics system.

## Overview

Graphics engines are becoming very sophisticated. 
Notably, they are resolution independent and hardware accelerated.
As they become more sophisticated, maintaining, optimizing, and enhancing these engines becomes painful and less accessible.

Due to the enormous costs of ownership, vendors have no incentives to build consistent, cross-platform systems.
Crushed by the overwhelming complexity, vendors choose to provide their APIs to a selective set of languages (in many cases, only one).  Without trivializing the difficult nature, I think there is a better solution to these problems.

## History

When first developing Fayde, I faced enormous trouble attracting contributors.
Upon years of reflection, I recognize that graphics systems require a very narrow set of skills and desire.
Generally speaking, developers with these skills are heavily involved in the gaming community.
They do not have the appetite to build a general purpose graphics engine.
Conversely, developers with the appetite are quickly discouraged from the overwhelming nature.
Further, choosing a language like Javascript heavily narrowed the desire of willing participants.

## Reaction

This has prompted me to take an aggressive approach to alleviate community problems.
This approach entails *layered*, *swappable* systems that individually provide value to a community of developers.
Dividing and conquering helps alleviate software stability issues while promoting ease of contribution.
At first, it may appear like this approach is to divide communities, but this is absolutely contrary to what I am proposing.
Instead, I would like to unite communities toward solving a common goal of consistent, cross-platform, easy-to-use, cross-language graphics engine; however, allowing developers to optimize for their specific strengths.

## Proposal

The following layers are a proposal toward achieving this goal.
Each layer represents a contractual agreement with its partners, but it does not preclude one layer from aiding another.

### Differentiator

This proposal has no new concepts from what the graphics community has already derived.
Most graphics systems contain 1 or more layers defined; however, they are coupled tightly. 
Instead, this proposal intends to define bounded contexts around commonly used patterns.

### Layers

NOTE: Naming is the hardest part of software, help out with suggestions.

- [Composer](composer.md)
- [Retainer](retainer.md)
- [Rasterizer](rasterizer.md)
