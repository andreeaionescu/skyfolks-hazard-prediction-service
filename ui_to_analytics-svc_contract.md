# 1. GET ALL Hazards Details

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
        id: "1",
        latitude: 14.021,
        longitude: -124.034,
        hazardType: "hurricane",
        name: "Cyclone Ema in 2015"
    },
    {
        id: "2",
        latitude: 85.021,
        longitude: 44.034,
        hazardType: "hurricane",
        name: "Tornado Thor in 2010"
    },
    {
        id: "3",
        latitude: -85.021,
        longitude: 124.034,
        hazardType: "wildfire",
        name: "Forest widlfire in Brazil"
    }
]
```

=====================================================================

# 2. GET Analytics for one particular Hazard

## UI To HAZARD-ANALYTICS-SERVICE Request =============
#### NAME: Get details of one Hazard by id
#### HTTP Operation: GET 
#### Path: /hazard/{id}
#### Format: JSON



## UI To HAZARD-ANALYTICS-SERVICE Response ============
#### Format: JSON

### Response Body:

```

{
    id: "1",
    latitude: 14.021,
    longitude: -124.034,
    hazardType: "hurricane",
    name: "Cyclone Ema in 2015"
    imageURL: "http://localhost:8888/images/hurricane-id-1.png"
    analytics:[
        {
            analyticType: "barchart",
            title: "Death Rate / Day",
            data: {
                columns: [
                    {
                        columnName: "Damage in Dollars",
                        columnType: "Double",
                    },
                    {
                        columnName: "Day",
                        columnType: "Date",
                        dateFormat: "dd-mm-yyyy"
                    } 
                ],
                rows: [
                    [ 8.4, "21-07-2020" ],
                    [ 12.4, "21-07-2020" ],
                    [ 3, "21-07-2020" ],
                    [ 6.5, "21-07-2020" ],
                    [ 10.2, "21-07-2020" ]                    
                ]
            }
        },

        {
            analyticType: "barchart",
            title: "Damage in $ millions / Day",
            data: {
                columns: [
                    {
                        columnName: "Damage in Dollars",
                        columnType: "Double",
                    },
                    {
                        columnName: "Day",
                        columnType: "Date",
                        dateFormat: "dd-mm-yyyy"
                    } 
                ],
                rows: [
                    [ 8.4, "21-07-2020" ],
                    [ 12.4, "21-07-2020" ],
                    [ 3, "21-07-2020" ],
                    [ 6.5, "21-07-2020" ],
                    [ 10.2, "21-07-2020" ]                    
                ]
            }
        },
        
        {
            analyticType: "tabularData",
            title: "Damage in Dollars per Day",
            data: {
                columns: [
                    {
                        columnName: "Damage in Dollars",
                        columnType: "Double",
                    },
                    {
                        columnName: "Day",
                        columnType: "Date",
                        dateFormat: "dd-mm-yyyy"
                    } 
                ],
                rows: [
                    [ 8.4, "21-07-2020" ],
                    [ 12.4, "21-07-2020" ],
                    [ 3, "21-07-2020" ],
                    [ 6.5, "21-07-2020" ],
                    [ 10.2, "21-07-2020" ]                    
                ]
            }
        }
    ]
}
```