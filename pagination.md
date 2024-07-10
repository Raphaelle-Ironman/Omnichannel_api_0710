[service-omnichannel](../../../README.md) / [API](../README.md) / [How to use](./README.md) / Pagination

# Pagination

# Pagination

Results of requests with list have a pagination system. The page number can be selected with the
key `page` in json query field `q`. The reponse's body `pagination` property give information about the total number
of pages, the number of elements by pages and the current page.
The number of entries by page can be selected by the key `limit` in json query field `q`.

## Example

```
GET /channels-attribution?q={"limit":2, "page":1}
```

```
{
  "data": [
    {
      "workspaceId": 1301,
      "analyseId": "fB1t5X73re5V991OVGus",
      "channelName": "Organic Video",
      "firstTouchConversions": "188",
      "lastTouchConversions": "132",
      "linearConversions": "34",
      "markovConversions": "97",
      "firstTouchValue": "141303",
      "lastTouchValue": "155685",
      "linearValue": "175396",
      "markovValue": "89805"
    },
    {
      "workspaceId": 1301,
      "analyseId": "fB1t5X73re5V991OVGus",
      "channelName": "Organic Video",
      "firstTouchConversions": "188",
      "lastTouchConversions": "132",
      "linearConversions": "34",
      "markovConversions": "97",
      "firstTouchValue": "141303",
      "lastTouchValue": "155685",
      "linearValue": "175396",
      "markovValue": "89805"
    }
  ],
  "count": 2,
  "page": 1,
  "total": 8,
  "pageCount": 4
}
```