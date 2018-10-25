
# Market

## Available ID's

```json
[
  2280028,
  2280130,
  910110,
  2021415,
  2603373,
  2021411,
  910127,
  910128,
  2280151
]
```

Returns a list of all ID's available under this method

`http://api.silveress.ie/bns/v3/market/<eu|na>/<current|history>` 

Example  
`http://api.silveress.ie/bns/v3/market/eu/current`


## Info based on ID

```json
[
  {
    "name": "Premium Transformation Stone",
    "id": 821515,
    "ISO": "2017-12-02T23:00:04.219Z",
    "listings": [
      {
        "price": 3340000,
        "count": 1,
        "each": 3340000
      },
      {
        "price": 3350000,
        "count": 1,
        "each": 3350000
      },
		...
    ],
    "totalListings": 19,
    "totalListed": 19
  }
]
```

Returns price info based on that ID.  
If timeframe is current it only returns the most recent set of listings.  
If timeframe is history it returns the last month of listings on an hourly interval.

`http://api.silveress.ie/bns/v3/market/<eu|na>/<current|history>/<ID>`  

Example  
`http://api.silveress.ie/bns/v3/market/eu/current/821515`

****

If the timeframe is history a daterange can be queried.  
Example  
`https://api.silveress.ie/bns/v3/market/eu/history/2280028?start=2017-12-01&end=2017-12-13`

Warning this isnt fully supported yet, its an early implimentation that somewhat works, I will be returning again to improve it.  
The dates are in yyyy-mm-dd format (ISO 8601)

## Current Modifiers

### `/current/all`

Returns all teh current listings on the marketplace from the last scrape

### `/current/lastListing`

Returns the last listing of all items listed on teh marketplace.  
So if an item is not currently listed on `/current/all` it will still be here.

### `/current/lowest`

Flat array designed to be easier to import into google sheets via the importJSON script.

### `/current/top/price`

Same as `/current/all` but ordered so most expensive listing is first.

### `/current/top/quantity`

Same as `/current/all` but ordered so listing with the most items is first.

### `/current/top/listings`

Same as `/current/all` but ordered so listing with teh most listings is first.