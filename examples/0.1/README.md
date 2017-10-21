
## Entity list

|Entity list|JSON-LD|
---|---
|all-agents|[http://werewolf.world/examples/0.1/all-agents.jsonld](http://werewolf.world/examples/0.1/all-agents.jsonld)|
|all-roles|[http://werewolf.world/examples/0.1/all-roles.jsonld](http://werewolf.world/examples/0.1/all-roles.jsonld)|

## System outline

![system outline](http://werewolf.world/diagram/werewolf_system_outline.png)

## Server-to-client message examples

|Example|JSON-LD|
---|---
|first_day|[http://werewolf.world/examples/0.1/server2client/first-day.jsonld](http://werewolf.world/examples/0.1/server2client/first-day.jsonld)|
|my-message-on-chat|[http://werewolf.world/examples/0.1/server2client/my-message-on-chat.jsonld](http://werewolf.world/examples/0.1/server2client/my-message-on-chat.jsonld)|
|their-message-on-chat|[http://werewolf.world/examples/0.1/server2client/their-message-on-chat.jsonld](http://werewolf.world/examples/0.1/server2client/their-message-on-chat.jsonld)|
|vote|[http://werewolf.world/examples/0.1/server2client/vote.jsonld](http://werewolf.world/examples/0.1/server2client/vote.jsonld)|
|night|[http://werewolf.world/examples/0.1/server2client/night.jsonld](http://werewolf.world/examples/0.1/server2client/night.jsonld)|
|results|[http://werewolf.world/examples/0.1/server2client/results.jsonld](http://werewolf.world/examples/0.1/server2client/results.jsonld)|
|post-mortem|[http://werewolf.world/examples/0.1/server2client/post-mortem.jsonld](http://werewolf.world/examples/0.1/server2client/post-mortem.jsonld)|
|error|[http://werewolf.world/examples/0.1/server2client/error.jsonld](http://werewolf.world/examples/0.1/server2client/error.jsonld)|

### first-day

* "Start day conversation phase" to "Display" and "Move to grave"

### my-message-on-chat

* "Broadcast a chat message" to "Display a chat message"

### their-message-on-chat

* "Broadcast a chat message" to "Display a chat message"

### vote

* "Start day vote phase" to "Display" and "Move to grave"

### night

* "Start night phase" to "Display" and "Move to grave"

### results

* "Send results" to "Display results in a modal"

### post-mortem

* "Start post mortem phase" to "Display"

## Client-to-server message examples

|Example|JSON-LD|
---|---
|board|[http://werewolf.world/examples/0.1/client2server/board.jsonld](http://werewolf.world/examples/0.1/client2server/board.jsonld)|
|chat|[http://werewolf.world/examples/0.1/client2server/chat.jsonld](http://werewolf.world/examples/0.1/client2server/chat.jsonld)|
|day-vote|[http://werewolf.world/examples/0.1/client2server/day-vote.jsonld](http://werewolf.world/examples/0.1/client2server/day-vote.jsonld)|
|night-vote|[http://werewolf.world/examples/0.1/client2server/night-vote.jsonld](http://werewolf.world/examples/0.1/client2server/night-vote.jsonld)|
|scroll|[http://werewolf.world/examples/0.1/client2server/scroll.jsonld](http://werewolf.world/examples/0.1/client2server/scroll.jsonld)|
|error|[http://werewolf.world/examples/0.1/client2server/error.jsonld](http://werewolf.world/examples/0.1/client2server/error.jsonld)|

### board

* "Update prediction board" to "Output a log"

### chat

* "Send a chat message" to "Receive a chat message" in both Day Conversation Phase or Post Mortem Phase

### day-vote

* "Vote" to "Collect votes" in Day Vote Phase

### scroll

* 

### night-vote

* "Vote" to "Collect votes" in Night Phase


