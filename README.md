# CSGO HUD GameState Integration
For official steam API's refer [Here](https://developer.valvesoftware.com/wiki/Counter-Strike:_Global_Offensive_Game_State_Integration).
## Install 

* If you have GIT, you can use `git clone https://github.com/ashtam55/csgo-game-integration.git` to download the project. Otherwise, Click the Download Zip button above
* Install Node.JS (NPM is included)
* Create a file named `gamestate_integration_hud.cfg` in your csgo cfg folder (`steamapps/common/Counter-Strike Global Offensive/csgo/cfg/`) and copy-paste this code :
```
"CSGO HUD"
{
 "uri" "http://127.0.0.1:3000"
 "timeout" "5.0"
 "buffer"  "0.1"
 "throttle" "0.1"
 "heartbeat" "60.0"
 "data"
 {
   "provider"            "1"
   "map"                 "1"
   "round"               "1"
   "player_id"           "1"
   "player_state"        "1"
   "player_weapons"      "1"
   "player_match_stats"  "1"
   "allplayers_match_stats"  "1"
 }
}
```
* in CMD: `npm install`
* in CMD: `node server.js`
* You should then be able to connect in a web browser by going to `http://localhost:2626`. Start up your game and connect to a match and data should begin streaming
* Linux and Mac setup is basically identical, just switch out CMD for Terminal

### TO DO:
* Support with IoT devices.
* Cloud connect.




