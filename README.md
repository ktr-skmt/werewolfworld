# werewolfworld
werewolf.world protocol based on JSON-LD

JSON-LD 1.1
https://json-ld.org/spec/latest/json-ld/

Repository
https://github.com/ktr-skmt/werewolfworld

## IRIs for message

|IRI|Purpose|
---|---
|http://werewolf.world/resource/0.1/boardMessage|Send a prediction board update to server|
|http://werewolf.world/resource/0.1/playerMessage|Send/receive a chat message to/from server|
|http://werewolf.world/resource/0.1/systemMessage|Receive a system message from server|
|http://werewolf.world/resource/0.1/voteMessage|Send a vote to server|


## IRIs

|IRI|Type|Values|
---|---|---
|http://werewolf.world/resource/0.1/agent|||
|http://werewolf.world/resource/0.1/agentIsMine|xsd:boolean|true, false|
|http://werewolf.world/resource/0.1/agentName|||
|http://werewolf.world/resource/0.1/agentId|xsd:integer|-1 <= (-1 means master)|
|http://werewolf.world/resource/0.1/agentImage|||
|http://werewolf.world/resource/0.1/agentStatus|||
|http://werewolf.world/resource/0.1/role|||
|http://werewolf.world/resource/0.1/roleIsMine|xsd:boolean|true, false|
|http://werewolf.world/resource/0.1/roleName|||
|http://werewolf.world/resource/0.1/roleImage|||
|http://werewolf.world/resource/0.1/roleNumber|xsd:integer|0 <=, <= 7|
|http://werewolf.world/resource/0.1/result||'win', 'lose'|
|http://werewolf.world/resource/0.1/userName|||
|http://werewolf.world/resource/0.1/token|||
|http://werewolf.world/resource/0.1/phase||'{n} day conversation', '{n} day vote', '{n} day night', 'results', 'post mortem'|
|http://werewolf.world/resource/0.1/phaseTimeLimit|||
|http://werewolf.world/resource/0.1/phaseStartTime|||
|http://werewolf.world/resource/0.1/timestamp|||
|http://werewolf.world/resource/0.1/board|||
|http://werewolf.world/resource/0.1/prediction|||
|http://werewolf.world/resource/0.1/boardAgentPolarity|||
|http://werewolf.world/resource/0.1/boardAgentId|||
|http://werewolf.world/resource/0.1/boardAgentPhase|||
|http://werewolf.world/resource/0.1/chatIsMine|xsd:boolean|true, false|
|http://werewolf.world/resource/0.1/chatId|xsd:integer|1<=|
|http://werewolf.world/resource/0.1/chatCounter|xsd:integer|0<=, <=chatCounter|
|http://werewolf.world/resource/0.1/chatLimit|xsd:integer|1<=|
|http://werewolf.world/resource/0.1/chatInterval||ex. '6s'|
|http://werewolf.world/resource/0.1/chatText|||
|http://werewolf.world/resource/0.1/chatLanguage||'en', 'ja', etc. ([java.util.Locale.toString](https://docs.oracle.com/javase/9/docs/api/java/util/Locale.html#toString--))|
|http://werewolf.world/resource/0.1/chatChannel||'public', 'private', 'limited', 'master', 'grave'|
|http://werewolf.world/resource/0.1/chatIsOver|xsd:boolean|true, false|

