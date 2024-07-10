[service-omnichannel](../../../../README.md) / [API](../README.md) / [Analyses](./README.md) / get analyse data 

# Get client anlayse data

Get analyse data  of client . 

```text
GET analyses/:id/data
```

## Body

| Name           | Description                                         |
|----------------|-----------------------------------------------------|
| `user`         | The client's user information                       |
| `workspaceId`  | The current workspaceId                             |


## Parameters

| Name           | Description                                         |
|----------------|-----------------------------------------------------|
| `id`           | analyse id                                          |



## Example

```text
GET analyses/665746252624a663d285deb0/data

{
  "user": {
    "id": "123-abc-456",
    "workspaces": ["fake-id24"]
  },
  "workspaceId": "fake-id24"
}
```

Response

```text
200
```

```json

{
  "analyseId": "667973e4b4233ee15adb76d5",
  "analyseName": "Test analyse name",
  "conversionsPaths": [
    {
      "workspaceId": "fake-id",
      "analyseId": "667973e4b4233ee15adb76d5",
      "path": " Direct",
      "nb_touchpoints": 1,
      "conversions": 1972,
      "CA": 4573829.251123
    },
    {
      "workspaceId": "fake-id",
      "analyseId": "667973e4b4233ee15adb76d5",
      "path": " Paid Search > Organic Search X 19",
      "nb_touchpoints": 20,
      "conversions": 365,
      "CA": 560368.204956
    }
  ],
  "channelsAttribution": [
    {
      "workspaceId": "fake-id",
      "analyseId": "667973e4b4233ee15adb76d5",
      "channelName": "Paid Search",
      "firstTouchConversions": "1780",
      "lastTouchConversions": "1062",
      "linearConversions": "479",
      "markovConversions": "1763",
      "firstTouchValue": "4224112",
      "lastTouchValue": "2779690",
      "linearValue": "2332525",
      "markovValue": "4449076"
    },
    {
      "workspaceId": "fake-id",
      "analyseId": "667973e4b4233ee15adb76d5",
      "channelName": "Organic Search",
      "firstTouchConversions": "2383",
      "lastTouchConversions": "2955",
      "linearConversions": "1691",
      "markovConversions": "2601",
      "firstTouchValue": "5760284",
      "lastTouchValue": "6956616",
      "linearValue": "7583847",
      "markovValue": "6472584"
    }
   ],
  "channelsSummaries": [
    {
      "workspaceId": "fake-id",
      "analyseId": "667973e4b4233ee15adb76d5",
      "channelName": "Paid Search",
      "initiatorConversions": 1356,
      "assistantConversions": 1459,
      "finisherConversions": 638,
      "autonomousConversions": 424,
      "presenceConversions": 2513,
      "role": "assistant"
    },
    {
      "workspaceId": "fake-id",
      "analyseId": "667973e4b4233ee15adb76d5",
      "channelName": "Organic Search",
      "initiatorConversions": 1198,
      "assistantConversions": 2860,
      "finisherConversions": 1770,
      "autonomousConversions": 1185,
      "presenceConversions": 2896,
      "role": "assistant"
    } 
  ],
  "channelsPresence": [
    {
      "channelName": "Paid Search",
      "presenceConversions": 2513
    },
    {
      "channelName": "Organic Search",
      "presenceConversions": 2896
    }
  ],
  "nbPaths": 2085,
  "turnover": 19808120.11594794,
  "mono": 2412,
  "multi": 5455,
  "conversions": 7867    

}    
            

```