
```C#

GraphServiceClient graphClient = new GraphServiceClient();
var messages = await graphClient.Me.Messages["AAMkADhAAAW-VPeAAA="]
	.Select("internetMessageHeaders")
	.Request().GetAsync();

```