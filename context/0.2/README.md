["@homepage": "https://werewolf.world"](https://werewolf.world)

"version": "0.2"

# Contexts

|Contexts|JSON-LD|
---|---
|base|[https://werewolf.world/context/0.2/base.jsonld](https://werewolf.world/context/0.2/base.jsonld)|
|error|[https://werewolf.world/context/0.2/error.jsonld](https://werewolf.world/context/0.2/error.jsonld)|
|agent|[https://werewolf.world/context/0.2/agent.jsonld](https://werewolf.world/context/0.2/agent.jsonld)|
|role|[https://werewolf.world/context/0.2/role.jsonld](https://werewolf.world/context/0.2/role.jsonld)|
|board|[https://werewolf.world/context/0.2/board.jsonld](https://werewolf.world/context/0.2/board.jsonld)|
|chat|[https://werewolf.world/context/0.2/chat.jsonld](https://werewolf.world/context/0.2/chat.jsonld)|
|vote|[https://werewolf.world/context/0.2/vote.jsonld](https://werewolf.world/context/0.2/vote.jsonld)|
|votingResult|[https://werewolf.world/context/0.2/votingResult.jsonld](https://werewolf.world/context/0.2/votingResults.jsonld)|
|scroll|[https://werewolf.world/context/0.2/scroll.jsonld](https://werewolf.world/context/0.2/scroll.jsonld)|

# IRIs

## message

|IRI|Purpose|
---|---
|https://werewolf.world/resource/0.2/boardMessage|Send a prediction board update to server|
|https://werewolf.world/resource/0.2/errorMessage|Send/Receive an error message to/from server|
|https://werewolf.world/resource/0.2/playerMessage|Send/receive a chat message to/from server|
|https://werewolf.world/resource/0.2/scrollMessage|Send a scroll information to server|
|https://werewolf.world/resource/0.2/systemMessage|Receive a system message from server|
|https://werewolf.world/resource/0.2/voteMessage|Send a vote to server|

## base

|IRI|Type|Values|
---|---|---
|https://werewolf.world/resource/0.2/token||"[0-9A-Fa-f]{8}-[0-9A-Fa-f]{4}-[0-9A-Fa-f]{4}-[0-9A-Fa-f]{4}-[0-9A-Fa-f]{12}"(GUID)|
|https://werewolf.world/resource/0.2/villageId|xsd:integer|0 <=|
|https://werewolf.world/resource/0.2/villageName||5 <= {# of Unicode code points} <= 30|
|https://werewolf.world/resource/0.2/totalNumberOfAgents|xsd:integer|4 <=|
|https://werewolf.world/resource/0.2/phase||'morning', 'day', 'night', 'result', 'post mortem'|
|https://werewolf.world/resource/0.2/date|xsd:integer|-1 <=, 0 when phase were post mortem, -1 when phase were result|
|https://werewolf.world/resource/0.2/phaseTimeLimit|xsd:integer|if nothing, -1. otherwise, how many seconds|
|https://werewolf.world/resource/0.2/phaseStartTime|xsd:dateTime|such as '2006-10-07T12:06:56.568+09:00'|
|https://werewolf.world/resource/0.2/serverTimestamp|xsd:dateTime|such as '2006-10-07T12:06:56.568+09:00'|
|https://werewolf.world/resource/0.2/clientTimestamp|xsd:dateTime|such as '2006-10-07T12:06:56.568+09:00'|
|https://werewolf.world/resource/0.2/directionality||'server to client' or 'client to server'|
|https://werewolf.world/resource/0.2/channel||'public', 'private', 'werewolf', 'seer', 'hunter', 'master', 'grave', 'onymousAudience', 'anonymousAudience'|


## error

|IRI|Type|Values|
---|---|---
|https://werewolf.world/resource/0.2/errorContent|||
|https://werewolf.world/resource/0.2/severity||'error', 'warning'|
|https://werewolf.world/resource/0.2/source||(JSON-LD)|

## agent

|IRI|Type|Values|
---|---|---
|https://werewolf.world/resource/0.2/agent|||
|https://werewolf.world/resource/0.2/agentId|xsd:integer|-1 <= (-1 means master)|
|https://werewolf.world/resource/0.2/agentIsMine|xsd:boolean|true, false|
|https://werewolf.world/resource/0.2/agentName||[https://werewolf.world/image/0.2/#agent](https://werewolf.world/image/0.2/#agent)|
|https://werewolf.world/resource/0.2/agentImage||[https://werewolf.world/image/0.2/#agent](https://werewolf.world/image/0.2/#agent)|
|https://werewolf.world/resource/0.2/agentStatus||'alive', 'dead', 'death by execution', 'death by werewolf attack', 'death by fear', 'unnatural death'|
|https://werewolf.world/resource/0.2/agentIsAChoice|xsd:boolean||

See [https://werewolf.world/image/0.2/#agent](https://werewolf.world/image/0.2/#agent)

## role

|IRI|Type|Values|
---|---|---
|https://werewolf.world/resource/0.2/role|||
|https://werewolf.world/resource/0.2/roleIsMine|xsd:boolean|true, false|
|https://werewolf.world/resource/0.2/roleName||[https://werewolf.world/image/0.2/#role](https://werewolf.world/image/0.2/#role)|
|https://werewolf.world/resource/0.2/roleImage||[https://werewolf.world/image/0.2/#role](https://werewolf.world/image/0.2/#role)|
|https://werewolf.world/resource/0.2/numberOfAgentsWhoPlayTheRole|xsd:integer|0 <=, <= 7|

See [https://werewolf.world/image/0.2/#role](https://werewolf.world/image/0.2/#role)

## board

|IRI|Type|Values|
---|---|---
|https://werewolf.world/resource/0.2/board|||
|https://werewolf.world/resource/0.2/boardPolarity||'positive', 'negative'|
|https://werewolf.world/resource/0.2/boardPrediction||'?','Δ','O','X'|

## chat

|IRI|Type|Values|
---|---|---
|https://werewolf.world/resource/0.2/chatIsMine|xsd:boolean|true, false|
|https://werewolf.world/resource/0.2/chatId|xsd:integer|1 <=|
|https://werewolf.world/resource/0.2/chatCounter|xsd:integer|0<=, <=chatLimit|
|https://werewolf.world/resource/0.2/chatLimit|xsd:integer|1 <=|
|https://werewolf.world/resource/0.2/chatInterval||such as '5s'|
|https://werewolf.world/resource/0.2/chatText||string such as 0 <= {# of Unicode code points} <= {chatCharacterLimit}|
|https://werewolf.world/resource/0.2/chatCharacterLimit|xsd:integer|1 <= {# of Unicode code points}|
|https://werewolf.world/resource/0.2/chatLanguage||'en', 'ja', etc. ([java.util.Locale.toString](https://docs.oracle.com/javase/9/docs/api/java/util/Locale.html#toString--))|
|https://werewolf.world/resource/0.2/chatIsOver|xsd:boolean|true, false|

## votingResult

|IRI|Type|Values|
---|---|---
|https://werewolf.world/resource/0.2/votingResultsSummary|||
|https://werewolf.world/resource/0.2/numberOfVotes|xsd:integer|0 <=, <= {number of alive agents except a master}|
|https://werewolf.world/resource/0.2/rankOfVotes|xsd:integer|1 <=, 1 is the highest. "1224" ranking.|
|https://werewolf.world/resource/0.2/votingResultsDetails|||

## result

|IRI|Type|Values|
---|---|---
|https://werewolf.world/resource/0.2/result||'win', 'lose'|
|https://werewolf.world/resource/0.2/userName||5 <= {# of Unicode code points} <= 15|
|https://werewolf.world/resource/0.2/userAvatar||(URL)|

## scroll

|IRI|Type|Values|
---|---|---
|https://werewolf.world/resource/0.2/nodeId|||
|https://werewolf.world/resource/0.2/scrollTop|xsd:integer||
|https://werewolf.world/resource/0.2/scrollHeight|xsd:integer||
|https://werewolf.world/resource/0.2/offsetHeight|xsd:integer||
