["@homepage": "https://werewolf.world"](https://werewolf.world)

"version": "0.3"

# Contexts

|Contexts|JSON-LD|
---|---
|base|[https://werewolf.world/village/context/0.3/base.jsonld](https://werewolf.world/village/context/0.3/base.jsonld)|
|error|[https://werewolf.world/village/context/0.3/error.jsonld](https://werewolf.world/village/context/0.3/error.jsonld)|
|character|[https://werewolf.world/village/context/0.3/character.jsonld](https://werewolf.world/village/context/0.3/character.jsonld)|
|role|[https://werewolf.world/village/context/0.3/role.jsonld](https://werewolf.world/village/context/0.3/role.jsonld)|
|board|[https://werewolf.world/village/context/0.3/board.jsonld](https://werewolf.world/village/context/0.3/board.jsonld)|
|chat|[https://werewolf.world/village/context/0.3/chat.jsonld](https://werewolf.world/village/context/0.3/chat.jsonld)|
|vote|[https://werewolf.world/village/context/0.3/vote.jsonld](https://werewolf.world/village/context/0.3/vote.jsonld)|
|votingResult|[https://werewolf.world/village/context/0.3/votingResult.jsonld](https://werewolf.world/village/context/0.3/votingResult.jsonld)|
|scroll|[https://werewolf.world/village/context/0.3/scroll.jsonld](https://werewolf.world/village/context/0.3/scroll.jsonld)|

# IRIs

## message

|IRI|Purpose|
---|---
|https://werewolf.world/resource/0.3/boardMessage|Send a prediction board update to server|
|https://werewolf.world/resource/0.3/errorMessage|Send/Receive an error message to/from server|
|https://werewolf.world/resource/0.3/playerMessage|Send/receive a chat message to/from server|
|https://werewolf.world/resource/0.3/scrollMessage|Send a scroll information to server|
|https://werewolf.world/resource/0.3/systemMessage|Receive a system message from server|
|https://werewolf.world/resource/0.3/voteMessage|Send a vote to server|

## base

|IRI|Type|Values|
---|---|---
|https://werewolf.world/resource/0.3/token||"[0-9A-Fa-f]{8}-[0-9A-Fa-f]{4}-[0-9A-Fa-f]{4}-[0-9A-Fa-f]{4}-[0-9A-Fa-f]{12}"(GUID)|
|https://werewolf.world/resource/0.3/villageId|xsd:integer|0 <=|
|https://werewolf.world/resource/0.3/villageName||5 <= {# of Unicode code points} <= 30|
|https://werewolf.world/resource/0.3/totalNumberOfCharacters|xsd:integer|4 <=|
|https://werewolf.world/resource/0.3/phase||'morning', 'noon', 'night', 'result', 'post mortem'|
|https://werewolf.world/resource/0.3/date|xsd:integer|-1 <=, 0 when phase were post mortem, -1 when phase were result|
|https://werewolf.world/resource/0.3/phaseTimeLimit|xsd:integer|if nothing, -1. otherwise, how many seconds|
|https://werewolf.world/resource/0.3/phaseStartTime|xsd:dateTime|such as '2006-10-07T12:06:56.568+09:00'|
|https://werewolf.world/resource/0.3/serverTimestamp|xsd:dateTime|such as '2006-10-07T12:06:56.568+09:00'|
|https://werewolf.world/resource/0.3/clientTimestamp|xsd:dateTime|such as '2006-10-07T12:06:56.568+09:00'|
|https://werewolf.world/resource/0.3/directionality||'server to client' or 'client to server'|
|https://werewolf.world/resource/0.3/channel||'public', 'private', 'werewolf', 'seer', 'hunter', 'master', 'grave', 'onymousAudience', 'anonymousAudience'|


## error

|IRI|Type|Values|
---|---|---
|https://werewolf.world/resource/0.3/errorContent|||
|https://werewolf.world/resource/0.3/severity||'error', 'warning'|
|https://werewolf.world/resource/0.3/source||(JSON-LD)|

## character

|IRI|Type|Values|
---|---|---
|https://werewolf.world/resource/0.3/character|||
|https://werewolf.world/resource/0.3/characterId|xsd:integer|-1 <= (-1 means master)|
|https://werewolf.world/resource/0.3/characterIsMine|xsd:boolean|true, false|
|https://werewolf.world/resource/0.3/characterName||[https://werewolf.world/image/0.3/#character](https://werewolf.world/image/0.3/#character)|
|https://werewolf.world/resource/0.3/characterImage||[https://werewolf.world/image/0.3/#character](https://werewolf.world/image/0.3/#character)|
|https://werewolf.world/resource/0.3/characterStatus||'alive', 'dead', 'death by execution', 'death by attack', 'death by fear', 'unnatural death'|
|https://werewolf.world/resource/0.3/characterIsAChoice|xsd:boolean||

See [https://werewolf.world/image/0.3/#character](https://werewolf.world/image/0.3/#character)

## role

|IRI|Type|Values|
---|---|---
|https://werewolf.world/resource/0.3/role|||
|https://werewolf.world/resource/0.3/roleIsMine|xsd:boolean|true, false|
|https://werewolf.world/resource/0.3/roleName||[https://werewolf.world/image/0.3/#role](https://werewolf.world/image/0.3/#role)|
|https://werewolf.world/resource/0.3/roleImage||[https://werewolf.world/image/0.3/#role](https://werewolf.world/image/0.3/#role)|
|https://werewolf.world/resource/0.3/numberOfCharactersWhoPlayTheRole|xsd:integer|0 <=, <= 7|

See [https://werewolf.world/image/0.3/#role](https://werewolf.world/image/0.3/#role)

## board

|IRI|Type|Values|
---|---|---
|https://werewolf.world/resource/0.3/board|||
|https://werewolf.world/resource/0.3/boardPolarity||'positive', 'negative'|
|https://werewolf.world/resource/0.3/boardPrediction||'?','Δ','O','X'|

## chat

|IRI|Type|Values|
---|---|---
|https://werewolf.world/resource/0.3/chatIsMine|xsd:boolean|true, false|
|https://werewolf.world/resource/0.3/chatId|xsd:integer|1 <=|
|https://werewolf.world/resource/0.3/chatCounter|xsd:integer|0<=, <=chatLimit|
|https://werewolf.world/resource/0.3/chatLimit|xsd:integer|1 <=|
|https://werewolf.world/resource/0.3/chatInterval||such as '5s'|
|https://werewolf.world/resource/0.3/chatText||string such as 0 <= {# of Unicode code points} <= {chatCharacterLimit}|
|https://werewolf.world/resource/0.3/chatCharacterLimit|xsd:integer|1 <= {# of Unicode code points}|
|https://werewolf.world/resource/0.3/chatLanguage||'en', 'ja', etc. ([java.util.Locale.toString](https://docs.oracle.com/javase/9/docs/api/java/util/Locale.html#toString--))|
|https://werewolf.world/resource/0.3/chatIsOver|xsd:boolean|true, false|

## votingResult

|IRI|Type|Values|
---|---|---
|https://werewolf.world/resource/0.3/votingResultsSummary|||
|https://werewolf.world/resource/0.3/numberOfVotes|xsd:integer|0 <=, <= {number of alive characters except a master}|
|https://werewolf.world/resource/0.3/rankOfVotes|xsd:integer|1 <=, 1 is the highest. "1224" ranking.|
|https://werewolf.world/resource/0.3/votingResultsDetails|||

## result

|IRI|Type|Values|
---|---|---
|https://werewolf.world/resource/0.3/result||'win', 'lose'|
|https://werewolf.world/resource/0.3/userName||5 <= {# of Unicode code points} <= 15|
|https://werewolf.world/resource/0.3/userAvatar||(URL)|

## scroll

|IRI|Type|Values|
---|---|---
|https://werewolf.world/resource/0.3/nodeId|||
|https://werewolf.world/resource/0.3/scrollTop|xsd:integer||
|https://werewolf.world/resource/0.3/scrollHeight|xsd:integer||
|https://werewolf.world/resource/0.3/offsetHeight|xsd:integer||
