
```C#

GraphServiceClient graphClient = new GraphServiceClient();
var users = await graphClient.Users
	.Select("displayName,givenName,postalCode")
	.Request().GetAsync();

```