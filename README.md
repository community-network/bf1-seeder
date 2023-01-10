# Gametools Autoseeding

#### Part of our cloud server manager https://manager.gametools.network/


Battlefield 1 and 4 Autoseeding app is made to improve starting of community servers.
It automaticly joins the requested server selected in the panel via the game client.
in order for it to work, you will need multiple pc's/people that run the script which you can control with a global command.
It supports both ea desktop and origin (if you somehow still manage to still origin...)

### Example of the config.txt file:
```py
# it will autogenerate one of these files when you run the script and it doesn't exist already.
# But without filling in your group_id it won't work!

# The unique identifier of your group: "https://manager.gametools.network/group/{group_id}"
group_id = ''
# where the shortcut of your game goes to to launch the game. If your didnt change when setting up the game, the defaults will be fine.
# bf4 example location: 'C:\Program Files\Origin Games\Battlefield 4\BFLauncher_x86.exe'
game_location = 'C:\Program Files (x86)\Origin Games\Battlefield 1\bf1.exe'
# what your pc will be called within the group 
hostname = 'seeder-1'
# Allow the script to shutdown your pc when asked from the panel (administrator rights needed)
allow_shutdown = false
# When you disable this option, the game will use less resources but renders nothing (doesn't change your ingame settings, only affects the script)
usable_client = true
# allow automated messages in chat (further settings below)
send_messages = false
# if disabled, anti-afk won't work when in fullscreen (some people play with the script still running, this stops the script from minimizing the game when fullscreen is detected)
fullscreen_anti_afk = true
# use ea desktop
use_ea_desktop = true

# what message has to be send to the server with automated messages. if you want multiple messages, seperate them with ";"
message = 'Join our discord, we are recruiting: discord.gg/...'
# in which server
message_server_name = ''
# start time
message_start_time_utc = '12:00'
# when to stop
message_stop_time_utc = '23:00'
# how many minutes between messages
message_timeout_mins = 8
# Which game you want to use the script for (Bf1 or Bf4) (dont forget the Capital B in the game name)
game = 'Bf1'
```