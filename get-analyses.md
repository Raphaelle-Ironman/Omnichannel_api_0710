[service-omnichannel](../../../../README.md) / [API](../README.md) / [Analyses](./README.md)/ Get analyses of  client

# Get client anlayses

Get all analyses of client .

```text
GET /analyses
```

## Body

| Name           | Description                                         |
|----------------|-----------------------------------------------------|
| `user`         | The client's user information                       |
| `workspaceId`  | The current workspaceId                             |

## Example

```text
GET /analyses

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
  "data": [
    
    {
      "workspaceId": 0,
      "analyseName": "test numero 2",
      "property": "Gold Avenue",
      "filter": "# All Users",
      "startDate": "2023-07-01T00:00:00.000Z",
      "endDate": "2023-12-21T00:00:00.000Z",
      "statut": "NotProcessed",
      "analyseId": "665746252624a663d285deb0"
    },
    {
      "workspaceId": 0,
      "analyseName": "test numero 1",
      "property": "Gold Avenue",
      "filter": "# All Users",
      "startDate": "2023-07-01T00:00:00.000Z",
      "endDate": "2023-12-21T00:00:00.000Z",
      "statut": "NotProcessed",
      "analyseId": "6657462f2624a663d285deb2"
    }
  ],
  "count": 2,
  "page": 1,
  "total": 9,
  "pageCount": 1
}
```
