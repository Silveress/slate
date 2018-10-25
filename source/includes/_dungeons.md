# Dungeons

## QuestBase

```json
[
  {
    "id": 1,
    "location": "Skybreak Spire",
    "quest": "Raven's Cry",
    "gold": 198000,
    "pve_or_pvp": "PvE",
    "reset_time": "Weekly",
    "party": 12,
    "xp": 60960
  },
  {
    "id": 2,
    "location": "Skybreak Spire",
    "quest": "Military Intervention",
    "gold": 181500,
    "pve_or_pvp": "PvE",
    "reset_time": "Weekly",
    "party": 12,
    "xp": 55770
  }
]
```

A flat array of information about dungeon quests.  
Queryable.

Example  
`https://api.silveress.ie/bns/v3/dungeons/questsbase`

## Daily Challenge

```json
[
 {
    "startDate": "2017-12-29T00:00:00.000Z",
    "Monday": [
      "Zakhan's Blade",
      "The Bonds that Bind Us",
      "In the Dead of Winter",
      "Frozen Phantasm",
      "One Win in the Beluga Lagoon",
      "Tag Match Win"
    ],
    "Tuesday": [
      "Roar of the Furnace",
      "Asura's Return",
      "Nightmare at the Necropolis",
      "Rose from the Past",
      "One Whirlwind Victory",
      "One on One"
    ],
    "Wednesday": [
      "..."
    ],
    "Thursday": [
      "..."
    ],
    "Friday": [
      "..."
    ],
    "Saturday": [
      "..."
    ],
    "Sunday": [
      "..."
    ],
    "Weekly": [
      "..."
    ]
  }
]
```

An ordered list with the current daily challenge on top, contains days and quests for that day.  
Queryable.

Example  
`https://api.silveress.ie/bns/v3/dungeons/daily`

## Merged Quests + Daily

```json
[
  {
    "id": 3,
    "location": "Skybreak Spire",
    "quest": "Dark Revival",
    "gold": 165000,
    "pve_or_pvp": "PvE",
    "reset_time": "Weekly",
    "party": 12,
    "xp": 50770,
    "daily_challenge": [],
    "weekly_challenge": true
  },
  {
    "id": 7,
    "location": "Sogun's Lament",
    "quest": "Asura's Return",
    "gold": 38300,
    "pve_or_pvp": "PvE",
    "reset_time": "Daily",
    "party": 6,
    "xp": 17300,
    "daily_challenge": [
      "Tuesday",
      "Sunday"
    ],
    "weekly_challenge": false
  }
]
```

Same as QuestBase but also contains the Daily Challenge info within it.  
Queryable.

Example  
`https://api.silveress.ie/bns/v3/dungeons/quests`  
`https://api.silveress.ie/bns/v3/dungeons/quests?weekly_challenge=true`  
`https://api.silveress.ie/bns/v3/dungeons/quests?daily_challenge=Monday,Tuesday`  

