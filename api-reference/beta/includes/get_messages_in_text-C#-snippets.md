
```C#

GraphServiceClient graphClient = new GraphServiceClient();
var messages = await graphClient.Me.Messages
	.Select("subject,body,bodyPreview,uniqueBody")
	.Request().GetAsync();

```