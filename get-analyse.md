[service-omnichannel](../../../../README.md) / [API](../README.md) / [Analyses](./README.md) / get analyse  

# Get client anlayse summary

Get analyse summary. 

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
GET analyses/665746252624a663d285deb0

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
  "_id": "667973e4b4233ee15adb76d5",
  "workspaceId": "fake-id",
  "analyseName": "Test analyse name",
  "property": "Gold Avenue",
  "filter": "# All Users",
  "startDate": "2023-07-01T00:00:00.000Z",
  "endDate": "2023-12-21T00:00:00.000Z",
  "statut": "finished"

}    
            

```