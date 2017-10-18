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
|http://werewolf.world/resource/0.1/agentIsMine|http://www.w3.org/2001/XMLSchema#boolean||
|http://werewolf.world/resource/0.1/agentName||*|
|http://werewolf.world/resource/0.1/agentId|http://www.w3.org/2001/XMLSchema#integer||
|http://werewolf.world/resource/0.1/agentImage|||
|http://werewolf.world/resource/0.1/agentStatus|||
|http://werewolf.world/resource/0.1/role|||
|http://werewolf.world/resource/0.1/roleIsMine|http://www.w3.org/2001/XMLSchema#boolean||
|http://werewolf.world/resource/0.1/roleName|||
|http://werewolf.world/resource/0.1/roleImage|||
|http://werewolf.world/resource/0.1/roleNumber|http://www.w3.org/2001/XMLSchema#integer||
|http://werewolf.world/resource/0.1/result|||
|http://werewolf.world/resource/0.1/userName|||
|http://werewolf.world/resource/0.1/token|||
|http://werewolf.world/resource/0.1/phase|||
|http://werewolf.world/resource/0.1/phaseTimeLimit|||
|http://werewolf.world/resource/0.1/phaseStartTime|||
|http://werewolf.world/resource/0.1/timestamp|||
|http://werewolf.world/resource/0.1/board|||
|http://werewolf.world/resource/0.1/prediction|||
|http://werewolf.world/resource/0.1/boardAgentPolarity|||
|http://werewolf.world/resource/0.1/boardAgentId|||
|http://werewolf.world/resource/0.1/boardAgentPhase|||
|http://werewolf.world/resource/0.1/chatIsMine|http://www.w3.org/2001/XMLSchema#boolean||
|http://werewolf.world/resource/0.1/chatId|http://www.w3.org/2001/XMLSchema#integer||
|http://werewolf.world/resource/0.1/chatCounter|http://www.w3.org/2001/XMLSchema#integer||
|http://werewolf.world/resource/0.1/chatLimit|http://www.w3.org/2001/XMLSchema#integer||
|http://werewolf.world/resource/0.1/chatInterval|||
|http://werewolf.world/resource/0.1/text|||
|http://werewolf.world/resource/0.1/language|||
|http://werewolf.world/resource/0.1/channel|||
|http://werewolf.world/resource/0.1/chatIsOver|http://www.w3.org/2001/XMLSchema#boolean||

