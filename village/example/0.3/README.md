["@homepage": "https://werewolf.world"](https://werewolf.world)

"version": "0.3"

# Examples

## Entity list

|Entity list|JSON-LD|
---|---
|allCharacters|[https://werewolf.world/village/example/0.3/allCharacters.jsonld](https://werewolf.world/village/example/0.3/allCharacters.jsonld)|
|allRoles|[https://werewolf.world/village/example/0.3/allRoles.jsonld](https://werewolf.world/village/example/0.3/allRoles.jsonld)|

## System outline

<a href="https://werewolf.world/diagram/0.3/werewolf_system_outline.svg" target="_blank">![system outline](https://werewolf.world/diagram/0.3/werewolf_system_outline.png)</a>

## Server-to-client message examples

|Example|JSON-LD|
---|---
|firstMorning|[https://werewolf.world/village/example/0.3/server2client/firstMorning.jsonld](https://werewolf.world/village/example/0.3/server2client/firstMorning.jsonld)|
|morning|[https://werewolf.world/village/example/0.3/server2client/morning.jsonld](https://werewolf.world/village/example/0.3/server2client/morning.jsonld)|
|noonVote|[https://werewolf.world/village/example/0.3/server2client/noon.jsonld](https://werewolf.world/village/example/0.3/server2client/noon.jsonld)|
|night|[https://werewolf.world/village/example/0.3/server2client/night.jsonld](https://werewolf.world/village/example/0.3/server2client/night.jsonld)|
|result|[https://werewolf.world/village/example/0.3/server2client/result.jsonld](https://werewolf.world/village/example/0.3/server2client/result.jsonld)|
|postMortemDiscussion|[https://werewolf.world/village/example/0.3/server2client/postMortemDiscussion.jsonld](https://werewolf.world/village/example/0.3/server2client/postMortemDiscussion.jsonld)|
|myMessageOnChat|[https://werewolf.world/village/example/0.3/server2client/myMessageOnChat.jsonld](https://werewolf.world/village/example/0.3/server2client/myMessageOnChat.jsonld)|
|theirMessageOnChat|[https://werewolf.world/village/example/0.3/server2client/theirMessageOnChat.jsonld](https://werewolf.world/village/example/0.3/server2client/theirMessageOnChat.jsonld)|
|error|[https://werewolf.world/village/example/0.3/server2client/error.jsonld](https://werewolf.world/village/example/0.3/server2client/error.jsonld)|
|onymousAudienceChat|[https://werewolf.world/village/example/0.3/server2client/onymousAudienceChat.jsonld](https://werewolf.world/village/example/0.3/server2client/onymousAudienceChat.jsonld)|
|anonymousAudienceChat|[https://werewolf.world/village/example/0.3/server2client/anonymousAudienceChat.jsonld](https://werewolf.world/village/example/0.3/server2client/anonymousAudienceChat.jsonld)|


### firstMorning

* "Start day conversation phase" to "Display" and "Move to grave"

### morning

* "Start day conversation phase" to "Display" and "Move to grave"

### noon

* "Start noon vote phase" to "Display" and "Move to grave"

### night

* "Start night phase" to "Display" and "Move to grave"

### result

* "Send results" to "Display results in a modal"

### postMortemDiscussion

* "Start post-mortem discussion phase" to "Display"

### myMessageOnChat

* "Broadcast a chat message" to "Display a chat message"

### theirMessageOnChat

* "Broadcast a chat message" to "Display a chat message"

### error

* ("Server error" in server to "Output a log" in server and "Show an error message" in client)

## Client-to-server message examples

|Example|JSON-LD|
---|---
|board|[https://werewolf.world/village/example/0.3/client2server/board.jsonld](https://werewolf.world/village/example/0.3/client2server/board.jsonld)|
|chat|[https://werewolf.world/village/example/0.3/client2server/chat.jsonld](https://werewolf.world/village/example/0.3/client2server/chat.jsonld)|
|noonVote|[https://werewolf.world/village/example/0.3/client2server/noonVote.jsonld](https://werewolf.world/village/example/0.3/client2server/noonVote.jsonld)|
|nightVote|[https://werewolf.world/village/example/0.3/client2server/nightVote.jsonld](https://werewolf.world/village/example/0.3/client2server/nightVote.jsonld)|
|scroll|[https://werewolf.world/village/example/0.3/client2server/scroll.jsonld](https://werewolf.world/village/example/0.3/client2server/scroll.jsonld)|
|error|[https://werewolf.world/village/example/0.3/client2server/error.jsonld](https://werewolf.world/village/example/0.3/client2server/error.jsonld)|
|onymousAudienceBoard|[https://werewolf.world/village/example/0.3/client2server/onymousAudienceBoard.jsonld](https://werewolf.world/village/example/0.3/client2server/onymousAudienceBoard.jsonld)|
|onymousAudienceChat|[https://werewolf.world/village/example/0.3/client2server/onymousAudienceChat.jsonld](https://werewolf.world/village/example/0.3/client2server/onymousAudienceChat.jsonld)|
|onymousAudienceScroll|[https://werewolf.world/village/example/0.3/client2server/onymousAudienceScroll.jsonld](https://werewolf.world/village/example/0.3/client2server/onymousAudienceScroll.jsonld)|
|anonymousAudienceChat|[https://werewolf.world/village/example/0.3/client2server/anonymousAudienceChat.jsonld](https://werewolf.world/village/example/0.3/client2server/anonymousAudienceChat.jsonld)|

### board

* "Update prediction board" to "Output a log"

### chat

* "Send a chat message" to "Receive a chat message" in both Day Conversation Phase or Post Mortem Phase

### noonVote

* "Vote" to "Collect votes" in Noon Vote Phase

### nightVote

* "Vote" to "Collect votes" in Night Phase

### scroll

* "Scroll" to "Output a log"

### error

* ("Client error" in client to "Output a log" in server and "Show an error message" in client)

## Server-to-logger message examples

Server has to fill concrete values with an extensionalDisclosureRange key in each JSON-LD message before logging it. Also, the server has to fille concrete values with both userName key and userAvatar key in each client2server JSON-LD message before logging it.

|Example|Directionality|Values|JSON-LD|
---|---|---|---
|nightVote|client to server|blank|[https://werewolf.world/village/example/0.3/client2server/nightVote.jsonld](https://werewolf.world/village/example/0.3/client2server/nightVote.jsonld)|
|nightVoteForLog|client to server|filled|[https://werewolf.world/village/example/0.3/server2logger/nightVoteForLog.jsonld](https://werewolf.world/village/example/0.3/server2logger/nightVoteForLog.jsonld)|
|myMessageOnChat|server to client|blank|[https://werewolf.world/village/example/0.3/server2client/myMessageOnChat.jsonld](https://werewolf.world/village/example/0.3/server2client/myMessageOnChat.jsonld)|
|myMessageOnChatForLog|server to client|filled|[https://werewolf.world/village/example/0.3/server2logger/myMessageOnChatForLog.jsonld](https://werewolf.world/village/example/0.3/server2logger/myMessageOnChatForLog.jsonld)|


