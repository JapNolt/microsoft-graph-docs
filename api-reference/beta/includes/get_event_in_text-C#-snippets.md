
```C#

GraphServiceClient graphClient = new GraphServiceClient();
var events = await graphClient.Me.Events["AAMkAGI1AAAoZDOFAAA="]
	.Select("subject,body,bodyPreview")
	.Request().GetAsync();

```