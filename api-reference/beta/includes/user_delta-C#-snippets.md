
```C#

GraphServiceClient graphClient = new GraphServiceClient();
var delta = await graphClient.Users.Delta()
	.Select("displayName,jobTitle,mobilePhone")
	.Request().GetAsync();

```