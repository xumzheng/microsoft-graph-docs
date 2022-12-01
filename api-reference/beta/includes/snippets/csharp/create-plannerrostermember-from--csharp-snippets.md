---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new PlannerRosterMember
{
	OdataType = "#microsoft.graph.plannerRosterMember",
	UserId = "String",
};
var result = await graphClient.Planner.Rosters["plannerRoster-id"].Members.PostAsync(requestBody);


```