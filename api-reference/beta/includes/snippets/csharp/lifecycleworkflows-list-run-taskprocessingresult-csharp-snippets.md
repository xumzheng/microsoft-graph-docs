---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var result = await graphClient.IdentityGovernance.LifecycleWorkflows.Workflows["workflow-id"].Runs["run-id"].UserProcessingResults["userProcessingResult-id"].TaskProcessingResults.GetAsync();


```