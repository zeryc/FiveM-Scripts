# vrp_notifypicture

Replace this with the original one in vrp\modules\player_state

or add manually , at line 54 replace this :

SetTimeout(15000,function()vRPclient.notify(player,{lang.common.welcome({tmpdata.last_login})})end)

with this :

SetTimeout(15000,function()vRPclient.notifyPicture(player,{"CHAR_ALL_PLAYERS_CONF",1, "Your server name", false,"~r~Welcome, ~g~Press K to open the ~r~menu.",lang.common.welcome({tmpdata.last_login})})end)

To change colors ~r~ for red ~g~ for green and so on. 