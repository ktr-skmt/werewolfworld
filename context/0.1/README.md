["@homepage": "https://werewolf.world"](https://werewolf.world)

"version": "0.1"

# Contexts

|Contexts|JSON-LD|
---|---
|base|[https://werewolf.world/context/0.1/base.jsonld](https://werewolf.world/context/0.1/base.jsonld)|
|error|[https://werewolf.world/context/0.1/error.jsonld](https://werewolf.world/context/0.1/error.jsonld)|
|agent|[https://werewolf.world/context/0.1/agent.jsonld](https://werewolf.world/context/0.1/agent.jsonld)|
|role|[https://werewolf.world/context/0.1/role.jsonld](https://werewolf.world/context/0.1/role.jsonld)|
|board|[https://werewolf.world/context/0.1/board.jsonld](https://werewolf.world/context/0.1/board.jsonld)|
|chat|[https://werewolf.world/context/0.1/chat.jsonld](https://werewolf.world/context/0.1/chat.jsonld)|
|vote|[https://werewolf.world/context/0.1/vote.jsonld](https://werewolf.world/context/0.1/vote.jsonld)|
|votingResults|[https://werewolf.world/context/0.1/votingResults.jsonld](https://werewolf.world/context/0.1/votingResults.jsonld)|
|scroll|[https://werewolf.world/context/0.1/scroll.jsonld](https://werewolf.world/context/0.1/scroll.jsonld)|

# IRIs

## message

|IRI|Purpose|
---|---
|https://werewolf.world/resource/0.1/boardMessage|Send a prediction board update to server|
|https://werewolf.world/resource/0.1/errorMessage|Send/Receive an error message to/from server|
|https://werewolf.world/resource/0.1/playerMessage|Send/receive a chat message to/from server|
|https://werewolf.world/resource/0.1/scrollMessage|Send a scroll information to server|
|https://werewolf.world/resource/0.1/systemMessage|Receive a system message from server|
|https://werewolf.world/resource/0.1/voteMessage|Send a vote to server|

## base

|IRI|Type|Values|
---|---|---
|https://werewolf.world/resource/0.1/token||(GUID)|
|https://werewolf.world/resource/0.1/villageId|xsd:integer|0 <=|
|https://werewolf.world/resource/0.1/villageName||5 <= {# of Unicode code points} <= 30|
|https://werewolf.world/resource/0.1/phase||'day conversation', 'day vote', 'night', 'results', 'post mortem'|
|https://werewolf.world/resource/0.1/date|xsd:integer|-1 <=, 0 when phase were post mortem, -1 when phase were results|
|https://werewolf.world/resource/0.1/phaseTimeLimit||'none' or such as '10m', '3m'|
|https://werewolf.world/resource/0.1/phaseStartTime|xsd:dateTime|such as '2006-10-07T12:06:56.568+09:00'|
|https://werewolf.world/resource/0.1/serverTimestamp|xsd:dateTime|such as '2006-10-07T12:06:56.568+09:00'|
|https://werewolf.world/resource/0.1/clientTimestamp|xsd:dateTime|such as '2006-10-07T12:06:56.568+09:00'|
|https://werewolf.world/resource/0.1/directionality||'server to client' or 'client to server'|
|https://werewolf.world/resource/0.1/channel||'public', 'private', 'werewolf', 'master', 'grave', 'onymousAudience', 'anonymousAudience'|


## error

|IRI|Type|Values|
---|---|---
|https://werewolf.world/resource/0.1/errorContent|||
|https://werewolf.world/resource/0.1/severity||'error', 'warning'|
|https://werewolf.world/resource/0.1/source||(JSON-LD)|

## agent

|IRI|Type|Values|
---|---|---
|https://werewolf.world/resource/0.1/agent|||
|https://werewolf.world/resource/0.1/agentId|xsd:integer|-1 <= (-1 means master)|
|https://werewolf.world/resource/0.1/agentIsMine|xsd:boolean|true, false|
|https://werewolf.world/resource/0.1/agentName||[https://werewolf.world/image/0.1/#agent](https://werewolf.world/image/0.1/#agent)|
|https://werewolf.world/resource/0.1/agentImage||[https://werewolf.world/image/0.1/#agent](https://werewolf.world/image/0.1/#agent)|
|https://werewolf.world/resource/0.1/agentStatus||'alive', 'dead', 'death by execution', 'death by werewolf attack', 'death by fear', 'unnatural death'|

See [https://werewolf.world/image/0.1/#agent](https://werewolf.world/image/0.1/#agent)

## role

|IRI|Type|Values|
---|---|---
|https://werewolf.world/resource/0.1/role|||
|https://werewolf.world/resource/0.1/roleIsMine|xsd:boolean|true, false|
|https://werewolf.world/resource/0.1/roleName||[https://werewolf.world/image/0.1/#role](https://werewolf.world/image/0.1/#role)|
|https://werewolf.world/resource/0.1/roleImage||[https://werewolf.world/image/0.1/#role](https://werewolf.world/image/0.1/#role)|
|https://werewolf.world/resource/0.1/roleNumber|xsd:integer|0 <=, <= 7|

See [https://werewolf.world/image/0.1/#role](https://werewolf.world/image/0.1/#role)

## board

|IRI|Type|Values|
---|---|---
|https://werewolf.world/resource/0.1/board|||
|https://werewolf.world/resource/0.1/boardPolarity||'positive', 'negative'|
|https://werewolf.world/resource/0.1/boardPrediction||'?','Δ','O','X'|

## chat

|IRI|Type|Values|
---|---|---
|https://werewolf.world/resource/0.1/chatIsMine|xsd:boolean|true, false|
|https://werewolf.world/resource/0.1/chatId|xsd:integer|1 <=|
|https://werewolf.world/resource/0.1/chatCounter|xsd:integer|0<=, <=chatCounter|
|https://werewolf.world/resource/0.1/chatLimit|xsd:integer|1 <=|
|https://werewolf.world/resource/0.1/chatInterval||such as '5s'|
|https://werewolf.world/resource/0.1/chatText||string such as 0 <= {# of Unicode code points} <= {chatCharacterLimit}|
|https://werewolf.world/resource/0.1/chatCharacterLimit|xsd:integer|1 <= {# of Unicode code points}|
|https://werewolf.world/resource/0.1/chatLanguage||'en', 'ja', etc. ([java.util.Locale.toString](https://docs.oracle.com/javase/9/docs/api/java/util/Locale.html#toString--))|
|https://werewolf.world/resource/0.1/chatIsOver|xsd:boolean|true, false|

## votingResults

|IRI|Type|Values|
---|---|---
|https://werewolf.world/resource/0.1/votingResultsSummary|||
|https://werewolf.world/resource/0.1/numberOfVotes|xsd:integer|0 <=, <= {number of alive agents except a master}|
|https://werewolf.world/resource/0.1/rankOfVotes|xsd:integer|1 <=, 1 is the highest. "1224" ranking.|
|https://werewolf.world/resource/0.1/votingResultsDetails|||

## result

|IRI|Type|Values|
---|---|---
|https://werewolf.world/resource/0.1/result||'win', 'lose'|
|https://werewolf.world/resource/0.1/userName||5 <= {# of Unicode code points} <= 15|
|https://werewolf.world/resource/0.1/userAvatar||(URL)|

## scroll

|IRI|Type|Values|
---|---|---
|https://werewolf.world/resource/0.1/nodeId|||
|https://werewolf.world/resource/0.1/scrollTop|xsd:integer||
|https://werewolf.world/resource/0.1/scrollHeight|xsd:integer||
|https://werewolf.world/resource/0.1/offsetHeight|xsd:integer||
