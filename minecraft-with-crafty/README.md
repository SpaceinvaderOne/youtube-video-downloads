# Minecraft on Unraid with Crafty

The Unraid Harbour Adventure world from [my video about setting up Minecraft with Crafty on Unraid](https://youtu.be/YFiJ3DsiF68), made for the official Uncast channel.

[Read the written guide: Set up a Minecraft Server on Unraid with Crafty 4](https://gist.github.com/SpaceinvaderOne/28bd93bfe0f31bb6acc4a8e2e8df780a)

This world is just a bit of fun. I made it for the video to show how you can upload a world into Crafty, and thought an Unraid themed town would be a fun way to do it.

I've hardly played Minecraft myself, so expect rough edges and things that don't quite work. Have a wander around, look at the buildings and try the little puzzles if you fancy it. I'm sharing it as it is, and I'm not planning to maintain it or fix the puzzles and other bits that might be broken.

## Download the world

[Download Unraid Harbour Adventure](https://github.com/SpaceinvaderOne/youtube-video-downloads/raw/refs/heads/main/minecraft-with-crafty/unraid-harbour-adventure.zip)

This world needs Minecraft Java Edition 26.3 and a matching server version. It includes the datapack that runs the puzzles. No extra plugins or client mods are needed.

The download contains the world only. Create your Java server in Crafty first, as shown in the video. Bedrock compatibility hasn't been tested.

## Load it into Crafty

Back up your existing world first.

1. Stop the Minecraft server inside Crafty and wait for it to finish. Leave the Crafty container running.
2. Open **Files** and create a folder called `unraid-harbour-adventure` beside `server.properties`.
3. Open that folder, upload the downloaded ZIP and choose **Unzip**. The file `level.dat` should be directly inside the folder you've just created.
4. Go back to the server's main folder and edit `server.properties`. Change the existing matching settings to these values.

   ```properties
   level-name=unraid-harbour-adventure
   gamemode=adventure
   difficulty=peaceful
   spawn-protection=0
   ```

5. Save the changes and start the Minecraft server. Paper may pause for about 30 seconds while converting the world storage on its first start. Wait for the server to finish starting before joining.
6. Join from Minecraft Java's **Multiplayer** menu using your server's address. Keep your whitelist enabled and add the players you want to allow.

The folder name and `level-name` must match exactly. Adventure mode lets players use buttons without breaking the scenery. If you've already joined this server in another game mode, change your player to Adventure in Crafty's **Terminal**, replacing the name below with your Minecraft username.

```text
gamemode adventure YourMinecraftUsername
```

## Exploring and playing

Right-click the small grey buttons to use them. The coloured blocks above them are markers.

At the welcome plaza, the button below the orange marker starts the shared mission and gives you a field guide. Select the book in your hotbar and right-click to read it. The blue marked board gives you another copy.

You can complete the challenges in any order. The guide explains where to find each one, and whenever you finish a task the chat messages show what still needs doing so you can choose where to head next.

[Back to all video downloads](../)
