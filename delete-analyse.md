[service-omnichannel](../../../../README.md) / [API](../README.md) / [Analyses](./README.md) / Delete a analyse

# Delete  analyse

Delete  analyse.

```text
DELETE /analyses/:id
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
DELETE /analyses/6657462f2624a663d285deb2

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
200 OK
```
