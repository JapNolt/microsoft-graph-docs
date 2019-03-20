
```C#

GraphServiceClient graphClient = new GraphServiceClient();
var privilegedRoleAssignments = await graphClient.PrivilegedRoleAssignments
	.Filter("isElevated eq true and expirationDateTime ne null or isElevated eq false")
	.Request().GetAsync();

```