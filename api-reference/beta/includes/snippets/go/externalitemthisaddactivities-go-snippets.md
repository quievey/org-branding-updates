---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphmodels "github.com/microsoftgraph/msgraph-beta-sdk-go/Connections/Item/Items/Item/MicrosoftGraphExternalConnectorsAddActivities"
	  //other-imports
)

graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphmodels.NewAddActivitiesPostRequestBody()


externalActivity := graphmodels.NewExternalActivity()
type := graphmodels.CREATED_EXTERNALACTIVITYTYPE 
externalActivity.SetType(&type) 
startDateTime , err := time.Parse(time.RFC3339, "2021-04-06T18:04:31.033Z")
externalActivity.SetStartDateTime(&startDateTime) 
performedBy := graphmodels.NewIdentity()
type := graphmodels.USER_IDENTITYTYPE 
performedBy.SetType(&type) 
id := "1f0c997e-99f7-43f1-8cca-086f8d42be8d"
performedBy.SetId(&id) 
externalActivity.SetPerformedBy(performedBy)

activities := []graphmodels.ExternalActivityable {
	externalActivity,

}
requestBody.SetActivities(activities)

result, err := graphClient.Connections().ByConnectionId("externalConnection-id").Items().ByItemId("externalItem-id").MicrosoftGraphExternalConnectorsAddActivities().Post(context.Background(), requestBody, nil)


```