
```C#

GraphServiceClient graphClient = new GraphServiceClient();
var events = await graphClient.Me.Events["AAMkADAGAADDdm4NAAA="]
	.Select("subject,body,bodyPreview,organizer,attendees,start,end,location,locations")
	.Request().GetAsync();

```