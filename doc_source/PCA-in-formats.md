# PCA Response Formats<a name="PCA-in-formats"></a>

## JSON<a name="PCA-json"></a>

Accept—application/json

```
{
    "projections": [
        {
            "projection": [1.0, 2.0, 3.0, 4.0, 5.0]
        },
        {
            "projection": [6.0, 7.0, 8.0, 9.0, 0.0]
        },
        ....
    ]
}
```

## RECORDIO<a name="PCA-recordio"></a>

Accept—application/x\-recordio\-protobuf

```
[
    Record = {
        features = {},
        labels = {
            'projection': {
                keys: [],
                values: [1.0, 2.0, 3.0, 4.0, 5.0]
            }
        }
    },
    Record = {
        features = {},
        labels = {
            'projection': {
                keys: [],
                values: [1.0, 2.0, 3.0, 4.0, 5.0]
            }
        }
    }  
]
```