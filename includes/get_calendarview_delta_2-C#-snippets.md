
```C#

GraphServiceClient graphClient = new GraphServiceClient();
var delta = await graphClient.Me.CalendarView.Delta()
	.SkipToken("R0usmcCM996atia_s")
	.Request().GetAsync();

```