
```C#

GraphServiceClient graphClient = new GraphServiceClient();
var children = await graphClient.Me.Drive.Items["{item-id}"].Children
	.Expand("thumbnails")
	.Request().GetAsync();

```