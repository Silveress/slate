# Characters



An endpoint to return information on either an individual character or character rankings.

## Character Info
```json
{
  "ap": 814,
  "hp": 69406,
  "piercing": 737,

  "...":"...",
  
  "accountName": "Silveress",
  "characterName": "Silveress Golden",
  "playerClass": "Blade Dancer",
  "playerLevel": 50,
  "playerLevelHM": 10,
  "server": "Jinsoyun",
  "faction": "Crimson Legion",
  "factionRank": "Aspirant",
  "guild": "Animals",
  "characterImg": "http://eu-gamepic.ncsoft.com/images/0201/45/zXlKAAAAAAA=.jpg"
}
```
### Full
Returns info on the character which can be pulled into google sheets by a template page I created.    
This endpoint also feeds my equipment endpoint.

Example  
`https://api.silveress.ie/bns/v3/character/full/<eu|na>/<Character Name>`  
`https://api.silveress.ie/bns/v3/character/full/eu/Silveress Golden`  
`https://api.silveress.ie/bns/v3/character/full/eu/Silveress%20Golden`  

### Ranking
This is the same as the above, but with one key difference.
In return for providing the stats you agree that I can:

 1. Display it in the ranking list.
 2. Can update the character info on a fixed schedule.
 
More on this below.

Example  
`https://api.silveress.ie/bns/v3/character/ranking/<eu|na>/<Character Name>`  
`https://api.silveress.ie/bns/v3/character/ranking/eu/Silveress Golden`  


## Ranking - endpoint

Returns list of all characters that were entered to the ranking and is sorted by the attribute chosen.  
The attributes are the names on the left hand side of the list.  
It is also queryable.  
All the characters on the list are updated daily at 00:00 UTC

Example  
`https://api.silveress.ie/bns/v3/character/rankings/<attribute>`  
`https://api.silveress.ie/bns/v3/character/rankings/ap`  
`https://api.silveress.ie/bns/v3/character/rankings/ap?region=eu`  
`https://api.silveress.ie/bns/v3/character/rankings/ap?region=eu&server=Jinsoyun`  
`https://api.silveress.ie/bns/v3/character/rankings/ap?region=eu&server=Jinsoyun&faction=Crimson Legion`  


## Disclaimer


In return for providing the stats you agree that I can:

 1. Display it in the ranking list.
 2. Can update the character info on a fixed schedule.

### Account Removal 
 
If you want your character removed from the rankings list please contact me and it will be removed.

 * [Discord](https://discord.gg/qhNZeMa) Channel: #api-stuff
 * [Reddit](https://www.reddit.com/message/compose?to=Silveress_Golden&subject=Api_Character_Removal&message=) 
 * [IRC](https://kiwiirc.com/client/irc.snoonet.org:6697/##Unoffical_BnS_API) Because why not, it will outlast us all.
