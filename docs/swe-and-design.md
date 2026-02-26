---
layout: default
title: Magdiel Rosario Orta
permalink: /swe-and-design/
---

[Home](/) · [Professional Self-Assessment](/self-assessment/) · [Code Review](https://youtu.be/7GYiDzha6yg) · **[Software Design and Engineering](/swe-and-design/)** · [Algorithms and Data Structures](/algorithms/) · [Database](/databases/)

## Software Design and Engineering

### Repository and Documentation

[Original Source Code](https://github.com/magdielrosario97/vault166/tree/vault166-original)

[Enhancement Source Code](https://github.com/magdielrosario97/vault166/tree/vault166-architecture)

[Technical Documentation](https://github.com/magdielrosario97/vault166/blob/main/docs/ARCHITECTURE.md)

### Artifact Overview

My chosen artifact is Vault 166, a Python-based text adventure survival game originally created as a final project for the IT-140 Introduction to Scripting course around June 2023. The game runs entirely in the command line and allows the player to explore a sealed vault by navigating between rooms, collecting items, and making decisions that determine whether they survive or lose the game. The concept of the game came from my own interest in the Fallout series, which inspired the setting and narrative direction of the project. The original implementation was created to meet the project requirements by designing a complete and playable experience that focused on exploration, item collection, and simple game logic.

### Justification for Inclusion and Enhancement

I wanted to include Vault 166 in my ePortfolio because it is a passion project that I can not only improve but also expand over time. I have been looking for a reason to return to this project, and the capstone provided an opportunity to continue developing it while applying what I have learned throughout the program. At the end of IT-140, the game’s code lived in a single file and relied on straightforward logic and conditional checks to control gameplay.

For the software design and engineering enhancement, I focused on restructuring the application instead of changing the gameplay. The code was refactored into separate modules and classes so that different parts of the game logic were no longer all handled in one place. This made the code easier to read, easier to follow, and easier to build on later, while keeping the original gameplay behavior intact and providing a stronger foundation for future enhancements.

### Course Outcome Alignment

Successfully completing this enhancement allowed me to meet course outcomes three and four that I planned for during Module One. By working with an existing, functional codebase, I analyzed the original structure and identified areas where the design could be improved without changing gameplay behavior. Refactoring the game required making design decisions about how responsibilities should be divided across classes and modules while still preserving the original logic and flow of the game.

Additionally, I applied software engineering techniques that support maintainable and scalable design. Introducing a central Game class and separating core responsibilities into dedicated modules improved the overall organization of the application and helped improve code quality while keeping the behavior of the game consistent.

### Reflection on the Enhancement Process

As I worked through enhancing the project, I found myself diving deeper into Python documentation and refreshing my understanding of technical concepts that I had not revisited in a while. Creating the different classes and modules was straightforward, though there were small issues along the way that required careful debugging and testing. This process helped reinforce the importance of planning changes before implementing them, especially when working with an existing codebase.

Two major improvements to my development process during this enhancement involved version control and testing. Instead of making large changes all at once, I broke the refactor into smaller steps and tested the game after each change to ensure that gameplay behavior remained the same. This made it easier to catch errors early and understand where issues were coming from. I also followed a structured Git workflow, committing incremental changes rather than pushing everything at the end. This approach helped me better document my progress and maintain a stable working version of the project throughout the enhancement.
