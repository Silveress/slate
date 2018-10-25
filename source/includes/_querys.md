# Queries

## Local Queries Information
Almost all of the endpoints are queryable based on the content they contain, so if you want to see equipment that is only soul's then `https://api.silveress.ie/bns/v3/equipment?type=soul` has you covered.

## Global Queries
### Limit
This changes the total responses you get from any endpoint and can be used to increase or decrease the amount returned.


`?limit=n`
### Skip
This often works in conjunction with limit, it skips the first n responses.


`?skip=n`
### Beautify
This is flag to change the JSON from human readable to a more compact version that works better with computers, 20%-50% space saving compared to normal.

`?beautify=min`  
`?beautify=human`  - Default

### Combined Example
the below will return the compact JSON of 100 items and skipping the first 1000


`?beautify=min&skip=1000&?limit=100`