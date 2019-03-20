
```C#

GraphServiceClient graphClient = new GraphServiceClient();
var secureScores = await graphClient.Security.SecureScores
	.Top("1")
	.Request().GetAsync();

```