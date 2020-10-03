## UI To HAZARD-ANALYTICS-SERVICE Request =============
#### NAME: Get All Hazards
#### HTTP Operation: GET 
#### Path: /hazards
#### Format: JSON




## UI To HAZARD-ANALYTICS-SERVICE Response ============
#### Format: JSON

### Response Body:

```
[
    {
        latitude: 14.021,
        longitude: -124.034,
        hazardType: "hurricane",
        name: "Cyclone Ema in 2015"
    },
    {
        latitude: 85.021,
        longitude: 44.034,
        hazardType: "hurricane",
        name: "Tornado Thor in 2010"
    },
    {
        latitude: -85.021,
        longitude: 124.034,
        hazardType: "wildfire",
        name: "Forest widlfire in Brazil"
    }
]
```