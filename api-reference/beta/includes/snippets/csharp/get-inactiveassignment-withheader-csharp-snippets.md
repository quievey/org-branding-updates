---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].GetAsync((requestConfiguration) =>
{
	requestConfiguration.Headers.Add("Prefer", "include-unknown-enum-members");
});


```