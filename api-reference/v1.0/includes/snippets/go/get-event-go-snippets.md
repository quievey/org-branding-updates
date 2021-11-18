---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.EventRequestBuilderGetQueryParameters{
	Select: "subject,body,bodyPreview,organizer,attendees,start,end,location,hideAttendees",
}
headers := map[string]string{
	"Prefer": "outlook.timezone="Pacific Standard Time""
}
options := &msgraphsdk.EventRequestBuilderGetOptions{
	Q: requestParameters,
	H: headers,
}
eventId := "event-id"
result, err := graphClient.Me().EventsById(&eventId).Get(options)


```