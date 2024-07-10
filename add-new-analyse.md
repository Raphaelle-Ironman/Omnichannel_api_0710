[service-omnichannel](../../../../README.md) / [API](../README.md) / [Analyses](./README.md) / Add new analyse

# Add new analyse

Add a new analyse for a client. 

```text
POST  /analyses
```

## Body

| Name           | Description                                         |
|----------------|-----------------------------------------------------|
| `user`         | The client's user information                       |
| `name`         | Analyse name                                        |  
| `workspaceId`  | The current workspaceId                             |
| `data`         | Google analytis data encoded in base 64             |

## Example

```text
POST  /analyses

{
  "name": "Test analyse name",
  "user": {
    "id": "123-abc-456",
    "workspaces": ["fake-id24"]
  },
  "workspaceId": "fake-id24",
  "data": "data:text/csv;base64,IyAtLS0tLS0tLS0tLS0tLS0tLS0tLS0t
}  

```

Response

```text
201 Created
```

```json
{
  "startDate": "20230701",
  "endDate": "20231221",
  "filter": "# All Users",
  "account": "Gold Avenue",
  "analyseName": "test numero 0",
  "workspaceId": 0,
  "analyseId": "6659ab30a6cde5595a613"
}
```
