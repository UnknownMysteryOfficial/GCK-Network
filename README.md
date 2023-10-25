# GCK-Network
Please note: This is a GEOPOL CREATION KIT, it is designed to act as a template for a new geopol. Therefore, it is incomplete in some aspects (dynmap, voting, ddos protection, monetization, etc.) and some details may not be to your needs. Please review every config and the luckperms permissions so that everything currently provided is acceptable to you, feel free to fork it with your changes.

Special thanks to Cendi and USS Enterprise for mythicmobs configs, gabrielito294 for structure builds, Dheyaa and Supertnt20 for models, and ArkySaw for custom planet worldpainter maps.

Credits can be found in the mortiscitations plugin config or other places throughout the project

# Basic setup
Create a folder and add the server jar (built with paper 1.18.2 in mind). 
Download github zip and unzip the project.
Add plugin config folders and server properties files to the server. Review the pluginlist text document for the links to all needed plugins and acquire said plugins. 
Download and add the earth map (linked in the maps text document) along with using worldpainter to build the custom planet maps (provided in the planets folder). 
Run a server startup script and let server unpack. Make necessary config changes and add new plugins or features at will.

# Dynmap and voting

Dynmap and voting are too personalized to include in the project, some things to note:
Consider using liveatlas (https://www.spigotmc.org/resources/liveatlas-alternative-map-ui-dynmap-squaremap-pl3xmap-overviewer.86939/) as a map addon
Disable being able to use the dynmap to chat ingame to prevent spammers, as chat filter plugins do not respond to the dynmap
Disable armor and health display on the dynmap to prevent players from being able to see vulnerabilities to eachother on the dynmap

Look up tutorials regarding dynmap for installation, should take a few days to fully render the planets and Earth.

The server is designed with missions being the source of income so for voting consider setting it so every vote but the 5th gets a mission, then on the 5th vote a vote crate is given. You can alternatively tie voting to a virtual currency and then set up a vote shop gui to buy crates and missions. In the current config default permissions have the ability to spawn random missions so disable that by setting mortismissions.random to false.

# Server protection

consider either using cloudflare or TCPshield for the server itself
https://tcpshield.com/

for the dynmap look into cloudflare and nginx:
https://www.digitalocean.com/community/tutorials/how-to-host-a-website-using-cloudflare-and-nginx-on-ubuntu-22-04

# Misc info:
Use either noobprotector or the combatlogx newbiehelper expansion for protecting new players

Mythicmobs mob removal on other planets may not work, perhaps use mob managers as well, unknown if that affects custom mob spawning on planets

gamerule reducedDebugInfo can be set to true to reduce f3 information players can get

if a player is invincible, they probably have an invincibility tag assigned to them, check your player data files and delete their file after they back up their gear.

Consider using the following texture pack (https://www.planetminecraft.com/texture-pack/earth-moon-1-19/) along with a plugin such as (https://www.spigotmc.org/resources/world-resourcepacks.18950/) in order to have the moon show up as an earth while on the moon world. alternatively can make the moon an end dimension.

Possible good tutorial for new players, recommend writing a custom book and adding it to the starter kit (essentialsx config) regarding how to play your version of the GCK.
https://youtu.be/A8DD8050SUI?list=PLvzvmyk0uI0WsLf4iyJZRhD_T2e-ANCmE&si=RnrJD51VGUeCNGfC
