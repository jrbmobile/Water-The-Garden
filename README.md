# Water-The-Garden
Outlet and switch sprinkler valve controller, reads PlantLink humidity and turns on a switch to open the valve and water your garden. SmartApp includes Dark Sky API to check if rain is coming and will override the watering cycle if desired. SmartApp executes on sensor events, which PlantLink reports usually every 15 minutes. If a watering cycle is running for a period longer than the reporting period, new events are ignored until the first cycle is complete. If an event is intercepted (failsafe) and the command is to turn off the valve as moisture is above selected value, pending events are cancelled and the valve is turned off immediately.

My setup is currently using a GE Z Wave Outdoor Outlet, and Orbit Sprinkler Valve attached to a 24vac HVAC transformer mounted in a water proof housing.

Future improvements are to add water valve device types and "water between" time selection.
