---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

var graphClient = new GraphServiceClient(requestAdapter);

await graphClient.Print.Printers["{printer-id}"].Jobs["{printJob-id}"].Cancel.PostAsync();


```