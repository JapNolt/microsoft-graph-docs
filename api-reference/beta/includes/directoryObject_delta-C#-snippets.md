
```C#

GraphServiceClient graphClient = new GraphServiceClient();
var directoryObjects = await graphClient.DirectoryObjects["delta"]
	.Filter("isOf('Microsoft.Graph.User')+or+isOf('Microsoft.Graph.Group')")
	.Request().GetAsync();

```