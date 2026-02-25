---
layout: default
title: Database
permalink: /databases/
---

## Database

[Enhancement Source Code](https://github.com/magdielrosario97/vault166/tree/vault166-database)

### Artifact Overview

My chosen artifact is Vault 166, a Python-based text adventure survival game originally created as a final project for the IT-140 Introduction to Scripting course around June 2023. The game runs entirely in the command line and allows the player to explore a sealed vault by navigating between rooms, collecting items, and making decisions that determine whether they survive or lose the game. The concept of the game came from my own interest in the Fallout series, which inspired the setting and narrative direction of the project. The original implementation was created to meet the project requirements by designing a complete and playable experience that focused on exploration and item collection. At the end of IT-140, the game’s code lived in a single file which relied on straightforward logic and conditional checks to control gameplay without persistent storage between sessions.

### Justification for Inclusion and Enhancement

I chose to continue enhancing Vault 166 for my ePortfolio because it allows me to further develop my software engineering capabilities after redesigning and refactoring my original project. Adding a database builds directly on the previous architectural and algorithmic improvements by integrating persistent storage into an existing program without restructuring the core gameplay logic.

This enhancement demonstrates my ability to design and implement a relational database schema that supports application state management while maintaining separation of concerns. Rather than modifying large portions of the existing logic, the persistence layer operates independently from the gameplay systems.

Instead of pickling or rewriting core logic, I designed a normalized schema that stores only mutable runtime state, such as player location, health, inventory contents, and per-room changes. Static world definitions, including room connections, descriptions, and hazard rules, remain defined in code and are reconstructed at startup. Saved state is then overlaid onto the rebuilt world, and save and load methods were implemented to handle slot management and state restoration.

### Course Outcome Alignment

My enhancements target course outcomes three, four, and five as planned from Module One. Outcome three is demonstrated through the design and evaluation of a computing solution that integrates persistent data storage into an existing program.

Using established database tools and techniques to implement a reliable solution supports outcome four. Integrating SQLite into the Python application required structured schema design, parameterized queries, foreign key constraints, composite primary keys, and transaction management to ensure consistent and predictable behavior.

Additionally, validating saved and loaded game data to prevent corruption or inconsistent state supports outcome five by demonstrating attention to data integrity and potential failure conditions within the application.

### Reflection on the Enhancement Process

Due to the structure of the game, adding the database in this enhancement was easier compared to the other enhancements. This category required a slight shift in focus, as working with SQL benefits from methodical thinking. Mapping runtime objects to relational tables forced me to think about what data needed to be stored and what should remain in code.

I debated storing entire room objects but decided it would make the system harder to manage and maintain. By storing only mutable values, I preserved the structure developed in earlier milestones while adding persistence in a controlled way. Another challenge was making sure the saved data could be restored without introducing inconsistencies or redundancies. I added validation checks during load operations and used a snapshot-based save strategy to prevent stale or partial data from remaining between sessions.
