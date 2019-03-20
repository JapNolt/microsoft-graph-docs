
```C#

GraphServiceClient graphClient = new GraphServiceClient();
var agreements = await graphClient.Agreements["<id>"]
	.Expand("files")
	.Request().GetAsync();

```