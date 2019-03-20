
```C#

GraphServiceClient graphClient = new GraphServiceClient();
var delta = await graphClient.Groups.Delta()
	.Select("displayName,description,mailNickname")
	.Request().GetAsync();

```