---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

await graphClient.Me.Tasks.Lists["baseTaskList-id"].Tasks["baseTask-id"].ChecklistItems["checklistItem-id"].DeleteAsync();


```