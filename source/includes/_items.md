# Items

## Marketable Items

```json
[
  {
    "id": 821515,
    "name": "Premium Transformation Stone",
    "img": "http://static.ncsoft.com/bns_resource/ui_resource/grocery/grocery_element_steel3_4_1.png",
    "rank": 4,
    "stats": "",
    "updated": "2017-12-02T22:00:03.870Z",
    "itemTaxRate": 0.2,
    "merchantValue": 1,
    "characterLevel": 1
  },
  {
    "id": 810603,
    "name": "Soulstone",
    "img": "http://static.ncsoft.com/bns_resource/ui_resource/grocery/gather_shiny_gemstone_4_1.png",
    "rank": 4,
    "stats": "",
    "updated": "2017-12-02T22:00:03.870Z",
    "itemTaxRate": 0.1,
    "merchantValue": 1,
    "characterLevel": 1
  }
]
```

`https://api.silveress.ie/bns/v3/items`

Returns basic info on all marketable items.  
Info here is obtained from my once hourly scraping of the marketplace on both EU and NA.

It is possible to see the same name twice as it can have a different ID ingame, eg "5 Soulstone Bundle" and "5-Soulstone Bundle"

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

`https://api.silveress.ie/bns/v3/items/count`

Returns the quantity of marketable items.

## ID

```json
[
  {
    "id": 821515,
    "name": "Premium Transformation Stone",
    "img": "http://static.ncsoft.com/bns_resource/ui_resource/grocery/grocery_element_steel3_4_1.png",
    "category": "69",
    "rank": 4,
    "stats": "",
    "updated": "2017-12-02T23:00:04.221Z",
    "guideUnitPrice": 3280000,
    "itemTaxRate": 0.2,
    "merchantValue": 1,
    "characterLevel": 1
  }
]
```

`https://api.silveress.ie/bns/v3/items/821515`

Gets info specific to that ID.

I have somewhat abandoned this but it still outputs more info that the regular page.