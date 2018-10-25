# Equipment
## Base
```json
[
  {
    "name": "Acrimor Earring - Stage 10",
    "img": "http://static.ncsoft.com/bns_resource/ui_resource/accessory/acc_earring_baekchung_5-4phase_5_10_1.png",
    "rank": "5",
    "firstAdded": "2017-11-30T01:05:40.040Z"
  },
  {
    "name": "Acrimor Necklace",
    "img": "http://static.ncsoft.com/bns_resource/ui_resource/accessory/acc_necklace_gunwon_1-1phase_5_1.png",
    "rank": "5",
    "firstAdded": "2017-11-30T13:03:08.531Z"
  },
  {
    "name": "After Midnight",
    "img": "http://static.ncsoft.com/bns_resource/ui_resource/costume/costume_60039_jinm_col2_5_1.png",
    "rank": "5",
    "firstAdded": "2017-11-30T13:02:40.751Z"
  }
]
```

`https://api.silveress.ie/bns/v3/equipment`

Returns basic info on equipable.  
This is obtained from whenever anyone uses my character endpoint, the info is scraped from the loaded page.  
Queryable
### New
`https://api.silveress.ie/bns/v3/equipment/new`  
Endpoint where Newest items are first.  
Queryable.

### Old
`https://api.silveress.ie/bns/v3/equipment/old`  
Endpoint where oldest items are first. Made for use with a spreadsheet so new rows are added at the bottom.  
Queryable.


## New

Marketable items but ordered by newest first.

## Count

```json
[
  {
    "ISO": "2017-12-02T22:05:20.395Z",
    "equipmentCount": 742,
    "itemCount": 2614
  },
  {
    "ISO": "2017-12-02T21:05:24.664Z",
    "equipmentCount": 742,
    "itemCount": 2614
  }
]
```

`https://api.silveress.ie/bns/v3/equipment/count`

Returns the quantity of equipable items and their type