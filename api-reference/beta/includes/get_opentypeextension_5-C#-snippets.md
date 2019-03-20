
```C#

GraphServiceClient graphClient = new GraphServiceClient();
var messages = await graphClient.Me.Messages
	.Filter("id eq 'Com.Contoso.Referral')")
	.Expand("extensions")
	.Request().GetAsync();

```