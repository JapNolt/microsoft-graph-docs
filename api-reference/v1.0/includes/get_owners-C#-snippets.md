
```C#

GraphServiceClient graphClient = new GraphServiceClient();
var installedApps = await graphClient.Teams["{id}"].InstalledApps
	.Expand("teamsAppDefinition")
	.Request().GetAsync();

```