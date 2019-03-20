
```C#

GraphServiceClient graphClient = new GraphServiceClient();
var contacts = await graphClient.Me.Contacts
	.Select("displayName,emailAddresses")
	.Request().GetAsync();

```