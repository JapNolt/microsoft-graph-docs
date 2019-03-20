
```C#

GraphServiceClient graphClient = new GraphServiceClient();
var sites = await graphClient.Sites
	.Filter("siteCollection/root ne null")
	.Request().GetAsync();

```