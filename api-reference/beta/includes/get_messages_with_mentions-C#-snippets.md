
```C#

GraphServiceClient graphClient = new GraphServiceClient();
var messages = await graphClient.Me.Messages
	.Filter("MentionsPreview/IsMentioned eq true,")
	.Select("subject,sender,receivedDateTime,mentionsPreview")
	.Request().GetAsync();

```