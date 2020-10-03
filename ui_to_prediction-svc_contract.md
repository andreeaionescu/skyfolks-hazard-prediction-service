## UI To PREDICTION-SERVICE Request =============
#### Name: Is Hazard at this latitude and longitude?
#### HTTP Operation: POST 
#### Path: /hazard/predict
#### Format: JSON

### Request Body:

```
{
    latitude: 14.021,
    longitude: -124.034,
    predict: [ "hurricane" ]
}
```


## UI To PREDICTION-SERVICE Response ============
#### Format: JSON

### Response Body:
```
{
    latitude: 14.021,
    longitude: -124.034,
    predicted: [
        {
            hazardType: "hurricane",
            probability: 0.80%
        }
    ]
```
