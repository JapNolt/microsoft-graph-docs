
```C#

GraphServiceClient graphClient = new GraphServiceClient();
var messages = await graphClient.Me.Messages["AAMkAGVmMDEz"]
	.Select("internetMessageHeaders")
	.Request().GetAsync();

```