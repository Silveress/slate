# Legacy Endpoints

## v2

```json
[
   {
    "Name": "5 Soulstone Bundle",
    "ID": 2280028
  },
  {
    "Name": "Acquired Taste Secret Technique - Cinderlands",
    "ID": 811039
  }
]
```

v3 emulates the older endpoints from v2


The below returns a list of IDs and Names.

Example  
`http://api.silveress.ie/bns/v2/market`

### Current

```json
[
    {
    "ISO": "2017-12-03T11:00:03.564Z",
    "ID": 2280028,
    "ItemPrice": 30000,
    "Quantity": 3
  },
  {
    "ISO": "2017-12-03T11:00:03.564Z",
    "ID": 2021120,
    "ItemPrice": 4200,
    "Quantity": 1
  }
]
```

Returns a flat array with little info

Example  
`http://api.silveress.ie/bns/v2/market/current/<eu|na>`  
`http://api.silveress.ie/bns/v2/market/current/eu`


### History


```json
[
     {
    "ID": 2280028,
    "timeDate": "2017-08-27T22:00:03.169Z",
    "minPrice": 45000,
    "avgPrice": 41193,
    "maxPrice": 35000,
    "totalItems": 15,
    "totalListings": 15
  },
  {
    "ID": 2280028,
    "timeDate": "2017-08-27T23:00:03.107Z",
    "minPrice": 40000,
    "avgPrice": 40764,
    "maxPrice": 39000,
    "totalItems": 14,
    "totalListings": 14
  }
]
```

Returns a flat array with basic info on an item over a period of time

Example  
`http://api.silveress.ie/bns/v2/market/history/<eu|na>/<ID>`  
`https://api.silveress.ie/bns/v2/market/history/eu/2280028`


## v1

> CSV


```csv

"Name","ID","Quantity","ItemPrice","LastUpdate"
"5 Soulstone Bundle",2280028,3,30000,"2017-12-03T13:00:03.141Z"
"Air Assassin Design",2280130,1,990000,"2017-12-03T04:00:03.207Z"
"Apron of Vanity",910128,1,2300,"2017-12-03T13:00:03.141Z"

```

v1 was offline for quite a  while as figuring out how to emulate it in v3 was quite a challenge.

It outputs data in the format of csv and can be used as a query in Excel or importData in Google Sheets.

Example:  
`http://api.silveress.ie/bns/market/current/<eu|na>`  
`http://api.silveress.ie/bns/market/current/eu`  
