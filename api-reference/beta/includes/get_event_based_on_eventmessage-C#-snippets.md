
```C#

GraphServiceClient graphClient = new GraphServiceClient();
var messages = await graphClient.Me.Messages["AAMkADYAAAImV_jAAA="]
	.Expand("")
	.Request().GetAsync();

```