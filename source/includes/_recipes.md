# Recipes

## All

```json
[
  {
    "id": 1,
    "active": "FALSE",
    "updated": "2017-09-13T14:55:51Z",
    "createdBy": "Acquired Taste",
    "type": "Food",
    "item": "Dumpling",
    "output": 2,
    "cost": 6,
    "guildRank": 1,
    "hours": 0.5,
    "xp": 24,
    "ingredients": [
      {
        "name": "Whole Chicken",
        "quantity": 10
      }
    ]
  },
  {
    "id": 417,
    "active": "TRUE",
    "updated": "2017-08-14T18:58:24Z",
    "createdBy": "process",
    "type": "material",
    "item": "Soulstone Crystal",
    "output": 1,
    "cost": 0,
    "ingredients": [
      {
        "name": "Soulstone",
        "quantity": 1
      }
    ]
  }
]
```

Returns a list of all the recipes recorded.

Example  
`https://api.silveress.ie/bns/v3/recipe/all`

## Current

```json
[
 {
    "id": 417,
    "active": "TRUE",
    "updated": "2017-08-14T18:58:24Z",
    "createdBy": "process",
    "type": "material",
    "item": "Soulstone Crystal",
    "output": 1,
    "cost": 0,
    "ingredients": [
      {
        "name": "Soulstone",
        "quantity": 1
      }
    ]
  },
  {
    "id": 418,
    "active": "TRUE",
    "updated": "2017-08-14T18:58:24Z",
    "createdBy": "process",
    "type": "material",
    "item": "Sacred Crystal",
    "output": 1,
    "cost": 0,
    "ingredients": [
      {
        "name": "Sacred Orb",
        "quantity": 1
      }
    ]
  }
]
```

Returns a list of all the active recipes recorded.

Example  
`https://api.silveress.ie/bns/v3/recipe/current`

## History

```json
[
  {
    "id": 1,
    "active": "FALSE",
    "updated": "2017-09-13T14:55:51Z",
    "createdBy": "Acquired Taste",
    "type": "Food",
    "item": "Dumpling",
    "output": 2,
    "cost": 6,
    "guildRank": 1,
    "hours": 0.5,
    "xp": 24,
    "ingredients": [
      {
        "name": "Whole Chicken",
        "quantity": 10
      }
    ]
  },
  {
    "id": 2,
    "active": "FALSE",
    "updated": "2017-09-13T14:55:51Z",
    "createdBy": "Acquired Taste",
    "type": "Food",
    "item": "Dumpling",
    "output": 5,
    "cost": 63,
    "guildRank": 2,
    "hours": 0.67,
    "xp": 33,
    "ingredients": [
      {
        "name": "Iron Ox Meat",
        "quantity": 20
      }
    ]
  }
]
```

Returns a list of all the inactive recipes recorded.

Example  
`https://api.silveress.ie/bns/v3/recipe/history`

## Search

```json
[
  {
    "id": 736,
    "active": "TRUE",
    "updated": "2017-08-15T12:09:37Z",
    "createdBy": "upgrade",
    "type": "weapon",
    "item": "Baleful Stage 9",
    "output": 1,
    "cost": 100000,
    "ingredients": [
      {
        "name": "Seraph Stage 9",
        "quantity": 1
      },
      {
        "name": "Pristine Oil",
        "quantity": 1
      }
    ]
  }
]
```

Returns a list of recipes that match the criteria.

Example  
`https://api.silveress.ie/bns/v3/recipe/search?item=Baleful Stage 9&active=true`  
`https://api.silveress.ie/bns/v3/recipe/search?item=Baleful%20Stage%209&active=true`

