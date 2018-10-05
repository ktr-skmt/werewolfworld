["@lobby": "https://werewolf.world/lobby"](https://werewolf.world/lobby)

"version": "0.2"

# Lobby Examples

## List

### Client to Server

1. [buildVillage.json](https://werewolf.world/lobby/example/0.2/client2server/buildVillage.json)
1. enterLobby.json
    1. [enterLobbyForAnonymousAudience.json](https://werewolf.world/lobby/example/0.2/client2server/enterLobbyForAnonymousAudience.json)
    1. [enterLobbyForHumanPlayer.json](https://werewolf.world/lobby/example/0.2/client2server/enterLobbyForHumanPlayer.json)
    1. [enterLobbyForOnymousAudience.json](https://werewolf.world/lobby/example/0.2/client2server/enterLobbyForOnymousAudience.json)
    1. [enterLobbyForRobotPlayer.json](https://werewolf.world/lobby/example/0.2/client2server/enterLobbyForRobotPlayer.json)
1. [getAvatar.json](https://werewolf.world/lobby/example/0.2/client2server/getAvatar.json)
1. [kickOutPlayer.json](https://werewolf.world/lobby/example/0.2/client2server/kickOutPlayer.json)
1. [leaveWaitingPage.json](https://werewolf.world/lobby/example/0.2/client2server/leaveWaitingPage.json)
1. [pong.json](https://werewolf.world/lobby/example/0.2/client2server/pong.json)
1. selectVillage.json
    1. [selectVillageForHumanPlayer.json](https://werewolf.world/lobby/example/0.2/client2server/selectVillageForHumanPlayer.json)
1. [advancedSearch.json](https://werewolf.world/lobby/example/0.2/client2server/advancedSearch.json)
1. [idSearch.json](https://werewolf.world/lobby/example/0.2/client2server/idSearch.json)
1. [play.json](https://werewolf.world/lobby/example/0.2/client2server/play.json)
1. [ready.json](https://werewolf.world/lobby/example/0.2/client2server/ready.json)
1. [getSettings.json](https://werewolf.world/lobby/example/0.2/client2server/getSettings.json)
1. [changeUserName.json](https://werewolf.world/lobby/example/0.2/client2server/changeUserName.json)
1. [changeUserEmail.json](https://werewolf.world/lobby/example/0.2/client2server/changeUserEmail.json)
1. [changeUserPassword.json](https://werewolf.world/lobby/example/0.2/client2server/changeUserPassword.json)
1. [changeLang.json](https://werewolf.world/lobby/example/0.2/client2server/changeLang.json)

### Server to Client

1. [avatar.json](https://werewolf.world/lobby/example/0.2/server2client/avatar.json)
1. lobby.json
    1. [lobbyForHumanPlayer.json](https://werewolf.world/lobby/example/0.2/server2client/lobbyForHumanPlayer.json)
1. [ping.json](https://werewolf.world/lobby/example/0.2/server2client/ping.json)
1. waitingPage.json
    1. [waitingPageForHumanPlayer.json](https://werewolf.world/lobby/example/0.2/server2client/waitingPageForHumanPlayer.json)
1. [searchResult.json](https://werewolf.world/lobby/example/0.2/server2client/searchResult.json)
1. [played.json](https://werewolf.world/lobby/example/0.2/server2client/played.json)
1. [settings.json](https://werewolf.world/lobby/example/0.2/server2client/settings.json)

## Flow

### Guest Human Player

1. main page (From AuthController)
1. (client to server) select a village list; [enterLobbyForHumanPlayer.json](https://werewolf.world/lobby/example/0.2/client2server/enterLobbyForHumanPlayer.json)
1. (server to client) go to a page of a village list; [lobbyForHumanPlayer.json](https://werewolf.world/lobby/example/0.2/server2client/lobbyForHumanPlayer.json)
1. (client to server) get avatar info; [getAvatar.json](https://werewolf.world/lobby/example/0.2/client2server/getAvatar.json)
1. (server to client) send avatar info; [avatar.json](https://werewolf.world/lobby/example/0.2/server2client/avatar.json)
1. (client to server) select a village; [selectVillageForHumanPlayer.json](https://werewolf.world/lobby/example/0.2/client2server/selectVillageForHumanPlayer.json)
1. (server to client) go to a waiting page; [waitingPageForHumanPlayer.json](https://werewolf.world/lobby/example/0.2/server2client/waitingPageForHumanPlayer.json)
1. (server to client) ping [ping.json](https://werewolf.world/lobby/example/0.2/server2client/ping.json)
1. (client to server) pong [pong.json](https://werewolf.world/lobby/example/0.2/client2server/pong.json)
1. a host player pushes a start button (To GameController)
1. (client to server) start a game [play.json](https://werewolf.world/lobby/example/0.2/client2server/play.json)
1. (server to client) [played.json](https://werewolf.world/lobby/example/0.2/server2client/played.json)
1. move from /lobby to /village
1. (client to server) [ready.json](https://werewolf.world/lobby/example/0.2/client2server/ready.json)

(client to server) leave a waiting page [leaveWaitingPage.json](https://werewolf.world/lobby/example/0.2/client2server/leaveWaitingPage.json)

### Host Human Player

1. main page (From AuthController)
1. (client to server) select a village list; [enterLobbyForHumanPlayer.json](https://werewolf.world/lobby/example/0.2/client2server/enterLobbyForHumanPlayer.json)
1. (server to client) go to a page of a village list; [lobbyForHumanPlayer.json](https://werewolf.world/lobby/example/0.2/server2client/lobbyForHumanPlayer.json)
1. (client to server) get avatar info; [getAvatar.json](https://werewolf.world/lobby/example/0.2/client2server/getAvatar.json)
1. (server to client) send avatar info; [avatar.json](https://werewolf.world/lobby/example/0.2/server2client/avatar.json)
1. (client) push a button for building a village
1. (client) go to a page for building a village
1. (client to server) build a village; [buildVillage.json](https://werewolf.world/lobby/example/0.2/client2server/buildVillage.json)
1. (server to client) go to a waiting page; [waitingPageForHumanPlayer.json](https://werewolf.world/lobby/example/0.2/server2client/waitingPageForHumanPlayer.json)
1. (server to client) ping [ping.json](https://werewolf.world/lobby/example/0.2/server2client/ping.json)
1. (client to server) pong [pong.json](https://werewolf.world/lobby/example/0.2/client2server/pong.json)
1. a host player pushes a start button (To GameController)
1. (server to client) [played.json](https://werewolf.world/lobby/example/0.2/server2client/played.json)
1. move from /lobby to /village
1. (client to server) [ready.json](https://werewolf.world/lobby/example/0.2/client2server/ready.json)

(client to server) leave a waiting page [leaveWaitingPage.json](https://werewolf.world/lobby/example/0.2/client2server/leaveWaitingPage.json)  
Then, a host of a waiting page is selected from remaining players if they exist.

(client to server) kick out a player [kickOutPlayer.json](https://werewolf.world/lobby/example/0.2/client2server/kickOutPlayer.json)  
The kicked out player moves to a lobby with an error message that a host kicked out the player

### Settings
1. settings page (From main page)
1. (client to server) get settings info; [getSettings.json](https://werewolf.world/lobby/example/0.2/client2server/getSettings.json)
1. (server to client) send settings info; [settings.json](https://werewolf.world/lobby/example/0.2/server2client/settings.json)
1. change settings info:
    1. (client to server) change user's name; [changeUserName.json](https://werewolf.world/lobby/example/0.2/client2server/changeUserName.json)
    1. (client to server) change user's email address; [changeUserEmail.json](https://werewolf.world/lobby/example/0.2/client2server/changeUserName.json)
    1. (client to server) change user's password; [changeUserPassword.json](https://werewolf.world/lobby/example/0.2/client2server/changeUserPassword.json)
    1. (client to server) change locale; [changeLang.json](https://werewolf.world/lobby/example/0.2/client2server/changeLang.json)
1. (server to client) send settings info; [settings.json](https://werewolf.world/lobby/example/0.2/server2client/settings.json)
1. leave settings page (To main page)
