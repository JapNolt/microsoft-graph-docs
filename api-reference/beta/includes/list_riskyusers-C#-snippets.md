
```C#

GraphServiceClient graphClient = new GraphServiceClient();
var riskyUsers = await graphClient.RiskyUsers
	.Filter("riskLevel eq microsoft.graph.riskLevel'medium'")
	.Request().GetAsync();

```