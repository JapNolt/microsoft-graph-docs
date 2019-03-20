
```C#

GraphServiceClient graphClient = new GraphServiceClient();
var privilegedOperationEvents = await graphClient.PrivilegedOperationEvents
	.Filter("requestType eq 'Assign'")
	.Request().GetAsync();

```