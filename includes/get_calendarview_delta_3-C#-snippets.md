
```C#

GraphServiceClient graphClient = new GraphServiceClient();
var delta = await graphClient.Me.CalendarView.Delta()
	.SkipToken("R0usmci39OQxqJrxK4")
	.Request().GetAsync();

```