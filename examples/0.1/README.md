
## Entity list

|Entity list|JSON-LD|
---|---
|all agents|[http://werewolf.world/examples/0.1/all_agents.jsonld](http://werewolf.world/examples/0.1/all_agents.jsonld)|
|all roles|[http://werewolf.world/examples/0.1/all_roles.jsonld](http://werewolf.world/examples/0.1/all_roles.jsonld)|

## System outline

![system outline](http://werewolf.world/werewolf_system_outline.png)

## Server-to-client message examples

|Example|JSON-LD|
---|---
|first_day|[http://werewolf.world/examples/0.1/server2client/first_day.jsonld](http://werewolf.world/examples/0.1/server2client/first_day.jsonld)|
|my_message_on_chat|[http://werewolf.world/examples/0.1/server2client/my_message_on_chat.jsonld](http://werewolf.world/examples/0.1/server2client/my_message_on_chat.jsonld)|
|their_message_on_chat|[http://werewolf.world/examples/0.1/server2client/their_message_on_chat.jsonld](http://werewolf.world/examples/0.1/server2client/their_message_on_chat.jsonld)|
|vote|[http://werewolf.world/examples/0.1/server2client/vote.jsonld](http://werewolf.world/examples/0.1/server2client/vote.jsonld)|
|night|[http://werewolf.world/examples/0.1/server2client/night.jsonld](http://werewolf.world/examples/0.1/server2client/night.jsonld)|
|results|[http://werewolf.world/examples/0.1/server2client/results.jsonld](http://werewolf.world/examples/0.1/server2client/results.jsonld)|
|postMortem|[http://werewolf.world/examples/0.1/server2client/postMortem.jsonld](http://werewolf.world/examples/0.1/server2client/postMortem.jsonld)|

### first_day

* "Start day conversation phase" to "Display" and "Move to grave"

### my_message_on_chat

* "Broadcast a chat message" to "Display a chat message"

### their_message_on_chat

* "Broadcast a chat message" to "Display a chat message"

### vote

* "Start day vote phase" to "Display" and "Move to grave"

### night

* "Start night phase" to "Display" and "Move to grave"

### results

* "Send results" to "Display results in a modal"

### postMortem

* "Start post mortem phase" to "Display"

## Client-to-server message examples

|Example|JSON-LD|
---|---
|board|[http://werewolf.world/examples/0.1/client2server/board.jsonld](http://werewolf.world/examples/0.1/client2server/board.jsonld)|
|chat|[http://werewolf.world/examples/0.1/client2server/chat.jsonld](http://werewolf.world/examples/0.1/client2server/chat.jsonld)|
|day_vote|[http://werewolf.world/examples/0.1/client2server/day_vote.jsonld](http://werewolf.world/examples/0.1/client2server/day_vote.jsonld)|
|night_vote|[http://werewolf.world/examples/0.1/client2server/night_vote.jsonld](http://werewolf.world/examples/0.1/client2server/night_vote.jsonld)|

### board

* "Update prediction board" to "Output a log"

### chat

* "Send a chat message" to "Receive a chat message" in both Day Conversation Phase or Post Mortem Phase

### day_vote

* "Vote" to "Collect votes" in Day Vote Phase

### night_vote

* "Vote" to "Collect votes" in Night Phase


