
version: 0.1

|   |contexts|
---|---
|agent|http://werewolf.world/contexts/0.1/agent.jsonld|
|base|http://werewolf.world/contexts/0.1/base.jsonld|
|board|http://werewolf.world/contexts/0.1/board.jsonld|
|chat|http://werewolf.world/contexts/0.1/chat.jsonld|
|role|http://werewolf.world/contexts/0.1/role.jsonld|
|vote|http://werewolf.world/contexts/0.1/vote.jsonld|

## agent


## base


## board


## chat


## role


## vote


"status": "http://werewolf.world/resource/0.1/agentStatus",//alive, dead, unnatural death, death by execution, death by werewolf attack, death by fear

"boardPrediction": "http://werewolf.world/resource/0.1/prediction"//?, Δ, O, X

"channel": "http://werewolf.world/resource/0.1/channel",//public, private, master, grave, werewolf,
"isOver": "http://werewolf.world/resource/0.1/chatIsOver"//true or false

"boardAgentPolarity": "http://werewolf.world/resource/0.1/boardAgentPolarity",//"positive" or "negative"

"vote": {
			"@id": "http://werewolf.world/resource/vote",
			"@type": "xsd:interger"//agent id
},
