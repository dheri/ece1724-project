# Ecological Simulator
## Motivation

Have you played Factorio and looked at your production graphs and wished if there was a game just to look at the graphs about how resource consumption works? This project aims to simulate an ecosystem and show results stats on population growths and resource consumption.

## Objective and key features
- Game starts a world with parameters of area and solar density.
- Able to simulate growth of autotrophs based on solar energy and time, and heterotrophs based on autotrophs and time.
- Will be homogenous, no localization of resources, plants or animals.
- Track time series data on poulation growths and resource consumption.
- Expose time series data either via rust native UI or via simple web server exposing data via web sockets.
- Ability to save and load back simulation state. (only the current state will be saved and past time series data will be lost)
- A (CLI or UI or Web) interface to change conditions on the fly.
- Try to use Bevy as game engine if possible. [This is a good resource](https://bevy-cheatbook.github.io/)

## Tentative plan
- Play around of Bevy.
- Add autotroph growth mechanism.
- Settle on UI (Web or Native UI).
- Add graphing for population growth.
- Add UI for changing parameters.
- Add save and load state feature.
