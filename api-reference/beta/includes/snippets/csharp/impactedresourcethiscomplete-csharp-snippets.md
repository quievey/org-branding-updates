---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.Directory.Recommendations["{recommendation-id}"].ImpactedResources["{impactedResource-id}"].Complete.PostAsync();


```