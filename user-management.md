[service-omnichannel](../../../README.md) / [API](../README.md) / [How to use](./README.md) / User management

# User management

Each request made must be done on behalf of a user defined on the body property `user`.

The `user` property must contains:

* `id`: The ID of the user,
* `worskpaces`: Array of workspace IDs the user have authorizations,
* `role`: Role of the user.