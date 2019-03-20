
```C#

GraphServiceClient graphClient = new GraphServiceClient();
var events = await graphClient.Me.Events
	.Select("subject,body,bodyPreview")
	.Request().GetAsync();

```