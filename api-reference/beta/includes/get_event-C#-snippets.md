
```C#

GraphServiceClient graphClient = new GraphServiceClient();
var events = await graphClient.Me.Events["AAMkAGIAAAoZDOFAAA="]
	.Select("subject,body,bodyPreview,organizer,attendees,start,end,location")
	.Request().GetAsync();

```