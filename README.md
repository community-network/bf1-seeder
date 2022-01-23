# Gametools Autoseeding

#### Part of our cloud server manager https://manager.gametools.network/


Battlefield One Autoseeding app design to improve starting of community servers. 
Automaticly join server to quickly populate it. 

### Example of the config.txt file:
```py
# it will autogenerate one of these files when you run the script and it doesn't exist already.
# But without filling in your group_id it won't work!

# The unique identifier of your group: "https://manager.gametools.network/group/{group_id}"
group_id = ''
# where the shortcut of your game goes to to launch the game. If your didnt change when setting up the game, the defaults will be fine.
game_location = 'C:\Program Files (x86)\Origin Games\Battlefield 1\bf1.exe'
# what your pc will be called within the group 
hostname = 'seeder-1'
# Allow the script to shutdown your pc when asked from the panel
allow_shutdown = false
# automated messages in chat when not seeding (further settings below)
send_messages = false
# if disabled, anti-afk won't work when in fullscreen (so you dont have to close the script before playing)
fullscreen_anti_afk = true

# what message has to be send to the server with automated messages
message = 'Join our discord, we are recruiting: discord.gg/...'
# in which server
message_server_name = ''
# start time
message_start_time_utc = '12:00'
# when to stop
message_stop_time_utc = '23:00'
# how many minutes between messages
message_timeout_mins = 8
```