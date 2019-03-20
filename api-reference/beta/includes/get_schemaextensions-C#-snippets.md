
```C#

GraphServiceClient graphClient = new GraphServiceClient();
var schemaExtensions = await graphClient.SchemaExtensions
	.Filter("id eq 'graphlearn_test'")
	.Request().GetAsync();

```