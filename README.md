# DandD-Campaign-Management-Tool
A tool for D&amp;D planning and managing table top role-playing games.


## Table of Contents
* [Feasibility Report](#feasibilit-report)

## Feasibility Report
* [Executive Summary](#executive-summary)
* [Background](#background)
* [Outline of Project](#outline-of-project)
* [Conclusion](#conclusion)

## Executive Summary

## Background
Running a D&D campaign requires a substantial amount of planning mainly in three main areas:
* [Locations]
* [Characters]
* [Items/Loot]
* [Battle Maps]

At the time of writing, there are no tools available for organising all of the above.  Currently, available tools typically cover either the first 3 or just battle maps.  The tools that facilitate the planning of the first 3 typically miss useful features like loot containers and usually require excessive navigation between web pages to access useful information like entity descriptions.  Both groups of tools also lack the ability to automatically handle passive ability checks that would otherwise require the GM to look between different tabs for each of the characters in a given session.
The separation of these tools can also lead to issues in a campaign especially if a party decides to initiate a fight where a combat encounter was not intended.  This would typically be resolved with a verbal description of the environment without a battle map, which can be disappointing to some players.

## Outline of Project

This project could reasonably be split into 2 main components, a battle map tool, and a campaign planning tool.  Where at any point in a campaign the battle map can be launched from the planning tool for any given location or encounter.  Both of these tools should have different information shown to the Game Master and to the Players in a campaign.

The campaign planning tool will have a strong focus on HCI to ensure that any additional menu functionality not present in other tools to not make it confusing for users to use.  In terms of specific functionality the planning tool should allow users to create entities such as:
* [Settings]
* [Locations]
* [Characters]
* [Loot Containers]
* [Loot Items]

When creating any of these items it will be simple for a user to create relationships between entities such as creating a character in a given location or placing loot items in a character's inventory.  These relationships should also be mutable by the Game Master, for example, if a player picks up a loot item the GM should be able to change the location of that item to a specific player character's inventory.  When the GM is running a game session they will be able to open a location in the planning tool and easily see a short description they have written for each of the entities in that location potentially through a dropdown menu.

The players in a campaign will be invited through the planning tool by the GM where they will only be able to see entities made visible to them by the GM.  If there are multiple players in a campaign then some entities may only be visible to a subset of the players.  Players will also be able to make private notes in their character journals and for each of the entities that are public to them.

The battle map tool component of this project will allow a GM to create a map from a set of prefab tiles, and arrange, non-player characters, loot items, and containers in the map they have created.  When creating the map the GM will be shown a list of all entities in the location that the map is for as defined in the planning tool.

Once the GM has created and launched a battle map they will place the relevant player characters in the map.  Once the map has been launched and the player characters have been placed the map tool should manage the initiative rolls for each player and non-player character (the result of a d20 determining the order of combat).  When it is a player's turn they should be shown the distance from their character to their mouse pointer and a circle showing the range of movement for their turn.  In combat, the GM should be able to, measure the distance between any two points, move non-player characters on their turn, and edit the attributes of entities such as health according to attack moves.  Due to the range of actions in D&D, the GM will handle the results of actions outside of movement.

In both the planning and battle map tools the GM should be able to set up passive perception checks that trigger at their discretion and use the passive perception of each player character to determine whether or not they pass the check.  This should open a text pop-up visible only to the players who passed the check.

## Conclusion

This project will aim to create a tool for D&D campaigns that combines two types of tools and adds additional useful functionality to both.  Especially in the addition of passive perception checks that streamlines the process to reduce the length of breaks in the flow of play.  Not only will this tool make D&D more simple to play but it will make campaigns easier to set up and plan.
