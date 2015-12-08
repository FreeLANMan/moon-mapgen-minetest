# moon-mapgen-minetest
Minetest mod that generates a world by default consisting of two flat discs, based on NASA LOLA spacecraft lunar terrain data. The upper disc is the nearside (flattened out), and the lower disc--far below--is the farside of the moon. (You can edit settings.conf if you want a spherical moon.)

You can control the mod by editing settings.conf before generating the world. Note that the scale (number of meters each node represents and the height-exaggeration factor) cannot be changed once the world has been generated, but you can change gravity and sky afterwards.

The mod adds two slash commands. The /where command returns the current latitude and longitude, and the /goto command lets you go to a particular location. There are two ways of using /goto:

    /goto latitude longitude

where negative is south or west, or:

    /goto name of feature

to go to a particular crater or other feature (e.g., /goto copernicus or /goto mare tranquillitatis). You don't need to list the full name if there is only one object that starts with the name, and you can omit spaces and punctuation; thus, you can go to Mare Tranquillitatis with /goto maretr.

Note that the sky textures are under a non-commercial use only license as they are generated by SpaceEngine. See the LICENSE file for more information. If you want a fully open source mod, just omit the textures and use the black sky mode.

![screenshot](../screenshots/screenshot.jpg?raw=true)