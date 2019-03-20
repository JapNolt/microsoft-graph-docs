
```C#

GraphServiceClient graphClient = new GraphServiceClient();
var driveItem = await graphClient.Shares["{shareIdOrUrl}"].DriveItem
	.Expand("children")
	.Request().GetAsync();

```