---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var executionScope = await graphClient.Identitygovernance.LifecycleWorkflows.Workflows["{identityGovernance.workflow-id}"].ExecutionScope
	.Request()
	.Select("id")
	.GetAsync();

```