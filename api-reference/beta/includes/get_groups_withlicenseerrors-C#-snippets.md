
```C#

GraphServiceClient graphClient = new GraphServiceClient();
var groups = await graphClient.Groups
	.Filter("hasMembersWithLicenseErrors+eq+true,")
	.Select("id,displayName")
	.Request().GetAsync();

```