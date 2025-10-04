# Ecological Simulator
## Motivation

Have you played Factorio and looked at your production graphs and wished there was a game just to look at the logistic graphs about how resource consumption works?
This project aims to simulate an ecosystem with at least 3 tropic levels and show stats on population growths and resource consumption.
It will also simulate a basic genetics where organism traits like metabolic efficiency and age will be mutated slightly to create new organism.
The motivation behind this project is to sharpen my rust skills in processing very large number of objects in memory efficiently, getting familiar with Bevy game engine and implementing a basic GUI interface.

## Objective and key features
- Game world will start with basic parameters of land area and solar density over that area.
- There will be day night cycles and seasons.
- There will be initial population of autotrophs (think algae or plant) and heterotrophs (think animals) and their predators.
- Each organism will have metabolic efficiency parameter that will determine how much of it's resource consumed will it be able to use, rest will be considered wasted.
- There will be logic for calculating starvation if they run out of resources and also logic for aging.
- Organisms can all reproduce if they make it to maturity age. New organisms will inherit slightly perturbed traits (metabolic efficiency and age) from their parents..
- The world will be homogenous, no localization of resources, plants or animals, if resource is available globally, organism can use it. (Some logic to ensure fair distribution and not first come first serve)
- Track and display time series data number of organisms of each type in the world.
- Ability to change world condtions like changing the solar energy input simulating a volcanic eruption.
- Ability to save and load back simulation state from disk. (only the current state will be saved and past time series data will be lost)
- Use Bevy as game engine if possible. [This is a good resource](https://bevy-cheatbook.github.io/)

## Tentative plan
- Play around of Bevy and get familiar with thier Entity model and clock.
- Add autotroph growth mechanism.
- Settle on UI (Web or Native UI).
- Add graphing for population growth.
- Add UI for changing parameters.
- Add save and load state feature.
