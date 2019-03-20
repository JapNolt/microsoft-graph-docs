
```C#

GraphServiceClient graphClient = new GraphServiceClient();
var events = await graphClient.Me.Events
	.Select("subject,body,bodyPreview,organizer,attendees,start,end,location")
	.Request().GetAsync();

```