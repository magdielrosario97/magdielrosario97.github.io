---
layout: default
title: Magdiel Rosario Orta
permalink: /algorithms/
---

[Home](/) · [Professional Self-Assessment](/self-assessment/) · [Code Review](https://youtu.be/7GYiDzha6yg) · [Software Design and Engineering](/swe-and-design/) · **[Algorithms and Data Structures](/algorithms/)** · [Database](/databases/)

## Algorithms and Data Structures

### Repository and Documentation

[Original Source Code](https://github.com/magdielrosario97/vault166/tree/vault166-original) · [Enhancement Source Code](https://github.com/magdielrosario97/vault166/tree/vault166-algorithms) · [Technical Documentation](https://github.com/magdielrosario97/vault166/blob/main/docs/ALGORITHM.md)

### Artifact Overview

My chosen artifact is Vault 166, a Python-based text adventure survival game originally created as a final project for the IT-140 Introduction to Scripting course around June 2023. The game runs entirely in the command line and allows the player to explore a sealed vault by navigating between rooms, collecting items, and making decisions that determine whether they survive or lose the game. The concept of the game came from my own interest in the Fallout series, which inspired the setting and narrative direction of the project. The original implementation was created to meet the project requirements by designing a complete and playable experience that focused on exploration and item collection. At the end of IT-140, the game’s code lived in a single file and relied on straightforward logic and conditional checks to control gameplay.

### Justification for Inclusion and Enhancement

I reselected Vault 166 to use in my ePortfolio because I can continue to improve and expand the gameplay and logic after completing the software engineering and design category. Prior to working on these enhancements, I used this artifact as my passion project to strengthen my development skills.

For this milestone, the artifact was enhanced to better demonstrate the application of algorithms and data structures within a structured and interactive system. Several components were improved to allow more dynamic gameplay based on player input, game state, and environmental conditions. Player inventory is now stored using a set, which enables efficient membership checks when evaluating hazards, locked rooms, and boss conditions. The vault layout is represented as a graph structure, with rooms acting as nodes connected by directional relationships. This enables clean movement validation and supports scalable expansion of the game world.

Two significant additions to this enhancement are the introduction of an input parsing system and a centralized rules system. Player commands are now tokenized and normalized using alias mapping and prefix matching, which allows players to use shorter commands while still maintaining predictable behavior. Gameplay rules such as environmental hazards, darkness restrictions, and boss conditions were also centralized into rule-based functions, replacing scattered conditional logic and improving reusability, readability, and modularity.

### Course Outcome Alignment

These enhancements allowed me to demonstrate course outcomes three and four that I planned to meet during Module One. The use of algorithmic principles and computer science practices is demonstrated through modeling the vault layout as connected rooms, using sets for inventory management, and evaluating gameplay rules based on player state and environmental conditions. My ability to use well-founded techniques and tools to deliver value within the artifact’s intended context is shown through the introduction of a dedicated input parsing system and the centralization of gameplay rules. These changes improved clarity, reusability, and scalability while maintaining predictable behavior.

In addition, updating documentation, polishing terminal output, and adding docstrings supported outcome two by improving the clarity of written and visual communication used to explain the system and its design decisions.

### Reflection on the Enhancement Process

This enhancement went beyond my initial refactoring of the artifact and opened new areas of improvement that were previously above my knowledge level. One important lesson I learned was the value of separating algorithmic logic from control flow, especially as complexity increases when additional mechanics are added. Moving rule evaluation and input normalization out of the main game loop made the code easier to read and understand while significantly reducing mental load when debugging or extending functionality. This separation became increasingly helpful as the codebase expanded and bugs were identified through testing.

I faced several challenges during this enhancement, particularly balancing usability with control and managing output flow without cluttering the terminal. Allowing partial or shorthand commands improved usability but required careful handling to avoid ambiguity. The final design prioritizes predictable behavior by explicitly rejecting certain inputs, which improved reliability and reduced bugs. Another challenge involved ensuring the player retained context without being overwhelmed by output, which required rethinking when and how information was displayed. This led to a clearer separation between persistent status output and room descriptions, reinforcing the importance of intentional design decisions in interactive systems.
