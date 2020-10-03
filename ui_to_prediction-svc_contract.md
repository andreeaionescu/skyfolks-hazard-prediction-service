## UI To PREDICTION-SERVICE Request ==================================================================================
#### HTTP Operation: GET 
#### Format: JSON

### Example:

```
{
    lattitude: 14.021,
    longitude: -124.034,
    predict: [ "hurricane" ]
}
```


## UI To PREDICTION-SERVICE Response==================================================================================
#### Format: JSON

### Example:
```
{
    lattitude: 14.021,
    longitude: -124.034,
    predicted: [
        {
            hazardType: "hurricane",
            probability: 0.80%
        }
    ]
```